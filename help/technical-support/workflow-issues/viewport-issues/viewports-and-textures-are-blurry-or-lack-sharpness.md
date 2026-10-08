---
breadcrumb-title: ""
description: Lerne, wie du in Substance 3D Painter unscharfe Viewport und Texturen korrigieren kannst, um eine gestochen scharfe Bildqualität zu gewährleisten.
title: Viewport und Texturen sind verschwommen oder nicht scharf
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 1%
---

# Viewport und Texturen sind verschwommen oder nicht scharf

Die Viewporte können aus verschiedenen Gründen verschwommen erscheinen.

## Einstellungen für HiDPI-Bildschirme (Retina)

Standardmäßig verkleinert Substance 3D Painter die Viewport-Auflösung auf HD-/Retina-Bildschirm, um die Leistung zu verbessern.

Dieses Verhalten kann in den [Haupteinstellungen](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/general-71008262.html) geändert werden, indem der **Parameter Skalierung des Viewports** geändert wird.

## Texturfilterung

Die Viewport verwenden Mipmaps und Textur-Filterungen, um [Dünn besetzte virtuelle Texturen](../../../features/sparse-virtual-textures.md) ein- und ausströmen zu können, um die Leistung zu verbessern. Dies kann in einigen Fällen zu verschwommenen Texturen führen.

Die Filterungen der Textur können im Fenster &quot;Anzeigeeinstellungen&quot; unter den [Parametereinstellungen](../../../interface/display-settings/viewport-settings.md)-Viewporten angepasst werden.
