---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/painting/fill-projections/warp-projection.html"
breadcrumb-title: ''
description: Nutze die Verkrümmungsprojektion in Substance 3D Painter, um Texturen mit Verzerrung-Effekten für kreatives Texturmalen zu projektieren.
helpx_creative_field: ""
helpx_description: Painter > Painting > Fill projections > Warp projection
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Verkrümmungsprojektion
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '1859'
ht-degree: 2%

---


# Verkrümmungsprojektion

![](../../assets/proj-warp.jpg)

Bei der Verkrümmen-Projektion der Fläche handelt es sich um eine 3D-Projektion, mit der sich eine Textur durch Bearbeiten der Punkte eines Rasters verformen lässt. Es kann verwendet werden, um Muster und Logo auf einer nicht ebenen Oberfläche einzupassen.

## Schnelles Setup

Es ist möglich, schnell eine Ebene mit der Verkrümmungsprojektion einzurichten, indem eine Ressource per Drag &amp; Drop aus dem Fenster [Elemente](../../interface/assets/assets.md) in das Gitter gezogen wird. Wenn Sie die Maustaste loslassen, öffnet sich ein Menü, in dem Sie wählen können, in welchem Kanal die Ressource zugewiesen werden soll.

Kompatible Ressourcentypen sind:

* **Alpha**
* **Procedural**
* **Struktur**
* **Material** (ALT-Taste erforderlich)

![](../../assets/drop-viewport-warp.gif)

## Eigenschaften

| Einstellung | Beschreibung |
| --- | --- |
| **Filtern** | Steuert, wie die Textur oder das Material gefiltert wird. Diese Einstellung kann sich darauf auswirken, wie die Textur aussieht, wenn sie mehrmals wiederholt wird. Wenn hohe Skalierungswerte mit einer anderen Filterung als der Standardeinstellung verwendet werden, kann das Ergebnis möglicherweise besser aussehen. Aktuelle Einstellungen verfügbar:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Bilinear | HQ</strong> (Standard): Erweiterte bilineare Filterung, die bei hohen Kachelwerten die Qualität der Textur verbessern soll.</li><li data-preserve-html="true"><strong>Bilinear | Sharp</strong>: Eine einfache bilineare Filterung glättet die Textur leicht, versucht aber, Details zu erhalten.</li><li data-preserve-html="true"><strong>Nächste</strong>: Keine Filterung, nützlich, wenn die bilineare Filterung zu einem verschwommenen Ergebnis führt und feine Details sprengt. Kann Aliasing in die Textur einführen.</li></ul> |
| **Abwicklung** | Lege fest, wie sich die Struktur in der Projektion wiederholt. Mögliche Werte sind:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Keine</strong>: die Textur wiederholt sich nicht. Alles, was außerhalb der Textur liegt, ist schwarz/transparent.</li><li data-preserve-html="true"><strong>Horizontal wiederholen</strong>: Die Textur wird nur horizontal wiederholt.</li><li data-preserve-html="true"><strong>Vertikal wiederholen</strong>: Die Textur wird nur vertikal wiederholt.</li><li data-preserve-html="true"><strong>Wiederholen</strong> (Standard): Die Textur wiederholt sich auf beiden Achsen.</li></ul> |
| **Formzuschnitt** | Legen Sie fest, ob die projizierte Textur außerhalb des Projektionsbereichs sichtbar sein soll. Mögliche Werte sind:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Projekt auf Form zugeschnitten</strong>: die Projektion ist innerhalb der Projektionsfläche begrenzt.</li><li data-preserve-html="true"><strong>Projektion erstreckt sich außerhalb von Form </strong> (Standard): die Projektion geht über die Projektionsfläche hinaus.</li></ul> <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r3-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/warp-extend.jpg" width="500px"/></div> |
| **Tiefe der Projektion** | Legen Sie fest, wie weit die Projektion entlang der Z-Achse geht. Diese Einstellung hilft beim Erreichen der Gitteroberfläche, wenn der Gitterpunkt oder die Projektionsebene zu weit entfernt ist.Die grünen Pfeile geben die Richtung und den Abstand der Projektion für jeden Punkt des Rasters an. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r4-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/warp-depth.gif"/></div> **Warnung:** Ein hoher Wert kann die Leistung stark beeinträchtigen. Es wird empfohlen, diesen Parameter so niedrig wie möglich zu halten. |
| **Tiefe ausblenden** | Lassen Sie die Projektion entsprechend der Entfernung verblassen. Ein Parameter ist verfügbar:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Härte</strong>: steuert, wie hart oder weich der Überblendungseffekt ist.</li></ul> <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r5-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/warp-hardness.gif"/></div> |

