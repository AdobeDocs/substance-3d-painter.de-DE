---
title: MatFX Peeling-Malen
description: Erfahren Sie, wie Sie den MatFX Peeling-Malen-Filter von Substance 3D Painter verwenden.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '295'
ht-degree: 2%
---

# MatFX Peeling-Malen

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![MatFX-Peeling-Malen-Symbol](./Resources/icon_matfx_peeling_paint.png "MatFX-Peeling-Malen")

<b>In:</b> Effekte/Weichzeichnen, Graustufen

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Beschreibung

Der MatFX Peeling-Malen-Filter erzeugt Flaking- und Peeling-Malen-Effekte.

Es wird auf Textur-Ebenen oder Material-Stapeln verwendet, um Peeling-Malen, Splitterbeschichtungen und den leg darunter liegenden Materials zu simulieren.

</td>
</tr>
</table>

>[!NOTE]
>
> Um ein zugrunde liegendes Material legen, verwenden Sie die MatFX Peeling-Malen in einer Gruppe. Ebenen, die sich außerhalb der Gruppe und unterhalb der Gruppe im Ebenenstapel befinden, werden gelegt, wenn sich der geschälte Malen von der Fläche löst.

<a name="parameters"></a>

## Parameter

| Parametername | Beschreibung |
| --- | --- |
| <b>Weichzeichnungsintensität:</b> | Passen Sie die Stärke des Unschärfe-Effekts an. |
| <b>Weichzeichnungsumbruch:</b> | Weichzeichnungsumbruch ein/aus. Wenn diese Option aktiviert ist, nimmt der Effekt Pixel von der gegenüberliegenden Seite der Textur auf. |
| <b>Peeling-Level:</b> | Passen Sie den allgemeinen Peeling-Pegel an. |
| <b>Peelingabstand:</b> | Passen Sie an, wie weit die Malen vom Bildschirm abgezogen werden soll. |
| <b>Flake-Level:</b> | Passen Sie die Stärke des Flakens an. |
| <b>Luftblasendichte:</b> | Passen Sie die Dichte der Luftblasen an. |
| <b>Abplatzdichte:</b> | Passen Sie die Dichte des Flockens an. |
| <b>X-Wert für Flackern:</b> | Passen Sie die Stärke des Abplatzens entlang der X-Achse an. |
| <b>Anzahl der Flackern in Y:</b> | Passen Sie die Stärke des Abplatzens entlang der Y-Achse an. |
| <b>Krümmung verwenden:</b> | Verwenden der Krümmung-Eingabe umschalten. |
| <b>Krümmung:</b> | Passen Sie den Sampling-Abstand für die Krümmung an. |
| <b>Kontrast der Krümmung:</b> | Passen Sie den Kontrast der Krümmung an. |

### Technische Parameter

Mit diesen Parametern können Sie die obere Fläche des geschälten Materials ändern.

| Parametername | Beschreibung |
| --- | --- |
| <b>Luminanz:</b> | Passe die Luminanz an. |
| <b>Kontrast:</b> | Passen Sie den Kontrast oder den Tonfall des Ergebnisses an. |
| <b>Farbtonverschiebung:</b> | Passe den Farbton an. |
| <b>Sättigung:</b> | Passe die Sättigung an. |
| <b>Normalintensität:</b> | Passe die normale Intensität an. |
| <b>Height-Bereich:</b> | Passen Sie den vom Height verwendeten Bereich an. |
| <b>Height-Position:</b> | Passen Sie die Position des Heights an, das vom Effekt verwendet wird. |
| <b>Ambient occlusion-Intensität:</b> | Passe die Intensität des ambient occlusion an. |
