---
breadcrumb-title: ""
description: Erfahren Sie, wie Sie das Verschwinden von Mesh-Flächen beheben, wenn sie von hinten in Substance 3D Painter Viewport angezeigt werden, um die Sichtbarkeit von Meshs zu gewährleisten.
title: Mesh-Flächen verschwinden, wenn man sie von hinten betrachtet
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '86'
ht-degree: 0%
---

# Mesh-Flächen verschwinden, wenn man sie von hinten betrachtet

Standardmäßig zeigen Mesh im Viewport nicht die Rückseite des Mesh-Polygons (Rückseite) an. Das liegt daran, dass sie vom aktuellen Shader gekeult werden.

Um die Rückseite der Flächen anzuzeigen, ändern Sie einfach den aktuellen Shader in **pbr-metal-raw-alpha-test** in den [Shader-Einstellungen](../../../interface/shader-settings/shader-settings.md).
