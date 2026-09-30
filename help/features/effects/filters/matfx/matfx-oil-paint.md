---
title: MatFX Öl-Malen
description: Erfahren Sie, wie Sie den MatFX Oil Malen-Filter von Substance 3D Painter verwenden.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 3%
---

# MatFX Öl-Malen

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![MatFX Oil Malen-Symbol](./Resources/icon_matfx_oil_paint.png "MatFX Oil-Malen")

<b>In:</b> Effekte/Weichzeichnen, Graustufen

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Beschreibung

Der Malen-Filter MatFX Oil stilisiert die Quelle mit einem Öl-Malen-Erscheinungsbild.

Es wird für Texturen verwendet, um malerische Konturen, Farbvariationen und Oberflächendetails zu erstellen, die vom Öl-Malen inspiriert wurden.

</td>
</tr>
</table>

## Eingaben

| Eingabename | Beschreibung |
| --- | --- |
| <b>Bildeingabe:</b> Farbe | Verwenden Sie die Bildeingabe. |

<a name="parameters"></a>

## Parameter

**Vorgaben** sind verfügbar und können mehrere andere Parameter im Filter schnell aktualisieren, um als Ausgangspunkt zu fungieren.

>[!NOTE]
>
> Wenn eine Vorgabe ausgewählt ist, werden alle Parameter auf einen voreingestellten Wert festgelegt. Wenn Sie Änderungen an dem Filter vorgenommen haben, die Sie nicht verlieren möchten, kann es sich lohnen, ein Duplikat des Filters zu erstellen und die Sichtbarkeit zu ändern, bevor Sie Vorgaben ausprobieren.

| Parametername | Beschreibung |
| --- | --- |
| <b>Eingabetyp:</b> | Wählen Sie den vom Effekt verwendeten Eingabetyp aus. |
| <b>Effektintensität:</b> | Passen Sie die Gesamtintensität des Effekts an. |
| <b>Feindetails:</b> | Passen Sie die Detailgenauigkeit an, die im Ergebnis erhalten bleibt. |
| <b>Schärfe:</b> | Passen Sie die Schärfe des Ergebnisses an. |
| <b>Rauheit:</b> | Passen Sie den Wert für die Rauheit an. |
| <b>Variation der Rauheit:</b> | Passen Sie die Variation der Rauheit im Ergebnis an. |
| <b>Details zur Rauheit:</b> | Passen Sie die Detailgenauigkeit der Rauheit an. |
| <b>Normalintensität:</b> | Passe die Intensität des Effekts an. |
| <b>Richtungseinfluss für normale Striche:</b> | Passen Sie an, wie stark die Strichrichtung das normale Ergebnis beeinflusst. |

### Eingabefarbkorrektur

| Parametername | Beschreibung |
| --- | --- |
| <b>Eingabebild-Kontrast:</b> | Passe den Kontrast des Eingabebilds an. |
| <b>Eingabebild-Farbton:</b> | Passen Sie den Farbton des Eingabebilds an. |
| <b>Eingabebild-Sättigung:</b> | Passe die Sättigung des Eingabebilds an. |
| <b>Eingabebild-Luminanz:</b> | Passen Sie die Luminanz des Eingabebilds an. |

### Konturen

| Parametername | Beschreibung |
| --- | --- |
| <b>Globaler Skalierungsmultiplikator:</b> | Passen Sie den globalen Skalierungsmultiplikator für die Striche an. |
| <b>Zufällige Skalierung:</b> | Passen Sie die Stärke der Zufallsskalierung an. |
| <b>Größe:</b> | Passen Sie die Konturgröße an. |
| <b>Zufällige Größe:</b> | Passen Sie die Stärke der zufälligen Größenvariation an. |
| <b>Zufallsfarbe:</b> | Passen Sie die Stärke der zufälligen Farbvariation an. |
| <b>Konturen-Härte:</b> | Passen Sie die Härte der Konturen an. |
| <b>Automatischer Ausrichtungsvervielfacher:</b> | Passen Sie an, wie stark die automatische Ausrichtung die Konturen beeinflusst. |
| <b>Smoothness der Ausrichtung:</b> | Passen Sie die Smoothness der Strichausrichtung an. |

### Lichter

| Parametername | Beschreibung |
| --- | --- |
| <b>Aktiviert:</b> | Schalte die Lichtebene ein oder aus. |
| <b>Raster-Unterteilung:</b> | Passen Sie die Raster-Unterteilung für die Lichtebene an. |
| <b>Konturgröße:</b> | Passe die Konturgröße der Lichterebene an. |
| <b>Konturgröße aus Details:</b> | Passe an, wie viele Details die Konturgröße in der Lichtebene beeinflussen. |
| <b>Verkrümmungsintensität:</b> | Passe die Verkrümmungsintensität der Lichtebene an. |

### Mitteltöne

| Parametername | Beschreibung |
| --- | --- |
| <b>Aktiviert:</b> | Schalte die Mitteltöne ein oder aus. |
| <b>Raster-Unterteilung:</b> | Passen Sie die Raster-Unterteilung für die Mitteltonebene an. |
| <b>Konturgröße:</b> | Passen Sie die Konturgröße der Mitteltonebene an. |
| <b>Konturgröße aus Details:</b> | Ändere die Stärke der Kontur in den Mitteltönen. |
| <b>Verkrümmungsintensität:</b> | Passen Sie die Verkrümmungsintensität der Mitteltonebene an. |

### Schatten

| Parametername | Beschreibung |
| --- | --- |
| <b>Aktiviert:</b> | Schalte die Schatten-Ebene ein oder aus. |
| <b>Raster-Unterteilung:</b> | Passen Sie die Raster-Unterteilung an, die für die Schattenebene verwendet wird. |
| <b>Konturgröße:</b> | Passen Sie die Konturgröße an, die für die Schatten-Ebene verwendet wird. |
| <b>Konturgröße aus Details:</b> | Ändere die Stärke der Kontur in der Schatten-Ebene. |
| <b>Verkrümmungsintensität:</b> | Passe die Verkrümmungsintensität der Schatten-Ebene an. |

### Hintergrund

| Parametername | Beschreibung |
| --- | --- |
| <b>Aktiviert:</b> | Schalte die Hintergrundebene ein oder aus. |
| <b>Raster-Unterteilung:</b> | Passen Sie die Raster-Unterteilung für die Hintergrundebene an. |
| <b>Konturgröße:</b> | Passen Sie die Konturgröße an, die für die Hintergrundebene verwendet wird. |
| <b>Verkrümmungsintensität:</b> | Passe die Verkrümmungsintensität der Hintergrundebene an. |

### Kontur

| Parametername | Beschreibung |
| --- | --- |
| <b>Betrag:</b> | Passen Sie den Konturbetrag an. |
| <b>Thickness:</b> | Passen Sie die Thickness der Kontur an. |

### Arbeitsfläche

| Parametername | Beschreibung |
| --- | --- |
| <b>Intensität der Textur:</b> | Passen Sie die Intensität der Textur der Arbeitsfläche an. |
| <b>Anzahl der Fasern:</b> | Passen Sie die Anzahl der Leinwandfasern an. |
