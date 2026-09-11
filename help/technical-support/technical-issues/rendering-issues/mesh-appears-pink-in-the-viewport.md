---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/technical-support/technical-issues/rendering-issues/mesh-appears-pink-in-the-viewport.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie das Aussehen rosa Meshs in Substance 3D Painter Viewport korrigieren, um das ordnungsgemäße Rendern von Materialien wiederherzustellen.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Rendering Issues > Mesh appears pink in the viewport
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Mesh erscheint rosa im Viewport
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '125'
ht-degree: 0%

---


# Mesh erscheint rosa im Viewport

![](../../../assets/pink-mesh.jpg){width="400px"}

Der Mesh kann **pink** im Viewport erscheinen, da der **Shader**, der zum Zeichnen verwendet wurde **, nicht mehr kompiliert wird** (wie vom **Protokollfenster** erwähnt). Dies kann durch einen veralteten Shader verursacht werden, der die neueste Version des Shader-API nicht unterstützt.

So kann es behoben werden:

* Für **Standardshader**: befolgen Sie die schrittweise Anleitung auf der Seite [Aktualisieren eines Shader](../../../interface/shader-settings/updating-a-shader.md).
* Für **benutzerdefinierten Shader**: sehen Sie sich die Fehlermeldung im Protokollfenster sowie auf der Seite [Shader-API](https://helpx.adobe.com/de/substance-3d/unlisted/documentation/spdoc/custom-shader-api-89686018.html) an.
