---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/workflow-issues/viewport-issues/mesh-faces-disappear-when-looking-at-them-from-behind.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie im Substance 3D Painter-Viewport für eine korrekte Gittersichtbarkeit festlegen können, dass bei einer rückwärtigen Betrachtung Gitterflächen verschwinden.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > Viewport Issues > Mesh faces disappear when looking at them from behind
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Gittergesichter verschwinden, wenn sie von hinten betrachtet werden
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '86'
ht-degree: 0%

---


# Gittergesichter verschwinden, wenn sie von hinten betrachtet werden

Standardmäßig wird bei Gittern im Viewport die Rückseite der Gitterpolygone (Rückseite) nicht angezeigt. Das liegt daran, dass sie vom aktuellen Shader gekeult werden.

Um die Rückseite der Gesichter anzuzeigen, ändern Sie einfach den aktuellen Shader in den [Shader-Einstellungen](../../../interface/shader-settings/shader-settings.md) in **pbr-metal-raw-alpha-test**.
