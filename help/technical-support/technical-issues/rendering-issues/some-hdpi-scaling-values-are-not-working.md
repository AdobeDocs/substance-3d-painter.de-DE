---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/rendering-issues/some-hdpi-scaling-values-are-not-working.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie Probleme mit dem HDPI-Skalierungswert in Substance 3D Painter für die richtige Unterstützung einer hochauflösenden Anzeige beheben können.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Rendering Issues > Some HDPI scaling values are not working
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Einige HDPI-Skalierungswerte funktionieren nicht
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '127'
ht-degree: 0%

---


# Einige HDPI-Skalierungswerte funktionieren nicht

Unter Windows funktionieren einige HDPI-Skalierungswerte (zur Skalierung der Schnittstelle auf Monitoren mit hoher Auflösung) möglicherweise nicht ordnungsgemäß.\
Das liegt daran, dass unser Fensterframework (Qt) sie nicht unterstützt. Wir sind nicht in der Lage, ihn zu beheben, bis er tatsächlich von den Anbietern des Rahmens selbst verwaltet wird.

Daher ist hier das Verhalten, auf das Sie je nach Ihren Einstellungen stoßen können:

* 120 DPI (**125%** Skalierung) - gerendert als 96 DPI (**100%** Skalierung)
* 144 DPI (**150%** Skalierung) - gerendert als 192 DPI (**200%** Skalierung)
* 168 DPI (**175%** Skalierung) - gerendert als 192 DPI (**200%** Skalierung)

Weitere Informationen finden Sie unter: <https://bugreports.qt.io/browse/QTBUG-55654>
