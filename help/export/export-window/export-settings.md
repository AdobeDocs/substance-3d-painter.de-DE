---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/getting-started/export/export-window/export-settings.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie Exporteinstellungen in Substance 3D Painter konfigurieren, um die Auflösung der Textur, das Format und die Ausgabeoptionen zu steuern.
helpx_creative_field: ""
helpx_description: Painter > Getting Started > Export > Export window > Export settings
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Exporteinstellungen
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '958'
ht-degree: 2%

---


# Exporteinstellungen

![](../../assets/image2023-1-30-13-22-30.png){width="500px"}

Auf der Registerkarte <b>Exporteinstellungen</b> des <b>Exporteinstellungen-Fensters</b> können Sie die Komposition, die Textur und den Speicherort der exportierten Texturen konfigurieren.

## Konfiguration von Allgemein und Textursätzen

![](../../assets/texture-set-list-1.png)

Das erste Element des Fensters ist die Liste der Textursatz auf der linken Seite. Der Abschnitt &quot;Globale Einstellungen&quot; bietet Zugriff auf allgemeine Parameter für alle Textursatz. Dadurch ist es ganz einfach, nur einen einzigen Einstellungssatz anzupassen, der auf alle Textursatz des Projekts angewendet wird. Änderungen an den Einstellungen einzelner Textursatz setzen die globalen Einstellungen für diesen Textursatz außer Kraft. Wenn Sie beispielsweise in den globalen Einstellungen die Auflösung 2048 und in einem Textursatz 1024 als irreguläres Format festlegen, werden alle Textursatz mit der Auflösung 2048 exportiert, mit Ausnahme des auf 1024 festgelegten Formats.

Das Kontrollkästchen neben dem Namen jedes Textursatzes gibt an, ob die zugehörigen Texturen exportiert werden oder nicht.

Das Dropdownmenü ist für Projekte mit einer großen Anzahl von Textursätzen geeignet, da Sie die Auswahl schnell mit <b>Alle überprüfen</b>, <b>Alle deaktivieren</b> und <b>Alle </b> Aktionen umkehren ändern können.

## Allgemeine Exportparameter

![](../../assets/image2023-1-30-13-23-7.png)

Dieser Abschnitt enthält die freigegebenen Einstellungen für jede zu generierende Textur:

| Einstellung | Beschreibung |
| --- | --- |
| <b>Ausgabeverzeichnis</b> | Speicherort für exportierte Texturen. |
| <b>Ausgabevorlage</b> | Wählen Sie die Ausgabevorlage aus, mit der die Kanäle benannt und in Textur-Dateien zusammengeführt werden sollen. Weitere Informationen zu Vorlagen finden Sie in der Liste [Ausgabevorlagen](../export-presets/export-presets.md). |
| <b>Dateityp </b> | Das Dateiformat und seine Bittiefe. Wenn die Option <b>Basierend auf Ausgabevorlage</b> aktiviert ist, wird das Dateiformat von der Exportvorgabe geerbt (wodurch Format und Bittiefe pro Textur und nicht global bestimmt werden können). Die verfügbare Bittiefe hängt vom Dateityp ab. Weitere Informationen finden Sie in der folgenden Tabelle. |
| <b>Größe </b> | Die Auflösung der exportierten Textur. Mögliche Werte:<ul data-preserve-html="true"> <li data-preserve-html="true"><b>Basierend auf der Größe jedes Textursatzes</b></li> <li data-preserve-html="true"><b>128</b></li> <li data-preserve-html="true"><b>256</b></li> <li data-preserve-html="true"><b>512</b></li> <li data-preserve-html="true"><b>1024</b></li> <li data-preserve-html="true"><b>2048</b></li> <li data-preserve-html="true"><b>4096</b></li> <li data-preserve-html="true"><b>8192</b> (nur für GPUs mit mehr als 1,5 GB Vram verfügbar)</li> </ul> |
| <b>Auffüllen von </b> | Füllung des Bereichs außerhalb der UV-Inseln in der Textur Mögliche Werte sind:<ul data-preserve-html="true"> <li data-preserve-html="true"><b>Kein Auffüllen (Passthrough)</b>: den aktuellen Status der Textur unverändert verwenden.</li> <li data-preserve-html="true"><b>Ausdehnung unendlich</b>: gedehnt UV-Inseln bis zu den Nachbargrenzen oder bis zum Ende der Textur.</li> <li data-preserve-html="true"><b>Ausdehnung + transparent</b>: Die Ränder der UV-Insel werden auf den angegebenen Abstand in Pixeln gedehnt, der Rest ist transparent.</li> <li data-preserve-html="true"><b>Ausdehnung + Standardhintergrundfarbe</b>: Die Ränder der UV-Insel werden auf die angegebene Entfernung in Pixel gedehnt. Die restlichen werden mit der Standardfarbe des Kanals des Textursatzes gefüllt.</li> <li data-preserve-html="true"><b>Ausdehnung + Standardhintergrundfarbe</b>: Die Ränder der UV-Insel werden auf die angegebene Entfernung in Pixel gedehnt. Die restlichen werden mit der Standardfarbe des Kanals des Textursatzes gefüllt.</li> <li data-preserve-html="true"><b>Ausdehnung + Diffusion</b>: Um die UV-Insel auf die angegebene Entfernung in Pixeln dehnen, wird der Rest mit einer verschwommenen Version der UV-Insel (basierend auf MIP-Maps) gefüllt.</li> </ul> |

