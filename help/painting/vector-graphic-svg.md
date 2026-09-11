---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/painting/vector-graphic-svg.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie in Substance 3D Painter Vektorgrafiken (SVG- und AI-Dateien) verwenden, um Texturen skalierbare Vektorgrafiken hinzuzufügen.
helpx_creative_field: ""
helpx_description: Substance 3D Painter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Vektorgrafik (SVG)
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 1%

---


# Vektorgrafik (.svg und .ai)

![Bild, das eine SVG-Datei zeigt, die auf ein Gitter neben einer Liste von Parametern projiziert wird](../assets/svg_overview.png)

Vektorgrafik-Dateien (sowohl <b>.svg</b> als auch Illustrator <b>.ai</b>) können wie normale Bilder in Painter importiert werden. Mit einigen wenigen verfügbaren Einstellungen kannst du das Aussehen der Grafik anpassen und sie an die restlichen Strukturen anpassen.

* Weitere Informationen zum SVG von Dateien [finden Sie auf dieser Seite &#x200B;](https://www.adobe.com/creativecloud/file-types/image/vector/svg-file.html).
* Weitere Informationen zu AI-Dateien [finden Sie auf dieser Seite &#x200B;](https://www.adobe.com/ie/creativecloud/file-types/image/vector/ai-file.html).

SVG- und AI-Dateien werden automatisch in Pixelbilder konvertiert, wenn sie innerhalb des [Ebenenstapels](../interface/layer-stack/layer-stack.md) verwendet werden (je nach ausgewählter Einstellung). Dies ist ein nicht destruktiver Prozess, bei dem das Ändern der Auflösung oder das Aktualisieren der Quelldatei das Endergebnis entsprechend aktualisiert.

## Eigenschaften

Nachdem Sie eine Vektordatei importiert und in eine Ebene oder ein Tool geladen haben, stehen verschiedene Parameter zur Verfügung:

| Abschnitt | Einstellung | Beschreibung |
| --- | --- | --- |
| <b>Zeichenfläche</b> | <b>Zeichenfläche</b> | Wählen Sie die in der Datei enthaltene Zeichenfläche aus.  **Hinweis:** Diese Einstellung ist nur für Illustrator-Dateien (.ai) verfügbar. |
| <b>Auflösung</b> | Auflösung | Lege fest, bei welcher Größe das SVG-Bild in ein Bitmapbild (Pixel) umgewandelt wird, wenn es für die Texturierung im Ebenenstapel verwendet wird.   Mögliche Werte:<ul data-preserve-html="true"> <li data-preserve-html="true"><b>Auto</b>: Die Auflösung wird durch die Auflösung des aktuellen Textursatzes (bei Verwendung in Füllebene/Effekt) oder 512 Pixel bei Verwendung in einem Pinselwerkzeug bestimmt.<br/> </li> <li data-preserve-html="true"><b>Asset</b>: Die Auflösung wird durch die Pixelgröße bestimmt, die in der SVG-Datei selbst definiert ist.<br/> </li> <li data-preserve-html="true"><b>Benutzerdefiniert</b>: Die Auflösung wird durch die Auflösungseinstellung bestimmt, die sich direkt unter der Benutzeroberfläche befindet.</li> </ul>  <div><img alt="SVG-Auflösung" class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_table_row-ad42696-column-7212622_image" src="../assets/svg_resolution_custom.png" title="SVG-Auflösung"/></div> |
|  |  |  |
| <b>Zuschneidebereich</b> | Zuschneiden auf | Legen Sie fest, wie die SVG-Formen auf den gerenderten Bereich beschränkt werden sollen.   Mögliche Werte:<ul data-preserve-html="true"> <li data-preserve-html="true"><b>Elementgrenzen</b>: Der Bereich wird durch die in der SVG-Datei definierten Grenzen definiert.</li> <li data-preserve-html="true"><b>Benutzerdefiniert</b>: Der Bereich wird durch explizite Werte über die Einstellungen der direkt darunter liegenden Schnittstelle definiert.<br/> </li> </ul> |
|  | Quadratisches Seitenverhältnis | Wenn der Zuschneidebereich durch <b>Elementgrenzen</b> definiert ist, stellt diese Einstellung sicher, dass das Originalverhältnis beibehalten wird, sodass beim Rendern der SVG als quadratisches Bild keine falschen dehnte entstehen.   Diese Einstellung kann dazu führen, dass einige Elemente unerwartet sichtbar werden. Um dieses Problem zu vermeiden, deaktivieren Sie diese Einstellung und passen Sie die UV-Einstellungen stattdessen manuell an, wenn Sie sich in einer Füllebene/einem Effekt befinden. |
|  | Oben links Unten rechts | Wenn für die Freistellungsbereiche der Bereich &quot;Benutzerdefiniert&quot; ausgewählt ist, können Sie den Bereich anhand dieser Einstellungen manuell definieren, indem Sie die obere linke und untere rechte Ecke angeben. |
|  |  |  |
| <b>Umfang</b> | Umfang | Definieren Sie, welche Elemente in der SVG-Datei enthalten sind, bevor Sie sie rendern.   Der Standardwert ist <b>Dokument</b>, was bedeutet, dass der gesamte Inhalt der SVG-Datei verwendet wird. Verwenden Sie die Schaltfläche <b>Ändern</b>, um die einzuschließenden Elemente anzupassen. |

### Bereichsfenster

Wenn Sie den Suchbereich einer Vektorgrafik bearbeiten (siehe Einstellung oben), wird ein Fenster mit einer Elementliste angezeigt, in der Sie die Elemente auswählen können, die ein- oder ausgeschlossen werden sollen.

Verwenden Sie das Kontrollkästchen <b>Miniaturansichten anzeigen</b>, um für jedes Element ein Bild anzuzeigen.

![](../assets/v10_ai_thumbs.jpg)
