---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/workflow-issues/tools-issues/normal-map-looks-incorrect-when-loaded-in-layer-or-tool-properties.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie Probleme mit der Normalen-Map-Anzeige in den Ebenen- und Werkzeugeigenschaften von Substance 3D Painter beheben, um präzise Oberflächendetails zu erhalten.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > Tools Issues > Normal map looks incorrect when loaded in layer or tool properties
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Normalen-Map sieht beim Laden in Ebenen- oder Werkzeugeigenschaften falsch aus
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '105'
ht-degree: 0%

---


# Normalen-Map sieht beim Laden in Ebenen- oder Werkzeugeigenschaften falsch aus

Wenn Sie eine Normalität in das aktuelle Tool von Füllebene laden, kann diese fehlerhaft erscheinen, wenn es sich um eine OpenGL-Normalen-Map handelt.\
Der Grund ist ganz einfach: Das Engine von Substance 3D Painter nimmt an, dass geladene Normalen-Map standardmäßig DirectX sind.

Dieses Material lässt sich einfach bearbeiten, indem man auf den kleinen Pfeil neben dem Substance-Kanal oder dem dedizierten Kanal klickt:

![](../../../assets/channel-format-override.png)
