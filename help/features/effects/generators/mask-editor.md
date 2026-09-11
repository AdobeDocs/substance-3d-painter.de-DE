---
title: Maskeneditor
description: Erfahren Sie, wie Sie den Masken-Editor-Generator von Substance 3D Painter verwenden.
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '1494'
ht-degree: 7%

---


# Maskeneditor

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_mask_editor_dark.png" alt=""/><strong>In:</strong>-Maske, Generator</td>
    <td style="border: 0;" valign="top"><strong>Beschreibung</strong><br>Der Maskeneditorgenerator ist ein Mehrzweck-Maskengenerator, mit dem Sie Texturen, Umgebungsmasken, Krümmung, Welt-Raum-Normale, Verlauf, Thickness und Mikrodetails zu einer einzigen Verdeckung kombinieren können.<br>Der Mask Builder-Generator ist sehr flexibel, kann jedoch aufgrund seiner Komplexität die Leistung stärker beeinträchtigen als die meisten Generatoren.<br><br>Der Maskeneditor-Generator gibt eine monochrome (Schwarz-Weiß) Textur aus. Daher eignet sie sich gut zum Generieren von Masken basierend auf den verschiedenen durch Baking erzeugte Map. <br><br> Baking geführt Positions-, Thicknessen-, Krümmungen-, ambient occlusion- und Welt-Raum-Normale-Maps sind als Bildeingaben erforderlich. <a href="../../../baking/baking.md">Weitere Informationen zum Baking</a>.</td>
  </tr>
</table>

## Eingaben

| Eingabename | Beschreibung |
| --- | --- |
| **Textur** Farbe | Verwenden einer benutzerdefinierten Textur oder eines Ankerpunkts. |
| **Textur (Sekundär)** Farbe | Verwenden einer benutzerdefinierten Textur oder eines Ankerpunkts. |
| **Welt-Raum-Normale** Farbe | Verwenden Sie die gebackene Weltraumnormalkarte. |
| **Positionsverlauf** Farbe | Verwenden Sie die Baking geführt Positionszuordnung. |
| **Thickness** Graustufen | Verwenden Sie die Baking geführt Dicken-Map. |
| **Krümmung** Graustufen | Verwenden Sie die Baking geführt Krümmungs-Map. |
| **Ambient occlusion** Graustufen | Verwenden Sie die Baking geführt Ambient occlusion-Map. |
| **Micro Normal** Farbe | Verwenden Sie eine spezielle normale Textur oder einen Ankerpunkt. |
| **Micro Height** Color | Verwenden einer benutzerdefinierten Textur oder eines Ankerpunkts. |

## Parameter

| Parametername | Beschreibung |
| --- | --- |
| **Globale Umkehr** | Kehren Sie das Endergebnis um, nachdem alle Ebenen kombiniert wurden. |
| **Globaler Weichzeichner** | Lasse die finale Maske nach dem Kombinieren aller Ebenen gleichmäßig verschwimmen. |
| **Globaler Saldo** | Passe die Balance der letzten Maske an, nachdem alle Ebenen zwischen Schwarz und Weiß kombiniert wurden, wie bei einer Helligkeitsanpassung. |
| **Globaler Kontrast** | Passen Sie den Kontrast der letzten Maske an, nachdem alle Ebenen kombiniert wurden. |
| **Deckkraft der Textur** | Passen Sie die Sichtbarkeit der benutzerdefinierten Textur an. |
| **Textur 2 Deckkraft** | Passen Sie die Sichtbarkeit der zweiten benutzerdefinierten Textur an. |
| **Ambient occlusion Deckkraft** | Passen Sie die Sichtbarkeit der ambient occlusion-Details an. |
| **Deckkraft der Krümmung** | Passen Sie die Sichtbarkeit der Krümmungen an. |
| **Deckkraft des Welt-Raum-Normale** | Passen Sie die Sichtbarkeit der Welt-Raum-Normale-Details an. |
| **Verlaufsdeckkraft positionieren** | Passen Sie die Sichtbarkeit der Positionsdetails an. |
| **Deckkraft der Thickness** | Passen Sie die Sichtbarkeit der Thicknessen an. |

### Textur

