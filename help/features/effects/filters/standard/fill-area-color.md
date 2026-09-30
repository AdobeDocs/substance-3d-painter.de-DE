---
title: Flächenfarbe
description: Erfahren Sie, wie Sie den Substance 3D Painter-Filter "Flächenfarbe" verwenden.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 1%
---

# Flächenfarbe

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![Symbol für Flächenfarbe](./Resources/icon_fill_area_color.png "Flächenfarbe")

<b>In:</b> Effekte/Füllung, Form, Umriss, RGBA, Farbe

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Beschreibung

Der Filter &quot;Flächenfarbe&quot; wandelt Konturen in gefüllte Formen um. Jeder Bereich mit einem durchgehenden Rahmen wird ausgefüllt. Die Farbversion verwendet Alpha, um die Bereichsgrenzen zu bestimmen.

Es wird auf einer Malebene (Farbkanal) verwendet, um gemalte Striche zu füllen.

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
| <b>Schwellenwert für UV-Rahmen:</b> | Passen Sie den Schwellenwert an, der verwendet wird, um UV-Bereiche zu ignorieren, die sonst durch den Bereichserkennungsprozess ausgefüllt werden könnten. |
| <b>Farbmodus:</b> | Wählen Sie die Methode aus, die zum Füllen der Innenseite des Bereichs verwendet wird. |
| <b>Füllfarbe:</b> | Passe die Flächenfarbe an. |
| <b>Weichzeichnungsintensität:</b> | Passe die Weichzeichnungsintensität an. |
| <b>Weichzeichnerbeispiele:</b> | Passen Sie die Anzahl der Weichzeichnungsproben an. |
| <b>Diffusion Iterationen:</b> | Passen Sie die Anzahl der auszuführenden Diffusion-Iterationen an. Höhere Werte verbessern das Ergebnis, sind jedoch langsamer. Nützliche Werte liegen im Bereich [8, 48]. |
