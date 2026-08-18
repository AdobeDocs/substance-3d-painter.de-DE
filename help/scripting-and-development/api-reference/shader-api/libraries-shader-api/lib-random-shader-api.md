---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/scripting-and-development/api-reference/shader-api/libraries-shader-api/lib-random-shader-api.html"
breadcrumb-title: ''
description: Greifen Sie auf die Lib Random Shader-API-Referenz für Substance 3D Painter zu, um zufällige Werte in der Entwicklung benutzerdefinierter Shader zu generieren.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Libraries - Shader API > Lib Random - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Lib Random - Shader-API
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '128'
ht-degree: 0%

---


# Lib Random - Shader-API

## lib-random.glsl

**Öffentliche Funktionen:** *getBlueNoiseThreshold* *getBlueNoiseThresholdTemporal* *fibonacci1D* *fibonacci2D* *fibonacci2DDitheredTemporal*

Aus Bibliothek importieren

```
import lib-defines.glsl
```


Eine 2D-Struktur für blaues Rauschen mit Skalarwerten

```
//: param auto texture_blue_noise 

uniform sampler2D texture_blue_noise;
```


Strukturauflösung für blaues Rauschen

```
const ivec2 texture_blue_noise_size = ivec2(256);
```


Aktuelle Frame-Zufallswert

```
//: param auto random_seed 

uniform int alg_random_seed;
```


Erhalten Sie einen einheitlichen Zufallswert basierend auf Pixelkoordinaten.

```
float getBlueNoiseThreshold() 

{ 

  return texture(texture_blue_noise, gl_FragCoord.xy / vec2(texture_blue_noise_size)).x + 0.5 / 65536.0; 

}
```


Erhalten Sie einen einheitlichen Zufallswert basierend auf Pixelkoordinaten und Frame-ID.

```
float getBlueNoiseThresholdTemporal() 

{ 

  return fract(getBlueNoiseThreshold() + M_GOLDEN_RATIO * alg_random_seed); 

}
```


Gibt die i *th*-Zahl aus der Fibonacci-Sequenz zurück.

```
float fibonacci1D(int i) 

{ 

  return fract((float(i) + 1.0) * M_GOLDEN_RATIO); 

}
```


Gibt das i *th*-Paar aus der Fibonacci-Sequenz zurück. nbSample ist erforderlich, um eine einheitliche Verteilung zu erhalten.

```
vec2 fibonacci2D(int i, int nbSamples) 

{ 

  return vec2( 

    (float(i)+0.5) / float(nbSamples), 

    fibonacci1D(i) 

  ); 

}
```


Gibt das i *th*-Paar aus der Fibonacci-Sequenz zurück. nbSample ist erforderlich, um eine einheitliche Verteilung zu erhalten. Bei dieser Version wird eine pseudozufällige Drehung pro Frame und Pixel angewendet.

```
vec2 fibonacci2DDitheredTemporal(int i, int nbSamples) 

{ 

  vec2 s = fibonacci2D(i, nbSamples); 

  s.x += getBlueNoiseThresholdTemporal(); 

  return s; 

} 

 
```
