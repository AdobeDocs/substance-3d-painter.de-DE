---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/painting/tool-list/paint-brush.html"
breadcrumb-title: ''
description: Verwende das Malen-Pinsel-Werkzeug in Substance 3D Painter, um Texturen mit anpassbaren Pinseleinstellungen direkt auf 3D-Modelle Malen.
helpx_creative_field: ""
helpx_description: Painter > Painting > Tool list > Paint brush
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Malen
user-guide-description: ''
user-guide-title: ''
source-git-commit: c20714f4cef21ccca0cdcd45dcdfd5ca6f4b96f2
workflow-type: tm+mt
source-wordcount: '1308'
ht-degree: 1%

---


# Malen

Das Malen-Werkzeug ist das Standardwerkzeug von Substance 3D Painter zum Anwenden von Farben und Material-Eigenschaften auf einen 3D-Mesh. Es verfügt über bestimmte Parameter, die über die [Eigenschaften](../../interface/properties.md) bearbeitet werden können.

Das Malen-Werkzeug simuliert Pinselstriche über verschiedene Verhaltensweisen und Einstellungen, um das Gefühl zu vermitteln, auf den 3D-Mesh gemalt zu werden.

## Symbolleiste

![](../../assets/paint-toolbar.png)

Die [Symbolleisten](../../interface/toolbars.md) zeigen die folgenden Tastaturbefehle an (siehe Erläuterung in den nächsten Abschnitten):

* Größe
* Fluss
* Konturdeckkraft
* Teilung

Es sind zusätzliche Tastaturbefehle verfügbar, die in einigen anderen Werkzeugen gleich sind:

* [Lazy Mouse](../lazy-mouse.md)
* [Symmetrie](../symmetry/symmetry.md)

## Vorschau

![](../../assets/brush-preview.png)

Am oberen Rand der [Eigenschaften](../../interface/properties.md) befinden sich die Pinsel- und Material-Vorschau. Sie können verwendet werden, um schnell einen Blick darauf zu werfen, wie das aktuelle Werkzeug eingerichtet ist.

| *Name* | *Beschreibung* |
| --- | --- |
| **Pinselvorschau** | In der Pinselvorschau wird basierend auf den Pinselparametern angezeigt, wie sich der Pinsel verhält. Sie können in die Vorschau klicken, um einen benutzerdefinierten Strich zu zeichnen.   <table> <tr style="border: 0;"> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/brush-preview-param.gif"/></div>  </td> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c1_dynamic_grid_items_grid-cell1_position-par_image" src="../../assets/brush-preview-draw.gif"/></div>  </td> </tr> </table>   **Hinweis:** Die Pinselvorschau unterstützt keinen Stift. |
| **Material-Vorschau** | Die Material-Vorschau zeigt die Eigenschaften des Materials an, das derzeit zum Malen verwendet wird. Sie können in die Vorschau klicken, um die Beleuchtung zu drehen und besser zu sehen, wie sich das Material vor dem Malen verhält.   <table> <tr style="border: 0;"> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/material-preview-lighting.gif"/></div>  </td> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_dynamic_grid_items_grid-cell1_position-par_image" src="../../assets/material-preview-properties-optim.gif"/></div>  </td> </tr> </table> |

## Pinsel

![](../../assets/brush-4.png)

Die Pinselparameter definieren das Aussehen des Pinselstrichs, wenn er auf dem 3D-Mesh ausgeführt wird.

>[!NOTE]
>
> Einige Parameter können bei Verwendung eines Grafiktabletts über den Stift-Druck eingestellt werden. Diese Informationen können auch in [Vorgaben](../presets/presets.md) gespeichert werden.\
> Klicken Sie auf die dedizierte Schaltfläche, um den Druck zu aktivieren oder zu deaktivieren :
> 
> ![](../../assets/pen-pressure.png)

