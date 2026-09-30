---
title: Tri-Planar Advanced
description: Erfahren Sie, wie Sie den Tri-Planar Advanced-Filter von Substance 3D Painter verwenden.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 2%
---

# Tri-Planar Advanced

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![Symbol &quot;Planarer Erweiterter Dreier&quot;](./Resources/icon_tri_planar_advanced_filter.png "Planarer Erweiterter Dreier")

<b>In:</b> Effekte/Projektion

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Beschreibung

Der Tri-Planar Advanced ist die Filterversion des Tri-Planar Advanced Generators, mit Handsteuerungen für die volle Projektion. Sie bietet Ihnen die Möglichkeit, die Werte für die Drehung und den Versatz für jede Achse zu steuern. Im Gegensatz zum Generator arbeitet dieser Filter direkt auf dem Ebeneninhalt, während der Generator eine benutzerdefinierte Maskeneingabe zum Überblenden benötigt.

Sie wird auf einer Maskenebene oder innerhalb einer Textur verwendet, um eine drei-planare Überblendung hinzuzufügen.

</td>
</tr>
</table>

## Eingaben

| Eingabename | Beschreibung |
| --- | --- |
| <b>Welt-Raum-Normale:</b> | Verwenden Sie die Baking geführt Welt-Raum-Normale-Map. |
| <b>Position:</b> | Verwenden Sie die Baking geführt Positionszuordnung. |

<a name="parameters"></a>

## Parameter

| Parametername | Beschreibung |
| --- | --- |
| <b>Projektion:</b> | Wählen Sie aus, über welche Achsen Sie projizieren möchten. |
| <b>Füllmethode:</b> | Lege fest, wie sich die Projektionen der Achse vermischen. |
| <b>Füllmethode:</b> | Passe den Kontrast der Projektion an. |
| <b>Textur Kachelung:</b> | Passen Sie die Kachelung der projizierten Textur an. |
| <b>Drehung X:</b> | Passen Sie die Drehung der X-Achse-Projektion an. |
| <b>Versatz X:</b> | Passen Sie den Versatz der Projektion der X-Achse an. |
| <b>Drehung Y:</b> | Passen Sie die Drehung der Projektion der Y-Achse an. |
| <b>Versatz Y:</b> | Passen Sie den Versatz der Projektion der Y-Achse an. |
| <b>Drehung Z:</b> | Passen Sie die Drehung der Z-Achse-Projektion an. |
| <b>Versatz Z:</b> | Passen Sie den Versatz der Z-Achse-Projektion an. |

### X-Achse

<table>
<tr>
<td><b>Drehung X:</b></td>
<td>Passen Sie die Drehung der Projektion der X-Achse-Textur an.</td>
</tr>
<tr>
<td><b>Versatz X X:</b></td>
<td>Passen Sie den Versatz der X-Achse-Projektion entlang der X-Achse an.</td>
</tr>
<tr>
<td><b>Versatz X Y:</b></td>
<td>Passen Sie den Versatz der X-Achse-Projektion entlang der Y-Achse an.</td>
</tr>
</table>

>[!NOTE]
>
> Die Versatzparameter enthalten zwei Achsen im Titel. Die erste Achse definiert die Projektion, die zweite die Offset-Achse. **Offset X Y** betrachtet also speziell die Projektion auf der X-Achse und verschiebt diese Projektion entlang der lokalen Y-Achse der Projektionen.
>
>Eine andere Denkweise ist, dass **Offset X X X** die X-Projektion **horizontal** verschiebt und **Offset X Y** die X-Projektion **vertikal** verschiebt.

### Y-Achse

<table>
<tr>
<td><b>Drehung X:</b></td>
<td>Passen Sie die Drehung der Projektion der Y-Achse-Textur an.</td>
</tr>
<tr>
<td><b>Versatz Y X:</b></td>
<td>Passen Sie den Versatz der Y-Achse-Projektion entlang der X-Achse an.</td>
</tr>
<tr>
<td><b>Versatz Y Y:</b></td>
<td>Passen Sie den Versatz der Y-Achse-Projektion entlang der Y-Achse an.</td>
</tr>
</table>

>[!NOTE]
>
> Die Versatzparameter enthalten zwei Achsen im Titel. Die erste Achse definiert die Projektion, die zweite die Offset-Achse. **Offset Y X** betrachtet also speziell die Projektion auf der Y-Achse und verschiebt diese Projektion entlang der lokalen X-Achse der Projektionen.
>
>Eine andere Denkweise ist, dass **Offset Y X** die Y-Projektion **horizontal** verschiebt und **Offset Y Y** die Y-Projektion **vertikal** verschiebt.

### Achse Z

<table>
<tr>
<td><b>Drehung X:</b></td>
<td>Passen Sie die Drehung der Z-Achse Textur Projektion an.</td>
</tr>
<tr>
<td><b>Versatz Z X:</b></td>
<td>Passen Sie den Versatz der Z-Achse-Projektion entlang der X-Achse an.</td>
</tr>
<tr>
<td><b>Versatz Z Y:</b></td>
<td>Passen Sie den Versatz der Z-Achse-Projektion entlang der Y-Achse an.</td>
</tr>
</table>

>[!NOTE]
>
> Die Versatzparameter enthalten zwei Achsen im Titel. Die erste Achse definiert die Projektion, die zweite die Offset-Achse. **Offset Z Y** betrachtet also speziell die Projektion auf der Z-Achse und verschiebt diese Projektion entlang der lokalen Y-Achse der Projektionen.
>
>Eine andere Denkweise ist, dass **Offset Z X** die Z-Projektion **horizontal** verschiebt und **Offset Z Y** die Z-Projektion **vertikal** verschiebt.
