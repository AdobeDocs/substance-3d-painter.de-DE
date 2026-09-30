---
title: Baking geführt Beleuchtung stilisiert
description: Erfahren Sie, wie Sie den stilisierten Filter "Baking geführt Beleuchtung" von Substance 3D Painter verwenden.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '651'
ht-degree: 1%
---

# Baking geführt Beleuchtung stilisiert

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![Symbol für stilisierte Beleuchtung Baking geführt](./Resources/icon_baked_lighting_stylized.png "Symbol für stilisierte Beleuchtung Baking geführt")

<b>In:</b> Effekte/stilisiert, hell, Farbe

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Beschreibung

Der Baking geführt stilisierte Beleuchtungsfilter Baking führe Material- und Beleuchtungsinformationen in den Farbkanal.

Es wird auf einer Malebene verwendet, die auf den Durchlaufmodus eingestellt und auf alle Kanäle angewendet ist. Sie ist nützlich für stilisierte Workflows, bei denen keine präzise simulierte Beleuchtung erforderlich ist oder wenn Ressourcen eingeschränkt sind, z. B. für mobile Projekte oder Assets, die nur auf einer Farbkarte basieren.

</td>
</tr>
</table>

## Eingaben

| Eingabename | Beschreibung |
| --- | --- |
| <b>Ambient occlusion:</b> Graustufen | Verwenden Sie die Baking geführt Ambient occlusion-Map. |
| <b>Krümmung:</b> Graustufen | Verwenden Sie die Baking geführt Krümmungs-Map. |
| <b>Normal:</b> Farbe | Verwenden Sie die Baking geführt Normalen-Map. |
| <b>Welt-Raum-Normale:</b> Farbe | Verwenden Sie die Baking geführt Welt-Raum-Normale-Map. |

<a name="parameters"></a>

## Parameter

| Parametername | Beschreibung |
| --- | --- |
| <b>Eingabe:</b> | Wählen Sie den Workflow für das Eingabe-Material aus. |
| <b>Ausgabe:</b> | Wählen Sie den Ausgabemodus. |
| <b>Dielektrische Reflexion:</b> | Passen Sie den dielektrischen Reflexionsgrad an. |
| <b>Diffuse AO:</b> | Passen Sie den ambient occlusion-Beitrag für die diffuse Beleuchtung an. |
| <b>Diffuse-Kavität:</b> | Passen Sie den Hohlraumbeitrag zur diffusen Beleuchtung an. |
| <b>Specular AO:</b> | Passen Sie den ambient occlusion-Beitrag für die Specular-Beleuchtung an. |
| <b>Specular-Kavität:</b> | Passen Sie den Hohlraumbeitrag zur Specular-Beleuchtung an. |
| <b>Smoothness der Kavität:</b> | Passen Sie die Smoothness des Hohlraumeffekts an. |
| <b>Kantenintensität:</b> | Passen Sie die Intensität des Kanteneffekts an. |
| <b>Kanten-Smoothness:</b> | Passen Sie die Smoothness des Kanteneffekts an. |
| <b>Typ für normale Details:</b> | Wählen Sie aus, welche normalen Details verwendet werden. |
| <b>Height auf Normalintensität:</b> | Passen Sie die Intensität der Umwandlung von Height in Normalzustand an. |
| <b>Sonnenintensität:</b> | Passe die Intensität des Sonnenlichts an. |
| <b>Horizontaler Sonnenwinkel:</b> | Passen Sie den horizontalen Winkel des Sonnenlichts an. |
| <b>Vertikaler Sonnenwinkel:</b> | Den vertikalen Winkel des Sonnenlichts anpassen. |
| <b>Sonnenfarbe:</b> | Passen Sie die Farbe des Sonnenlichts an. |
| <b>Sky-Intensität:</b> | Passe die Intensität des Himmels an. |
| <b>Himmelsfarbe:</b> | Die Farbe des Himmels anpassen. |
| <b>Horizontfarbe:</b> | Passe die Farbe des Horizontlichts an. |
| <b>Farbe des Bodens:</b> | Passen Sie die Lichtfarbe des Bodens an. |
| <b>Horizontaler Winkel:</b> | Passe den horizontalen Winkel des zusätzlichen Lichts an. |
| <b>Vertikaler Winkel:</b> | Passen Sie den vertikalen Winkel des zusätzlichen Lichts an. |
| <b>Intensität:</b> | Passe die Intensität des zusätzlichen Lichts an. |
| <b>Farbe:</b> | Passe die Farbe des zusätzlichen Lichts an. |
| <b>Horizontaler Winkel:</b> | Passe den horizontalen Winkel des zweiten zusätzlichen Lichts an. |
| <b>Vertikaler Winkel:</b> | Passen Sie den vertikalen Winkel des zweiten zusätzlichen Lichts an. |
| <b>Intensität:</b> | Passe die Intensität des zweiten zusätzlichen Lichts an. |
| <b>Farbe:</b> | Passe die Farbe des zweiten zusätzlichen Lichts an. |

