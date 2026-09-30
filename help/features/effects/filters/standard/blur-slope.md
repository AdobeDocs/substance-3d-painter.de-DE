---
title: Weichzeichnen-Steigung
description: Erfahren Sie, wie Sie den Weichzeichner-Steigung-Filter von Substance 3D Painter verwenden.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '215'
ht-degree: 3%
---

# Weichzeichnen-Steigung

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![Symbol für Weichzeichnungs-Steigung](./Resources/icon_blur_slope.png "Steigung weichzeichnen")

<b>In:</b> Effekte/Weichzeichnen, Graustufen

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Beschreibung

Der Farbweichzeichner-Filter erzeugt einen Verschmierungs- oder Verblassungseffekt, der sich vor allem bei kontrastreichen Kanten zwischen Steigungen bemerkbar macht.

Sie wird entweder direkt auf einer Maskenebene verwendet, um ganze Materials oder bestimmte Texturen zu verwischen, oder auf einer Textur, um die Maske zu verschmieren. Es kann zu undichten oder verwitterten Kanten, undichtem Dirt oder verschmiertem Rost führen.

</td>
</tr>
</table>

## Eingaben

| Eingabename | Beschreibung |
| --- | --- |
| <b>Benutzerdefinierte Rauschen:</b> Graustufen | Verwenden Sie eine benutzerdefinierte Textur oder einen Ankerpunkt als benutzerdefiniertes Rauschen. |

<a name="parameters"></a>

## Parameter

| Parametername | Beschreibung |
| --- | --- |
| <b>Seed:</b> | Weisen Sie einen zufälligen Wert zu, um eine andere Variation zu erstellen, ohne die Gesamteinstellungen zu ändern. |
| <b>Intensität:</b> | Passe die Weichzeichnungsintensität an. |
| <b>Intensitätsteilung:</b> | Lege fest, wie die Intensität des Weichzeichners aufgeteilt wird. |
| <b>Füllmethode:</b> | Wählen Sie die Füllmethode aus, die für die Weichzeichnung der Steigung verwendet wird. |
| <b>Qualität:</b> | Passen Sie die Qualität des Effekts an. |

### Quellparameter

<table>
<tr>
<td><b>Quelltyp:</b></td>
<td>Wählen Sie aus, ob die Quelle die Standard-Rauschen, die vorherige Eingabe oder eine benutzerdefinierte Rauschen verwendet.</td>
</tr>
<tr>
<td><b>Weichzeichnen:</b></td>
<td>Passen Sie die Weichzeichnungsintensität des Quell-Rauschen oder der Eingabe an.</td>
</tr>
<tr>
<td><b>Position:</b></td>
<td>Passen Sie den Mittelpunkt des Quell-Rauschen oder -Eingangs ähnlich wie bei einer Helligkeitssteuerung an.</td>
</tr>
<tr>
<td><b>Kontrast:</b></td>
<td>Passen Sie den Kontrast des Quell-Rauschen oder der Eingabe an.</td>
</tr>
<tr>
<td><b>Quellaufhellung:</b></td>
<td>Passen Sie die Kachelung der Quell-Rauschen oder -Eingabe an.</td>
</tr>
</table>
