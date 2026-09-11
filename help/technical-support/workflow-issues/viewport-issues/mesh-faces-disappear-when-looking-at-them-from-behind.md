---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/technical-support/workflow-issues/viewport-issues/mesh-faces-disappear-when-looking-at-them-from-behind.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie das Verschwinden von Mesh-Flächen beheben, wenn sie von hinten in Substance 3D Painter Viewport angezeigt werden, um die Sichtbarkeit von Meshs zu gewährleisten.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > Viewport Issues > Mesh faces disappear when looking at them from behind
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Mesh-Flächen verschwinden, wenn man sie von hinten betrachtet
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '86'
ht-degree: 0%

---


# Mesh-Flächen verschwinden, wenn man sie von hinten betrachtet

Standardmäßig zeigen Mesh im Viewport nicht die Rückseite des Mesh-Polygons (Rückseite) an. Das liegt daran, dass sie vom aktuellen Shader gekeult werden.

Um die Rückseite der Flächen anzuzeigen, ändern Sie einfach den aktuellen Shader in **pbr-metal-raw-alpha-test** in den [Shader-Einstellungen](../../../interface/shader-settings/shader-settings.md).