<table>
  <tr>
    <th>Parametername</th>
    <th>Beschreibung</th>
  </tr>
  <tr>
    <td><strong>Invertieren</strong></td>
    <td>Kehrt die benutzerdefinierte Textur um.</td>
  </tr>
  <tr>
    <td><strong>Graustufenkonvertierung</strong></td>
    <td>Legen Sie die Methode fest, die für die Konvertierung von Vollfarben in Graustufen verwendet wird. Der <a href="grayscale-conversion.md">Graustufen-Konvertierungsgenerator enthält weitere Informationen über die Funktionsweise der einzelnen Methoden.</a></td>
  </tr>
  <tr>
    <td><strong>Überblendmodus</strong></td>
    <td>Wählen Sie den <a href="../../../interface/layer-stack/blending-modes.md">Mischmodus</a> für die aktuelle Ebene aus.</td>
  </tr>
  <tr>
    <td><strong>Skalieren</strong></td>
    <td>Passen Sie die Größe der benutzerdefinierten Textur an.</td>
  </tr>
  <tr>
    <td><strong>Kontrast</strong></td>
    <td>Passen Sie Kontrast und Abfall der benutzerdefinierten Textur an.</td>
  </tr>
  <tr>
    <td><strong>Helligkeit</strong></td>
    <td>Passen Sie die Luminanz der benutzerdefinierten Textur an.</td>
  </tr>
  <tr>
    <td><strong>Triplanar</strong></td>
    <td>Wenn <strong>Triplanar </strong> verwenden aktiviert ist, wird die Textur aus drei Richtungen projiziert (X-, Y-, Z-Achsen), anstatt sich nur auf UVs zu verlassen. <br><ul><li>Ohne die Option "Triplanar" folgt die Textur dem UV-Layout.</li><li>Wenn die Option "Dreidimensional" aktiviert ist, wird die Textur aus mehreren Winkeln projiziert und verblendet.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Triplanarer Kontrast</strong></td>
    <td>Passen Sie an, wie glatt eine Textur übergeht, wenn sie mithilfe von triplanarem Mapping projiziert wird. Dadurch wird die Weichheit der Überblendung zwischen den Projektionen aus jeder Richtung angepasst.</td>
  </tr>
  <tr>
    <td><strong>Keine quadratischen Kacheln</strong></td>
    <td>Schalten Sie die nicht quadratische Kachelung ein oder aus.</td>
  </tr>
</table>

### Struktur 2

<table>
  <tr>
    <th>Parametername</th>
    <th>Beschreibung</th>
  </tr>
  <tr>
    <td><strong>Invertieren</strong></td>
    <td>Kehrt die benutzerdefinierte sekundäre Textur um.</td>
  </tr>
  <tr>
    <td><strong>Graustufenkonvertierung</strong></td>
    <td>Legen Sie die Methode fest, die für die Konvertierung von Vollfarben in Graustufen verwendet wird. Der <a href="grayscale-conversion.md">Graustufen-Konvertierungsgenerator enthält weitere Informationen über die Funktionsweise der einzelnen Methoden.</a></td>
  </tr>
  <tr>
    <td><strong>Überblendmodus</strong></td>
    <td>Wählen Sie den <a href="../../../interface/layer-stack/blending-modes.md">Mischmodus</a> für die aktuelle Ebene aus.</td>
  </tr>
  <tr>
    <td><strong>Skalieren</strong></td>
    <td>Passen Sie die Größe der benutzerdefinierten Textur an.</td>
  </tr>
  <tr>
    <td><strong>Kontrast</strong></td>
    <td>Passen Sie Kontrast und Abfall der benutzerdefinierten Textur an.</td>
  </tr>
  <tr>
    <td><strong>Helligkeit</strong></td>
    <td>Passen Sie die Luminanz der benutzerdefinierten Textur an.</td>
  </tr>
  <tr>
    <td><strong>Triplanar</strong></td>
    <td>Wenn <strong>Triplanar </strong> verwenden aktiviert ist, wird die Textur aus drei Richtungen projiziert (X-, Y-, Z-Achsen), anstatt sich nur auf UVs zu verlassen. <br><ul><li>Ohne die Option "Triplanar" folgt die Textur dem UV-Layout.</li><li>Wenn die Option "Dreidimensional" aktiviert ist, wird die Textur aus mehreren Winkeln projiziert und verblendet.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Triplanarer Kontrast</strong></td>
    <td>Passen Sie an, wie glatt eine Textur übergeht, wenn sie mithilfe von triplanarem Mapping projiziert wird. Dadurch wird die Weichheit der Überblendung zwischen den Projektionen aus jeder Richtung angepasst.</td>
  </tr>
  <tr>
    <td><strong>Keine quadratischen Kacheln</strong></td>
    <td>Schalten Sie die nicht quadratische Kachelung ein oder aus.</td>
  </tr>
