---
breadcrumb-title: ""
description: Greifen Sie auf die Shader-API-Referenz für "Stapel deklarieren für Ebenen" für Substance 3D Painter zu, um benutzerdefinierte Stapel für Materialien zu erstellen.
title: Declare-Stapel überlagern - Shader-API
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '101'
ht-degree: 0%
---

# Declare-Stapel überlagern - Shader-API

## Material-Ebenen: Deklarieren bearbeitbarer Stapel

Ein bearbeitbarer Stapel wird durch eine eindeutige Identifizierung und eine Liste von Dokumentkanälen definiert. Mögliche Kanal-ID(en): *Ambientocclusion* *Anisotropyangle* *Anisotropylevel* *Basisfarbe* *Mischmaske* *diffuse* *Versatz* *emissive* *Glanz* *Height* *Älter* *metallic 23&rbrace;* Normal **&#x200B; Deckkraft &#x200B;** Reflexion **&#x200B; Rauheit &#x200B;** Streuung **&#x200B; Specular &#x200B;** Spiegelebene **&#x200B; transmissive &#x200B;** Benutzer0 **&#x200B; Benutzer1 &#x200B;** Benutzer2 45&rbrace; *Benutzer3* *Benutzer4* *Benutzer5* *Benutzer6* *Benutzer7***

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


Um einen Kanal von einem Stapel an einen Samplerparameter zu binden, setzen Sie dem Kanal-Tag die Stapel-Identifizierung voran:

```
//: param auto Mask1.channel_opacity 

uniform sampler2D mask_tex1; 

//: param auto Mask2.channel_opacity 

uniform sampler2D mask_tex2; 

 
```
