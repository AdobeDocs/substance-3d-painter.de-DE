---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/painting/fill-projections/uv-projection.html"
breadcrumb-title: ''
description: Mit der Funktion "UV-Projektion" in Substance 3D Painter kannst du Texturen anhand von UV-Koordinaten projizieren, um die Textur präzise zu platzieren.
helpx_creative_field: ""
helpx_description: Painter > Painting > Fill projections > UV projection
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: UV-Projektion
user-guide-description: ''
user-guide-title: ''
source-git-commit: 2903c7fdf6a9fe0da149b61fa9064033bb88926a
workflow-type: tm+mt
source-wordcount: '788'
ht-degree: 4%

---


# UV-Projektion

![](../../assets/uv-proj.png)

Die UV-Projektion der Füllung ist eine 2D-Projektion, die nur im Raum der 2D-Textur funktioniert. Es bietet Steuerelemente zum Verschieben, Drehen und Skalieren eines Bildes.

## Eigenschaften

| *Einstellung* | *Beschreibung* |
| --- | --- |
| **Filtern** | Steuert, wie die Textur oder das Material gefiltert wird. Diese Einstellungen können sich darauf auswirken, wie die Textur aussieht, wenn sie mehrmals wiederholt wird. Bei hohen Skalierungswerten kann die Verwendung einer anderen Filterung als der Standardmethode zu einem besser aussehenden Ergebnis führen. Derzeit verfügbare Einstellungen:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Bilinear `\|` HQ </strong>: (Standard) Erweiterte bilineare Filterungen, die versuchen, die Qualität der Textur zu verbessern, wenn die Werte der Kachelung hoch sind.</li><li data-preserve-html="true"><strong>Bilinear `\|` Sharp </strong>: Einfache bilineare Filterung, die die Textur etwas glättet, aber versucht, Details zu erhalten.</li><li data-preserve-html="true"><strong>Nächste </strong>: Keine Filterung, nützlich, wenn die Bilineare Filterung zu einem verschwommenen Ergebnis führt und feine Details aufbricht. Kann Aliasing in die Textur einführen.</li></ul> |
| **Abwicklung** | Steuert, wie das projizierte Material/Bild in der Form der Projektion wiederholt werden soll. Mögliche Werte sind:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Keine</strong> : Es gibt keine Wiederholung der Projektion.</li><li data-preserve-html="true"><strong>Horizontal wiederholen</strong> : Wiederholen Sie diesen Vorgang nur horizontal.</li><li data-preserve-html="true"><strong>Vertikal wiederholen</strong> : Wiederholen Sie diesen Vorgang nur vertikal.</li><li data-preserve-html="true"><strong>Wiederholen</strong> (Standard) : Wiederholen Sie diesen Vorgang sowohl horizontal als auch vertikal.</li></ul> <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/2d-repeat.jpg" width="500px"/></div> |

### UV-Transformation

Die UV-Transformationseinstellungen steuern die Textur/das Material innerhalb der Projektion.

<table data-preserve-html="true" style="width: 100.0%;"><colgroup> <col style="width: 40.0%;"/> <col style="width: 20.0%;"/> <col style="width: 40.0%;"/> </colgroup><tbody><tr><th>Skalierungsmodus</th><th>Einstellung</th><th>Beschreibung</th></tr><tr><td><p><strong>Kachelung</strong> (Standard)<strong> <br/></strong></p><p>Ermöglicht die manuelle Festlegung des wiederholenden Betrags für die aktuelle Textur.</p></td><td><strong>Wiederholen</strong></td><td>Steuert, wie oft die Textur wiederholt wird.</td></tr><tr><td rowspan="2"><br/><br/></td><td colspan="1"><strong>Drehung</strong></td><td colspan="1">Steuert den Winkel, in dem die Textur auf das Gitter projiziert wird.</td></tr><tr><td colspan="1"><strong>Versatz</strong></td><td colspan="1">Steuert, von wo aus die Textur projiziert wird. Der Standardwert bedeutet, dass sich der Mittelpunkt der Textur in der Mitte der UVs des Gitters befindet.</td></tr><tr><th colspan="1"><br/></th><th colspan="1"><br/></th><th colspan="1"><br/></th></tr><tr><td rowspan="4"><p><strong>Physische Größe</strong></p><p>Automatische Einstellung einer Textur entsprechend der Größe des Meshs und der eingebetteten Physische Größe. Die richtige Physische Größe wird anhand der Längen- und Breitenwerte (X- und Y-Werte) berechnet. Die Z-Messung wird nicht berücksichtigt.</p><p>(Weitere Informationen finden Sie auf der speziellen [Dokumentationsseite](https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/features/physical-size))</p></td><td><strong>Benutzerdefinierte Größe</strong></td><td><p>Wenn diese Option aktiviert ist, können Sie eine Physische Größe manuell eingeben und die von einem Asset bereitgestellte Version überschreiben.</p><p>Sie wird automatisch ausgewählt, wenn keine Physische Größe erkannt wird oder wenn mehrere Assets mit unterschiedlichen Physische Größen innerhalb derselben Ebene/desselben Effekts verwendet werden.</p></td></tr><tr><td colspan="1"><strong>Größe (cm)</strong></td><td colspan="1">Eingebettete Physische Größen werden in Zentimetern angegeben. Es ist möglich, mit einer Gitterdatei zu arbeiten, die mit unterschiedlichen Maßeinheiten erstellt wurde. Die Proportionen bleiben dabei erhalten. Die Elementgröße wird derzeit jedoch nur in Zentimetern angezeigt.</td></tr><tr><td colspan="1"><strong>Drehung</strong></td><td colspan="1">Steuert den Winkel, in dem die Textur auf das Gitter projiziert wird.</td></tr><tr><td colspan="1"><strong>Versatz</strong></td><td colspan="1"><p>Steuert, von wo aus die Textur projiziert wird. Der Standardwert bedeutet, dass sich der Mittelpunkt der Textur in der Mitte der UVs des Gitters befindet.</p></td></tr></tbody></table>