| Name | Beschreibung |
| --- | --- |
| **Größe** | Bestimmt, wie groß die Stempel innerhalb eines Pinselstrichs sind. Die Pinselgröße ist relativ und kann je nach dem in definierten relativen Abstand geändert werden (siehe den Parameter &quot;Abstand der Ausrichtungsgröße&quot; unten). *Dieser Stift kann durch den Parameterdruck gesteuert werden.* |
| **Flow** | Intensität oder Deckkraft der einzelnen Stempel innerhalb des Pinselstrichs. *Dieser Stift kann durch den Parameterdruck gesteuert werden.* |
| **Konturdeckkraft** | Maximale globale Deckkraft eines Pinselstrichs. Im Gegensatz zum Parameter &quot;Fluss&quot; kann die Konturdeckkraft nicht über den Stift &quot;Druck&quot; gesteuert werden, da sie am Ende des Konturzeichnungsvorgangs angewendet wird.Differenz zwischen Fluss- und Konturdeckkraft :<ul data-preserve-html="true"><li data-preserve-html="true"><strong> Links </strong> : Fluss bei 50 %, Konturdeckkraft bei 100 %</li><li data-preserve-html="true"><strong> Rechts </strong> : Fluss bei 100 %, Konturdeckkraft 50 %</li></ul> <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r3-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/brush-combined.gif" width="500px"/></div> **Hinweis:** Es ist möglich, einen vorherigen Strich wie in der obigen Animation fortzusetzen, indem Sie den Tastaturbefehl &quot;A&quot; drücken. |
| **Abstand** | Abstand zwischen den einzelnen Stempeln eines Pinselstrichs. Kleine Werte ermöglichen durchgehende Linien, sind aber umfangreicher zu berechnen, da sie insgesamt viel mehr Stempel zeichnen. Hohe Werte ermöglichen es, Lücken zwischen den Stempeln zu schaffen, die für bestimmte Muster (wie Nägel auf Holz) besser geeignet sein können. |
| **Winkel** | Ausrichtung der Stempel innerhalb des Pinselstrichs Dies ist hilfreich, um das Alpha zu drehen, wenn es nicht richtig ausgerichtet ist. Kann mit dem Pfad folgen kombiniert werden. |
| **Pfad folgen** | Richtet die Stempel innerhalb des Pinselstrichs so aus, dass sie der Malrichtung folgen. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r6-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/follow-path-demo.png" width="400px"/></div> **Hinweis:** Um die Strichrichtung zu berechnen, vergleicht Substance 3D Painter den vorherigen Stempel mit dem aktuellen. Aus diesem Grund führt ein einzelner Klick auf den Malen bei aktivierter Option &quot;Pfad verfolgen&quot; zu keinen Ergebnissen. Mindestens zwei Stempel sind erforderlich, um einen Pinselstrich mit dieser Funktion Malen. |
| **Größe Jitter** | Wenden Sie innerhalb des Pinselstrichs einen zufälligen Größenwert pro Stempel an. Ein Wert von 0 bedeutet keine Zufälligkeit, ein Wert von 1 bedeutet volle Zufälligkeit. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r7-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/brush-size-3.png"/></div> |
| **Flow-Jitter** | Wenden Sie einen zufälligen Flusswert pro Stempel innerhalb des Pinselstrichs an. Ein Wert von 0 bedeutet keine Zufälligkeit, ein Wert von 1 bedeutet volle Zufälligkeit. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r8-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/brush-flow.png"/></div> |
| **Winkel-Jitter** | Wenden Sie einen zufälligen zusätzlichen Drehwinkel pro Stempel innerhalb des Pinselstrichs an. Ein Wert von 0 bedeutet keine Zufälligkeit, ein Wert von 1 bedeutet volle Zufälligkeit. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r9-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/brush-rotation.png"/></div> |
| **Positions-Jitter** | Wenden Sie einen zufälligen Positionsversatz pro Stempel innerhalb des Pinselstrichs an. Ein Wert von 0 bedeutet keine Zufälligkeit, ein Wert von 1 bedeutet volle Zufälligkeit. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r10-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/brush-position.png"/></div> |
| **Ausrichtung** | Legt fest, wie die Stempel innerhalb des Pinselstrichs auf die Oberfläche des 3D-Mesh projiziert/ausgerichtet werden. Die folgenden Werte sind verfügbar:<ul data-preserve-html="true"><li data-preserve-html="true"><strong> Kamera </strong> : Richten Sie den Stempel auf die Perspektive des Viewports aus</li><li data-preserve-html="true"><strong> Tangente `\|` Umbruch (Standard) </strong> : Richten Sie den Stempel so aus, dass er auf die 3D-Mesh-Oberfläche ausgerichtet ist. Der Stempel wird ebenfalls so verformt, dass er der Oberfläche entspricht.</li><li data-preserve-html="true"><strong> Tangente `\|` Planar </strong> :  Richten Sie den Stempel so aus, dass er auf die 3D-Mesh-Oberfläche ausgerichtet ist. Die Briefmarke wird Verblassen seine Grenze sind zu weit von der Oberfläche des 3D-Meshs. </li><li data-preserve-html="true"><strong> UV </strong> : Richten Sie den Stempel nach den 3D-Mesh-UVs aus.</li></ul> |
| **Rückseiten-Ausblendung** | Ermöglicht das Ignorieren von Flächen auf dem 3D-Mesh, die nicht mit dem Stempel ausgerichtet sind. Um zu berechnen, welche Teile des 3D-Mesh ignoriert werden sollen, schaut das Engine auf die Normalität an der Oberfläche des 3D-Mesh und vergleicht seinen Winkel mit dem definierten Wert. |
| **Speicherkapazität** | Steuert, in welchem relativen Abstand die Pinselgröße berechnet wird. Mögliche Werte sind:<ul data-preserve-html="true"><li data-preserve-html="true"><strong> Objekt (Standard) </strong> : Die Pinselgröße wird mit der 3D-Gittergröße synchronisiert. Das Verschieben der Kamera im Viewport wirkt sich auf die Größe aus, damit sie im Verhältnis zum 3D-Mesh bleibt.</li><li data-preserve-html="true"><strong> Viewport </strong> : Die Pinselgröße ist mit dem Viewport verknüpft. Die Änderung der Größe der Benutzeroberfläche wirkt sich auf die Pinselgröße aus. Das Bewegen der Kamera hat keine Auswirkungen.</li><li data-preserve-html="true"><strong> Textur </strong> : Die Pinselgröße ist mit der 2D-Viewport-Ebene des Zooms verknüpft.</li></ul> |

