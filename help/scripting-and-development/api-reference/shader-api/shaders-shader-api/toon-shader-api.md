---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/scripting-and-development/api-reference/shader-api/shaders-shader-api/toon-shader-api.html"
breadcrumb-title: ''
description: Greifen Sie auf die Referenz "Toon Shader-API" für Substance 3D Painter zu, um benutzerdefinierte Rendering-Effekte im Toon-Stil zu erstellen.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Shaders - Shader API > Toon - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Toon - Shader-API
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '195'
ht-degree: 0%

---


# Toon - Shader-API

## Grundlegender Shader

Aus Bibliotheken importieren.

```
import lib-sampler.glsl
```


Wir definieren die globale Lichtposition

```
const vec3 light_pos = vec3(10.0, 10.0, 10.0);
```


Wir **binden** die automatische param-Weltaugenposition an unsere Uniform **Kamera\_pos**.

```
//: param auto world_eye_position 

uniform vec3 camera_pos;
```


Wir **binden** den Dokumentkanal **Grundfarbe** an unsere Uniform **Grundfarbe\_Text**.

```
//: param auto channel_basecolor 

uniform SamplerSparse basecolor_tex;
```


Wir **binden** die **Mesh-Krümmung** an unsere einheitliche **Krümmung\_tex**. Wenn keine Krümmung verfügbar ist, wird eine durchsichtige Textur bereitgestellt.

```
//: param auto texture_curvature 

uniform SamplerSparse curvature_tex;
```


Wir definieren eine neue benutzerdefinierte Anpassung für diesen Shader zusammen mit dem Standardwert. Dieses Werkzeug wird verwendet, um die Thickness der Kontur beim Schatten zu optimieren.

```
//: param custom { 

//:  "default": 0.4, 

//:   "min": 0.0, 

//:   "max": 1.0, 

//:   "label": "Unlit outline thickness" 

//: } 

uniform float unlit_outline_thickness;
```


Wir definieren eine neue benutzerdefinierte Anpassung für diesen Shader zusammen mit dem Standardwert. Dieses dient dazu, die Thickness der Kontur zu optimieren, wenn sie beleuchtet wird.

```
//: param custom { 

//:   "default": 0.1, 

//:   "min": 0.0, 

//:   "max": 1.0, 

//:   "label": "Lit outline thickness" 

//: } 

uniform float lit_outline_thickness;
```


Ob wir die Krümmung lieber benutzen oder nicht.

```
//: param custom { 

//:   "default": false, 

//:   "label": "Use curvature" 

//: } 

uniform bool use_curvature;
```


Einstiegspunkt des Shaders.

```
void shade(V2F inputs) 

{
```


Wir berechnen einige nützliche Werte.

```
  vec3 V = normalize(camera_pos - inputs.position); 

  vec3 N = normalize(inputs.normal); 

  vec3 L = normalize(light_pos - inputs.position); 

  float NdV = dot(N, V); 

  float NdL = max(0.0, dot(N, L));
```


**Priorität** ist, die **Gliederungserkennung** auszuführen. Erlauben Sie dem Benutzer, auszuwählen, ob er die Krümmungs-Map für die Konturerkennung bevorzugt oder nicht.

```
  if (use_curvature) { 

    float curv = textureSparse(curvature_tex, inputs.sparse_coord).r; 

    NdV = 1.0 - curv; 

  }
```


Wenn die Umrissbedingung erfüllt ist, beenden Sie die Prüfung mit schwarzer Farbe.

```
  if (NdV < mix(unlit_outline_thickness, lit_outline_thickness, NdL)) { 

    return; 

  }
```


Hier führen wir eine 4-stufige Diskretisierung der Farbe.

```
  vec3 color = getBaseColor(basecolor_tex, inputs.sparse_coord); 

  if (NdL > 0.75) { 

    color = color; 

  } else if (NdL > 0.5) { 

    color = color * 0.5; 

  } else if (NdL > 0.1) { 

    color = color * 0.1; 

  } 

  else
```


Fallback ist schwarz.

```
    color = vec3(0.0); 

 

  diffuseShadingOutput(color); 

} 

 
```
