---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/scripting-and-development/api-reference/shader-api/parameters-shader-api/all-rendering-states-params-shader-api.html"
breadcrumb-title: ''
description: Rufen Sie die Shader-API-Referenz "Alle Rendering-Status-Parameter" für Substance 3D Painter auf, um die Rendering-Status-Parameter zu steuern.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Parameters - Shader API > All Rendering States Params - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Alle Rendering-Status-Parameter - Shader-API
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '107'
ht-degree: 2%

---


# Alle Rendering-Status-Parameter - Shader-API

## Beispiele für Rendering-Status

## Rückseiten ausblenden

Flächen zurücknehmen:

```
//: state cull_face on
```


Flächen vorne und hinten zeichnen:

```
//: state cull_face off
```


## Überblenden

Keine Überblendung, vollständig deckende Objekte:

```
//: state blend none
```


Standard-Mischmodus für die Zeichenreihenfolge von hinten nach vorne:

```
//: state blend over
```


Standard-Mischmodus für die Zeichenreihenfolge von hinten nach vorne. Angenommen, die Farbe wird mit Alpha vormultipliziert:

```
//: state blend over_premult
```


Additive Füllmethode:

```
//: state blend add
```


Multiplikative Füllmethode:

```
//: state blend multiply
```


## Ort der Shader-Probenahme

Standardmäßig werden für die Darstellung von Optimierungen beim Malen Dokumentkanäle mit nicht transformierten Textur-Koordinaten aufgenommen.

Wenn Artefakte angezeigt werden, setzen Sie den Status *nicht lokal* auf *am* .

```
//: state nonlocal on 

 
```