## Alpha

![](../../assets/alpha-1.png)

Das Alpha ist die Graustufenmaske, die auf jeden Stempel innerhalb des Pinselstrichs angewendet wird. Es kann sich um eine Substance-Datei oder eine Bitmap handeln.

>[!NOTE]
>
> Wenn einem Substance-Graf der Parameter &quot;Härte&quot; (Identifizierung) gelegt ist, kann er mit der Härte [Tastaturbefehle](../../interface/settings/shortcuts.md) gesteuert werden.

## Physik

![](../../assets/physics-1.png)

Mit den Eigenschaften unter &quot;Physik&quot; können Sie die Partikeln steuern, die beim Malen projiziert werden.

Standardmäßig sind die Eigenschaften &quot;Physik&quot; nicht verfügbar, können jedoch auf zwei Arten aktiviert werden:

* Durch Umschalten des Tools auf &quot;Physisch&quot; in den [Symbolleisten](../../interface/toolbars.md) (oder über den Tastatur-Tastaturbefehl).
* Durch Klicken auf eine Partikel-Pinselvorgabe im Fenster [Elemente](../../interface/assets/assets.md).

## Schablone

![](../../assets/stencil.png)

Die Schablone ist eine zusätzliche Graustufenmaske für den Pinselstrich. Im Gegensatz zu dem Alpha, das für jeden individuellen Stempel angewendet wird, ist die Schablone eine globale Maske, die aus der Sicht von [Viewport](../../interface/viewport/viewport.md) angewendet wird.

