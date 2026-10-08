---
breadcrumb-title: ""
description: Greifen Sie auf die Shader-API-Referenz zu Lib Alpha für Substance 3D Painter zu, um mit Alphakanälen und Transparenz in benutzerdefinierten Shadern zu arbeiten.
title: Lib Alpha - Shader-API
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
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


Deckkraftkarte, vom Engine bereitgestellt.

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


Alpha Test Dithering.

```
//: param custom { 

//:   "default": false, 

//:   "label": "Alpha dithering", 

//:   "group": "Common Parameters" 

//: } 

uniform bool alpha_dither;
```


Alphatest emulieren: Aktuelles Fragment verwerfen, wenn seine Deckkraft unter einem benutzerdefinierten Schwellenwert liegt. Nach Textur-Sampling-Aufrufen aufrufen: er kann Derivate zerschlagen

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