## Kontextabhängige Symbolleiste

Mehrere Einstellungen und Werkzeuge sind in der [Kontextsymbolleiste](../../interface/toolbars.md) am oberen Rand des Viewports verfügbar, die die Steuerung des Manipulators und der Projektion ermöglichen:

| Symbol | Name | Beschreibung |
| --- | --- | --- |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r1-column-c0_image" src="../../assets/icon-manipulator-2d-hide.png" width="50px"/></div> | Manipulator anzeigen/ausblenden | Wenn diese Option aktiviert ist, ist der Manipulator im Viewport sichtbar und steuerbar. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r2-column-c0_image" src="../../assets/icon-manipulator-settings-2d.png" width="50px"/></div> | Größe der Manipulator-Handles | Dieses Menü enthält drei Einstellungen, die festlegen, wie groß die Griffe des transformieren Objekts im Viewport sind:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Klein</strong></li><li data-preserve-html="true"><strong>Medium</strong></li><li data-preserve-html="true"><strong>Groß</strong></li></ul> |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r3-column-c0_image" src="../../assets/icon-flip-x.png" width="50px"/></div> | Spiegeln auf X | Spiegeln Sie die Transformation auf der X-Achse. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r4-column-c0_image" src="../../assets/icon-flip-y.png" width="50px"/></div> | Spiegeln auf Y | Spiegeln Sie die Transformation an der Y-Achse. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r5-column-c0_image" src="../../assets/icon-pivot.png" width="50px"/></div> | Drehpunkt zurücksetzen | Setzt den Drehpunkt wieder auf den Mittelpunkt der Transformation. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r6-column-c0_image" src="../../assets/icon-reset.png" width="50px"/></div> | Umwandlung zurücksetzen | Stellen Sie die Transformation der Projektion wieder auf ihren Standardzustand zurück. |

## Manipulator

Die UV-Projektion verwendet einen Manipulator, der nur in der [2D-Ansicht](../../interface/viewport/2d-view.md) verfügbar ist.

| Aktion | Tastaturbefehl | Beschreibung |
| --- | --- | --- |
| **Kamera beweg** | Mausklick | Klicke auf einen Bereich innerhalb der Transformation, und ziehe, um ihn zu verschieben. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r1-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/uv-translate.gif"/></div> |
| **Eingeschränkt Kamera bewogen** | UMSCHALT+Mausklick | Klicken und ziehen Sie einen beliebigen Bereich innerhalb der Transformation, während Sie den Tastaturbefehl drücken und halten, um ihn nur entlang einer Achse zu verschieben. Die Achse kann horizontal oder vertikal ausgerichtet werden und richtet sich nach der Kamera. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r2-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/uv-translate-constrained.gif"/></div> |
| **Drehung** | Mausklick | Durch Klicken und Ziehen von außerhalb der Transformation können Sie sie drehen. Durch Verschieben des Drehpunkts kann auch der Drehpunkt geändert werden.   <table> <tr style="border: 0;"> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r3-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/uv-rotation.gif"/></div>  </td> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r3-column-c2_dynamic_grid_items_grid-cell1_position-par_image" src="../../assets/uv-rotation-pivot.gif"/></div>  </td> </tr> </table> |
| **Drehungseinschränkung** | UMSCHALT+Mausklick | Durch Klicken und Ziehen von außerhalb der Transformation, während Sie den Tastaturbefehl drücken und beibehalten, können Sie ihn nur um alle 45 Grad drehen. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r4-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/uv-rotation-constrained.gif"/></div> |
| **Skalierung** | Mausklick | Durch Klicken und Ziehen der Griffe des Manipulators können Sie die Transformation verformen.   <table> <tr style="border: 0;"> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r5-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/uv-scale-free.gif"/></div>  </td> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r5-column-c2_dynamic_grid_items_grid-cell1_position-par_image" src="../../assets/uv-scale-middle.gif"/></div>  </td> </tr> </table> |
| **Einschränkung der Skalierung** | UMSCHALT+Mausklick | Durch Drücken und Beibehalten des Kurzbefehls beim Ziehen eines Handles wird die Transformation gezwungen, ihr Verhältnis beizubehalten.   <table> <tr style="border: 0;"> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r6-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/uv-scale-ratio.gif"/></div>  </td> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r6-column-c2_dynamic_grid_items_grid-cell1_position-par_image" src="../../assets/uv-scale-middle-ratio.gif"/></div>  </td> </tr> </table> |
| **Gespiegelte Skalierung** | STRG + Mausklick | Wenn Sie einen Handle verschieben, während Sie den Kurzbefehl drücken, führen die anderen Handles eine ähnliche Bewegung aus. Sie erlaubt es, die Transformation in der Symmetrie um den Drehpunkt zu verformen.   <table> <tr style="border: 0;"> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r7-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/uv-scale-mirror.gif"/></div>  </td> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r7-column-c2_dynamic_grid_items_grid-cell1_position-par_image" src="../../assets/uv-scale-mirror-pivot.gif"/></div>  </td> </tr> </table> |
| **Gespiegelte und eingeschränkte Skalierung** | UMSCHALT + STRG + Mausklick | Durch das Kombinieren beider Tastaturbefehle können Sie die Transformation in Symmetrie verformen und gleichzeitig das Seitenverhältnis beibehalten. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r8-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/uv-scale-mirror-ratio.gif"/></div> |
