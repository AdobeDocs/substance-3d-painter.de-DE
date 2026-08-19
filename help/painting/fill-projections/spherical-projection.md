---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/painting/fill-projections/spherical-projection.html"
breadcrumb-title: ''
description: In Substance 3D Painter kannst du mit sphärische Projektion Strukturen aus einer Kugel projizieren, um Strukturen um Objekte zu legen.
helpx_creative_field: ""
helpx_description: Painter > Painting > Fill projections > Spherical projection
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Sphärische Projektion
user-guide-description: ''
user-guide-title: ''
source-git-commit: 7e24e45387178db5efa813e64e4b86ac2ae2e5aa
workflow-type: tm+mt
source-wordcount: '855'
ht-degree: 2%

---


# Sphärische Projektion

![](../../assets/spherical-proj.jpg)

Mit der Sphärische Projektion &quot;Füllen&quot; können Bilder und Muster um ein Objekt projiziert werden. Es kann nützlich sein, auf runde Objekte zu projizieren oder Texturen in kreisförmige Muster zu verzerren.

## Eigenschaften

| Einstellung | Beschreibung |
| --- | --- |
| **Filtern** | Steuert, wie die Textur oder das Material gefiltert wird. Diese Einstellung kann sich darauf auswirken, wie die Textur aussieht, wenn sie mehrmals wiederholt wird. Wenn hohe Skalierungswerte mit einer anderen Filterung als der Standardeinstellung verwendet werden, kann das Ergebnis möglicherweise besser aussehen. Aktuelle Einstellungen verfügbar:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Bilinear `\|` HQ</strong> (Standard): Erweiterte bilineare Filterung, die bei hohen Kachelwerten die Qualität der Textur verbessern soll.</li><li data-preserve-html="true"><strong>Bilinear `\|` Sharp</strong>: Eine einfache bilineare Filterung glättet die Textur leicht, versucht aber, Details zu erhalten.</li><li data-preserve-html="true"><strong>Nächste</strong>: Keine Filterung, nützlich, wenn die bilineare Filterung zu einem verschwommenen Ergebnis führt und feine Details sprengt. Kann Aliasing in die Textur einführen.</li></ul> |
| **Abwicklung** | Lege fest, wie sich die Struktur in der Projektion wiederholt. Mögliche Werte sind:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Keine</strong>: die Textur wiederholt sich nicht. Alles, was außerhalb der Textur liegt, ist schwarz/transparent.</li><li data-preserve-html="true"><strong>Horizontal wiederholen</strong>: Die Textur wird nur horizontal wiederholt.</li><li data-preserve-html="true"><strong>Vertikal wiederholen</strong>: Die Textur wird nur vertikal wiederholt.</li><li data-preserve-html="true"><strong>Wiederholen</strong> (Standard): Die Textur wiederholt sich auf beiden Achsen.</li></ul> <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/spherical-repeat.jpg" width="500px"/></div> |
| **Formzuschnitt** | Legen Sie fest, ob die projizierte Textur außerhalb des Projektionsbereichs sichtbar sein soll. Mögliche Werte sind:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Projekt auf Form zugeschnitten</strong>: die Projektion ist innerhalb der Projektionsfläche begrenzt.</li><li data-preserve-html="true"><strong>Projektion erstreckt sich außerhalb von Form </strong> (Standard): die Projektion geht über die Projektionsfläche hinaus.</li></ul> <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r3-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/spherical-shape-crop.jpg" width="500px"/></div> |

### UV-Transformation

Die Einstellungen für die UV-Transformation steuern die Textur innerhalb der Projektion.

| *Einstellung* | *Beschreibung* |
| --- | --- |
| **Skalierung** | Definiere, wie oft die Struktur in der Projektion wiederholt werden soll. |
| **Drehung** | Steuere den Winkel der Struktur, die auf die Projektion angewendet wird. |
| **Offset** | Lege den Ursprung der projizierten Textur fest. Der Standardwert bedeutet, dass sich die Textur in der Mitte der Projektion befindet. |

