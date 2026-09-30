---
title: Graustufenkonvertierung
description: Erfahren Sie, wie Sie den Substance 3D Painter-Filter "Graustufenkonvertierung" verwenden.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 4%
---

# Graustufenkonvertierung

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![Graustufenkonvertierung-Symbol](./Resources/icon_grayscale_conversion.png "Graustufenkonvertierung")

<b>In:</b> Effekte/Farbe, Entsättigung, Min., Max.

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Beschreibung

Der Graustufenkonvertierung-Filter wandelt ein Kanal-/Farbbild in Graustufen um, indem die Luminanz jedes Farbkanals gewichtet wird. Sie haben viele Optionen, um die Konvertierung zu optimieren.

Es wird auf einer Textur- oder Maskenebene verwendet, um die Kanäle in Graustufen zu konvertieren oder ein Farbbild in Graustufen zu konvertieren und es als Maske zu verwenden.

</td>
</tr>
</table>

## Eingaben

| Eingabename | Beschreibung |
| --- | --- |
| <b>Benutzerdefinierte Eingabe:</b> Farbe | Verwenden einer benutzerdefinierten Textur oder eines Ankerpunkts. |

<a name="parameters"></a>

## Parameter

| Parametername | Beschreibung |
| --- | --- |
| <b>Kanaleingabe:</b> | Wählen Sie den Kanaleingang aus, der für die Konvertierung verwendet wird. |
| <b>Umkehren:</b> | Kehrt die Umkehrung des Ergebnisses um. |
| <b>Saldo:</b> | Passen Sie die Balance des Ergebnisses zwischen Schwarz und Weiß an, ähnlich wie bei einer Helligkeitsanpassung. |
| <b>Kontrast:</b> | Passen Sie den Kontrast/Abfall des Ergebnisses an. |
| <b>Modus:</b> | Wählen Sie den Graustufen-Konvertierungsmodus aus. |
| <b>Rot:</b> | Passen Sie die Gewichtung für den roten Kanal an. Diese Gewichtung wird zur Berechnung des Graustufenergebnisses verwendet. |
| <b>Grün:</b> | Passen Sie die Gewichtung für den grünen Kanal an. Diese Gewichtung wird zur Berechnung des Graustufenergebnisses verwendet. |
| <b>Blau:</b> | Passen Sie die Gewichtung für den Blaukanal an. Diese Gewichtung wird zur Berechnung des Graustufenergebnisses verwendet. |
| <b>Alpha:</b> | Passen Sie die Gewichtung des Alphakanals an. Diese Gewichtung wird zur Berechnung des Graustufenergebnisses verwendet. |