### UV-Transformation

Die Einstellungen für die UV-Transformation steuern die Textur/das Material innerhalb der Projektion.

<table data-preserve-html="true" style="width: 100.0%;"><colgroup> <col style="width: 40.0%;"/> <col style="width: 20.0%;"/> <col style="width: 40.0%;"/> </colgroup><tbody><tr><th>Skalierungsmodus</th><th>Einstellung</th><th>Beschreibung</th></tr><tr><td><p><strong>Kacheln</strong> (Standard)<strong> <br/></strong></p><p>Ermöglicht die manuelle Einstellung des sich wiederholenden Betrags für die aktuelle Textur.</p></td><td><strong>Wiederholen</strong></td><td>Steuert, wie oft die Textur wiederholt wird.</td></tr><tr><td rowspan="2"><br/><br/></td><td colspan="1"><strong>Drehung</strong></td><td colspan="1">Steuert den Winkel, in dem die Textur auf das Gitter projiziert wird.</td></tr><tr><td colspan="1"><strong>Versatz</strong></td><td colspan="1">Steuert, von wo aus die Textur projiziert wird. Der Standardwert bedeutet, dass sich der Mittelpunkt der Textur in der Mitte der UVs des Gitters befindet.</td></tr><tr><th colspan="1"><br/></th><th colspan="1"><br/></th><th colspan="1"><br/></th></tr><tr><td rowspan="4"><p><strong>Physische Größe</strong></p><p>Die Textur wird automatisch an die Maschenweite und die eingebettete Physische Größe angepasst. Die richtige Physische Größe wird anhand der Längen- und Breitenwerte (X- und Y-Werte) berechnet. Die Z-Messung wird nicht berücksichtigt.</p><p>(Weitere Informationen finden Sie auf der speziellen [Dokumentationsseite](https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/features/physical-size))</p></td><td><strong>Benutzerdefinierte Größe</strong></td><td><p>Wenn diese Option aktiviert ist, können Sie eine Physische Größe manuell eingeben und die von einem Asset bereitgestellte Version überschreiben.</p><p>Sie wird automatisch ausgewählt, wenn keine Physische Größe erkannt wird oder wenn mehrere Assets mit unterschiedlichen Physische Größen innerhalb derselben Ebene/desselben Effekts verwendet werden.</p></td></tr><tr><td colspan="1"><strong>Größe (cm)</strong></td><td colspan="1">Eingebettete Physische Größen werden in Zentimetern angegeben. Es ist möglich, mit einer Gitterdatei zu arbeiten, die mit unterschiedlichen Maßeinheiten erstellt wurde. Die Proportionen bleiben dabei erhalten. Die Elementgröße wird derzeit jedoch nur in Zentimetern angezeigt.</td></tr><tr><td colspan="1"><strong>Drehung</strong></td><td colspan="1">Steuert den Winkel, in dem die Textur auf das Gitter projiziert wird.</td></tr><tr><td colspan="1"><strong>Versatz</strong></td><td colspan="1"><p>Steuert, von wo aus die Textur projiziert wird. Der Standardwert bedeutet, dass sich der Mittelpunkt der Textur in der Mitte der UVs des Gitters befindet.</p></td></tr></tbody></table>

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
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r1-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-hide-manipulator.png" width="50px"/></div> | Manipulator anzeigen/ausblenden | Wenn diese Option aktiviert ist, ist der Manipulator im Viewport sichtbar und steuerbar, um die Projektionstransformation oder die Rasterpunkte zu bearbeiten. Wenn diese Option deaktiviert ist, sind sowohl der Manipulator als auch das Raster ausgeblendet. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r2-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-manipulator-settings.png" width="50px"/></div> | Einstellungen für Manipulatoren | Dieses Menü enthält drei Einstellungen:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Manipulatorgröße</strong>: steuert, wie groß der Manipulator im Viewport ist.</li><li data-preserve-html="true"><strong>Rasterschritte</strong>: die Größe des Schritts bei der Übersetzung mit einer Einschränkung zu definieren.</li><li data-preserve-html="true"><strong>Winkelschritte</strong>: den Winkel des Schritts beim Drehen mit einer Bedingung definieren.</li></ul> |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r3-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-warp-tools.png" width="50px"/></div> | Menü &quot;Warp Edition&quot; | Dieses Menü enthält fünf Aktionen:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Transformationsverkrümmung</strong>: die Verkrümmungstransformation zu bearbeiten. Erlaubt die Bearbeitung der globalen Rasterposition, Drehung und Skalierung.</li><li data-preserve-html="true"><strong>Eckpunkte bearbeiten</strong>: die Punkte des Verkrümmungsrasters einzeln (oder in der Gruppe) bearbeiten.</li><li data-preserve-html="true"><strong>Verzerrung in Querrichtung aufteilen</strong>: starte das Krümmungs-Werkzeug, um eine neue Rasterteilung sowohl horizontal als auch vertikal einzufügen.</li><li data-preserve-html="true"><strong>Verzerrung horizontal teilen</strong>: starte das Krümmungs-Werkzeug, um eine neue Rasterteilung horizontal einzufügen.</li><li data-preserve-html="true"><strong>Vertikale Verformung teilen</strong>: starte das Krümmungs-Werkzeug, um eine neue Rasterteilung vertikal einzufügen.</li></ul> |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r4-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-warp-setting.png" width="50px"/></div> | Einstellungen für Verkrümmungsprojektion | In diesem Menü werden Einstellungen neu gruppiert, die sich nur auf die aktuelle Verkrümmungsprojektion auswirken:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Zeile und Spalten</strong>: geben die Anzahl der Trennflächen an, die das Verkrümmungsraster hat. Diese Einstellung kann nur bearbeitet werden, wenn keine Punkte des Rasters geändert wurden.</li><li data-preserve-html="true"><strong>Handle-Größe</strong>: die Größe der Rasterpunkte im Modus <strong>Eckpunkte bearbeiten</strong> definieren.</li><li data-preserve-html="true"><strong>Rasterfarbe</strong>: definieren die Farbe der Verzerrungsrasterlinien.</li></ul> |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r5-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-lock-tangent.png" width="50px"/></div> | Automatische Tangenten | Wenn diese Option aktiviert ist, richten Sie die Tangenten eines Punkts automatisch an den benachbarten Punkten aus, wenn sie verschoben werden. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r6-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-translate.png" width="50px"/></div> | Übersetzungs-Manipulator | Lassen Sie zu, dass die Projektion oder die Rasterpunkte entlang der Hauptachsen (X, Y, Z) verschoben werden. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r7-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-rotate.png" width="50px"/></div> | Rotationsmanipulator | Lassen Sie zu, dass die Projektion oder die Rasterpunkte in der Mitte entlang der Hauptachsen (X, Y, Z) gedreht werden. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r8-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-scale.png" width="50px"/></div> | Skalenmanipulator | Lassen Sie zu, dass die Projektion in der Szene entlang der Hauptachsen (X, Y, Z) skaliert wird. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r9-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-surface.png" width="50px"/></div> | Oberflächenmanipulator | Lassen Sie zu, dass die Projektions- oder Rasterpunkte verschoben werden, indem Sie sie an der 3D-Modelloberfläche ausrichten. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r10-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-space.png" width="50px"/></div> | Manipulatorraum | Definieren Sie, in welchem Raum die Transformationen durchgeführt werden. Mögliche Werte:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Lokaler Speicherplatz</strong>: -Achsen mit der aktuellen Transformation ausgerichtet.</li><li data-preserve-html="true"><strong>Weltraum</strong>: Die Achsen werden an der Szene ausgerichtet.</li></ul> |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r11-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-flip-x.png" width="50px"/></div> | Spiegeln auf X | Spiegeln Sie die Transformation an der X-Achse. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r12-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-flip-y.png" width="50px"/></div> | Spiegeln auf Y | Spiegeln Sie die Transformation an der Y-Achse. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r13-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-flip-z.png" width="50px"/></div> | Spiegeln auf Z | Spiegeln Sie die Transformation an der Z-Achse. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r14-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-warp-reset.png" width="50px"/></div> | Umwandlung zurücksetzen | Dieses Menü enthält drei Aktionen:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Globale Transformation wiederherstellen</strong>: Position, Drehung und Skalierung der Projektion auf die Ausgangswerte zurücksetzen. Diese Aktion hat keine Auswirkungen auf die Rasterpunkte selbst.</li><li data-preserve-html="true"><strong>Alle Eckpunkte zurücksetzen</strong>: werden alle Positionen und Tangenten der Rasterpunkte des Verkrümmungsrasters zurückgesetzt.</li><li data-preserve-html="true"><strong>Ausgewählte Eckpunkte zurücksetzen</strong>: werden nur die Position und die Tangenten der ausgewählten Punkte des Verkrümmungsrasters zurückgesetzt.</li></ul> |

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

