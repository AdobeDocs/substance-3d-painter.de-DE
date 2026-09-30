---
title: PBR-Validierung
description: Erfahren Sie, wie Sie den PBR-Validierungen-Filter von Substance 3D Painter verwenden.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '117'
ht-degree: 2%
---

# PBR-Validierung

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![PBR-Validierung-Symbol](./Resources/icon_pbr_validate.png "PBR-Validierung")

<b>In:</b> Effects/pbr, metallic, Rauheit

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Beschreibung

Der Datenfilter validiert PBR-PBR-Validierungen, indem er Dunkelwerte der Albedo und Reflexionsbereiche aus Metall überprüft.

Es wird auf einer Füllebene verwendet, um zu überprüfen, ob die Material-Werte innerhalb der erwarteten PBR-Bereiche bleiben. PBR-Validierungen sollten beim Exportieren von Materialien nicht aktiviert sein.

</td>
</tr>
</table>

<a name="parameters"></a>

## Parameter

| Parametername | Beschreibung |
| --- | --- |
| <b>Validierungsmodus:</b> | Legen Sie fest, ob Albedo, Metallreflexion oder beides validiert werden soll. |
| <b>Schwellenwert für dunklen Bereich der Albedo:</b> | Wählen Sie den minimalen zulässigen Dunkelwert-Schwellenwert für die Validierung der Albedo aus. |
| <b>Reflexionsbereich des Metalls:</b> | Wählen Sie den Reflexionsbereich aus, der zur Validierung metallic Werte verwendet wird. |
| <b>Überlagerungszuordnung:</b> | Schalten Sie die Überprüfungsüberlagerung über den Kartendaten um. |

