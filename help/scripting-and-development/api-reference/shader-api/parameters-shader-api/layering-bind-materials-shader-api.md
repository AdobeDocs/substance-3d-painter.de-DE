---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/scripting-and-development/api-reference/shader-api/parameters-shader-api/layering-bind-materials-shader-api.html"
breadcrumb-title: ''
description: Greifen Sie auf die Shader-API-Referenz für den Layering Bind Materials für Substance 3D Painter zu, um Materialien in Arbeitsabläufen mit Ebenen zu binden.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Parameters - Shader API > Layering Bind Materials - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Schichtung von Bind-Materialien - Shader-API
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '106'
ht-degree: 0%

---


# Schichtung von Bind-Materialien - Shader-API

## Materialschichtung: Materialien als Shader-Parameter binden

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