### Material

<table>
<tr>
<td><b>Dielektrischer Reflexionsgrad:</b></td>
<td>Stellen Sie den dielektrischen Reflexionsgrad ein.</td>
</tr>
<tr>
<td><b>Diffuse AO:</b></td>
<td>Steuere, wie stark das ambient occlusion die Streuungsdetails beeinflusst.</td>
</tr>
<tr>
<td><b>Diffuse Kavität:</b></td>
<td>Lege fest, wie stark die Hohlräume die diffusen Details beeinflussen.</td>
</tr>
<tr>
<td><b>Specular AO:</b></td>
<td>Legen Sie fest, wie stark das ambient occlusion die Specular-Details beeinflusst.</td>
</tr>
<tr>
<td><b>Specular-Hohlraum:</b></td>
<td>Passen Sie an, wie stark die Hohlraumbereiche die Specular-Details beeinflussen.</td>
</tr>
<tr>
<td><b>Smoothness der Kavität:</b></td>
<td>Passen Sie an, wie weich die Hohlraumbereiche angezeigt werden.</td>
</tr>
<tr>
<td><b>Kantenintensität:</b></td>
<td>Legen Sie die Stärke der Kantendetails fest.</td>
</tr>
<tr>
<td><b>Kanten-Smoothness:</b></td>
<td>Passen Sie die Smoothness der Kantenbereiche an.</td>
</tr>
<tr>
<td><b>Normale Detailart:</b></td>
<td>Wählen Sie aus, welche Details für die Normalen verwendet werden: Nur Mesh oder Mesh + Height + Normal.</td>
</tr>
<tr>
<td><b>Height bis Normalintensität:</b></td>
<td>Passen Sie die Stärke der generierten Normalendetails an.</td>
</tr>
</table>

### Sonne und Himmel

<table>
<tr>
<td><b>Sonnenintensität:</b></td>
<td>Kontrolliere die Stärke der Sonne.</td>
</tr>
<tr>
<td><b>Horizontaler Sonnenwinkel:</b></td>
<td>Passen Sie den horizontalen Winkel der Sonne an.</td>
</tr>
<tr>
<td><b>Vertikaler Sonnenwinkel:</b></td>
<td>Passen Sie den vertikalen Winkel der Sonne an.</td>
</tr>
<tr>
<td><b>Farbe der Sonne:</b></td>
<td>Lege die Farbe der Sonne fest.</td>
</tr>
<tr>
<td><b>Sky-Intensität:</b></td>
<td>Die Stärke des Himmels anpassen.</td>
</tr>
<tr>
<td><b>Himmelsfarbe:</b></td>
<td>Lege die Farbe des Himmels fest.</td>
</tr>
<tr>
<td><b>Horizontfarbe:</b></td>
<td>Passe die Farbe des Horizonts an.</td>
</tr>
<tr>
<td><b>Farbe des Bodens:</b></td>
<td>Legen Sie die Farbe des Bodens fest.</td>
</tr>
</table>

### Licht 1

<table>
<tr>
<td><b>Horizontaler Winkel:</b></td>
<td>Passe den horizontalen Winkel des zusätzlichen Lichts an.</td>
</tr>
<tr>
<td><b>Vertikaler Winkel:</b></td>
<td>Passen Sie den vertikalen Winkel des zusätzlichen Lichts an.</td>
</tr>
<tr>
<td><b>Intensität:</b></td>
<td>Passe die Stärke des zusätzlichen Lichts an.</td>
</tr>
<tr>
<td><b>Farbe:</b></td>
<td>Legen Sie die Farbe des zusätzlichen Lichts fest.</td>
</tr>
</table>

### Licht 2

<table>
<tr>
<td><b>Horizontaler Winkel:</b></td>
<td>Passe den horizontalen Winkel des zweiten zusätzlichen Lichts an.</td>
</tr>
<tr>
<td><b>Vertikaler Winkel:</b></td>
<td>Passen Sie den vertikalen Winkel des zweiten zusätzlichen Lichts an.</td>
</tr>
<tr>
<td><b>Intensität:</b></td>
<td>Passe die Stärke des zweiten zusätzlichen Lichts an.</td>
</tr>
<tr>
<td><b>Farbe:</b></td>
<td>Legt die Farbe des zweiten zusätzlichen Lichts fest.</td>
</tr>
</table>
