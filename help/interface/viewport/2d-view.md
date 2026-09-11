---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/interface/viewport/2d-view.html"
breadcrumb-title: ''
description: Lerne, wie du mit den 2D-Ansichten von Substance 3D Painter Texturen im UV-Raum anzeigen und bearbeiten kannst, um präzise Texturen zu malen.
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

In der 2D-Ansicht werden die Mesh-UV-Inseln des aktuell ausgewählten [Textursatzes](../texture-set/texture-set.md) angezeigt. Es ermöglicht, die Texturen vom Ebenenstapel zu sehen, sondern auch auf dem Mesh UV-Inseln zu Malen.

## Anzeigemodus

![](../../assets/display-mode-1.png)

Oben rechts im Viewport befindet sich das Dropdown-Menü für den Anzeigemodus. Mit diesem Steuerelement können Sie ändern, welche Informationen im Viewport angezeigt werden sollen. Es ermöglicht die Anzeige von Ein Kanal, Mesh-Map oder das endgültige Material Ergebnis mit Beleuchtung.

## Achse

![](../../assets/2d-axis.png)

Unten rechts im Viewport befinden sich die **Richtungsinformationen**, die die Achse der zweidimensionalen Achsen angeben. In dem Fall, wenn die 2D-Ansicht die Achsen U und V sind.

## UV-Kachel

![](../../assets/2d-view-button.png)

Neben dem **Anzeigemodus** befindet sich die Schaltfläche **Informationen zur UV-Kachel**, mit der Informationen zu UV-Kacheln ein- oder ausgeblendet werden können. Diese Schaltfläche ist bei regulären Projekten nicht sichtbar.

## Projekt-Workflow

Abhängig vom Workflow, der beim Erstellen eines Projekts definiert wurde, können die 2D-Ansichten anders aussehen und sich anders verhalten:

| *Projektarbeitsablauf* | *Verhalten* |
| --- | --- |
| **Standardprojekt** | Bei regulärem Projekt kann nur die UV mit dem UV-Bereich [0-1] angestrichen werden. Alles, was außerhalb dieses Bereichs liegt, ist sichtbar, aber nicht interaktiv.In diesem Beispiel können nur die UV-Inseln auf der linken Seite (mit hellgrauem Hintergrund) gemalt werden. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/2d-view-range-regular.jpg" width="500px"/></div> |
| **UV-Kachel-Projekt** | Beim UV-Kachel-Projekt ist jeder UV-Bereich eine neue Gruppe von Texturen, auf die gemalt werden kann. Die 2D-Ansicht wird ebenfalls als Raster angezeigt, um besser sehen zu können, wie jede Kachel organisiert ist. Jeder Kachel wird eine UDIM-Nummer zugewiesen. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/2d-view-range-uvtiles.jpg" width="500px"/></div> |