### 3D-Projektionseinstellungen

Die 3D-Projektionseinstellungen steuern die Transformation der Projektion im 3D-Raum.

| Einstellung | Beschreibung |
| --- | --- |
| **Offset** | Position des Ursprungs der Projektion im 3D-Raum. Die Einheiten basieren auf dem Begrenzungsrahmen der gesamten Szene. 0 ist die Mitte dieser Box. |
| **Drehung** | Winkel in Grad, um die gesamte Projektion auf jeder Achse zu drehen. |
| **Skalierung** | Größe der gesamten Projektion auf jeder Achse. |

## Kontextabhängige Symbolleiste

Mehrere Einstellungen und Werkzeuge sind in der [Kontextsymbolleiste](../../interface/toolbars.md) am oberen Rand des Viewports verfügbar, die Steuerelemente für den Manipulator und die Projektion bereitstellen:

| Symbol | Name | Beschreibung |
| --- | --- | --- |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r1-column-c0_image" src="../../assets/icon-hide-manipulator.png" width="50px"/></div> | Manipulator anzeigen/ausblenden | Wenn diese Option aktiviert ist, ist der Manipulator im Viewport sichtbar und steuerbar. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r2-column-c0_image" src="../../assets/icon-manipulator-settings.png" width="50px"/></div> | Einstellungen für Manipulatoren | Dieses Menü enthält drei Einstellungen:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Manipulatorgröße</strong>: steuert, wie groß der Manipulator im Viewport ist.</li><li data-preserve-html="true"><strong>Rasterschritte</strong>: die Größe des Schritts bei der Übersetzung mit einer Einschränkung zu definieren.</li><li data-preserve-html="true"><strong>Winkelschritte</strong>: den Winkel des Schritts beim Drehen mit einer Bedingung definieren.</li></ul> |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r3-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-translate.png" width="50px"/></div> | Übersetzungs-Manipulator | Lassen Sie zu, dass die Projektion in der Szene entlang der Hauptachsen (X, Y, Z) verschoben wird. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r4-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-rotate.png" width="50px"/></div> | Rotationsmanipulator | Lassen Sie zu, dass die Projektion in der Szene entlang der Hauptachsen (X, Y, Z) gedreht wird. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r5-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-scale.png" width="50px"/></div> | Skalenmanipulator | Lassen Sie zu, dass die Projektion in der Szene entlang der Hauptachsen (X, Y, Z) skaliert wird. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r6-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-surface.png" width="50px"/></div> | Oberflächenmanipulator | Lassen Sie zu, dass die Projektion verschoben wird, indem Sie sie auf der 3D-Modelloberfläche ausrichten.  **Hinweis:** Dieser Manipulator ist nur für die Projektionstypen &quot;Planar&quot; und &quot;Verformen&quot; verfügbar. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r7-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-space.png" width="50px"/></div> | Manipulatorraum | Definieren Sie, in welchem Raum die Transformation durchgeführt wird. Mögliche Werte sind:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Lokaler Speicherplatz</strong>: -Achsen mit der aktuellen Transformation ausgerichtet.</li><li data-preserve-html="true"><strong>Weltraum</strong>: Die Achsen werden an der Szene ausgerichtet.</li></ul> |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r8-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-flip-x.png" width="50px"/></div> | Spiegeln auf X | Spiegeln Sie die Transformation an der X-Achse. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r9-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-flip-y.png" width="50px"/></div> | Spiegeln auf Y | Spiegeln Sie die Transformation an der Y-Achse. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r10-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-flip-z.png" width="50px"/></div> | Spiegeln auf Z | Spiegeln Sie die Transformation an der Z-Achse. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r11-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-reset.png" width="50px"/></div> | Umwandlung zurücksetzen | Stellen Sie den Standardzustand der Projektionstransformation wieder her. |

## Manipulator

