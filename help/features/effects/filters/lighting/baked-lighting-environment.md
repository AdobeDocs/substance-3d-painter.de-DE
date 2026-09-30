---
title: Umgebung mit vorberechnete Beleuchtung
description: Erfahren Sie, wie Sie den Substance 3D Painter-Filter "Umgebung mit vorberechnete Beleuchtung" verwenden.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 2%
---

# Umgebung mit vorberechnete Beleuchtung

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![Umgebung mit vorberechnete Beleuchtung-Symbol](./Resources/icon_baked_lighting_environment.png "Umgebung mit vorberechnete Beleuchtung")

<b>In:</b> Effekte/Beleuchtung, Baking, Umgebung, PBR

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Beschreibung

Der Filter &quot;Umgebung mit vorberechnete Beleuchtung&quot; Baking führe Material- und Umgebungsbeleuchtungsinformationen in den Farbkanal.

Es wird auf einer Malebene verwendet, die auf den Durchlaufmodus eingestellt und auf alle Kanäle angewendet ist. Sie ist nützlich für stilisierte Workflows, bei denen keine präzise simulierte Beleuchtung erforderlich ist oder wenn Ressourcen eingeschränkt sind, z. B. für mobile Projekte oder Assets, die nur auf einer Farbkarte basieren.

</td>
</tr>
</table>

## Eingaben

| Eingabename | Beschreibung |
| --- | --- |
| <b>Ambient occlusion:</b> Graustufen | Verwenden Sie die Baking geführt Ambient occlusion-Map. |
| <b>Umgebungs-Map:</b> Graustufen | Verwenden Sie die Umgebungs-Map. |
| <b>Normal:</b> Farbe | Verwenden Sie die Baking geführt Normalen-Map. |

<a name="parameters"></a>

## Parameter

| Parametername | Beschreibung |
| --- | --- |
| <b>Horizontale Drehung:</b> | Passen Sie die horizontale Drehung der Umgebungsbeleuchtung an. |
| <b>Vertikale Drehung:</b> | Passen Sie die vertikale Drehung der Umgebungsbeleuchtung an. |
| <b>Belichtung:</b> | Passen Sie die Belichtung des Baking geführt Ergebnisses an. |
| <b>Height-Intensität:</b> | Passen Sie an, wie stark Height-Informationen das Ergebnis beeinflussen. |
| <b>Ambient occlusion-Intensität:</b> | Passe die Intensität des ambient occlusion in den Baking an. |
| <b>Intensität der Specular-Verdeckung:</b> | Passen Sie die Intensität der Specular-Verdeckung im Baking an. |