</table>

### Umgebungsverdeckung

| Parametername | Beschreibung |
| --- | --- |
| **Umkehren** | Kehren Sie die Ebenen &quot;Ambient occlusion&quot; und &quot;Mikrodetails&quot; um. |
| **Füllmethode** | Wählen Sie den [Mischmodus](../../../interface/layer-stack/blending-modes.md) für die aktuelle Ebene aus. |
| **Weichzeichnen** | Passen Sie die Ambient occlusion- und Micro Detail-Weichheit an. |
| **Saldo** | Passe die Balance des Ambient occlusion und die Mikrodetails an, und verschiebe den Mittelpunkt wie bei einem Helligkeitsregler in Richtung Schwarz oder Weiß. |
| **Kontrast** | Passen Sie den Kontrast/Abfall des Ambient occlusion und der Mikrodetails an. |

### Biegung

<table>
  <tr>
    <th>Parametername</th>
    <th>Beschreibung</th>
  </tr>
  <tr>
    <td><strong>Invertieren</strong></td>
    <td>Krümmung umkehren.</td>
  </tr>
  <tr>
    <td><strong>Überblendmodus</strong></td>
    <td>Wählen Sie den <a href="../../../interface/layer-stack/blending-modes.md">Mischmodus</a> für die aktuelle Ebene aus.</td>
  </tr>
  <tr>
    <td><strong>Modus</strong></td>
    <td>Legen Sie den Krümmung-Modus fest. <br><ul><li><strong>Kanten</strong>: Maskiert die Kanten (konvexe Bereiche).</li><li><strong>Hohlräume</strong>: Maskiert die Hohlräume (konkave Bereiche)</li><li><strong>Dual</strong>: Masken für konkave und konvexe Bereiche.</li><li><strong>Unverarbeitet</strong>: Normale Krümmung.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Scharf</strong></td>
    <td>Passen Sie die Sichtbarkeit der Details der scharfen Krümmung an.</td>
  </tr>
  <tr>
    <td><strong>Fein</strong></td>
    <td>Passen Sie die Sichtbarkeit der Details der Krümmung an.</td>
  </tr>
  <tr>
    <td><strong>Weich</strong></td>
    <td>Passen Sie die Sichtbarkeit der Details der weichen Krümmung an.</td>
  </tr>
  <tr>
    <td><strong>Mittel</strong></td>
    <td>Passen Sie die Sichtbarkeit der Details der mittleren Krümmung an.</td>
  </tr>
  <tr>
    <td><strong>Groß</strong></td>
    <td>Passen Sie die Sichtbarkeit der großen Krümmungen an.</td>
  </tr>
  <tr>
    <td><strong>Groß</strong></td>
    <td>Passe die Sichtbarkeit der großen Krümmungen an.</td>
  </tr>
  <tr>
    <td><strong>Riesig</strong></td>
    <td>Passen Sie die Sichtbarkeit der großen Krümmungen Details.</td>
  </tr>
  <tr>
    <td><strong>Kontrast</strong></td>
    <td>Passen Sie den Kontrast/Abfall der Krümmung an.</td>
  </tr>
  <tr>
    <td><strong>Helligkeit</strong></td>
    <td>Passen Sie die Luminanz der Krümmung an.</td>
  </tr>
</table>

### Raum-Normale

| Parametername | Beschreibung |
| --- | --- |
| **Umkehren** | Welt-Raum-Normale umkehren. |
| **Füllmethode** | Wählen Sie den [Mischmodus](../../../interface/layer-stack/blending-modes.md) für die aktuelle Ebene aus. |
| **Weichzeichnen** | Passe die Weichheit des Welt-Raum-Normale an. |
| **Saldo** | Passen Sie die Balance der Welt-Raum-Normale an, indem Sie den Mittelpunkt wie einen Helligkeitsregler in Richtung Schwarz oder Weiß verschieben. |
| **Kontrast** | Passen Sie den Kontrast/Abfall der Welt-Raum-Normale an. |
| **Helligkeit** | Passen Sie die Luminanz der Welt-Raum-Normale an. |
| **Rechts nach links** | Passen Sie an, wie der Effekt von links nach rechts über den Mesh angewendet wird. |
| **Von oben nach unten** | Passen Sie an, wie der Effekt auf den Mesh angewendet wird. |
| **Von vorne nach hinten** | Passen Sie an, wie der Effekt auf den Mesh angewendet wird. |

