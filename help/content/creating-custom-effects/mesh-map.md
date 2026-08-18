---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/content/creating-custom-effects/mesh-map.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie Gitterzuordnungen in benutzerdefinierten Effekten für Substance 3D Painter verwenden, um auf geometriebasierte Texturinformationen zuzugreifen.
helpx_creative_field: ""
helpx_description: Painter > Content > Creating custom effects > Mesh Map
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Gitterkarte
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '120'
ht-degree: 3%

---


# Gitterkarte

Um beim Hinzufügen eines Effekts zu einer Ebene automatisch Gitterzuordnungen (baked textures) zu verbinden, muss eine bestimmte Benennungskonvention eingehalten werden.

>[!NOTE]
>
> Es ist möglich, in einem Eingabeknoten entweder **usage** oder **identifier** zu verwenden (die Verwendung hat die Priorität).

Hier ist die Benennungskonvention für jede Meshmap:

| Mesh-Map | Nutzung | Kennung |
| --- | --- | --- |
| *Umgebungs-Verdeckung* | **ambientOcclusionBase** | **Ambient\_Verdeckung** |
| *ID* | **id** | **id** |
| *Krümmung* | **Krümmung** | **Krümmung** |
| *Normal* | **normalBase** | **normal\_base** |
| *Normale im Weltraum* | **normalWS** | **Welt\_Raum\_Normale** |
| *Position* | **Position** | **Position** |
| *Thickness* | **Thickness** | **Thickness** |
| *Height* | **heightBase** | **Height\_base** |
| *Gebeugte Normale* | **bentNormalsBase** | **verbogen\_normals\_base** |
| *Deckkraft* | **opacityBase** | **Deckkraft\_Basis** |
