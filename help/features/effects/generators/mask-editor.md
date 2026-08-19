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
    <td style="border: 0;" valign="top"><strong>Beschreibung</strong><br>Der Maskeneditor ist ein Mehrzweck-Maskengenerator, mit dem Sie Texturen, Umgebungsmasken, Krümmung, World Space Normal, Verlauf, Thickness und Mikrodetails zu einer einzigen Verdeckung kombinieren können.<br>Der Mask Builder-Generator ist sehr flexibel, kann jedoch aufgrund seiner Komplexität die Leistung stärker beeinträchtigen als die meisten Generatoren.<br><br>Der Maskeneditor-Generator gibt eine monochrome (schwarz-weiß) Textur aus. Daher eignet sie sich gut zum Generieren von Masken basierend auf den verschiedenen durch Baking erzeugte Map. <br><br>Als Bildeingabe sind die gebackene Position, die Thickness, die Krümmung, die umgebende Verdeckung und die Normal-Weltraumkarten erforderlich. <a href="../../../baking/baking.md">Weitere Informationen zum Backen</a>.</td>
  </tr>
</table>

## Eingaben

| Eingabename | Beschreibung |
| --- | --- |
| **Textur** Farbe | Verwenden einer benutzerdefinierten Struktur oder eines Ankerpunkts. |
| **Struktur (sekundär)** Farbe | Verwenden einer benutzerdefinierten Struktur oder eines Ankerpunkts. |
| **Normale im Weltraum** Farbe | Verwenden Sie die gebackene Weltraumnormalkarte. |
| **Positionsverlauf** Farbe | Verwenden Sie die Positionskarte. |
| **Thickness** Graustufen | Verwenden Sie die Karte mit den gebackenen Thicknessen. |
| **Krümmung** Graustufen | Verwenden Sie die Kurvenzeichner-Map. |
| **Umgebungs-Verdeckung** Graustufen | Verwenden Sie die Karte mit der Verdeckung &quot;Umgebung&quot;. |
| **Micro Normal** Farbe | Verwenden Sie eine spezielle normale Textur oder einen Ankerpunkt. |
| **Micro Height** Color | Verwenden einer benutzerdefinierten Struktur oder eines Ankerpunkts. |

## Parameter

| Parametername | Beschreibung |
| --- | --- |
| **Globale Umkehr** | Kehren Sie das Endergebnis um, nachdem alle Ebenen kombiniert wurden. |
| **Globaler Weichzeichner** | Lasse die finale Maske nach dem Kombinieren aller Ebenen gleichmäßig verschwimmen. |
| **Globaler Saldo** | Passe die Balance der letzten Maske an, nachdem alle Ebenen zwischen Schwarz und Weiß kombiniert wurden, wie bei einer Helligkeitsanpassung. |
| **Globaler Kontrast** | Passen Sie den Kontrast der letzten Maske an, nachdem alle Ebenen kombiniert wurden. |
| **Texturdeckkraft** | Passen Sie die Sichtbarkeit der benutzerdefinierten Textur an. |
| **Struktur 2 Deckkraft** | Passen Sie die Sichtbarkeit der zweiten benutzerdefinierten Textur an. |
| **Umgebungsdeckkraft der Verdeckung** | Passen Sie die Sichtbarkeit der Umgebungsdetails an. Verdeckung |
| **Krümmungsdeckkraft** | Passen Sie die Sichtbarkeit der Kurvendetails an. |
| **Standarddeckkraft des Weltraums** | Passen Sie die Sichtbarkeit der normalen Details des Weltraums an. |
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
    <td>Passe die Größe der benutzerdefinierten Struktur an.</td>
  </tr>
  <tr>
    <td><strong>Kontrast</strong></td>
    <td>Passen Sie den Kontrast/Abfall der benutzerdefinierten Textur an.</td>
  </tr>
  <tr>
    <td><strong>Helligkeit</strong></td>
    <td>Passen Sie die Luminanz der benutzerdefinierten Textur an.</td>
  </tr>
  <tr>
    <td><strong>Triplanar</strong></td>
    <td>Wenn <strong>Triplanar </strong> verwenden aktiviert ist, wird die Textur aus drei Richtungen (X-, Y-, Z-Achsen) projiziert, anstatt sich nur auf UVs zu verlassen. <br><ul><li>Ohne aktiviertes Triplanar folgt die Textur dem UV-Layout.</li><li>Wenn die Option "Dreidimensional" aktiviert ist, wird die Textur aus mehreren Winkeln projiziert und verblendet.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Triplanarer Kontrast</strong></td>
    <td>Passen Sie an, wie glatt eine Textur übergeht, wenn sie mithilfe von triplanarer Zuordnung projiziert wird. Dadurch wird die Weichheit der Überblendung zwischen den Vorsprüngen aus jeder Richtung eingestellt.</td>
  </tr>
  <tr>
    <td><strong>Keine quadratischen Kacheln</strong></td>
    <td>Schalten Sie die nicht quadratische Unterteilung ein oder aus.</td>
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
    <td>Kehre die spezielle sekundäre Textur um.</td>
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
    <td>Passe die Größe der benutzerdefinierten Struktur an.</td>
  </tr>
  <tr>
    <td><strong>Kontrast</strong></td>
    <td>Passen Sie den Kontrast/Abfall der benutzerdefinierten Textur an.</td>
  </tr>
  <tr>
    <td><strong>Helligkeit</strong></td>
    <td>Passen Sie die Luminanz der benutzerdefinierten Textur an.</td>
  </tr>
  <tr>
    <td><strong>Triplanar</strong></td>
    <td>Wenn <strong>Triplanar </strong> verwenden aktiviert ist, wird die Textur aus drei Richtungen (X-, Y-, Z-Achsen) projiziert, anstatt sich nur auf UVs zu verlassen. <br><ul><li>Ohne aktiviertes Triplanar folgt die Textur dem UV-Layout.</li><li>Wenn die Option "Dreidimensional" aktiviert ist, wird die Textur aus mehreren Winkeln projiziert und verblendet.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Triplanarer Kontrast</strong></td>
    <td>Passen Sie an, wie glatt eine Textur übergeht, wenn sie mithilfe von triplanarer Zuordnung projiziert wird. Dadurch wird die Weichheit der Überblendung zwischen den Vorsprüngen aus jeder Richtung eingestellt.</td>
  </tr>
  <tr>
    <td><strong>Keine quadratischen Kacheln</strong></td>
    <td>Schalten Sie die nicht quadratische Unterteilung ein oder aus.</td>
  </tr>
