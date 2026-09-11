---
title: Umgebungsverdeckung
description: Erfahren Sie, wie Sie den Ambient occlusion-Generator von Substance 3D Painter verwenden.
source-git-commit: b095b9b437f75bbb3a3b85ee84a6850026c3bf98
workflow-type: tm+mt
source-wordcount: '542'
ht-degree: 5%

---


# Umgebungsverdeckung

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_ambient_occlusion.webp" alt=""/><br><strong>In:</strong> Maske, Generator, Graustufen, Überblendung</td>
    <td style="border: 0;" valign="top"><strong>Beschreibung</strong><br>Der Umgebungsmaskengenerator erstellt eine Verdeckung, die auf der gebackenen Umgebungsmaskenkarte basiert, mit der Option, eine Textur oder Mikrodetails in die Verdeckung einzufügen.<br><br>Wenn Sie den Ambient occlusion-Generator zum Erstellen einer Ebenenmaske verwenden, müssen Sie möglicherweise die Ambient occlusion-Ausgabe invertieren. Standardmäßig gibt der Generator verdeckte Bereiche als dunkle und nicht verdeckte Bereiche als helle aus. Wenn sie als Maske verwendet wird, ist die maskierte Ebene nur in nicht verdeckten Bereichen sichtbar. Durch Umkehren der Ausgabe wird sichergestellt, dass die maskierte Ebene nur in verdeckten Bereichen angezeigt wird.<br><br> Baking geführt Positions-, ambient occlusion- und Welt-Raum-Normale-Maps sind als Bildeingaben erforderlich. <a href="../../../baking/baking.md">Weitere Informationen zum Baking</a>.</td>
  </tr>
</table>

## Eingaben

| Eingabename | Beschreibung |
| --- | --- |
| Textur | Verwenden einer benutzerdefinierten Textur oder eines Ankerpunkts. |
| Micro-Normalfarbe | Verwenden Sie eine spezielle normale Textur oder einen Ankerpunkt. |
| Farbe eines Micro Heights | Verwenden einer benutzerdefinierten Textur oder eines Ankerpunkts. |
| Ambient occlusion Graustufen | Verwenden Sie die Baking geführt Ambient occlusion-Map. |
| Welt-Raum-Normale-Farbe | Verwenden Sie die gebackene Weltraumnormalkarte. |
| Positionsverlaufsfarbe | Verwenden Sie die Baking geführt Positionszuordnung. |

## Parameter

| Parametername | Beschreibung |
| --- | --- |
| **Globale Umkehr** | Kehrt das Endergebnis um, nachdem alle Effekte kombiniert wurden. |
| **Globaler Weichzeichner** | Glätten Sie die endgültige Maske gleichmäßig, nachdem alle Effekte kombiniert wurden. |
| **Globaler Saldo** | Verschiebe den Wert der letzten Maske, nachdem alle Effekte wie eine Helligkeitsanpassung zwischen Schwarz und Weiß kombiniert wurden. |
| **Globaler Kontrast** | Passen Sie den Kontrast der letzten Maske an, nachdem alle Effekte kombiniert wurden. |
| **Textur verwenden** | Schaltet die Verwendung einer benutzerdefinierten Textur-Map ein oder aus. |
| **Micro-Details verwenden** | Schalten Sie die Verwendung benutzerdefinierter Mikrodetails ein oder aus. |

### Umgebungsverdeckung

| Parametername | Beschreibung |
| --- | --- |
| **Umkehren** | Invertieren Sie nur Ambient occlusion- und Mikrodetails. |
| **Weichzeichnen** | Glätten Sie nur Ambient occlusion- und Mikrodetails. |
| **Saldo** | Passe die Balance von Ambient occlusion- und Mikrodetails an und verschiebe den Mittelpunkt in Richtung Schwarz oder Weiß, wie bei einer Helligkeitsregelung. |
| **Kontrast** | Passen Sie den Kontrast/Abfall nur des Ambient occlusion und der Mikrodetails an. |

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
    <td>Kehre nur die Textur um.</td>
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
    <td>Wenn Triplanar aktiviert ist, wird die Textur aus drei Richtungen projiziert (X-, Y-, Z-Achsen), anstatt sich nur auf UVs zu verlassen.<br><ul><li>Ohne triplanar folgt die Textur dem UV-Layout.</li><li>Bei der Dreiecksform wird die Textur aus mehreren Winkeln projiziert und verblendet.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Triplanarer Kontrast</strong></td>
    <td>Mit der Option "Triplanar Mapping" legst du fest, wie glatt eine Textur bei der Projektion übergeht. Diese Einstellung passt die Weichheit der Überblendung zwischen den Vorsprüngen aus jeder Richtung an.</td>
  </tr>
</table>

### Mikrodetails

| Parametername | Beschreibung |
| --- | --- |
| **Micro-Height** | Aktivieren oder deaktivieren Sie die Verwendung einer benutzerdefinierten Micro Höhen-Map. |
| **Micro Normal** | Aktivieren oder deaktivieren Sie die Verwendung einer benutzerdefinierten Micro Normalen-Map. |
| **AO Radius** | Passen Sie den Radius (Bereich) der Verdeckung &quot;Umgebung&quot; in den Mikrodetails an. |
| **AO-Tiefe** | Passen Sie die Tiefe (Intensität) des Ambient occlusion in Mikrodetails an. |
