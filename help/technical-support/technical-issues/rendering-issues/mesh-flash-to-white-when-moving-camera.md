---
breadcrumb-title: ""
description: Erfahren Sie, wie Sie den Mesh, der weiß blinkt, wenn Sie die Kamera in Substance 3D Painter Viewport für ein stabiles Rendering verschieben, beheben können.
title: Mesh blinkt bei Bewegung der Kamera weiß
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '140'
ht-degree: 0%
---

# Mesh blinkt bei Bewegung der Kamera weiß

![](../../../assets/white-flash-svt-optim.gif){width="300px"}

Bei alten Projekten, die sich um die Kamera bewegen, kann der Viewport kurze Weiß-Blitze anzeigen, die durch weiße/leere Texturen erzeugt werden. Dies liegt daran, dass das System [Dünn besetzte virtuelle Texturen](https://substance3d.adobe.com/display/DRAFTPAINTER/Sparse+Virtual+Textures) (SVT) auf bestimmten Shader-Konfigurationen basiert, die von älteren Shadern nicht verwendet werden.

Um den weißen Blitz zu entfernen, **aktualisieren** Sie einfach den **Projekt-Shader**:

* Für **Standardshader**: befolgen Sie die schrittweise Anleitung auf der Seite [Aktualisieren eines Shader](../../../interface/shader-settings/updating-a-shader.md).
* Für **benutzerdefinierte Shader**: Sehen Sie sich die Fehlermeldung(en) im Protokoll sowie die [Shader-API](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/custom-shader-api-89686018.html)-Seite an.