>[!NOTE]
>
> Sie können die Transformation der Schablone zurücksetzen, indem Sie die Taste **S** drücken und dann rechts oben auf dem Viewport auf die Schaltfläche **Zurücksetzen** klicken:
> 
> ![](../../assets/stencil-reset.png)

| *Modus* | *Viewport* |
| --- | --- |
| **Keine Ressource geladen** | Wenn keine Ressource geladen wird, hat die Schablone keine Auswirkungen. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r1-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/stencil-viewport-none.png" width="350px"/></div> **Hinweis:** Sie können die Ressourcenmaske vorübergehend deaktivieren, ohne die Schablone zu entfernen, indem Sie die [Tastaturbefehle](../../interface/settings/shortcuts.md) &quot;N&quot; drücken und beibehalten. |
| **Schablone verschieben** | Das Verschieben der Schablone kann durch Drücken der Taste **S** und Klicken und Ziehen mit der Schaltfläche **Mittlere Maustaste** erfolgen. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/stencil-move.gif" width="350px"/></div> |
| **Schablone drehen** | Das Drehen der Schablone kann durch Drücken der Taste **S** und Klicken und Ziehen mit der Schaltfläche **Linke Maustaste** erfolgen. Außerdem kann durch Drücken der **Umschalttaste** die Drehung alle **90 Grad** einrasten werden. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r3-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/stencil-rotate.gif" width="350px"/></div> |
| **Größe der Schablone ändern** | Sie können die Größe der Schablone ändern, indem Sie die Taste **S** drücken und mit der Schaltfläche **Rechte Maustaste** klicken und ziehen. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r4-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/stencil-resize.gif" width="350px"/></div> |

Die Einstellung für den Kachelmodus steuert, wie die Schablonenmaske über dem Viewport wiederholt wird (diese Einstellung wirkt sich auch auf die Texturierung aus):

| *Kachelmodus* | *Beschreibung* |
| --- | --- |
| **Keine Kachelung (Standard)** | Die Schablone wird nicht wiederholt. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table3_row-r1-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/stencil-viewport-notiling.png" width="350px"/></div> |
| **Horizontale Kachelung** | Wiederholen Sie die Schablonenmaske nur auf der horizontalen Achse. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table3_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/stencil-viewport-horizontal.png" width="350px"/></div> |
| **Vertikale Kachelung** | Wiederholen Sie die Schablonenmaske nur auf der vertikalen Achse. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table3_row-r3-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/stencil-viewport-vertical.png" width="350px"/></div> |
| **H- und V-Kachelung** | Wiederholen Sie die Schablone auf der horizontalen und der vertikalen Achse. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table3_row-r4-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/stencil-viewport-both.png" width="350px"/></div> |

## Material

![](../../assets/material.png)

Ein Material besteht aus mehreren Kanälen, wobei jeder Kanal bestimmte Eigenschaften beibehält. Die Kanalliste ist von den Kanälen abhängig, die in den [Kanaleinstellungen](../../interface/texture-set/texture-set-settings.md) definiert sind. Textursatz:

Mit der Schaltfläche **Materialmodi** können Sie ganz einfach eine Substance-Datei oder eine Vorgabe laden, um schnell mehrere Kanäle gleichzeitig zuzuweisen und zu bearbeiten.

Wenn Sie auf einen Kanal klicken, wird er ausgewählt oder die Auswahl wird aufgehoben. Wenn diese Option deaktiviert ist, kann die Kanaleigenschaft nicht geändert werden und wird während des Malvorgangs nicht verwendet.

![](../../assets/enable-channel.gif)
