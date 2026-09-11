---
title: Graustufenkonvertierung
description: Erfahren Sie, wie Sie den Graustufenkonvertierung-Generator von Substance 3D Painter verwenden.
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 7%

---


# Graustufenkonvertierung

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_grayscale_conversion.png" alt=""/><br><strong>In:</strong> Generator, Graustufen, Farbe</td>
    <td style="border: 0;" valign="top"><strong>Beschreibung</strong><br>Der Graustufen-Konvertierungsgenerator konvertiert eine Textur oder Map in Graustufenwerte.<br><br>Der Graustufen-Konvertierungsgenerator gibt eine monochrome (Schwarz-Weiß-)Textur aus. Daher eignet sie sich gut zum Generieren von Masken von einem Vollfarben-Eingabe-Map.</td>
  </tr>
</table>

## Eingaben

| Eingabename | Beschreibung |
| --- | --- |
| **Quellfarbe** | Mit einer eigenen Textur oder einem Ankerpunkt |

## Parameter

<table>
  <tr>
    <th>Parametername</th>
    <th>Beschreibung</th>
  </tr>
  <tr>
    <td><strong>Graustufentyp</strong></td>
    <td>Legen Sie die Graustufen-Konvertierungsmethode fest: <br><ul><li><strong>Entsättigung</strong>: Verwendet den Wert auf halbem Weg zwischen dem stärksten und dem schwächsten der RGB-Kanäle.</li><li><strong>Luminanz</strong>: Verwendet gewichtete RGB-Koeffizienten, die die wahrgenommene Helligkeit mit dem menschlichen Auge abgleichen (wobei Grün bevorzugt wird).</li><li><strong>Durchschnitt</strong>: Mischt die roten, grünen und blauen Kanäle in gleichen Mengen.</li><li><strong>Max</strong>: Verwendet den höchsten Wert aus den RGB-Kanälen.</li><li><strong>Min</strong>: Verwendet den niedrigsten Wert aus den RGB-Kanälen.<ul><li>Roter Kanal: Verwendet nur den roten Kanal.</li><li>Grüner Kanal: Verwendet nur den grünen Kanal.</li><li>Blauer Kanal: Verwendet nur den blauen Kanal.</li></ul></li></ul></td>
  </tr>
  <tr>
    <td><strong>Invertieren</strong></td>
    <td>Kehrt die Maske um.</td>
  </tr>
  <tr>
    <td><strong>Balance</strong></td>
    <td>Passt die Balance des konvertierten Quellbilds an und verschiebt den Mittelpunkt wie bei einem Helligkeitsregler in Richtung Schwarz oder Weiß.</td>
  </tr>
  <tr>
    <td><strong>Kontrast</strong></td>
    <td>Definiert den Kontrast/Abfall des konvertierten Quellbilds.</td>
  </tr>
  <tr>
    <td><strong>Kachel</strong></td>
    <td>Legt die Unterteilung des konvertierten Quellbilds fest.</td>
  </tr>
  <tr>
    <td><strong>Drehung</strong></td>
    <td>Ändert den Winkel des konvertierten Quellbilds.</td>
  </tr>
  <tr>
    <td><strong>Sichere Drehung</strong></td>
    <td>Schaltet den abgesicherten Rotationsmodus ein bzw. aus. Bei "true" sperrt die sichere Drehung die Drehung auf 45-Grad-Winkel.</td>
  </tr>
</table>
