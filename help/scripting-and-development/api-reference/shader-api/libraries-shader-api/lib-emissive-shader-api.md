---
breadcrumb-title: ""
description: Greifen Sie auf die Lib Emissive-Referenz für Substance 3D Painter zu, um emissive-Materials und leuchtende Effekte zu erstellen.
title: Lib Emissive - Shader-API
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
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


Die emissive-Kanal-Textur.

```
//: param auto channel_emissive 

uniform SamplerSparse emissive_tex;
```


Ein Wert, der zum Anpassen der emissive-Intensität verwendet wird.

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


Berechnen der emissive-Strahlung für den Betrachter

```
vec3 pbrComputeEmissive(SamplerSparse emissive, SparseCoord coord) 

{ 

  return emissive_intensity * textureSparse(emissive, coord).rgb; 

} 

 
```
