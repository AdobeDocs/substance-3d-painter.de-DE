---
title: Maskenbildner
description: Erfahren Sie, wie Sie den Maskenbildner-Generator von Substance 3D Painter verwenden.
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '1146'
ht-degree: 5%

---


# Maskenbildner

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_mask_builder_dark.png" alt=""/><strong>In:</strong>-Maske, Generator</td>
    <td style="border: 0;" valign="top"><strong>Beschreibung</strong><br>Der Generator für den Maskengenerator ist eine ältere Version des Generators für den Maskeneditor. Es ist ein Multifunktionsmaskengenerator, mit dem Sie Schmutz, AO, Krümmung, Verlauf, World Space Normal, Scratches, Streuung und Mikrodetails in einer einzigen Maske kombinieren können.<br><br>Der Mask Builder-Generator ist sehr flexibel, kann jedoch aufgrund seiner Komplexität die Leistung stärker beeinträchtigen als die meisten Generatoren.<br><br>Der Maskenbildner-Generator gibt eine monochrome (schwarz-weiß) Textur aus. Daher eignet sie sich gut zum Generieren von Masken basierend auf den verschiedenen durch Baking erzeugte Map. <br><br>Als Bildeingabe sind die gebackene Position, die Krümmung, die Umgebungs-Verdeckung und die Weltraum-Normalmaps erforderlich. <a href="../../../baking/baking.md">Weitere Informationen zum Backen</a>.</td>
  </tr>
</table>

## Eingaben

| Eingabename | Beschreibung |
| --- | --- |
| **Normaler Weltraum** Farbe | Verwenden Sie die gebackene Weltraumnormalkarte. |
| **Benutzerdefinierter Schmutz 1** Graustufen | Verwenden einer benutzerdefinierten Struktur oder eines Ankerpunkts. |
| **Benutzerdefinierter Schmutz 2** Graustufen | Verwenden einer benutzerdefinierten Struktur oder eines Ankerpunkts. |
| **Streuung-Eingabe** Graustufen | Verwenden einer benutzerdefinierten Struktur oder eines Ankerpunkts. |
| **Position** Farbe | Verwenden Sie die Positionskarte. |
| **Krümmung** Graustufen | Verwenden Sie die Kurvenzeichner-Map. |
| **Umgebungs-Verdeckung** Graustufen | Verwenden Sie die Karte mit der Verdeckung &quot;Umgebung&quot;. |
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
    <td><strong>Stufe</strong></td>
    <td>Nachdem alle Effekte in Schwarz oder Weiß kombiniert wurden, kannst du den Mittelpunkt der finalen Maske anpassen, z. B. die Helligkeit.</td>
  </tr>
  <tr>
    <td><strong>Kontrast</strong></td>
    <td>Passen Sie den Kontrast/Abfall der endgültigen Maske an.</td>
  </tr>
  <tr>
    <td><strong>Invertieren</strong></td>
    <td>Kehrt das Ergebnis der kombinierten Maske um.</td>
  </tr>
  <tr>
    <td><strong>Triplanar verwenden</strong></td>
    <td>Wenn <strong>Triplanar </strong> verwenden aktiviert ist, wird die Textur aus drei Richtungen (X-, Y-, Z-Achsen) projiziert, anstatt sich nur auf UVs zu verlassen. <br><ul><li>Ohne aktiviertes Triplanar folgt die Textur dem UV-Layout.</li><li>Wenn die Option "Dreidimensional" aktiviert ist, wird die Textur aus mehreren Winkeln projiziert und verblendet.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Triplanarer Überblendkontrast</strong></td>
    <td>Passen Sie mit der Option "Triplanares Mapping" an, wie glatt eine Textur bei der Projektion übergeht. Er passt die Weichheit der Überblendung zwischen den Vorsprüngen aus jeder Richtung an.</td>
  </tr>
  <tr>
    <td><strong>Schmutz</strong></td>
    <td>Passen Sie an, wie sehr sich die Schmutz-Einstellungen auf das endgültige Maskenergebnis auswirken.</td>
  </tr>
  <tr>
    <td><strong>AO</strong></td>
    <td>Passen Sie an, wie sehr sich die AO-Einstellungen (Umgebungsmaske) auf das endgültige Maskenergebnis auswirken.</td>
  </tr>
  <tr>
    <td><strong>Biegung</strong></td>
    <td>Passen Sie an, wie sehr sich die Kurveneinstellungen auf das endgültige Maskenergebnis auswirken.</td>
  </tr>
  <tr>
    <td><strong>Verlauf von oben nach unten</strong></td>
    <td>Passen Sie an, wie stark der Verlauf "Oben/Unten" das endgültige Maskenergebnis beeinflusst.</td>
  </tr>
  <tr>
    <td><strong>Raum-Normale</strong></td>
    <td>Passen Sie an, wie stark die Einstellungen für "World Space Normal" das Endergebnis der Maske beeinflussen.</td>
  </tr>
  <tr>
    <td><strong>Kratzer</strong></td>
    <td>Passen Sie an, wie stark sich die Maskeneinstellungen auf das endgültige Maskenergebnis auswirken. Damit die Scratches sichtbar sind, müssen Schmutz, AO oder Krümmung über 0 liegen.</td>
  </tr>
  <tr>
    <td><strong>Streuung</strong></td>
    <td>Legt fest, wie stark die Streuung die Maske beeinflusst.</td>
  </tr>
