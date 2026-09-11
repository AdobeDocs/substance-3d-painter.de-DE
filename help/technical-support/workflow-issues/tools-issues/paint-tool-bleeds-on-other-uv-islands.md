---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/workflow-issues/tools-issues/paint-tool-bleeds-on-other-uv-islands.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie das Malen-Werkzeug über UV-Inseln hinweg in Substance 3D Painter ineinander verlaufen lassen können, um saubere Texturen zu erhalten.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > Tools Issues > Paint Tool bleeds on other UV islands
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Malen Tool-Anschnitte auf anderen UV-Inseln
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '126'
ht-degree: 0%

---


# Malen Tool-Anschnitte auf anderen UV-Inseln

Einige Standardverhalten des [Malen-Tools](../../../features/effects/paint.md) wirken in bestimmten Situationen möglicherweise nicht intuitiv. Substance 3D Painter ist eine Anwendung, die hauptsächlich im 3D-Raum arbeitet. Das gilt auch für das Malen. Die Standardeinstellung für den Malen-Pinsel ist der Versuch, beim Malen nahtlos über UVs hinweg zu arbeiten. Aus diesem Grund können bei der Interaktion mit den 2D-Ansichten einige Ergebnisse unerwartet erscheinen.

Um das Anbluten anderer UV-Inseln beim Malen in der 2D-Ansicht zu vermeiden, ändern Sie einfach die Einstellung **Ausrichtung** in den Werkzeugparametern:

| *Ausrichtungsmodus* | *Vorschau* |
| --- | --- |
| **Tangenten-Wrap** | <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../../assets/paint-mode-tangent-optim.gif"/></div> |
| **UV** | <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../../assets/paint-mode-uv.gif" width="450px"/></div> |
