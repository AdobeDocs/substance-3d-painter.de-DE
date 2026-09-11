---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/interface/layer-stack.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie den Ebenenstapel in Substance 3D Painter verwenden, um mehrere Texturen-Malebenen zu organisieren und zu verwalten.
helpx_creative_field: ""
helpx_description: Painter > Interface > Layer stack
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Ebenenstapel
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '615'
ht-degree: 5%

---


# Ebenenstapel

![](../../assets/layer-stack.png)

Mit dem **Ebenenstapel** können Sie die Ebenen eines Textursatzes bearbeiten. Eine Ebene enthält die Bilder und Effekte, mit denen die Textur auf das 3D-Objekt in der Szene erstellt wird. Sie können Ebenen ein- und ausblenden, in Ordner einfügen und ihre Deckkraft und Füllmethode ändern.

Weitere Informationen finden Sie auf den folgenden Seiten :

* [Erstellen von Ebenen](creating-layers.md)
* [Verwalten von Ebenen](managing-layers.md)
* [Maskierung und Effekte](masking-and-effects.md)
* [Füllmethoden](blending-modes.md)
* [Ebeneninstanzierung](layer-instancing.md)
* [Geometriemaske](geometry-mask.md)

## Überblick

Im Ebenenstapel werden Ebenen mit einer bestimmten Hierarchie angezeigt: Wenn die Ebene am unteren Rand zuerst auf dem Mesh gezeichnet wird, folgt die Ebene darüber. Daher ist die Ebene oben im Stapel das letzte Element, während die Ebene ganz unten das erste Element ist. Dasselbe Prinzip gilt für Ordner, der Inhalt des Ordners hat jedoch Priorität. Das bedeutet, dass der Inhalt eines Ordners vor den Ebenen verarbeitet wird, die sich auf derselben Ebene befinden.

**Allgemeine Eigenschaften:**

* Jede Ebene ist **mehrere Kanäle**.
* Das Malwerkzeug zeichnet **auf allen entsprechenden Kanälen**, abhängig von den Materialeinstellungen (der Kanal, den Sie derzeit im Ebenenstapel anzeigen, hat keine Auswirkungen).
* Jede Ebene verfügt über einen **Mischmodus** und eine **Deckkraft** pro Kanal (Sie können über das Dropdown-Menü oben links zwischen den Kanälen wechseln).

**Ebenentypen :**

* **Ebene** malen: Diese Ebenenart kann mit Pinseln und Partikeln bemalt werden.
* **Füllebene** : Diese Ebene kann nicht aufgemalt werden. Sie können stattdessen ein Material in diese Ebene laden, um die Kanäle auszufüllen. (Du kannst die Transformation auch bearbeiten, um das Material beispielsweise zu wiederholen.)
* **Ordner** : Dieser Ebenentyp enthält nur andere Ebenen, er wird hauptsächlich zum Organisieren des Ebenenstapels verwendet

Auf jeder Ebene können Sie **eine Maske hinzufügen**, mit der der Inhalt nur auf bestimmte Teile der Kanäle des aktuellen Textursatzes angewendet werden kann.\
Sie können entweder manuell (in Graustufen mit einem Malen) auf die Maske klicken oder Filter und Substanzen verwenden, um dynamischere/prozeduralere Ergebnisse zu erzielen.

## Ansichtsmodus

![](../../assets/switch-viewmode-optim.gif)

Die obere linke Dropdown-Liste des Ebenenstapels steuert den Ansichtsmodus des Ebenenstapels. Da eine Ebene mehrere Kanäle abdecken kann, ist es nicht möglich, alle diese Eigenschaften auf einmal anzuzeigen. Daher kann der Ansichtsmodus verwendet werden, um den aktuellen Anzeigekontext zu definieren. Wenn Sie diese Dropdown-Liste verwenden, können Sie festlegen, welche Kanäle in den Ebenen-Miniaturansichten angezeigt werden sollen, sowie den Mischmodus und die Deckkraft nur für diesen Kanal steuern.

Die Liste in dieser Dropdown-Liste basiert auf der Kanalliste, die in den [Kanaleinstellungen](../texture-set/texture-set-settings.md) des Textursatzes verfügbar ist.

## Aktionen

![](../../assets/image2020-9-30-12-2-13.png)

Die obere rechte Liste von Symbolen sind die allgemeinen Aktionen, die im Ebenenstapel ausgeführt werden können:

| Aktion | Beschreibung |
| --- | --- |
| Effekt hinzufügen <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-effect.png"/></div> | Erstelle einen neuen Effekt, und füge ihn zur ausgewählten Ebene hinzu. Weitere Informationen zu Effekten finden Sie auf den [dedizierten Seiten](../../features/effects/effects.md). |
| Maske erstellen <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-mask.png"/></div> | Öffnen Sie das Menü &quot;Maskenaktion&quot;, das die folgenden Elemente enthält:<ul data-preserve-html="true"><li data-preserve-html="true">Weiße Maske hinzufügen</li><li data-preserve-html="true">Schwarze Maske hinzufügen</li><li data-preserve-html="true">Bitmap-Maske hinzufügen</li><li data-preserve-html="true">Maske mit Farbauswahl hinzufügen</li><li data-preserve-html="true">Maske mit Höhenkombination hinzufügen</li></ul> |
| Neue Malebene erstellen <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r3-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/image2020-9-30-11-52-41.png"/></div> | Erstelle eine neue Farb-Ebene über der aktuell ausgewählten Ebene. |
| Neue Füllebene erstellen <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r4-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/image2020-9-30-12-0-49.png"/></div> | Erstellen Sie eine neue [Füllebene](../../painting/fill-projections/fill-projections.md) über der aktuell ausgewählten. |
| Neue Intelligente Materialien hinzufügen <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r5-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-smartmat.png"/></div> | Fügt ein neues Intelligente Material über der aktuell ausgewählten Ebene ein.Wenn Sie auf diese Schaltfläche klicken, wird ein Mini-Regal geöffnet, um die Liste der in den aktuellen [Elementen](../../interface/assets/assets.md) verfügbaren Intelligente Material zu durchsuchen. |
| Neuen Ordner hinzufügen <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r6-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/image2020-9-30-12-1-13.png"/></div> | Erstellen Sie einen neuen leeren Ordner über der aktuell ausgewählten Ebene. |
| Ebene löschen <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r7-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-trash.png"/></div> | Löschen Sie das aktuell ausgewählte Element (Ebene, Ordner oder Effekt). |
