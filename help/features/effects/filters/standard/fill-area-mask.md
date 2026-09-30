---
title: Flächenmaske füllen
description: Erfahren Sie, wie Sie den Substance 3D Painter-Filter "Flächenmaske füllen" verwenden.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 2%
---

# Flächenmaske füllen

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![Symbol für Flächenmaske füllen](./Resources/icon_fill_area_mask.png "Flächenmaske füllen")

<b>In:</b> Effekte/Füllung, Form, Umriss, Graustufen

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Beschreibung

Der Filter &quot;Flächenmaske füllen&quot; wandelt Konturen in gefüllte Formen um. Jeder Bereich mit einem durchgehenden Rahmen wird ausgefüllt.

Es wird auf einer Maskenebene (Schwarzweiß-Ausgabe) verwendet, nachdem eine Malebene zum Füllen geschlossener gemalter Striche hinzugefügt wurde.

</td>
</tr>
</table>

<a name="parameters"></a>

## Parameter

| Parametername | Beschreibung |
| --- | --- |
| <b>Bereichserkennung:</b> | Wählen Sie aus, wie der auszufüllende Bereich identifiziert wird. |
| <b>Schwellenwert für Bereichserkennung:</b> | Passen Sie den Schwellenwert für die Bereichserkennung an. |
| <b>Erkennung von Debugbereichen:</b> | Schaltet die Anzeige des Umrisses um, der von der Einstellung Bereichserkennung erkannt wird. Dies kann dazu beitragen, Bereiche zu identifizieren, die möglicherweise nicht vollständig geschlossen sind. |
| <b>UV-Randverhalten:</b> | Legen Sie fest, wie UV-Rahmen beim Ausfüllen von Bereichen behandelt werden. |
| <b>Schwellenwert für die Erkennung von UV-Rändern:</b> | Passen Sie den Schwellenwert an, der verwendet wird, um UV-Bereiche zu ignorieren, die sonst durch den Bereichserkennungsprozess ausgefüllt werden könnten. |
