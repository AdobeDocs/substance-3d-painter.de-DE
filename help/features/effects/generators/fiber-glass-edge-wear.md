---
title: Glasfaser-Edge Wear
description: Erfahren Sie, wie Sie den Glasfaser-Edge Wear-Generator von Substance 3D Painter verwenden.
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '533'
ht-degree: 8%

---


# Glasfaser-Edge Wear

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_fiber_glass_edge_wear.webp" alt=""/><br><strong>In:</strong>-Maske, Generator</td>
    <td style="border: 0;" valign="top"><strong>Beschreibung</strong><br>Der Edge Wear-Generator für Glasfaser fügt realistischen Kantenverschleiß und Ausfransungsdetails auf der Grundlage von Karten mit gebackener Krümmung und umgebender Verdeckung hinzu. Optional können Sie auch Micro Height- und Micro Normal-Maps verwenden, um weitere Details anzuzeigen.<br><br>Der Edge Wear-Generator für Glasfaser gibt eine monochrome (schwarz-weiß) Textur aus. Aus diesem Grund ist es nützlich, Masken zu generieren, um einer Ebene Details zum Verschleiß von Glasfaserkanten hinzuzufügen.<br><br>Als Bildeingabe sind die gebackene Position, die Krümmung, die Umgebungs-Verdeckung und die Weltraum-Normalmaps erforderlich. <a href="../../../baking/baking.md">Weitere Informationen zum Backen</a>.</td>
  </tr>
</table>

## Eingaben

| Eingabename | Beschreibung |
| --- | --- |
| **Benutzerdefinierter Schmutz** Graustufen | Verwenden einer benutzerdefinierten Struktur oder eines Ankerpunkts. |
| **Krümmung** Graustufen | Verwenden Sie die Kurvenzeichner-Map. |
| **Umgebungs-Verdeckung** Graustufen | Verwenden Sie die Karte mit der Verdeckung &quot;Umgebung&quot;. |
| **Normaler Weltraum** Farbe | Verwenden Sie die gebackene Weltraumnormalkarte. |
| **Position** Farbe | Verwenden Sie die Positionskarte. |
| **Micro Normal** Farbe | Verwenden Sie eine spezielle normale Textur oder einen Ankerpunkt. |
| **Micro Height** Color | Verwenden einer benutzerdefinierten Struktur oder eines Ankerpunkts. |

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
    <td>Kehren Sie bestimmte interne Karten um (z. B. Krümmung, AO), bevor sie zur endgültigen Maske kombiniert werden.</td>
  </tr>
  <tr>
    <td><strong>Abnutzungsstufe</strong></td>
    <td>Passen Sie den Gesamtverschleiß und die Gesamtsichtbarkeit des Generatoreffekts an.</td>
  </tr>
  <tr>
    <td><strong>Abnutzungskontrast</strong></td>
    <td>Passen Sie den Kontrast des endgültigen Verschleißergebnisses an.</td>
  </tr>
  <tr>
    <td><strong>Triplanar verwenden</strong></td>
    <td>Wenn <strong>Triplanar </strong> verwenden aktiviert ist, wird die Textur aus drei Richtungen (X-, Y-, Z-Achsen) projiziert, anstatt sich nur auf UVs zu verlassen. <br><ul><li>Ohne aktiviertes Triplanar folgt die Textur dem UV-Layout.</li><li>Wenn die Option "Dreidimensional" aktiviert ist, wird die Textur aus mehreren Winkeln projiziert und verblendet.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Triplanarer Überblendkontrast</strong></td>
    <td>Passen Sie an, wie glatt eine Textur übergeht, wenn sie mithilfe von triplanarer Zuordnung projiziert wird. Dadurch wird die Weichheit der Überblendung zwischen den Vorsprüngen aus jeder Richtung eingestellt.</td>
  </tr>
  <tr>
    <td><strong>Schmutzmenge</strong></td>
    <td>Passen Sie die Intensität der Schmutz-Details an.</td>
  </tr>
  <tr>
    <td><strong>Benutzerdefinierten Schmutz verwenden</strong></td>
    <td>Schalten Sie die Verwendung einer benutzerdefinierten Schmutz-Karte ein oder aus.</td>
  </tr>
  <tr>
    <td><strong>Kantenglättung</strong></td>
    <td>Passen Sie die Weichheit des Kantenverschleißeffekts an.</td>
  </tr>
  <tr>
    <td><strong>Maskierung Umgebungsverdeckung</strong></td>
    <td>Passen Sie an, wie stark die Umgebungszuordnung die Verdeckung auf das Ergebnis auswirkt.</td>
  </tr>
  <tr>
    <td><strong>Biegungsstärke</strong></td>
    <td>Passen Sie an, wie stark die Krümmungszuordnung das Ergebnis beeinflusst.</td>
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
    <td>Aktivieren oder deaktivieren Sie die Verwendung einer benutzerdefinierten Micro Height Map.</td>
  </tr>
  <tr>
    <td><strong>Mikro-Normale</strong></td>
    <td>Aktivieren oder deaktivieren Sie die Verwendung einer benutzerdefinierten Micro Normal-Karte.</td>
  </tr>
  <tr>
    <td><strong>Biegungstyp</strong></td>
    <td>Legt den Kurvenzeichentyp fest. <br><ul><li><strong>Standard</strong>: Erstellt ein normalerweise recht scharfes Ergebnis, kann jedoch größere Details vermissen lassen.</li><li><strong>Sobel</strong>: Ergibt ähnliche Ergebnisse wie bei der Standardeinstellung, jedoch leicht unschärfer, da die Normalmap mit einem Sobel-Filter ausgewertet wird.</li><li><strong>Glatt</strong>: Erzeugt verschiedene Weichzeichnungsstufen (wie Mipmaps), um Informationen zu sammeln. Dadurch entstehen in der Regel glattere Kurven, aber Details können verloren gehen.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Biegungsstärke</strong></td>
    <td>Passen Sie die Stärke der Krümmung im Modus "Standardkrümmung" und "Sobelkrümmung" an.</td>
  </tr>
  <tr>
    <td><strong>Höhendetailstärke</strong></td>
    <td>Passen Sie die Anzahl der Details des Micro-Heights an.</td>
  </tr>
  <tr>
    <td><strong>AO-Radius</strong></td>
    <td>Passen Sie den Radius (Bereich) der Verdeckung "Umgebung" in den Mikrodetails an.</td>
  </tr>
  <tr>
    <td><strong>AO-Tiefe</strong></td>
    <td>Passen Sie die Tiefe (Intensität) der Umgebungsintensität in den Mikrodetails an.</td>
  </tr>
</table>
