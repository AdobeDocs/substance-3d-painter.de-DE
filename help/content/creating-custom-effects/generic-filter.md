---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/content/creating-custom-effects/generic-filter.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie generische Filtereffekte für Substance 3D Painter erstellen, um benutzerdefinierte Bildverarbeitungs- und Texturfilter anzuwenden.
helpx_creative_field: ""
helpx_description: Painter > Content > Creating custom effects > Generic filter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Generischer Filter
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '144'
ht-degree: 0%

---


# Generischer Filter

Ein generischer Effekt wird auf alle Dokumentkanäle angewendet, einschließlich der Deckkraft. Ein generischer Filter kann sein:

* **grayscale**, wird auf jede Komponente (R, G, B und A) jedes Kanals (Grundfarbe, Metallic, Raueit usw.) angewendet
* **color**, wird auf den farbigen Kanal unverändert angewendet oder intern in Graustufen konvertiert, um Graustufen-Kanäle zu beeinflussen

Der Eingabeknoten des Effekts muss den **Bezeichner** oder **Verwendung** aufweisen, der **Eingabe** definiert ist, und sein Ausgabeknoten muss **Ausgabe** aufweisen. Beachten Sie, dass **Farbfilter** nicht auf der Maske einer Ebene verwendet werden können, nur **Graustufen** Filter sind kompatibel.

>[!NOTE]
>
> Es ist möglich, in einem Eingabeknoten entweder **usage** oder **identifier** zu verwenden (die Verwendung hat die Priorität).

Beispiel :

![](../../assets/generic-filter.png)![](../../assets/generic-rgba.png){width="575px"}
