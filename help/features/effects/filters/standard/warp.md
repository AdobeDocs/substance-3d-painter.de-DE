---
title: Verformen
description: Erfahren Sie, wie Sie den Verkrümmungsfilter von Substance 3D Painter verwenden.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 3%
---

# Verformen

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![Verkrümmungssymbol](./Resources/icon_warp.png "Verkrümmen")

<b>In:</b> Effekte/Graustufen

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Beschreibung

Der Verkrümmungsfilter wird für verschiedene Deformationseffekte verwendet. Der Verzerrungsfilter bietet Zugriff auf die reguläre Verzerrung, eine Richtungsverkrümmung, die sich in einer bestimmten Richtung verkrümmt, und eine multidirektionale Verkrümmung für mehr Variation.

&quot;Verformen&quot; wird auf einer Maskenebene oder innerhalb einer Textur (Schwarzweißausgabe) verwendet, um Materialien, Formen, Masken, Konturen usw. zu verformen.

</td>
</tr>
</table>

## Eingaben

| Eingabename | Beschreibung |
| --- | --- |
| <b>Benutzerdefinierte Rauschen</b> | Verwenden Sie eine benutzerdefinierte Textur als Rauschen Eingabe-Map. |

<a name="parameters"></a>

## Parameter

| Parametername | Beschreibung |
| --- | --- |
| <b>Seed:</b> | Weisen Sie einen zufälligen Wert zu, um eine andere Variation zu erstellen, ohne die Gesamteinstellungen zu ändern. |
| <b>Verkrümmungsmodus:</b> | Wählen Sie den Verformungsmodus aus. |
| <b>Intensität:</b> | Passe die Intensität der Verformung an. |
| <b>Intensitätsteilung:</b> | Lege fest, wie die Intensität der Verformung aufgeteilt wird. |
| <b>Winkel:</b> | Verzerrungswinkel anpassen. |
| <b>Füllmethode:</b> | Wählen Sie die Füllmethode aus, die von der Verformung verwendet wird. |
| <b>Richtungen:</b> | Wählen Sie die Anzahl der Verformungsrichtungen aus. |

### Quellparameter

<table>
<tr>
<td><b>Quellmodus:</b></td>
<td>Bestimmt den Quellmodus.<br><br> - Standard-Rauschen: Verwendet die Standard-Rauschen für den Verkrümmungseffekt.<br> - Vorherige Eingabe: Verwendet die vorherige Eingabe für den Verkrümmungseffekt. Wenn auf eine Füllebene ein bestimmtes Rauschen-Muster angewendet wird, wird bei Verwendung eines Verkrümmungseffekts im Modus "Vorherige Eingabe" das gleiche Rauschen-Muster wie für die Füllebene verwendet.<br> - Benutzerdefiniertes Rauschen: Verwendet die benutzerdefinierte Rauschen-Eingabe für den Verkrümmungseffekt.</td>
</tr>
<tr>
<td><b>Quelle weichzeichnen:</b></td>
<td>Lässt die Quell-Rauschen verschwimmen.</td>
</tr>
<tr>
<td><b>Quellensaldo:</b></td>
<td>Passt die Balance des Quell-Rauschen an und verschiebt den Mittelpunkt wie bei einem Helligkeitsregler in Richtung Schwarz oder Weiß.</td>
</tr>
<tr>
<td><b>Quellkontrast:</b></td>
<td>Verfeinert den Kontrast der Quell-Rauschen.</td>
</tr>
<tr>
<td><b>Quellaufhellung:</b></td>
<td>Steuert die Kachelung der Quell-Rauschen.</td>
</tr>
</table>