</table>

### Schmutz

| Parametername | Beschreibung |
| --- | --- |
| **Skalierung** | Passen Sie die Größe der Schmutz-Textur an. |
| **Benutzerdefinierten Schmutz verwenden** | Schalten Sie die Verwendung einer benutzerdefinierten Schmutz-Karte ein oder aus. Es ist nur die Sichtbarkeit des Custom Schmutz 1. Um die Sichtbarkeit des benutzerdefinierten Schmutz 2 zu steuern, passen Sie den Schieberegler Sekundärer benutzerdefinierter Schmutz an. |
| **Sekundärer benutzerdefinierter Schmutz** | Passen Sie die Sichtbarkeit der Custom Schmutz 2-Textur an. |
| **Umkehren** | Schmutz-Maps umkehren. |

### Umgebungsverdeckung

| Parametername | Beschreibung |
| --- | --- |
| **Bereich** | Passen Sie den Bereich der AO-Maske an. |
| **Kontrast** | Passen Sie den Kontrast/Abfall der AO-Maske an. |
| **Rauschen** | Füge dem AO-Ergebnis Rauschen hinzu, um die Helligkeit der Maske effektiv zu verringern. |
| **Umkehren** | AO-Maske umkehren. |

### Biegung

| Parametername | Beschreibung |
| --- | --- |
| **Konvexbereich** | Passen Sie den minimalen konvexen Winkel an, der von der Maske hervorgehoben werden muss. |
| **Konvexkontrast** | Passen Sie den Kontrast der konvexen Maske an. |
| **Konvex invertieren** | Kehrt die konvexe Maske um. |
| **Konkaver Bereich** | Passen Sie den minimalen konkaven Winkel an, der durch die Maske hervorgehoben werden soll. |
| **Konkaver Kontrast** | Passen Sie den Kontrast der konkaven Maske an. |
| **Konkave Umkehr** | Kehre die konkave Maske um. |
| **Smoothness** | Passen Sie den Übergang zwischen hellen und dunklen Bereichen der Kurvenmaske an. |
| **Leistungssteigerung** | So erweitern Sie den Bereich des maskierten Bereichs. Dies verhält sich wie ein Multiplikator für die Parameter **Konvexer Bereich** und **Konkaver Bereich**. |
| **Rauschen** | Füge Rauschen zum Ergebnis der Krümmung hinzu, um die Helligkeit der Maske effektiv zu verringern. |

### Verlauf

