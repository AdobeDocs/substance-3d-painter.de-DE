---
breadcrumb-title: ""
description: Erfahren Sie, wie Sie Probleme mit dem HDPI-Skalierungswert in Substance 3D Painter für die richtige Unterstützung einer hochauflösenden Anzeige beheben können.
title: Einige HDPI-Skalierungswerte funktionieren nicht
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
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
