---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/interface/viewport/2d-view.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie die 2D-Ansicht in Substance 3D Painter verwenden, um Texturen im UV-Raum anzuzeigen und zu bearbeiten und so präzise Strukturen zu malen.
helpx_creative_field: ""
helpx_description: Painter > Interface > Viewport > 2D view
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 2D-Ansicht
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 1%

---


# 2D-Ansicht

![](../../assets/2d-view.jpg){width="450px"}

Die 2D-Ansicht zeigt die Gitteransicht aus dem aktuell ausgewählten [Textursatz](../texture-set/texture-set.md) an. Die UV-Inseln werden in der 2D-Ansicht angezeigt. Du kannst die Strukturen des Ebenenstapels sehen, aber auch die Gitter-UV-Inseln aufmalen.

## Anzeigemodus

![](../../assets/display-mode-1.png)

Oben rechts im Viewport befindet sich das Dropdown-Menü für den Anzeigemodus. Mit diesem Steuerelement können Sie ändern, welche Informationen im Viewport angezeigt werden sollen. Es ermöglicht die Anzeige einzelner Kanäle, Mesh-Maps oder des endgültigen Materialergebnisses mit Beleuchtung.

## Achseninformationen

![](../../assets/2d-axis.png)

Unten rechts im Viewport befindet sich die **Achseninformation**, die die Richtung der zweidimensionalen Achsen angibt. In der 2D-Ansicht sind die Achsen U und V.

## Informationen zur UV-Kachel

![](../../assets/2d-view-button.png)

Neben dem **Anzeigemodus** befindet sich die Schaltfläche **UV-Kachelinformationen**, mit der Informationen zu UV-Kacheln ein- bzw. ausgeblendet werden können. Diese Schaltfläche ist bei regulären Projekten nicht sichtbar.

## Projekt-Workflow

Abhängig vom Workflow, der beim Erstellen eines Projekts definiert wurde, kann die 2D-Ansicht anders aussehen und sich anders verhalten:

| *Projektarbeitsablauf* | *Verhalten* |
| --- | --- |
| **Standardprojekt** | Bei regulärem Projekt kann nur die UV mit dem UV-Bereich [0-1] angestrichen werden. Alles, was außerhalb dieses Bereichs liegt, ist sichtbar, aber nicht interaktiv.In diesem Beispiel können nur die UV-Inseln auf der linken Seite (mit hellgrauem Hintergrund) gemalt werden. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/2d-view-range-regular.jpg" width="500px"/></div> |
| **UV-Kachelprojekt** | Mit dem UV Tile-Projekt ist jeder UV-Bereich ein neuer Satz von Texturen, die aufgemalt werden können. Die 2D-Ansicht wird ebenfalls als Raster angezeigt, um die Anordnung der einzelnen Kacheln zu verdeutlichen. Jeder Kachel wird eine UDIM-Nummer zugewiesen. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/2d-view-range-uvtiles.jpg" width="500px"/></div> |
