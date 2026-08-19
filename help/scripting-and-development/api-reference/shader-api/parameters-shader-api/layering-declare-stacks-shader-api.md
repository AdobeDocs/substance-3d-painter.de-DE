---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/scripting-and-development/api-reference/shader-api/parameters-shader-api/layering-declare-stacks-shader-api.html"
breadcrumb-title: ''
description: Greifen Sie auf die Shader-API-Referenz für "Ebenen deklarieren" für Substance 3D Painter zu, um benutzerdefinierte Materialebenen-Stapel zu erstellen.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Parameters - Shader API > Layering Declare Stacks - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Declare Stacks - Shader-API
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '101'
ht-degree: 0%

---


# Declare Stacks - Shader-API

## Materialschichtung: Bearbeitbare Stapel deklarieren

Ein bearbeitbarer Stapel wird durch eine eindeutige Kennung und eine Liste von Dokumentkanälen definiert. Mögliche Kanal-ID(en): *Ambientocclusion* *Anisotropyangle* *Anisotropylevel* *Basisfarbe* *Mischmaske* *diffuse* *Versatz* *emittierend* *Glanzgrad* *Height* *Metallisch* *Metallisch* *Normal* *Deckkraft* *Reflexion* *Raueit* *Streuung* *Specular* *Spiegelebene* *durchlässig* *Benutzer0* *Benutzer1* *user2* *user3* *user4* *user5* *user6* *user7*

Beispiel:

```
//:  stacks [ 

//:    { 

//:      "id": "Mask1", 

//:      "channels": [ 

//:        {"id": "opacity"} 

//:      ] 

//:    }, { 

//:      "id": "Mask2", 

//:      "channels": [ 

//:        {"id": "opacity"}, 

//:        {"id": "user0"} 

//:      ] 

//:    } 

//:  ]
```


Um einen Kanal aus einem Stapel an einen Samplerparameter zu binden, setzen Sie dem Kanal-Tag die Stapelkennung voran:

```
//: param auto Mask1.channel_opacity 

uniform sampler2D mask_tex1; 

//: param auto Mask2.channel_opacity 

uniform sampler2D mask_tex2; 

 
```
