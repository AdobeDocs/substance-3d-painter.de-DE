---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/technical-support/technical-issues/gpu-issues/gpu-drivers-compatibility.html"
breadcrumb-title: ''
description: Erfahren Sie mehr über die Anforderungen an die GPU-Treiberkompatibilität für Substance 3D Painter, um ein stabiles Rendering und eine stabile Leistung zu gewährleisten.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > GPU Issues > GPU drivers compatibility
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Kompatibilität mit GPU-Treibern
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '144'
ht-degree: 2%

---


# Kompatibilität mit GPU-Treibern

Auf dieser Seite werden Informationen über GPU-Treiber zusammengefasst, die zu Problemen mit Substance 3D Painter führen können.

## Nvidia

Die folgende Tabelle listet alle Treiberversionen auf, die bekannt sind, um Probleme für Nvidia GPU (GeForce- oder Quadro-Modelle) zu erstellen:

| *Treiberversion* | *Problembeschreibung* |
| --- | --- |
| <b> 425.xx </b> | GPU-Raytracing-Artefakte. |
| <b> 429.xx oder älter </b> | Schwarze Texturen blockieren Artefakte. |
| <b> 435.xx oder älter </b> | sRGB-Farbprobleme bei der Berechnung von Texturen. |
| <b> 439.xx </b> | Texturen korrumpieren. |
| <b> 441.08 </b> | Absturz- oder Stabilitätsprobleme. |
| <b> 442.19 </b> | Absturz- oder Stabilitätsprobleme. |
| <b>528.09</b> | Betriebssystem friert ein. |
| <b>572.16 bis 572.42</b> | Artefakte oder Absturz beim Baking führ von Texturen. |

### AMD

| *Treiberversion* | *Problembeschreibung* |
| --- | --- |
| **20.7.x** bis **20.11.2** | Texturen treten auf oder sind beschädigt. |
| **20.11.3** bis **21.2.1** | Texturen treten auf oder sind beschädigt, und es treten Absturz- oder Stabilitätsprobleme auf. |
| **21.2.3** bis **21.6.1** | Absturz- oder Stabilitätsprobleme. |