### Raum-Normale/von rechts nach links

| Parametername | Beschreibung |
| --- | --- |
| **Umkehren** | Kehren Sie die Richtung von rechts nach links um. |
| **Füllmethode** | Wählen Sie den [Mischmodus](../../../interface/layer-stack/blending-modes.md) für die aktuelle Ebene aus. |

### Raum-Normale/von oben nach unten

| Parametername | Beschreibung |
| --- | --- |
| **Umkehren** | Oben nach unten umkehren. |
| **Füllmethode** | Wählen Sie den [Mischmodus](../../../interface/layer-stack/blending-modes.md) für die aktuelle Ebene aus. |

### Raum-Normale/von vorne nach hinten

| Parametername | Beschreibung |
| --- | --- |
| **Umkehren** | Kehren Sie die Vorder- und Rückwärtsrichtung um. |
| **Füllmethode** | Wählen Sie den [Mischmodus](../../../interface/layer-stack/blending-modes.md) für die aktuelle Ebene aus. |

### Position Verlauf

| Parametername | Beschreibung |
| --- | --- |
| **Umkehren** | Kehre die Ebene mit dem Positionsverlauf um. |
| **Saldo** | Passe die Balance der Ebene mit dem Positionsverlauf an. Verschiebe den Mittelpunkt wie bei einem Helligkeitsregler in Richtung Schwarz oder Weiß. |
| **Kontrast** | Passen Sie den Kontrast bzw. das Falloff der Positionsverlaufsebene an. |
| **Helligkeit** | Passen Sie die Luminanz der Positionsverlaufsebene an. |
| **Füllmethode** | Wählen Sie den [Mischmodus](../../../interface/layer-stack/blending-modes.md) für die aktuelle Ebene aus. |
| **Rechts nach links** | Passen Sie an, wie der Effekt von links nach rechts über den Mesh angewendet wird. |
| **Von oben nach unten** | Passen Sie an, wie der Effekt auf den Mesh angewendet wird. |
| **Von vorne nach hinten** | Passen Sie an, wie der Effekt auf den Mesh angewendet wird. |

>[!TIP]
>
> Der Positionsverlauf besteht aus bis zu drei Farbverläufen, von rechts nach links, von oben nach unten und von vorne nach hinten. Jeder der Unterfarbverläufe verfügt über eine eigene Füllmethode, mit der verschiedene Effekte erzeugt oder verschiedene Bereiche des Modells maskiert werden können. Die Füllmethoden für diese Verläufe interagieren nur miteinander, um eine endgültige Positionsverlaufsebene zu erstellen. Sie interagieren nicht direkt mit anderen Ebenen im Generator außerhalb des Positionsverlaufs.

### Positionsverlauf - von rechts nach links

| Parametername | Beschreibung |
| --- | --- |
| **Umkehren** | Kehren Sie die Verlaufsrichtung von rechts nach links um. |
| **Füllmethode** | Wählen Sie den [Mischmodus](../../../interface/layer-stack/blending-modes.md) aus, der für den Rechts-Links-Verlauf verwendet werden soll. |

### Positionsverlauf - von oben nach unten

| Parametername | Beschreibung |
| --- | --- |
| **Umkehren** | Kehren Sie die Verlaufsrichtung von oben nach unten um. |
| **Füllmethode** | Wählen Sie den [Mischmodus](../../../interface/layer-stack/blending-modes.md) aus, der für den oberen bis unteren Farbverlauf verwendet werden soll. |

### Positionsverlauf - von vorne nach hinten

| Parametername | Beschreibung |
| --- | --- |
| **Umkehren** | Kehren Sie die Verlaufsrichtung von vorne nach hinten um. |
| **Füllmethode** | Wählen Sie den [Mischmodus](../../../interface/layer-stack/blending-modes.md) aus, der für den Vorder-/Rückwärtsverlauf verwendet werden soll. |

### Stärke

| Parametername | Beschreibung |
| --- | --- |
| **Umkehren** | Thickness umkehren. |
| **Weichzeichnen** | Passe die Weichheit der Details auf der Thickness-Ebene an. |
| **Kontrast** | Passe den Kontrast und das Falloff der Ebene mit der Thickness an. |
| **Helligkeit** | Passe die Luminanz der Thickness an. |

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
    <td>Passen Sie die Intensität der Krümmung im <strong>Standardmodus</strong> und im <strong>Sobelmodus </strong>Krümmung an.</td>
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