>[!NOTE]
>
> Das Dateiformat **psd** ist ein Container. Das bedeutet, dass Ausgabemaps in einer einzelnen Datei auf dem Datenträger gesammelt werden.

### Dither

Das Exportieren von 8-Bit-Texturen kann zu Streifenbildung in Farbverläufen führen. Dies macht sich besonders bei Normal und Höhen-Map bemerkbar. Es gibt zwei Möglichkeiten, dieses Problem zu lösen: mit höherer Präzision oder mit Dithering kompensieren.

Eine höhere Präzision (16 oder 32 Bit) ist ideal, aber möglicherweise nicht mit allen Anwendungen kompatibel. Vor allem Game-Engine werden oft auf 8 Bit komprimiert. Dithering führt Rauschen ein, mit dem Banding-Probleme gemildert werden können, während weiterhin 8 Bit an Informationen verwendet werden.

![](../../assets/dither-1.jpg)

### Dateiformate für Texturen

Im Folgenden finden Sie eine Liste aller von Painter unterstützten Exportdateiformate:

| Formatname | Formaterweiterung | Unterstützte Bit-Tiefe |
| --- | --- | --- |
| **Bitmap** | BMP | 8, 8 + Dithering |
| **OpenEXR** | exr | 16 (schwebend), 32 (schwebend) |
| **Graphics Interchange Format** | gif | 8, 8 + Dithering |
| **HDR.** | HDR | 32 (schwebend) |
| **Symbol** | ico | 8, 8 + Dithering |
| **JPEG 2000** | j2k | 8, 8 + Dithering, 16 |
| **JPEG-Netzwerkgrafiken** | jng | 8, 8 + Dithering, 16 |
| **JPEG 2000** | jp2 | 8, 8 + Dithering, 16 |
| **JPEG** | JPEG | 8, 8 + Dithering |
| **JPEG des erweiterten Bereichs** | jpeg-xr | 8, 8 + Dithering, 16, 32 (schwebend) |
| **Portable Bit Map** | PBM | 8, 8 + Dithering, 16 |
| **Portable Fließkommazahl Map** | pfm | 32 (schwebend) |
| **Tragbare Graukarte** | pgm | 8, 8 + Dithering, 16 |
| **Portable Network Graphics** | png | 8, 8 + Dithering, 16 |
| **Portable Pixel Map** | ppm | 8, 8 + Dithering, 16 |
| **Photoshop-Dokument** | psd | 8, 8 + Dithering, 16 |
| **TGA für Truevision** | Targa | 8, 8 + Dithering |
| **Tag-Bilddateiformat** | tiff | 8, 8 + Dithering, 16, 32 (schwebend) |
| **Bitmapformat für das Wireless-Anwendungsprotokoll** | wbmp | 8, 8 + Dithering |
| **WebP** | schlagen | 8, 8 + Dithering |
| **X PixMap** | xpm | 8, 8 + Dithering |

## Ausgabe-Maps

Wenn ein bestimmter Textursatz ausgewählt ist, wird der Abschnitt Ausgabemaps für diesen Textursatz angezeigt.

![](../../assets/export-output-maps.png)

In diesem Abschnitt werden alle Texturen aufgeführt, die basierend auf der aktuellen Exportvorgabe generiert werden. Sie gibt die Vorlage für den Namen der Textur, das Dateiformat und die Bittiefe sowie den Farbraum an, wenn [Farbmanagement](../../features/color-management/color-management.md) aktiviert ist.

In diesem Abschnitt können Sie den Export bestimmter Dateien deaktivieren oder das <b>Dateiformat</b> und die <b>Bittiefe</b> überschreiben.

![](../../assets/export-override.gif)

## USD-Element exportieren

Wenn Sie dieses Kontrollkästchen aktivieren, können Sie in USD Format exportieren. Im Gegensatz zur USDz-Vorgabe (Apple AR), die in <b>Ausgabevorlagen</b> verfügbar ist, berücksichtigt dieser Export alle Vorlagen oder Parameter, die Sie für Ihren Export konfiguriert haben. Die folgenden Dateien werden exportiert, wenn Sie das Kontrollkästchen &quot;Element USD&quot; aktivieren:

* Ein Ordner mit Textur Maps
* Eine *.usda*, die auf den Ordner &quot;Textur Maps&quot; verweist.
* Eine optionale USD, die Material mit der ursprünglichen Meshdatei zusammenfügt. Es kann direkt in Omniverse verwendet werden, um Ihren Mesh mit automatisch angewendeten Materialien zu zeigen.
* Eine optionale USD-Datei, die den im Projekt verwendeten Mesh enthält. Es wird nur exportiert, wenn die ursprüngliche Meshdatei kein USD ist oder wenn der automatische entpack von Painter zum Generieren von UVs verwendet wurde.
