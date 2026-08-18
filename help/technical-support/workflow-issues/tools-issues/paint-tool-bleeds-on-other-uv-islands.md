---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/technical-support/workflow-issues/tools-issues/paint-tool-bleeds-on-other-uv-islands.html"
breadcrumb-title: ''
description: Hier erfahren Sie, wie Sie in Substance 3D Painter die Anschnitte von Malwerkzeugen über UV-Inseln hinweg korrigieren, um saubere Strukturgrenzen zu erhalten.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > Tools Issues > Paint Tool bleeds on other UV islands
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Anschnitt mit dem Malwerkzeug auf anderen UV-Inseln
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '126'
ht-degree: 0%

---


# Anschnitt mit dem Malwerkzeug auf anderen UV-Inseln

Einige Standardverhalten des [Malwerkzeugs](../../../features/effects/paint.md) wirken in bestimmten Situationen möglicherweise nicht intuitiv. Substance 3D Painter ist eine Anwendung, die hauptsächlich im 3D-Raum arbeitet. Das gilt auch für das Malen. Die Standardeinstellung für den Pinsel ist der Versuch, beim Malen über UVs hinweg nahtlos zu arbeiten. Aus diesem Grund können bei der Interaktion mit der 2D-Ansicht einige Ergebnisse unerwartet erscheinen.

Um beim Malen in der 2D-Ansicht das Anlaufen anderer UV-Inseln zu verhindern, ändern Sie einfach die Einstellung **Ausrichtung** in den Werkzeugparametern:

| *Ausrichtungsmodus* | *Vorschau* |
| --- | --- |
| **Tangentenumbruch** | <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../../assets/paint-mode-tangent-optim.gif"/></div> |
| **UV** | <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../../assets/paint-mode-uv.gif" width="450px"/></div> |
