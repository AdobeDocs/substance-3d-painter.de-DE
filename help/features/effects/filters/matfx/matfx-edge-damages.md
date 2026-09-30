---
title: MatFX Edge Damages
description: Erfahren Sie, wie Sie den Substance 3D Painter-Kantenschadensfilter MatFX verwenden.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 1%
---

# MatFX Edge Damages

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![MatFX Edge Damages-Symbol](./Resources/icon_matfx_edge_damages.png "MatFX Edge Damages")

<b>In:</b> Effekte/Weichzeichnen, Graustufen

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Beschreibung

Der MatFX Edge Damages-Filter erzeugt zersplitterte und beschädigte Kantendetails. Edge Damage verhält sich anders als der MatFX Detail Edge Wear-Filter, da Edge Damage die Farbe des beschädigten Bereichs nicht ändert. Dies bedeutet, dass es für die Simulation von Schäden an Materialien wie Kunststoff oder Harz besser geeignet sein kann als Edge Wear, der besser für Materialien wie lackiertes Metall verwendet wird.

MatFX Edge Damages wird auf Texturen oder Material-Stapeln verwendet, um verschlissene, zerkratzte und beschädigte Kantendetails hinzuzufügen.

</td>
</tr>
</table>

>[!NOTE]
>
> Damit der MatFX-Kantenschadensfilter den Kanal des Heights ändern kann, müssen bereits vorhandene Height-Daten im Kanal vorhanden sein. Wenn also keine Ebenen unterhalb der Filterebene vorhanden sind, die über Height-Daten verfügen, hat der Filter keine erkennbare Auswirkung auf den Height-Kanal.

<a name="parameters"></a>

## Parameter

| Parametername | Beschreibung |
| --- | --- |
| <b>Weichzeichnungsintensität:</b> | Passen Sie die Stärke des Unschärfe-Effekts an. |
| <b>Weichzeichnungsumbruch:</b> | Weichzeichnungsumbruch ein/aus. Wenn diese Option aktiviert ist, nimmt der Effekt Pixel von der gegenüberliegenden Seite der Textur auf. |
| <b>Ebene:</b> | Passen Sie die Schadenshöhe insgesamt an. |
| <b>Kontrast:</b> | Passen Sie den Kontrast oder den Tonfall des Ergebnisses an. |
| <b>Intensität der Scratches:</b> | Passen Sie die Intensität der Kratzer an. |
| <b>Beschädigte Rauheit:</b> | Passen Sie die Rauheit der beschädigten Bereiche an. |
| <b>Beschädigte Tiefe:</b> | Passen Sie die Tiefe der beschädigten Bereiche an. |
