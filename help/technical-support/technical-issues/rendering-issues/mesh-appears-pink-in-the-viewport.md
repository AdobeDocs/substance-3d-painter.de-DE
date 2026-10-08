---
breadcrumb-title: ""
description: Erfahren Sie, wie Sie das Aussehen rosa Meshs in Substance 3D Painter Viewport korrigieren, um das ordnungsgemäße Rendern von Materialien wiederherzustellen.
title: Mesh erscheint rosa im Viewport
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '125'
ht-degree: 0%
---

# Mesh erscheint rosa im Viewport

![](../../../assets/pink-mesh.jpg){width="400px"}

Der Mesh kann **pink** im Viewport erscheinen, da der **Shader**, der zum Zeichnen verwendet wurde **, nicht mehr kompiliert wird** (wie vom **Protokollfenster** erwähnt). Dies kann durch einen veralteten Shader verursacht werden, der die neueste Version des Shader-API nicht unterstützt.

So kann es behoben werden:

* Für **Standardshader**: befolgen Sie die schrittweise Anleitung auf der Seite [Aktualisieren eines Shader](../../../interface/shader-settings/updating-a-shader.md).
* Für **benutzerdefinierten Shader**: sehen Sie sich die Fehlermeldung im Protokollfenster sowie auf der Seite [Shader-API](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/custom-shader-api-89686018.html) an.
