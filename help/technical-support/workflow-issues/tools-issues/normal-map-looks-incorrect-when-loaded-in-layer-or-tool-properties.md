---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/workflow-issues/tools-issues/normal-map-looks-incorrect-when-loaded-in-layer-or-tool-properties.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie Probleme mit der Normalmap-Anzeige in den Ebenen- und Werkzeugeigenschaften von Substance 3D Painter beheben, um präzise Oberflächendetails zu erhalten.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > Tools Issues > Normal map looks incorrect when loaded in layer or tool properties
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Normale Karte sieht falsch aus, wenn sie in Ebenen- oder Werkzeugeigenschaften geladen wird
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '105'
ht-degree: 0%

---


# Normale Karte sieht falsch aus, wenn sie in Ebenen- oder Werkzeugeigenschaften geladen wird

Wenn Sie eine Normale in das aktuelle Werkzeug der Füllebene laden, kann diese falsch erscheinen, wenn es sich um eine OpenGL-Normalmap handelt.\
Der Grund ist ganz einfach: Die Engine von Substance 3D Painter geht davon aus, dass die geladene Normalmap standardmäßig DirectX ist.

Dieses Verhalten lässt sich leicht bearbeiten, indem Sie auf den kleinen Pfeil neben dem Substance-Material oder dem dedizierten Kanal klicken:

![](../../../assets/channel-format-override.png)
