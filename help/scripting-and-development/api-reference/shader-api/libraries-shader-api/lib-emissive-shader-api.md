---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/scripting-and-development/api-reference/shader-api/libraries-shader-api/lib-emissive-shader-api.html"
breadcrumb-title: ''
description: Greifen Sie auf die Lib Emissive Shader-API-Referenz für Substance 3D Painter zu, um Emissionsmaterialien und glühende Effekte zu erzeugen.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Libraries - Shader API > Lib Emissive - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Lib Emissive - Shader-API
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '54'
ht-degree: 0%

---


# Lib Emissive - Shader-API

## lib-emissive.glsl

**Öffentliche Funktionen:** *pbrComputeEmissive*

Aus Bibliothek importieren

```
import lib-sparse.glsl
```


Die Struktur des Emissionskanals.

```
//: param auto channel_emissive 

uniform SamplerSparse emissive_tex;
```


Ein Wert, der zum Anpassen der Emissionsintensität verwendet wird.

```
//: param custom { 

//:   "default": 1.0, 

//:   "label": "Emissive Intensity", 

//:   "min": 0.0, 

//:   "max": 100.0, 

//:   "group": "Common Parameters" 

//: } 

uniform float emissive_intensity;
```


Berechnen der emittierenden Strahlung für das Auge des Betrachters

```
vec3 pbrComputeEmissive(SamplerSparse emissive, SparseCoord coord) 

{ 

  return emissive_intensity * textureSparse(emissive, coord).rgb; 

} 

 
```
