---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/interface/layer-stack/geometry-mask.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie in Substance 3D Painter mithilfe von Geometriemasken Ebenen auf der Grundlage von Mesh-Geometrie und Oberflächeneigenschaften maskieren.
helpx_creative_field: ""
helpx_description: Painter > Interface > Layer stack > Geometry mask
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Geometriemaske
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '736'
ht-degree: 1%

---


# Geometriemaske

![](../../assets/geometry-mask.png)\
Die Geometriemaske ist eine sekundäre Maske auf Ebenen, mit der eine Ebene auf der Grundlage der 3D-Modellgeometrie des zugehörigen Textursatzes maskiert werden kann. Es kann nach Mesh-Namen oder UV-Kacheln maskiert werden.

## Überblick

Die Maske &quot;Geometrie&quot; legt fest, auf welchen Teil des 3D-Modells die Ebene über eine Einschluss-/Ausschlussliste angewendet werden soll.

Die Geometriemaske ist ein nützliches Werkzeug, um schnell große Teile der 3D-Modellgeometrie zu verwerfen. Es bietet verschiedene Vorteile für die Malen-Maske:

* Es ist in der Regel schneller einzurichten und mit Viewport-Auswahlmodi zu verwenden.
* Es bietet eine bessere Leistung, da die Geometrie bei der Erzeugung der Texturen vollständig verworfen werden kann.
* Es ist nicht-destruktiv und wird aktualisiert, wenn sich das 3D-Modell nach einem erneuten Import ändert.
* Es erlaubt das Malen von Geometrie, die sich unter maskierter Geometrie befindet, und das Malen von verborgenen Teilen.
* Wie beim Malen einer Maske kann die Geometriemaske auf eine Gruppe angewendet werden, um mehrere Ebenen gleichzeitig zu beeinflussen.

### Symbolstatus

Das Symbol für die Geometriemaske kann anzeigen, in welchem Zustand es sich befindet:

| Symbol | Beschreibung |
| --- | --- |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/geo-mask-icon-default.png"/></div> | Es wurde keine Geometrie ausgeschlossen. Die Ebene wird auf den gesamten Mesh des zugehörigen Textursatzes angewendet. Dies ist der Standardstatus aller neuen Ebenen und Ordner. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/geo-mask-icon-selection.png"/></div> | Ein oder mehrere Mesh-Namen wurden ausgeschlossen. Die Zahl gibt die Anzahl der verbleibenden Elemente an, auf die sich die Ebene auswirkt. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r3-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/geo-mask-icon-uvtiles.png"/></div> | Eine oder mehrere UV-Kacheln wurden ausgeschlossen. Die Zahl gibt die Anzahl der verbleibenden Elemente an, auf die sich die Ebene auswirkt. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r4-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/geo-mask-icon-empty.png"/></div> | Es werden keine Mesh-Namen angegeben. Die Ebene hat keine Auswirkungen. |

## Bearbeiten der Geometriemaske

Um die Geometriemaske einer bestimmten Ebene zu ändern, klicken Sie einfach auf das entsprechende Symbol. Um den Bearbeitungsmodus zu beenden, klicken Sie einfach auf einen anderen Teil der Ebene, z. B. auf den Inhalt oder die Malen-Maske:

![](../../assets/geo-mask-editing.gif)

### Maskierungstypen

Die Geometriemaske unterstützt zwei Arten der Maskierung:

| Typ | Beschreibung |
| --- | --- |
| **UV-Kacheln** | Die Maskierung erfolgt durch die Angabe der UV-Kachel (UDIM)-Nummer. Dies ist die leistungsstärkste Methode, die es ermöglicht, eine Textur vollständig von der Berechnung zu verwerfen. |
| **Mesh-Namen** | Zum Maskieren wird festgelegt, welcher Unter-Mesh in das 3D-Modell aufgenommen werden soll. Die Geometrie wird nach dem Namen des Meshs gruppiert. |

### Ebenenstapel-Aktionen

![](../../assets/geo-mask-actions.png)

Der Maskenzustand &quot;Geometrie&quot; kann direkt vom Ebenenstapel aus durch einen Rechtsklick auf das Symbol schnell verändert werden.

Es bietet die folgenden Aktionen:

| Aktion | Beschreibung |
| --- | --- |
| **Geometriemaske kopieren** | Kopiere den Typ und die Auswahl der Geometriemaske der angegebenen Ebene. |
| **In Geometriemaske einfügen.** | Fügen Sie die zuvor kopierten Geometrie-Maskeneigenschaften ein. |
| **Alle einschließen** | Markieren Sie alle Elemente der angegebenen Maske als ausgewählt. |
| **Alle ausschließen** | Markieren Sie alle Elemente der angegebenen Maske als &quot;Deaktiviert&quot;. |

## Malen durch maskierte Geometrie

Wenn Teile der Geometrie ausgeschlossen wurden, können diese im Viewport ausgeblendet werden. Dies ermöglicht das Malen auf der Geometrie, die zuvor darunter lag und nicht zugänglich war.

Um die ausgeschlossene Geometrie auszublenden, verwenden Sie die Schaltfläche oben im Viewport in der Kontextsymbolleiste:

![](../../assets/hide-excluded-geo-button.png)

Im folgenden Beispiel wurde das 3D-Modell in zwei Objekte aufgeteilt: ein oberes und unteres Teil. Standardmäßig kollidieren Pinselstriche mit allen Objekten. Durch den Ausschluss des Oberteils ist es nun möglich, ausschließlich auf dem Unterteil zu Malen.

>[!NOTE]
>
> Die Ein-/Ausschlussliste der Geometriemaske ist dynamisch. Wenn Sie ihren Status ändern, wird eine neue Berechnung der Pinselstriche in der Ebene ausgelöst. Auf diese Weise können Sie die Maskierung anpassen, ohne die Pinselstriche zu verlieren, wenn Sie einen Mesh mit neuen UV-Kacheln erneut importieren oder wenn sich die Namen der Mesh geändert haben. Es bedeutet aber auch, dass Pinselstriche nicht Baking geführt werden, sodass jede Veränderung der Geometriemaske danach zu einer fehlerhaften Projektion der Pinselstriche führen kann.

| Visuell | Beschreibung |
| --- | --- |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r1-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/no-geo-excluded.jpg" width="420px"/></div> | Es wurde keine Geometrie in der Geometriemaske ausgeschlossen. Die Malebene, auf der der weiße Pinselstrich durchgeführt wurde, kollidiert mit der gesamten Geometrie.Die Schaltfläche **Ausgeschlossene Geometrie ausblenden** ist deaktiviert. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r2-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/geo-excluded-hidden.jpg" width="420px"/></div> | Der obere Teil wurde in der Geometriemaske ausgeschlossen, und der weiße Pinselstrich kollidiert nur mit dem unteren Teil der Geometrie.Die Schaltfläche **Ausgeschlossene Geometrie ausblenden** ist aktiviert. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r3-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/geo-excluded-visible.jpg" width="420px"/></div> | Der obere Teil wurde in der Geometriemaske ausgeschlossen, und der weiße Pinselstrich kollidiert nur mit dem unteren Teil der Geometrie.Die Schaltfläche **Ausgeschlossene Geometrie ausblenden** ist deaktiviert. |
