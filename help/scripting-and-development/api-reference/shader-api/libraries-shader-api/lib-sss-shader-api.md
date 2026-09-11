---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/scripting-and-development/api-reference/shader-api/libraries-shader-api/lib-sss-shader-api.html"
breadcrumb-title: ''
description: Greifen Sie auf die Bibliothek SSS Shader-API reference für Substance 3D Painter zu, um Volumenstreuung-Effekte in benutzerdefinierten Shadern zu erstellen.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Libraries - Shader API > Lib SSS - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Lib SSS - Shader-API
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '78'
ht-degree: 0%

---


# Lib SSS - Shader-API

## lib-sss.glsl

**Öffentliche Funktionen:** *getSSSCoeffizienten*

Aus Bibliothek importieren

```
import lib-sampler.glsl
```


Die skalare SSS-Koeffizient-Textur

```
//: param auto channel_scattering 

uniform SamplerSparse sss_tex; 

 

//: param auto scene_original_radius 

uniform float sssSceneScale; 

 

//: param custom { 

//:   "label": "Enable", 

//:   "default": true, 

//:   "group": "Subsurface Scattering Parameters", 

//:   "description": "<html><head/><body><p>Enable the Subsurface Scattering. It needs to be activated in the Display Settings and a Scattering channel needs to be present for these parameters to have an effect.</p></body></html>" 

//: } 

uniform bool sssEnabled;
```


Wählen Sie, ob das Licht direkt durch das Material eindringt (lichtdurchlässig) oder diffus ist, bevor Sie mit der Streuung beginnen (Haut).

```
//: param custom { 

//:   "default": 1, 

//:   "label": "Scattering Type", 

//:   "widget": "combobox", 

//:   "values": { 

//:     "Translucent": 0, 

//:     "Skin": 1 

//:   }, 

//:   "group": "Subsurface Scattering Parameters", 

//:   "description": "<html><head/><body><p>Skin or Translucent/Generic. It needs to be activated in the Display Settings and a Scattering channel needs to be present for these parameters to have an effect.</p></body></html>" 

//: } 

uniform int sssType;
```


Globale Skalierung bis zum Effekt &quot;Volumenstreuung&quot;

```
//: param custom { 

//:   "default": 0.5, 

//:   "label": "Scale", 

//:   "min": 0.01, 

//:   "max": 1.0, 

//:   "group": "Subsurface Scattering Parameters", 

//:   "description": "<html><head/><body><p>Controls the radius/depth of the light absorption in the material. It needs to be activated in the Display Settings and a Scattering channel needs to be present for these parameters to have an effect.</p></body></html>" 

//: } 

uniform float sssScale;
```


Wellenlängenabhängigkeit des SSS des Materials

```
//: param custom { 

//:   "default": [0.701, 0.301, 0.305], 

//:   "label": "Color", 

//:   "widget": "color", 

//:   "group": "Subsurface Scattering Parameters", 

//:   "description": "<html><head/><body><p>The color of light when absorbed by the material. It needs to be activated in the Display Settings and a Scattering channel needs to be present for these parameters to have an effect.</p></body></html>" 

//: } 

uniform vec3 sssColor;
```


Gibt die Material-SSS-Koeffizienten zurück

```
vec4 getSSSCoefficients(float scattering) { 

  if (sssEnabled) { 

    vec3 sss = sssScale / sssSceneScale * scattering * sssColor; 

    return vec4(sss, sss == vec3(0.0) ? 0.0 : 1.0); 

  } 

  return vec4(0.0); 

} 

vec4 getSSSCoefficients(SparseCoord coord) { 

  if (sssEnabled) { 

    return getSSSCoefficients(getScattering(sss_tex, coord)); 

  } 

  return vec4(0.0); 

} 

 
```