Die Verlaufsposition basiert auf der Positionsmap, die entweder mit der Normalisierungsskala &quot;Vollständige Szene&quot; oder &quot;Pro Material&quot; gebacken werden kann. Wenn Ihr Material nur in einem kleinen Bereich Ihrer Szene erscheint, die Positionskarte aber mit einer Skala für die vollständige Szenennormalisierung vorliegt, ist es möglicherweise schwierig, den Verlaufsbereich anzupassen, um das gewünschte Ergebnis zu erzielen.

| Parametername | Beschreibung |
| --- | --- |
| **Bereich** | Passen Sie den Verlaufsbereich an. |
| **Kontrast** | Verringert den Kontrast des Verlaufs. |
| **Umkehren** | Kehrt den Verlauf um. |

### Raum-Normale

**Die Werte von**, **Zurück**, **Links** und **Rechts** stimmen möglicherweise nicht mit der Vorder-, Rückseite, linken und rechten Seite des Gitters überein. Standardmäßig entspricht **Front** der positiven X-Achse, und Rechts der positiven Z-Achse.

| Parametername | Beschreibung |
| --- | --- |
| **Höchste Intensität** | Passen Sie den Bereich (Intensität) des Verlaufs nach unten an. |
| **Tiefe unten** | Passen Sie den Bereich (Intensität) des Gradienten von unten nach oben an. |
| **Intensität vorne** | Passen Sie den Bereich (die Intensität) des Vorder- und Rückwärtsverlaufs an. |
| **Intensität zurücksetzen** | Passen Sie den Bereich (die Intensität) des Verlaufs auf der Rückseite an. |
| **Intensität rechts** | Passen Sie den Bereich (Intensität) des Verlaufs nach rechts links an. |
| **Linke Intensität** | Passen Sie den Bereich (Intensität) des Links-Rechts-Verlaufs an. |

### Kratzer

| Parametername | Beschreibung |
| --- | --- |
| **Betrag** | Passen Sie die Dichte der Kratzer an. |
| **Skalierung** | Passen Sie die Größe der Kratzer an. |

### Streuung

| Parametername | Beschreibung |
| --- | --- |
| **Skalierung** | Passe die Größe der Streuung an. Je höher die Skala, desto kleiner die Stempelgröße. Je niedriger die Skala, desto geringer die sichtbare Stempelgröße. |
| **Dichte** | Passen Sie die Anzahl der verstreuten Stempel an. |
| **Größe** | Passen Sie die Größe der Streustempel an. |
| **Größenänderung** | Passen Sie die Größe der einzelnen Instanzen des gestreuten Stempels nach dem Zufallsprinzip an. Eine höhere Größenvariation reduziert zufällig Stempelgrößen, sodass eine größere Größenvariation bedeuten kann, dass Sie auch den Größenwert erhöhen müssen, um die gleiche durchschnittliche Größe beizubehalten. |
| **Deckkraftvariation** | Passen Sie an, wie stark die Deckkraft der einzelnen Instanzen des Streustempels vom Zufall abhängt. |

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
    <td>Lege den Kurvenzeichner fest. <br><ul><li><strong>Standard</strong>: Erstellt ein normalerweise recht scharfes Ergebnis, kann jedoch größere Details vermissen lassen.</li><li><strong>Sobel</strong>: Ergibt ähnliche Ergebnisse wie bei der Standardeinstellung, jedoch leicht unschärfer, da die Normalmap mit einem Sobel-Filter ausgewertet wird.</li><li><strong>Glatt</strong>: Erzeugt verschiedene Weichzeichnungsstufen (wie Mipmaps), um Informationen zu sammeln. Dadurch entstehen in der Regel glattere Kurven, aber Details können verloren gehen.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Biegungsstärke</strong></td>
    <td>Passen Sie die Intensität der Krümmung im Modus <strong>Standard </strong> und <strong>Sobel </strong>Krümmung an.</td>
  </tr>
  <tr>
    <td><strong>Höhendetailstärke</strong></td>
    <td>Passen Sie die Stärke der Micro Height-Details an.</td>
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
