---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/scripting-and-development/api-reference/shader-api/shaders-shader-api/pixelated-shader-api.html"
breadcrumb-title: ''
description: Greifen Sie auf die Referenz "Verpixelter Shader-API" für Substance 3D Painter zu, um benutzerdefinierte pixelierte Rendereffekte zu erstellen.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Shaders - Shader API > Pixelated - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Verpixelt - Shader-API
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '179'
ht-degree: 0%

---


# Verpixelt - Shader-API

## Grundlegender pixelierender Shader

Aus Bibliotheken importieren.

```
import lib-sampler.glsl
```


Wir definieren die globale Lichtposition

```
const vec3 light_pos = vec3(10.0, 10.0, 10.0);
```


Wir **binden** die automatische param-Weltaugenposition an unsere einheitliche **Kamera\_Pos**.

```
//: param auto world_eye_position 

uniform vec3 camera_pos;
```


Wir **binden** den Kanal **Grundfarbe** des Dokuments an unsere einheitliche **Grundfarbe\_Text**.

```
//: param auto channel_basecolor 

uniform SamplerSparse basecolor_tex;
```


Wir definieren ein neues benutzerdefiniertes Tweak für diesen Shader, zusammen mit seinem Standardwert. Dieses Werkzeug wird verwendet, um die Thickness der Kontur beim Schatten zu optimieren.

```
//: param custom { 

//:  "default": 0.4, 

//:   "min": 0.0, 

//:   "max": 1.0, 

//:   "label": "Unlit outline thickness" 

//: } 

uniform float unlit_outline_thickness;
```


Wir definieren ein neues benutzerdefiniertes Tweak für diesen Shader, zusammen mit seinem Standardwert. Dieses dient dazu, die Thickness der Kontur zu optimieren, wenn sie beleuchtet wird.

```
//: param custom { 

//:   "default": 0.1, 

//:   "min": 0.0, 

//:   "max": 1.0, 

//:   "label": "Lit outline thickness" 

//: } 

uniform float lit_outline_thickness;
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


**Priorität** ist, die **Gliederungserkennung** auszuführen. Wenn die Umrissbedingung erfüllt ist, beenden Sie die Prüfung mit schwarzer Farbe.

```
  if (NdV < mix(unlit_outline_thickness, lit_outline_thickness, NdL)) { 

    return; 

  } 

 

  vec3 baseColor = getBaseColor(basecolor_tex, inputs.sparse_coord);
```


Jitter in der Maskengröße basierend auf der Luminanz der Grundfarbe hinzufügen.

```
  float maskRadiusJitter = pow(dot(baseColor, vec3(0.3333)), 0.1);
```


Berechnen Sie einen Maskenwert basierend auf der Bildschirmraumposition des Fragments. Dadurch wird ein Raster wie ein Muster erstellt.

```
  float mask = pow(1.0 - length(fract(gl_FragCoord.xy / 7.0) - vec2(0.5)), maskRadiusJitter * 5.0) * 5.0;
```


Hier nehmen wir die Grundfarbe auf und wenden eine einfache diffuse Dämpfung an

```
  vec3 color = baseColor * NdL; 

 

  diffuseShadingOutput(mask * color); 

} 

 
```
