---
description: Erfahren Sie, wie Sie den Welt-Raum-Normale-Generator von Substance 3D Painter verwenden.
title: Raum-Normalen
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '567'
ht-degree: 8%

---


# Raum-Normalen

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_world_space_normals.png" alt=""/><br><strong>In:</strong> Maske, Generator, Graustufen, Überblendung</td>
    <td style="border: 0;" valign="top"><strong>Beschreibung</strong><br>Der Modellgenerator verwendet die Baking geführt Weltraum-Normalen-Map, um Ihr Welt-Raum-Normale zu färben oder Effekte anzuwenden, die auf der Richtung basieren, in die jede Fläche im 3D-Raum zeigt. Zum Beispiel von oben nach unten.<br><br>Der Welt-Raum-Normale-Generator gibt eine Schwarzweiß-Textur aus. Aus diesem Grund eignet sie sich gut zum Generieren von Masken, um verschiedene Effekte wie Dirt, Dust, Schnee oder Rost basierend auf den Gesichtsrichtungen anzuwenden.<br><br> Baking geführt Positions- und Welt-Raum-Normale-Maps sind als Bildeingaben erforderlich. <a href="../../../baking/baking.md">Weitere Informationen zum Baking</a>.</td>
  </tr>
</table>

## Eingaben

| Eingabename | Beschreibung |
| --- | --- |
| **Textur** Farbe | Verwenden einer benutzerdefinierten Textur oder eines Ankerpunkts. |
| **Welt-Raum-Normale** Farbe | Verwenden Sie die gebackene Weltraumnormalkarte. |
| **Positionsverlauf** Farbe | Verwenden Sie die Baking geführt Positionszuordnung. |

## Parameter

| Parametername | Beschreibung |
| --- | --- |
| **Globale Umkehr** | Kehrt das Endergebnis um, nachdem alle Effekte kombiniert wurden. |
| **Globaler Weichzeichner** | Wende eine gleichmäßige Weichzeichnung der finalen Maske an, nachdem alle Effekte kombiniert wurden. |
| **Globaler Saldo** | Verschiebe den Wert der letzten Maske, nachdem alle Effekte wie eine Helligkeitsanpassung zwischen Schwarz und Weiß kombiniert wurden. |
| **Globaler Kontrast** | Passen Sie den Kontrast der letzten Maske an, nachdem alle Effekte kombiniert wurden. |
| **Textur verwenden** | Schaltet die Verwendung einer benutzerdefinierten Textur-Map ein oder aus. |

### Raum-Normale

| Parametername | Beschreibung |
| --- | --- |
| **Umkehren** | Kehre nur die Weltraum-Normalen um. |
| **Weichzeichnen** | Glätten Sie nur die Weltraum-Normalen. |
| **Saldo** | Passen Sie nur die Balance der Welt-Raum-Normale an, indem Sie den Mittelpunkt wie einen Helligkeitsregler in Richtung Schwarz oder Weiß verschieben. |
| **Kontrast** | Passen Sie nur den Kontrast/Abfall von Normalen im Weltraum an. |
| **Helligkeit** | Passe die Luminanz der Welt-Raum-Normale an. |
| **Rechts nach links** | Passen Sie an, wie der Effekt von links nach rechts über den Mesh angewendet wird. |
| **Von oben nach unten** | Passen Sie an, wie der Effekt auf den Mesh angewendet wird. |
| **Von vorne nach hinten** | Passen Sie an, wie der Effekt auf den Mesh angewendet wird. |

#### Raum-Normale/von rechts nach links

| Parametername | Beschreibung |
| --- | --- |
| **Umkehren** | Kehren Sie die Verlaufsrichtung von rechts nach links um. |
| **Füllmethode** | Wählen Sie den [Mischmodus](../../../interface/layer-stack/blending-modes.md) für die aktuelle Ebene aus. |

#### Raum-Normale/von oben nach unten

| Parametername | Beschreibung |
| --- | --- |
| **Umkehren** | Verlauf von oben nach unten umkehren. |
| **Füllmethode** | Wählen Sie den [Mischmodus](../../../interface/layer-stack/blending-modes.md) für die aktuelle Ebene aus. |

#### Raum-Normale/von vorne nach hinten

| Parametername | Beschreibung |
| --- | --- |
| **Umkehren** | Kehren Sie die Verlaufsrichtung von vorne nach hinten um. |
| **Füllmethode** | Wählen Sie den [Mischmodus](../../../interface/layer-stack/blending-modes.md) für die aktuelle Ebene aus. |

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
    <td>Nur die benutzerdefinierte Textur umkehren.</td>
  </tr>
  <tr>
    <td><strong>Graustufenkonvertierung</strong></td>
    <td>Legen Sie die Methode fest, die für die Konvertierung von Vollfarben in Graustufen verwendet wird. Der <a href="grayscale-conversion.md">Graustufen-Konvertierungsgenerator enthält weitere Informationen über die Funktionsweise der einzelnen Methoden.</a></td>
  </tr>
  <tr>
    <td><strong>Überblendmodus</strong></td>
    <td>Passen Sie den zu verwendenden Mischvorgang an. Weitere Informationen finden Sie auf der entsprechenden Seite zu Füllmethoden.</td>
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
    <td>Passen Sie an, wie glatt eine Textur übergeht, wenn sie mithilfe von triplanarem Mapping projiziert wird. Dadurch wird die Weichheit der Überblendung zwischen den Projektionen aus jeder Richtung angepasst.</td>
  </tr>
</table>
