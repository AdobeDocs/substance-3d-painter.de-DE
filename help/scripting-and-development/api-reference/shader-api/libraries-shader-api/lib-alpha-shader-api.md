---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/scripting-and-development/api-reference/shader-api/libraries-shader-api/lib-alpha-shader-api.html"
breadcrumb-title: ''
description: Greifen Sie auf die Lib Alpha Shader-API-Referenz für Substance 3D Painter zu, um mit Alphakanälen und Transparenz in benutzerdefinierten Shadern zu arbeiten.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Libraries - Shader API > Lib Alpha - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Lib Alpha - Shader-API
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '72'
ht-degree: 0%

---


# Lib Alpha - Shader-API

## lib-alpha.glsl

**Öffentliche Funktionen:** *alphaKill*

```
import lib-sampler.glsl 

import lib-random.glsl
```


Deckkraftkarte, vom Motor geliefert.

```
//: param auto channel_opacity 

uniform SamplerSparse opacity_tex;
```


Alpha-Prüfschwelle.

```
//: param custom { 

//:   "default": 0.33, 

//:   "label": "Alpha threshold", 

//:   "min": 0.0, 

//:   "max": 1.0, 

//:   "group": "Common Parameters" 

//: } 

uniform float alpha_threshold;
```


Alpha-Test-Dithering.

```
//: param custom { 

//:   "default": false, 

//:   "label": "Alpha dithering", 

//:   "group": "Common Parameters" 

//: } 

uniform bool alpha_dither;
```


Alphatest emulieren: Aktuelles Fragment verwerfen, wenn seine Deckkraft unter einem benutzerdefinierten Schwellenwert liegt. Sollte AFTER-Textursampling-Aufrufe heißen: er kann Derivate zerschlagen

```
void alphaKill(float alpha) 

{ 

  float threshold = alpha_dither ? getBlueNoiseThresholdTemporal() : alpha_threshold; 

  if (alpha < threshold) discard; 

} 

 

void alphaKill(SparseCoord coord) 

{ 

  alphaKill(getOpacity(opacity_tex, coord)); 

} 

 
```
