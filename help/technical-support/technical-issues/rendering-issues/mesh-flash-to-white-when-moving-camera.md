---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/rendering-issues/mesh-flash-to-white-when-moving-camera.html"
breadcrumb-title: ''
description: Erfahre, wie du das Blinken von Gittern auf Weiß korrigierst, wenn du die Kamera im Substance 3D Painter-Viewport bewegst, um ein stabiles Rendering zu erreichen.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Rendering Issues > Mesh flash to white when moving camera
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Gitterblitz zu Weiß beim Verschieben der Kamera
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '140'
ht-degree: 0%

---


# Gitterblitz zu Weiß beim Verschieben der Kamera

![](../../../assets/white-flash-svt-optim.gif){width="300px"}

Bei alten Projekten, die sich im Viewport um die Kamera bewegen, werden manchmal kurze weiße Blitze angezeigt, die durch weiße/leere Texturen erzeugt wurden. Dies liegt daran, dass das [SVT-System (Sparse Virtual Textures](https://substance3d.adobe.com/display/DRAFTPAINTER/Sparse+Virtual+Textures)) auf bestimmten Shader-Konfigurationen basiert, die von älteren Shadern nicht verwendet werden.

Um den weißen Blitz zu entfernen, **aktualisieren** Sie einfach den **Projekt-Shader**:

* Für **Standardshader**: befolgen Sie die schrittweise Anleitung auf der Seite [Aktualisieren eines Shaders](../../../interface/shader-settings/updating-a-shader.md).
* Für **benutzerdefinierte Shader**: Sehen Sie sich die Fehlermeldung(en) im Protokoll sowie die [Shader-API](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/custom-shader-api-89686018.html)-Seite an.
