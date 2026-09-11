---
title: Metal-Edge Wear
description: Erfahren Sie, wie Sie den Metal-Edge Wear-Generator von Substance 3D Painter verwenden.
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 8%

---


# Metal-Edge Wear

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_metal_edge_wear.webp" alt=""/><br><strong>In:</strong>-Maske, Generator</td>
    <td style="border: 0;" valign="top"><strong>Beschreibung</strong><br>Der Metal-Edge Wear-Generator verursacht den Anschein von Beschädigung und Verschleiß an Bereichen Ihres Meshs, die am ehesten gekratzt oder gekratzt werden.<br><br>Der Metal-Edge Wear-Generator gibt eine Schwarzweiß-Textur aus. Aus diesem Grund ist es nützlich, Masken zu generieren, um einer Ebene Kantenverschleißdetails hinzuzufügen.<br><br> Baking geführt Positions-, Krümmungen-, ambient occlusion- und Welt-Raum-Normale-Maps sind als Bildeingaben erforderlich. <a href="../../../baking/baking.md">Weitere Informationen zum Baking</a>.</td>
  </tr>
</table>

## Eingaben

| Eingabename | Beschreibung |
| --- | --- |
| **Normaler Weltraum** Farbe | Verwenden Sie die Baking geführt Welt-Raum-Normale-Map. |
| **Position** Farbe | Verwenden Sie die Baking geführt Positionszuordnung. |
| **Benutzerdefinierter Schmutz** Graustufen | Verwenden einer benutzerdefinierten Textur oder eines Ankerpunkts. |
| **Krümmung** Graustufen | Verwenden Sie die Baking geführt Krümmungs-Map. |
| **Ambient occlusion** Graustufen | Verwenden Sie die Baking geführt Ambient occlusion-Map. |
| **Micro Normal** Farbe | Verwenden Sie eine spezielle normale Textur oder einen Ankerpunkt. |
| **Micro Height** Color | Verwenden einer benutzerdefinierten Textur oder eines Ankerpunkts. |

## Parameter

<table>
  <tr>
    <th>Parametername</th>
    <th>Beschreibung</th>
  </tr>
  <tr>
    <td><strong>Zufalls-Startwert</strong></td>
    <td>Legen Sie den Startwert fest, der zum Generieren der Textur des Dirts verwendet wird. <br><ul><li>Klicken Sie auf "Zufällig", um zu einer anderen Zufallsverteilung zu wechseln.</li><li>Klicken Sie auf den Stift, um den aktuellen Wert für das Seed anzuzeigen, und geben Sie bei Bedarf einen bestimmten Wert ein.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Invertieren</strong></td>
    <td>Umkehren der Verschleißmaske der Metallkanten.</td>
  </tr>
  <tr>
    <td><strong>Abnutzungsstufe</strong></td>
    <td>Stellen Sie den Gesamtverschleiß ein.</td>
  </tr>
  <tr>
    <td><strong>Abnutzungskontrast</strong></td>
    <td>Passen Sie den Kontrast des endgültigen Verschleißergebnisses an.</td>
  </tr>
  <tr>
    <td><strong>Triplanar verwenden</strong></td>
    <td>Wenn <strong>Triplanar </strong> verwenden aktiviert ist, wird die Textur aus drei Richtungen projiziert (X-, Y-, Z-Achsen), anstatt sich nur auf UVs zu verlassen. <br><ul><li>Ohne die Option "Triplanar" folgt die Textur dem UV-Layout.</li><li>Wenn die Option "Dreidimensional" aktiviert ist, wird die Textur aus mehreren Winkeln projiziert und verblendet.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Triplanarer Überblendkontrast</strong></td>
    <td>Passen Sie an, wie glatt eine Textur übergeht, wenn sie mithilfe von triplanarem Mapping projiziert wird. Dadurch wird die Weichheit der Überblendung zwischen den Projektionen aus jeder Richtung angepasst.</td>
  </tr>
  <tr>
    <td><strong>Schmutzmenge</strong></td>
    <td>Passen Sie die Anzahl der Schmutz-Details an.</td>
  </tr>
  <tr>
    <td><strong>Schmutzstufe</strong></td>
    <td>Passen Sie die Skalierung der Schmutz-Details an.</td>
  </tr>
  <tr>
    <td><strong>Benutzerdefinierten Schmutz verwenden</strong></td>
    <td>Schalten Sie die Verwendung einer benutzerdefinierten Schmutz-Karte ein oder aus.</td>
  </tr>
  <tr>
    <td><strong>Kantenglättung</strong></td>
    <td>Passe die Smoothness der Kanten an.</td>
  </tr>
  <tr>
    <td><strong>Maskierung Umgebungsverdeckung</strong></td>
    <td>Verwenden Sie den ambient occlusion als Maske, um zu verhindern, dass verdeckte Bereiche den Effekt "Verwitterung" erhalten.</td>
  </tr>
  <tr>
    <td><strong>Biegungsstärke</strong></td>
    <td>Passen Sie an, wie stark der Krümmungs-Map das Endergebnis beeinflusst. Die Kurvenzeichner-Map wird verwendet, um Kanten zu definieren, sodass eine sehr niedrige Kurvenzeichner-Gewichtung alle Kanten verschleißen kann, sodass nur der Schmutz übrig bleibt.</td>
  </tr>
</table>

### Mikrodetails

<table>
  <tr>
    <th>Parametername</th>
    <th>Beschreibung</th>
  </tr>
  <tr>
    <td><strong>Mikrohöhe</strong></td>
    <td>Aktivieren oder deaktivieren Sie die Verwendung einer benutzerdefinierten Micro Höhen-Map.</td>
  </tr>
  <tr>
    <td><strong>Mikro-Normale</strong></td>
    <td>Aktivieren oder deaktivieren Sie die Verwendung einer benutzerdefinierten Micro Normalen-Map.</td>
  </tr>
  <tr>
    <td><strong>Biegungstyp</strong></td>
    <td>Legen Sie die Krümmung fest. <br><ul><li><strong>Standard</strong>: Erstellt ein normalerweise recht scharfes Ergebnis, kann jedoch größere Details vermissen lassen.</li><li><strong>Sobel</strong>: Ergibt ähnliche Ergebnisse wie bei der Standardausgabe, ist jedoch leicht unscharf, da die Normalen-Map mit einem Sobel-Filter ausgewertet wird.</li><li><strong>Glatt</strong>: Erzeugt verschiedene Weichzeichnungsstufen (wie Mipmaps), um Informationen zu sammeln. Dadurch entstehen in der Regel glattere Kurven, aber Details können verloren gehen.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Biegungsstärke</strong></td>
    <td>Passen Sie die Intensität der Krümmung im <strong>Standardmodus </strong> und im <strong>Sobelmodus </strong>Krümmung an.</td>
  </tr>
  <tr>
    <td><strong>Höhendetailstärke</strong></td>
    <td>Passen Sie die Intensität der Height-Details an.</td>
  </tr>
  <tr>
    <td><strong>AO-Radius</strong></td>
    <td>Passen Sie den Radius (Bereich) der Verdeckung "Umgebung" in den Mikrodetails an.</td>
  </tr>
  <tr>
    <td><strong>AO-Tiefe</strong></td>
    <td>Passen Sie die Tiefe (Intensität) des Ambient occlusion in Mikrodetails an.</td>
  </tr>
</table>
