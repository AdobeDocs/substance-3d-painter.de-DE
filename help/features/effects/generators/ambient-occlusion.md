---
title: Umgebungsverdeckung
description: Erfahren Sie, wie Sie den Umgebungslichtgenerator von Substance 3D Painter verwenden.
source-git-commit: b095b9b437f75bbb3a3b85ee84a6850026c3bf98
workflow-type: tm+mt
source-wordcount: '542'
ht-degree: 5%

---


# Umgebungsverdeckung

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_ambient_occlusion.webp" alt=""/><br><strong>In:</strong> Maske, Generator, Graustufen, Überblendung</td>
    <td style="border: 0;" valign="top"><strong>Beschreibung</strong><br>Der Umgebungsmaskengenerator erstellt eine Verdeckung, die auf der gebackenen Umgebungsmaskenkarte basiert, mit der Option, eine Textur oder Mikrodetails in die Verdeckung einzufügen.<br><br>Wenn Sie den Umgebungsmaskengenerator zum Erstellen einer Ebenenmaske verwenden, müssen Sie möglicherweise die Verdeckung für die Umgebungsmaske umkehren, um die Verdeckung zu erzeugen. Standardmäßig gibt der Generator verdeckte Bereiche als dunkle und nicht verdeckte Bereiche als helle aus. Wenn sie als Maske verwendet wird, ist die maskierte Ebene nur in nicht verdeckten Bereichen sichtbar. Durch Umkehren der Ausgabe wird sichergestellt, dass die maskierte Ebene nur in verdeckten Bereichen angezeigt wird.<br><br>Als Bildeingabe sind eine gebackene Verdeckung, eine Umgebungsposition und eine Normalmap für den Weltraum erforderlich. <a href="../../../baking/baking.md">Weitere Informationen zum Backen</a>.</td>
  </tr>
</table>

## Eingaben

| Eingabename | Beschreibung |
| --- | --- |
| Texturfarbe | Verwenden einer benutzerdefinierten Struktur oder eines Ankerpunkts. |
| Micro-Normalfarbe | Verwenden Sie eine spezielle normale Textur oder einen Ankerpunkt. |
| Farbe eines Micro Heights | Verwenden einer benutzerdefinierten Struktur oder eines Ankerpunkts. |
| Graustufen der Umgebungsluft-Verdeckung | Verwenden Sie die Karte mit der Verdeckung &quot;Umgebung&quot;. |
| Normale Farbe im Weltraum | Verwenden Sie die gebackene Weltraumnormalkarte. |
| Positionsverlaufsfarbe | Verwenden Sie die Positionskarte. |

## Parameter

| Parametername | Beschreibung |
| --- | --- |
| **Globale Umkehr** | Kehrt das Endergebnis um, nachdem alle Effekte kombiniert wurden. |
| **Globaler Weichzeichner** | Glätten Sie die endgültige Maske gleichmäßig, nachdem alle Effekte kombiniert wurden. |
| **Globaler Saldo** | Verschiebe den Wert der letzten Maske, nachdem alle Effekte wie eine Helligkeitsanpassung zwischen Schwarz und Weiß kombiniert wurden. |
| **Globaler Kontrast** | Passen Sie den Kontrast der letzten Maske an, nachdem alle Effekte kombiniert wurden. |
| **Textur verwenden** | Schaltet die Verwendung einer benutzerdefinierten Texturmap ein oder aus. |
| **Micro-Details verwenden** | Schalten Sie die Verwendung benutzerdefinierter Mikrodetails ein oder aus. |

### Umgebungsverdeckung

| Parametername | Beschreibung |
| --- | --- |
| **Umkehren** | Kehre einfach die Verdeckung der Umgebung um, und zeichne Mikrodetails auf. |
| **Weichzeichnen** | Glätten Sie einfach Umgebungsgeräusche und Verdeckung-Mikrodetails. |
| **Saldo** | Passe die Balance von Verdeckung und Mikrodetails an. Verschiebe den Mittelpunkt in Richtung Schwarz oder Weiß, wie bei einer Helligkeitseinstellung. |
| **Kontrast** | Passen Sie den Kontrast/das Falloff nur der Umgebungsfarbe und der Mikrodetails an. |

### Textur

<table>
  <tr>
    <th>Parametername</th>
    <th>Beschreibung</th>
  </tr>
  <tr>
    <td><strong>Strukturdeckkraft</strong></td>
    <td>Passen Sie die Sichtbarkeit der benutzerdefinierten Textur an.</td>
  </tr>
  <tr>
    <td><strong>Invertieren</strong></td>
    <td>Kehre nur die eigene Struktur um.</td>
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
    <td>Wenn "Triplanar" aktiviert ist, wird die Textur aus drei Richtungen (X-, Y-, Z-Achse) projiziert, anstatt sich nur auf UVs zu verlassen.<br><ul><li>Ohne triplanar folgt die Textur dem UV-Layout.</li><li>Mit der Option "Dreidimensional" wird die Struktur aus mehreren Winkeln projiziert und verblendet.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Triplanarer Kontrast</strong></td>
    <td>Mit der Option "Triplanar Mapping" legst du fest, wie glatt eine Textur bei der Projektion übergeht. Diese Einstellung passt die Weichheit der Überblendung zwischen den Vorsprüngen aus jeder Richtung an.</td>
  </tr>
</table>

### Mikrodetails

| Parametername | Beschreibung |
| --- | --- |
| **Micro-Height** | Aktivieren oder deaktivieren Sie die Verwendung einer benutzerdefinierten Micro Height Map. |
| **Micro Normal** | Aktivieren oder deaktivieren Sie die Verwendung einer benutzerdefinierten Micro Normal-Karte. |
| **AO Radius** | Passen Sie den Radius (Bereich) der Verdeckung &quot;Umgebung&quot; in den Mikrodetails an. |
| **AO-Tiefe** | Passen Sie die Tiefe (Intensität) der Umgebungsintensität in den Mikrodetails an. |