</table>

### Umgebungsverdeckung

| Parametername | Beschreibung |
| --- | --- |
| **Umkehren** | Kehren Sie die Ebenen &quot;Umgebungs-Verdeckung&quot; und &quot;Mikrodetails&quot; um. |
| **Füllmethode** | Wählen Sie den [Mischmodus](../../../interface/layer-stack/blending-modes.md) für die aktuelle Ebene aus. |
| **Weichzeichnen** | Passen Sie die Verdeckung des Hintergrunds und die Detailweichheit des Mikros an. |
| **Saldo** | Passen Sie die Verdeckung der Umgebung und die Mikrodetails an, und verschieben Sie den Mittelpunkt wie bei einem Helligkeitsregler in Richtung Schwarz oder Weiß. |
| **Kontrast** | Passen Sie den Kontrast/Abfall der Verdeckung &quot;Umgebung&quot; und der Mikrodetails an. |

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
    <td>Setze den Kurvenmodus. <br><ul><li><strong>Kanten</strong>: Maskiert die Kanten (konvexe Bereiche).</li><li><strong>Hohlräume</strong>: Maskiert die Hohlräume (konkave Bereiche)</li><li><strong>Dual</strong>: Masken für konkave und konvexe Bereiche.</li><li><strong>Unverarbeitet</strong>: Normale Kurvenmaske.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Scharf</strong></td>
    <td>Passen Sie die Sichtbarkeit der scharfen Krümmungsdetails an.</td>
  </tr>
  <tr>
    <td><strong>Fein</strong></td>
    <td>Passen Sie die Sichtbarkeit feiner Krümmungsdetails an.</td>
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
    <td>Passen Sie die Sichtbarkeit der großen Krümmungsdetails an.</td>
  </tr>
  <tr>
    <td><strong>Groß</strong></td>
    <td>Passen Sie die Sichtbarkeit der großen Krümmungsdetails an.</td>
  </tr>
  <tr>
    <td><strong>Riesig</strong></td>
    <td>Passen Sie die Sichtbarkeit der riesigen Krümmungsdetails an.</td>
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
| **Umkehren** | Kehre die Normalen des Weltraums um. |
| **Füllmethode** | Wählen Sie den [Mischmodus](../../../interface/layer-stack/blending-modes.md) für die aktuelle Ebene aus. |
| **Weichzeichnen** | Passen Sie die normale Weichheit des Weltraums an. |
| **Saldo** | Passe das Gleichgewicht der Weltraum-Normalen an und verschiebe den Mittelpunkt in Richtung Schwarz oder Weiß, wie bei einer Helligkeitsregelung. |
| **Kontrast** | Passen Sie den Kontrast/Abfall der Weltraum-Normalen an. |
| **Helligkeit** | Passen Sie die Luminanz der Weltraum-Normalen an. |
| **Rechts nach links** | Passen Sie an, wie der Effekt von links nach rechts über das Gitter angewendet wird. |
| **Von oben nach unten** | Passen Sie an, wie der Effekt über das Gitter hinweg von oben nach unten angewendet wird. |
| **Von vorne nach hinten** | Passen Sie an, wie der Effekt über das Gitter hinweg von vorne nach hinten angewendet wird. |

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
| **Rechts nach links** | Passen Sie an, wie der Effekt von links nach rechts über das Gitter angewendet wird. |
| **Von oben nach unten** | Passen Sie an, wie der Effekt über das Gitter hinweg von oben nach unten angewendet wird. |
| **Von vorne nach hinten** | Passen Sie an, wie der Effekt über das Gitter hinweg von vorne nach hinten angewendet wird. |

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
    <td>Passen Sie die Intensität der Krümmung im Modus <strong>Standard</strong> und <strong>Sobel </strong>Krümmung an.</td>
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
    <td>Passen Sie die Tiefe (Intensität) der Umgebungsintensität in den Mikrodetails an.</td>
  </tr>
</table>
