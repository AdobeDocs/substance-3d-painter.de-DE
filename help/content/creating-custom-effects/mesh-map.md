---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/content/creating-custom-effects/mesh-map.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie Mesh-Map in benutzerdefinierten Effekten für Substance 3D Painter verwenden, um auf Informationen zu geometriebasierten Texturen zuzugreifen.
helpx_creative_field: ""
helpx_description: Painter > Content > Creating custom effects > Mesh Map
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Mesh-Map
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '120'
ht-degree: 3%

---


# Mesh-Map

Damit Mesh-Map (Baking geführt Texturen) beim Hinzufügen eines Effekts zu einer Ebene automatisch verbunden werden, muss eine bestimmte Benennungskonvention eingehalten werden.

>[!NOTE]
>
> Es ist möglich, die **Verwendung** oder die **Identifizierung** in einem Eingabeknoten zu verwenden (die Verwendung hat die Priorität).

Hier ist die Namenskonvention für jede Mesh-Map:

| Mesh-Map | Nutzung | Kennung |
| --- | --- | --- |
| *Ambient occlusion* | **ambientOcclusionBase** | **Ambient\_Verdeckung** |
| *ID* | **id** | **id** |
| *Krümmung* | **Krümmung** | **Krümmung** |
| *Normal* | **normalBase** | **normal\_base** |
| *Welt-Raum-Normale* | **normalWS** | **Welt\_Raum\_Normale** |
| *Position* | **Position** | **Position** |
| *Thickness* | **Thickness** | **Thickness** |
| *Height* | **heightBase** | **Height\_base** |
| *Gebeugte Normale* | **bentNormalsBase** | **verbogen\_normals\_base** |
| *Deckkraft* | **opacityBase** | **Deckkraft\_Basis** |