Dieser Projektionsmanipulator ist nur im [3D-Viewport](../../interface/viewport/3d-view.md) verfügbar.

| Aktion | Tastaturbefehl | Beschreibung |
| --- | --- | --- |
| **Übersetzung** | Mausklick | Klicken Sie mit dem Translationsmanipulator auf die Achsen, um die Projektion zu verschieben:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Eine Achse</strong>: sich nur in eine Richtung der Projektion bewegen.</li><li data-preserve-html="true"><strong>Zwei Achsen</strong>: Verschieben Sie die Projektion auf den Plänen, die an den Achsen ausgerichtet sind.</li><li data-preserve-html="true"><strong>Drei Achsen</strong>: die Projektion in den Raum der Kamera zu bewegen (Plan gegenüber).</li></ul>   <table> <tr style="border: 0;"> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r1-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/3d-translate.gif" width="200px"/></div>  </td> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r1-column-c2_dynamic_grid_items_grid-cell1_position-par_image" src="../../assets/3d-translate-2axes.gif" width="200px"/></div>  </td> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r1-column-c2_dynamic_grid_items_grid-cell2_position-par_image" src="../../assets/3d-translate-3axes.gif" width="200px"/></div>  </td> </tr> </table> |
| **Einschränkung der Übersetzung** | UMSCHALT+Mausklick | Bewegen Sie die Projektion mit dem Translationsmanipulator entlang der ausgewählten Achsen, jedoch nur in bestimmten Intervallen (schrittweise Schritte). Die Größe des Intervalls wird über die Manipulatoreinstellungen festgelegt. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r2-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/3d-translate-step.gif" width="200px"/></div> |
| **Drehung** | Mausklick | Klicken Sie mit dem Drehungsmanipulator auf eine Achse, um die Projektion zu drehen. Klicken Sie zwischen die Achsen, um alle Achsen gleichzeitig zu drehen.   <table> <tr style="border: 0;"> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r3-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/3d-rotate.gif" width="200px"/></div>  </td> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r3-column-c2_dynamic_grid_items_grid-cell1_position-par_image" src="../../assets/3d-rotate-3axes.gif" width="200px"/></div>  </td> </tr> </table> |
| **Drehungseinschränkung** | UMSCHALT+Mausklick | Wenn du mit dem Drehungs-Manipulator auf eine Achse klickst, um die Projektion zu drehen, kannst du dies nur in bestimmten Intervallen tun. Die Stufe wird durch einen Winkel über die Manipulatoreinstellungen definiert. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r4-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/3d-rotate-step.gif" width="200px"/></div> |
| **Skalierung** | Mausklick | Wenn du mit dem Skalierungsmanipulator auf einen Achsgriff klickst, veränderst du die Größe der Projektion entlang der Achse.   <table> <tr style="border: 0;"> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r5-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/scale-one-axis.gif" width="200px"/></div>  </td> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r5-column-c2_dynamic_grid_items_grid-cell1_position-par_image" src="../../assets/scale-two-axis.gif" width="200px"/></div>  </td> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r5-column-c2_dynamic_grid_items_grid-cell2_position-par_image" src="../../assets/scale-3-axes.gif" width="200px"/></div>  </td> </tr> </table> |
| **Einschränkung der Skalierung** | UMSCHALT+Mausklick | Wenn du mit dem Skalierungsmanipulator auf einen Achsengriff klickst und dabei den Tastaturbefehl aufrechterhältst, wird die Größe der Projektion in Schritten angepasst. Die Schrittgröße ist die gleiche wie für den Übersetzungsmanipulator. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r6-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/scale-1-axis-constrained.gif" width="200px"/></div> |
| **Oberfläche** | Mausklick | Wenn du den Flächen-Manipulator aktivierst und über das 3D-Modell ziehst, wird es an der Oberfläche ausgerichtet. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r7-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/surface.gif" width="200px"/></div> **Hinweis:** Dieser Manipulator ist nur für die Projektionstypen **Planar** und **Warp** verfügbar. |
