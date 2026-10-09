---
breadcrumb-title: ""
description: Greifen Sie auf die Shader-API-Referenz für den Material "Ebenenbindung" für Substance 3D Painter zu, um Materialien in Workflows mit Ebenen zu binden.
title: Schichtung von Bind-Materialien - Shader-API
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '106'
ht-degree: 0%
---

# Schichtung von Bind-Materialien - Shader-API

## Material-Ebenen: Materialien als Shader-Parameter binden

Ein Material wird durch eine eindeutige Identifizierung &quot;id&quot; definiert. Zusätzliche Parameter:

* &#39;default&#39;: den standardmäßigen Namen der Material-Ressource, die verwendet werden soll.
* &#39;Größe&#39;: die Textur der Material Maps.
* Gruppe: der UI-Gruppe des Material-Auswahlwerkzeugs.

Beispiel:

```
//:  materials [ 

//:    { 

//:       "id": "Material1", 

//:       "default": "Concrete 044", 

//:       "size": 512, 

//:       "group": "Material 1" 

//:    }, { 

//:       "id": "Material2", 

//:       "default": "Leaves elm", 

//:       "size": 1024, 

//:       "group": "Material 2" 

//:    } 

//:  ]
```


Um einen Kanal von einem Material an einen Sampler zu binden, definieren Sie einen automatischen Parameter mit der ID des Materials, gefolgt vom Channel-Tag (siehe die verfügbaren Kanäle in [all-Engine-params.glsl](all-engine-params-shader-api.md)):

```
//: param auto Material1.channel_basecolor 

uniform sampler2D basecolor_tex1; 

//: param auto Material1.channel_metallic 

uniform sampler2D metallic_tex1; 

//: param auto Material1.channel_roughness 

uniform sampler2D roughness_tex1; 

 

//: param auto Material2.channel_basecolor 

uniform sampler2D basecolor_tex2; 

//: param auto Material2.channel_metallic 

uniform sampler2D metallic_tex2; 

//: param auto Material2.channel_roughness 

uniform sampler2D roughness_tex2; 

 
```
