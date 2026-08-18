---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/rendering-issues/mesh-appears-pink-in-the-viewport.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie das rosa Gitteraussehen im Substance 3D Painter-Viewport korrigieren, um das richtige Material-Rendering wiederherzustellen.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Rendering Issues > Mesh appears pink in the viewport
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Gitter wird im Darstellungsfenster rosa angezeigt
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '125'
ht-degree: 0%

---


# Gitter wird im Darstellungsfenster rosa angezeigt

![](../../../assets/pink-mesh.jpg){width="400px"}

Das Gitter kann **pink** im Viewport erscheinen, da der **Shader**, der es gezeichnet hat **, nicht mehr kompiliert** (wie vom **Protokollfenster** erwähnt). Dies kann durch einen veralteten Shader verursacht werden, der die neueste Version des Shader-API nicht unterstützt.

So kann es behoben werden:

* Für **Standardshader**: befolgen Sie die schrittweise Anleitung auf der Seite [Aktualisieren eines Shaders](../../../interface/shader-settings/updating-a-shader.md).
* Für **benutzerdefinierten Shader**: sehen Sie sich die Fehlermeldung im Protokollfenster sowie auf der Seite [Shader-API](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/custom-shader-api-89686018.html) an.
