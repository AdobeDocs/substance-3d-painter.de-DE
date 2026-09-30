---
title: Tonwerte limitieren
description: Erfahren Sie, wie Sie den Beschränkt Filter von Substance 3D Painter verwenden.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 2%
---

# Tonwerte limitieren

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![Symbol Beschränkt](./Resources/icon_clamp.png "Beschränkt")

<b>In:</b> Effekte/Anpassungen

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Beschreibung

Der Beschränkt Filter fixiert die Werte auf definierte Grenzwerte.

Sie wird entweder direkt auf einer Füllebene verwendet, um bestimmte Bereiche eines Materials zu beschränken, oder auf einer Maske, um Werte auf einen bestimmten Bereich zu beschränken.

</td>
</tr>
</table>

>[!NOTE]
>
> Bei Verwendung auf einer Füllebene oder als Durchgang für Farbinformationen wirkt sich die Klammer auf jeden Farbkanal einzeln aus. Wenn ein Pixel also eine Farbe von (R 0, G 0,5, B 1,0) hat und auf 0,5 geklemmt wird, ist die resultierende Farbe dieses Pixels (R 0, G 0,5, B 0,5). Der Grund dafür ist, dass der Blaukanal einen ausreichend hohen Wert hatte, um geklemmt zu werden, die anderen Kanäle jedoch nicht. Das bedeutet, dass der Farbfilter den Farbton des Beschränkt Inhalts ändern kann.
>
>Wenn Sie den Farbton nicht ändern möchten, sind möglicherweise andere Filter wie die Tonwertkorrektur besser geeignet.

<a name="parameters"></a>

## Parameter

| Parametername | Beschreibung |
| --- | --- |
| <b>Min.:</b> | Passen Sie den Mindestwert an. |
| <b>Max.:</b> | Passen Sie den Maximalwert an. |
