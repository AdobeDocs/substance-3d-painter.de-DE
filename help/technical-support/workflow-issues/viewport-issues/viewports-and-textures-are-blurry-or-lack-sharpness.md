---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/technical-support/workflow-issues/viewport-issues/viewports-and-textures-are-blurry-or-lack-sharpness.html"
breadcrumb-title: ''
description: Erfahre, wie du in Substance 3D Painter unscharfe Viewports und Strukturen anpasst, um eine scharfe, klare Bildqualität zu erzielen.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > Viewport Issues > Viewports and textures are blurry or lack sharpness
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Viewports und Texturen sind verschwommen oder nicht scharf
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 1%

---


# Viewports und Texturen sind verschwommen oder nicht scharf

Die Viewports können aus verschiedenen Gründen verschwommen angezeigt werden.

## Einstellungen für HiDPI-Bildschirme (Retina)

Standardmäßig verkleinert Substance 3D Painter die Viewport-Auflösung auf dem Bildschirm mit hoher DPI-/Retina-Auflösung, um die Leistung zu verbessern.

Dieses Verhalten kann in den [Haupteinstellungen](https://helpx.adobe.com/de/substance-3d/unlisted/documentation/spdoc/general-71008262.html) geändert werden, indem der Parameter **Viewport-Skalierung** geändert wird.

## Texturfilterung

Die Viewports verwenden Mipmaps und Texturfilterung, um [Virtuelle Texturen mit geringer Dichte](../../../features/sparse-virtual-textures.md) zu streamen und zu streamen und so die Leistung zu verbessern. Das kann in manchen Fällen zu unscharfen Strukturen führen.

Die Texturfilterung kann über das Fenster Anzeigeeinstellungen unter den [Viewport-Einstellungen](../../../interface/display-settings/viewport-settings.md)-Parametern angepasst werden.