## Bearbeiten von Rasterpunkten

Die Verkrümmungsprojektion wird durch eine Ebene und ein Punktraster dargestellt. Jeder Punkt kann so angepasst werden, dass die Projektion besser in das 3D-Modell passt, aber auch um die Textur zu verzerren.

Um den Rasterpunkt zu bearbeiten, wechseln Sie in der kontextabhängigen Symbolleiste in den Editionsmodus zu **Eckpunkte bearbeiten**:

![](../../assets/edit-vertices.png)

>[!NOTE]
>
> Ein Tastaturbefehl ist verfügbar, um schnell zwischen **Transformationsverkrümmung** und **Eckpunkte bearbeiten** zu wechseln. Siehe **Warp-Edition-Modus umschalten** auf der Seite [Tastaturbefehle](../../interface/settings/shortcuts.md).

### Auswählen von Punkten

| Aktion | Beschreibung |
| --- | --- |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table3_row-r1-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/grid-point-selection-single-click.gif" width="250px"/></div> | <ul data-preserve-html="true"><li data-preserve-html="true">Ein Klick auf einen Punkt genügt, um ihn auszuwählen.</li><li data-preserve-html="true">Wenn Sie außerhalb eines Punktes klicken, hebt der Manipulator die Auswahl von Punkten auf.</li><li data-preserve-html="true">Durch Klicken auf Punkte beim Drücken von <strong>UMSCHALT</strong> können mehrere Punkte ausgewählt werden.</li><li data-preserve-html="true">Wenn Sie beim Drücken von <strong>STRG</strong> auf einen Punkt klicken, können Sie die Auswahl nur für diesen Punkt aufheben, nicht für den anderen.</li></ul> |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table3_row-r2-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/grid-point-selection-rectangle.gif" width="250px"/></div> | <ul data-preserve-html="true"><li data-preserve-html="true">Durch Klicken und Ziehen können Sie eine rechteckige Auswahl erstellen. Alle Punkte innerhalb des Rechtecks werden ausgewählt, wenn die Maustaste losgelassen wird.</li><li data-preserve-html="true">Durch Klicken und Ziehen beim Drücken von <strong>UMSCHALT</strong> können Sie der aktuellen Auswahl weitere Punkte hinzufügen.</li><li data-preserve-html="true">Durch Klicken und Ziehen beim Drücken von <strong>STRG</strong> können Sie Punkte aus der aktuellen Auswahl entfernen.</li></ul> |

