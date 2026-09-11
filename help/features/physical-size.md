---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/physical-size.html"
breadcrumb-title: ''
description: Erfahre, wie du in Substance 3D Painter die Physische Größe festlegst, um realistische Abmessungen für eine präzise Skalierung der Textur festzulegen.
helpx_creative_field: ""
helpx_description: Painter > Features > Physical size
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Physische Größe
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 2%

---


# Physische Größe

![](../assets/banner-physicalsize-2.png)

Die Physische Größe ist eine Eigenschaft innerhalb von Substance-Materialien, die ihre tatsächliche Größe definiert. Sie kann verwendet werden, um die Größe und das Aussehen von Materialien über 3D-Oberflächen genau abzustimmen. Painter verwendet Zentimeter als interne Standardeinheit.

Wenn Sie Physische Größe verwenden möchten, wenden Sie ein Material mit dieser Eigenschaft an, das einen anderen Wert als 0,0,0 hat, und aktivieren Sie dann den Physische Größe-Modus in Füllebene (oder Effekt) unter UV-Transformation > Skalieren.

Weitere Informationen finden Sie unter:

* <b>Parameter für Physische Größe</b> in [Projektionen füllen](../painting/fill-projections/fill-projections.md)
* <b>Raster</b>-Parameter in [Viewport-Einstellungen](../interface/display-settings/viewport-settings.md)
* <b>Versatz basiert auf Physische Größe</b> in [Shader-Einstellungen](../interface/shader-settings/shader-settings.md)

>[!NOTE]
>
> * Ab Painter Version 8.3 ist Physische Größe für alle Arten von Projektionen verfügbar.
> * Die meisten Importformate geben die Meshdatei an, die während der Erstellung des Meshs verwendet wird. Diese Maßeinheit wird beim Importieren automatisch in Zentimeter konvertiert.
> * Einige Formate, z. B. .obj, verfügen nicht über Einheitsinformationen. Wenn ein Projekt also mit einem .obj-Mesh erstellt wird, wird es standardmäßig ohne Konvertierungen in Zentimetern gemessen.
