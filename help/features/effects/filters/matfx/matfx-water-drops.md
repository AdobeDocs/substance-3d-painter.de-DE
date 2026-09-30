---
title: MatFX Wassertropfen
description: Erfahren Sie, wie Sie den MatFX Water Drops-Filter von Substance 3D Painter verwenden.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 3%
---

# MatFX Wassertropfen

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![MatFX-Wassertropfen-Symbol](./Resources/icon_matfx_water_drops.png "MatFX-Wassertropfen")

<b>In:</b> Effekte/Weichzeichnen, Graustufen

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Beschreibung

Der MatFX-Wassertropfen-Filter erzeugt Wassertropfen- und Abflusseffekte auf ein Material.

Es wird auf Textur-Ebenen oder Material-Stapeln verwendet, um Tröpfchen, gerichtete Streifen und Schwankungen der Nassoberfläche hinzuzufügen.

</td>
</tr>
</table>

## Eingaben

| Eingabename | Beschreibung |
| --- | --- |
| <b>Ambient occlusion:</b> Graustufen | Verwenden Sie die Baking geführt ambient occlusion-Map. |
| <b>Welt-Raum-Normale:</b> Farbe | Verwenden Sie die Baking geführt Welt-Raum-Normale-Map. |
| <b>Position:</b> Farbe | Verwenden Sie die Baking geführt Positionsabbildung. |

<a name="parameters"></a>

## Parameter

| Parametername | Beschreibung |
| --- | --- |
| <b>Anzahl der Einbrüche:</b> | Stellen Sie die Menge der Wassertropfen ein. |
| <b>Drops-Skalierung X:</b> | Passen Sie die X-Skalierung der Tropfen an. |
| <b>Drops-Skalierung Y:</b> | Passen Sie die Y-Skalierung der Tropfen an. |
| <b>Drops-Skalierung zufällig:</b> | Passen Sie die Stärke der zufälligen Skalierungsvariation in den Tropfen an. |
| <b>Absenkrichtungsintensität:</b> | Passe die Intensität der Tropfen in die gewünschte Richtung an. |

### Position

| Parametername | Beschreibung |
| --- | --- |
| <b>Einfluss X:</b> | Passen Sie den X-Einfluss der Positionseingabe an. |
| <b>Einfluss Y:</b> | Passen Sie den Y-Einfluss der Positionseingabe an. |
| <b>Einfluss Z:</b> | Passen Sie den Z-Einfluss der Positionseingabe an. |

### Wasserakkumulation

| Parametername | Beschreibung |
| --- | --- |
| <b>Intensität:</b> | Passen Sie die Intensität der Wasserakkumulation an. |
| <b>Druckbogen:</b> | Passen Sie die Ausbreitung der Wasserakkumulation an. |
| <b>AO-basierte Intensität:</b> | Passen Sie an, wie stark ambient occlusion die Wasserakkumulation beeinflusst. |

### Welt Raum

| Parametername | Beschreibung |
| --- | --- |
| <b>Maskierungsintensität:</b> | Passe die Intensität der Weltall-Maskierung an. |
| <b>Höchste Intensität:</b> | Passen Sie die Intensität der Tropfen an nach oben zeigenden Bereichen an. |
| <b>Intensität unten:</b> | Passen Sie die Intensität der Tropfen an nach unten zeigenden Bereichen an. |
| <b>Intensität vorne:</b> | Passen Sie die Intensität der Tropfen in den nach vorne zeigenden Bereichen an. |
| <b>Rückwärtsintensität:</b> | Passen Sie die Intensität der Tropfen an den nach hinten gerichteten Bereichen an. |
| <b>Intensität rechts:</b> | Passen Sie die Intensität der Tropfen in nach rechts zeigenden Bereichen an. |
| <b>Linke Intensität:</b> | Passen Sie die Intensität der Tropfen in nach links zeigenden Bereichen an. |

### Material

| Parametername | Beschreibung |
| --- | --- |
| <b>Verringert die Verkrümmungsintensität der Grundfarbe:</b> | Passe die Intensität der Verformung an, die auf die Grundfarbe unter den Tropfen angewendet wird. |
| <b>Drops-Rotationsvektorzuordnungsvervielfacher:</b> | Passen Sie den Multiplikator an, der auf die Vektorgrafik der Ablagedrehung angewendet wird. |
| <b>Verringert die Height-Intensität:</b> | Passe die Intensität des Effekts &quot;Height ablegen&quot; an. |
| <b>Drops-Rauheit:</b> | Passen Sie die Rauheit der Tropfen an. |
| <b>Drops Rauheit-Überblendung:</b> | Passen Sie an, wie sich die Rauheit mit dem Material vermischt. |
| <b>Metallic Einfügungen:</b> | Passen Sie den metallic Wert der Tropfen an. |
| <b>Verwirft die Metallic Füllmethode:</b> | Passen Sie an, wie sich der metallic Ablagewert mit dem Material vermischt. |
| <b>Normalintensität:</b> | Passe die Intensität des Effekts an. |
