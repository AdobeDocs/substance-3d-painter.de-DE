---
title: Quantisieren
description: Erfahren Sie, wie Sie den Quantisierungsfilter von Substance 3D Painter verwenden.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '220'
ht-degree: 1%
---

# Quantisieren

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![Symbol &quot;Quantisieren&quot;](./Resources/icon_quantize.png "Quantisieren")

<b>In:</b> Effekte/Quantisierung, Farbe

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Beschreibung

Der Filter &quot;Quantisieren&quot; reduziert ein Bild auf einen begrenzten Farbsatz.

Es wird auf einer Textur-Ebene verwendet, um flachere, posterisierte oder stilisierte Farbbereiche zu erstellen.

</td>
</tr>
</table>

<a name="parameters"></a>

## Parameter

| Parametername | Beschreibung |
| --- | --- |
| <b>Farbmenge:</b> | Passen Sie die maximale Anzahl der im quantisierten Bild verwendeten Farben an. Dieser Wert steuert auch die extrahierte Palette, obwohl der tatsächliche Zähler je nach Quantisierungsmethode niedriger sein kann. Überprüfen Sie die Ausgabe Farbmenge der Palette auf die endgültige Anzahl der extrahierten Farben. |
| <b>Konturglättung:</b> | Passen Sie den Glättungsradius an, der auf das Eingabebild angewendet wird, um das quantisierte Ergebnis in einheitlichere Formen zu vereinfachen. Höhere Werte führen zu einer deutlichen Verlängerung der Berechnung. |
| <b>Dithering:</b> | Passen Sie die Menge an Dithering an, die zur Neuerstellung von Verläufen und Farbübergängen verwendet wird, während Sie weiterhin nur die nach der Quantisierung verbleibenden Farben verwenden. Verwenden Sie für den erwarteten Dithering-Effekt einen Konturglättungswert von 0. |
| <b>Dithering-Muster:</b> | Wählen Sie das Dithering-Muster aus, mit dem Verläufe und Farbübergänge im Originalbild neu erstellt werden. |
| <b>Entfernungsfarbraum:</b> | Wählen Sie den Farbraum aus, der zum Vergleichen und Verteilen der Farben während der Quantisierung verwendet wird. Verwenden Sie Labor (Farbe) für perzeptive Farbbilder und RGB (Daten) für Rohdaten wie Normalen-Map. |
| <b>Auf Alpha anwenden:</b> | Schaltet die Quantisierung des Alphakanals der Ebene um. |
| <b>Schwellenwert für Alpha:</b> | Passen Sie den Alpha-Schwellenwert an. |