### Bewegliche Punkte

| Aktion | Beschreibung |
| --- | --- |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table4_row-r1-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/point-move.gif" width="250px"/></div> | <ul data-preserve-html="true"><li data-preserve-html="true">Verwenden Sie den Übersetzungsmanipulator, um einen Punkt zu verschieben.</li><li data-preserve-html="true">Verwenden Sie den Oberflächenmanipulator, um sich auf einem Punkt auf der Oberfläche des 3D-Modells zu bewegen.</li></ul> |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table4_row-r2-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/point-move-clickdrag.gif" width="250px"/></div> | <ul data-preserve-html="true"><li data-preserve-html="true">Klicken und ziehen Sie einen Punkt, um ihn schnell zu verschieben, ohne ihn zuerst auswählen zu müssen.</li><li data-preserve-html="true">Durch Klicken und Ziehen eines Punktes wird er wie der Oberflächenmanipulator verschoben.</li><li data-preserve-html="true">Durch Klicken und Ziehen eines Punkts, während Sie <strong>STRG</strong> drücken, wird er wie der Übersetzungsmanipulator (im Kameraraum auf drei Achsen) verschoben.</li></ul> |

### Tangenten anpassen

Das Verkrümmungsprojektionsraster ist ein [Bézier-Patch](https://en.wikipedia.org/wiki/B%C3%A9zier_surface). Das bedeutet, dass jeder Punkt über eine eigene Tangente verfügt, um die Kurve der Linien zu steuern, die Punkte miteinander verbinden. Durch Anpassen der Tangenten hast du mehr Kontrolle über die Verformung der Struktur.

| Aktion | Beschreibung |
| --- | --- |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table5_row-r1-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/tangent-rotate-scale.gif" width="250px"/></div> | <ul data-preserve-html="true"><li data-preserve-html="true">Um die Tangenten eines Punkts zu ändern (wird in Rot angezeigt), wählen Sie einfach den angegebenen Punkt aus und verwenden Sie dann den Manipulator Drehung oder Skalierung .</li></ul> |

>[!NOTE]
>
> Die Tangente wird zurückgesetzt und automatisch angepasst, wenn Punkte verschoben werden, wenn die Einstellung **Automatische Tangenten** aus der kontextbezogenen Symbolleiste aktiviert ist.
> 
> ![](../../assets/warp-tangent-adjustment.gif)

### Erhöhen oder Verringern der Punktzahl

Das Verkrümmungsraster kann unterteilt werden, um die Anzahl der Punkte zu erhöhen und mehr Kontrolle darüber zu haben, wie die Textur verformt wird.

| Aktion | Beschreibung |
| --- | --- |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table6_row-r1-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/warp-split.gif" width="300px"/></div> | <ul data-preserve-html="true"><li data-preserve-html="true">Teile das Raster über das Einstellungsmenü &quot;Verformen&quot; nach Zeilen und Spalten. (Dies ist nur möglich, wenn keine Punkte verschoben wurden)</li><li data-preserve-html="true">Unterteilen Sie das Raster, indem Sie eines der drei Teilungswerkzeuge verwenden.</li><li data-preserve-html="true">Alle Teilungswerkzeuge können durch Drücken von <strong>Esc</strong> abgebrochen werden.</li></ul> |
