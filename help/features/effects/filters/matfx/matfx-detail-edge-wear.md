---
title: MatFX Detail-Edge Wear
description: Erfahren Sie, wie Sie den MatFX-Detailfilter für Edge Wear in Substance 3D Painter verwenden.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 1%
---

# MatFX Detail-Edge Wear

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="./Resources/icon_matfx_detail_edge_wear.png" alt="MatFX Detail Edge Wear-Symbol" title="MatFX Detail-Edge Wear"/><br><strong>In:</strong> Effekte/Verschleiß, Kante, Material</td>
    <td style="border: 0;" valign="top">Beschreibung<br>Der MatFX-Detailfilter erstellt verschlissene Kantendetails, die in ein Material Edge Wear werden können.<br>Es wird auf einer Maskenebene oder einem Material-Stapel verwendet, um einen Kantenverschleiß, einen Schmutz-Ausbruch und unterstützende Maskenanpassungen, die durch Texturen und Krümmung-Daten gesteuert werden, hinzuzufügen.</td>
  </tr>
</table>

>[!NOTE]
>
> Damit der MatFX-Detailfilter einen sichtbaren Edge Wear hat, müssen im Ebenenstapel unterhalb des Filters verschiedene Normalinformationen vorhanden sein. Wenn der normale Kanal keine Daten oder keine Variation enthält, kann der Filter keine Kanten finden, die beschädigt werden, und hat keine sichtbaren Auswirkungen.

## Parameter

| Parametername | Beschreibung |
| --- | --- |
| **Weichzeichnungsintensität:** | Passen Sie die Stärke des Unschärfe-Effekts an. |
| **Weichzeichnungsumbruch:** | Weichzeichnungsumbruch ein/aus. Wenn diese Option aktiviert ist, nimmt der Effekt Pixel von der gegenüberliegenden Seite der Textur auf. |
| **Eingabemodus:** | Wählen Sie den Eingabemodus aus, mit dem der Verschleißeffekt gesteuert wird. |
| **Verschleißstufe:** | Passen Sie die Gesamtverschleißstärke an. |
| **Kontrast:** | Den Kontrast der Verschleißmaske einstellen. |
| **Kanten-Smoothness:** | Passen Sie die Smoothness der abgenutzten Kanten an. |
| **Schmutz:** | Passen Sie die Menge des Schmutzes an, der dem Verschleiß hinzugefügt wird. |
| **Schmutz-Skalierung:** | Passen Sie die Skalierung des Schmutzes an. |

### Material

**PBR-Metallische Rauheit**

|  |  |
| --- | --- |
| **Grundfarbe:** | Passen Sie den Beitrag der Grundfarbe an. |
| **Metallic:** | Passen Sie den metallic Wert an. |
| **Rauheit:** | Passen Sie den Wert für die Rauheit an. |

**PBR Specular-Glanz**

|  |  |
| --- | --- |
| **Diffuse:** | Passen Sie den diffusen Beitrag an. |
| **Specular-Farbe:** | Passen Sie die Specular-Farbe an. |
| **Glanz:** | Passen Sie den Wert für den Glanz an. |

### Einstellungen

|  |  |
| --- | --- |
| **Generator-Maskensteuerung:** | Passen Sie den Einfluss der Generatormaske an. |
| **Generator-Maskenkontrast:** | Den Kontrast der Generatormaske anpassen. |
| **Generator-Maskenunschärfe:** | Passen Sie den Weichzeichner an, der auf die Generatormaske angewendet wird. |
| **Hintergrundwert für Alpha:** | Passen Sie den Alpha-Wert für den Hintergrund an. |
| **Intensität der Krümmung:** | Passen Sie die Intensität der Krümmung an. |
| **Krümmung umkehren:** | Umkehren der Krümmung-Eingabe umschalten. |
| **Krümmung zusammenführen:** | Kombinieren der invertierten und nicht invertierten Krümmungen aktivieren/deaktivieren. |
| **Normalintensität:** | Passe die normale Intensität an. |
| **AO-Verteilung:** | Passen Sie die Streuung des ambient occlusion-Effekts an. |
