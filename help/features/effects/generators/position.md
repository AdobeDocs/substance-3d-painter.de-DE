---
title: Position
description: Erfahren Sie, wie Sie den Positionsgenerator von Substance 3D Painter verwenden.
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '537'
ht-degree: 7%

---


# Position

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_position.webp" alt=""/><br><strong>In:</strong> Mesh, UV, Abstand</td>
    <td style="border: 0;" valign="top"><strong>Beschreibung</strong><br>Der Positionsgenerator verwendet die Karten für die gebackene Position und den Weltraum, um eine Verlaufsmaske basierend auf der Position des Materials im 3D-Raum (wie von oben nach unten oder von Seite zu Seite) zu erstellen.<br><br>Der Positionsgenerator gibt eine monochrome (schwarz-weiß) Textur aus. Daher eignet sie sich gut zum Generieren von Verlaufsmasken basierend auf der Position im Weltraum.<br><br>Als Bildeingabe sind eine gepufferte Position und eine Normalmap für den Weltraum erforderlich. <a href="../../../baking/baking.md">Weitere Informationen zum Backen</a>.</td>
  </tr>
</table>

## Eingaben

| Eingabename | Beschreibung |
| --- | --- |
| **Textur** Farbe | Verwenden einer benutzerdefinierten Struktur oder eines Ankerpunkts. |
| **Positionsverlauf** Farbe | Verwenden Sie die Positionskarte. |
| **Normale im Weltraum** Farbe | Verwenden Sie die gebackene Weltraumnormalkarte. |

## Parameter

| Parametername | Beschreibung |
| --- | --- |
| **Globale Umkehr** | Kehrt das Endergebnis um, nachdem alle Effekte kombiniert wurden. |
| **Globaler Weichzeichner** | Lasse die finale Maske nach der Kombination aller Verläufe gleichmäßig verschwimmen. |
| **Globaler Saldo** | Passe die Balance der letzten Maske an, nachdem alle Verläufe zwischen Schwarz und Weiß kombiniert wurden, wie bei einer Helligkeitsanpassung. |
| **Globaler Kontrast** | Passen Sie den Kontrast der letzten Maske an, nachdem alle Verläufe kombiniert wurden. |
| **Textur verwenden** | Schaltet die Verwendung einer benutzerdefinierten Texturmap ein oder aus. |

### Position Verlauf

| Parametername | Beschreibung |
| --- | --- |
| **Umkehren** | Nur den Positionsverlauf umkehren. |
| **Saldo** | Passe die Balance nur des Positionsverlaufs an und verschiebe den Mittelpunkt wie bei einem Helligkeitsregler in Richtung Schwarz oder Weiß. |
| **Kontrast** | Passen Sie den Kontrast/Abfall nur des Positionsverlaufs an. |
| **Helligkeit** | Passe die Luminanz des Positionsverlaufs an. |
| **Rechts nach links** | Passen Sie an, wie der Effekt von links nach rechts über das Gitter angewendet wird. |
| **Von oben nach unten** | Passen Sie an, wie der Effekt über das Gitter hinweg von oben nach unten angewendet wird. |
| **Von vorne nach hinten** | Passen Sie an, wie der Effekt über das Gitter hinweg von vorne nach hinten angewendet wird. |

#### Position Verlauf/von rechts nach links

| Parametername | Beschreibung |
| --- | --- |
| **Umkehren** | Kehren Sie die Verlaufsrichtung von rechts nach links um. |
| **Füllmethode** | Wählen Sie den [Mischmodus](../../../interface/layer-stack/blending-modes.md) aus, der für den Rechts-Links-Verlauf verwendet werden soll. |

#### Position Verlauf/von oben nach unten

| Parametername | Beschreibung |
| --- | --- |
| **Umkehren** | Kehren Sie die Verlaufsrichtung von oben nach unten um. |
| **Füllmethode** | Wählen Sie den [Mischmodus](../../../interface/layer-stack/blending-modes.md) aus, der für den oberen bis unteren Farbverlauf verwendet werden soll. |

#### Position Verlauf/von vorne nach hinten

| Parametername | Beschreibung |
| --- | --- |
| **Umkehren** | Kehren Sie die Verlaufsrichtung von vorne nach hinten um. |
| **Füllmethode** | Wählen Sie den [Mischmodus](../../../interface/layer-stack/blending-modes.md) aus, der für den Vorder-/Rückwärtsverlauf verwendet werden soll. |

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
    <td>Umkehren der benutzerdefinierten Texturmap.</td>
  </tr>
  <tr>
    <td><strong>Graustufenkonvertierung</strong></td>
    <td>Legen Sie die Methode fest, die für die Konvertierung von Vollfarben in Graustufen verwendet wird. Der <a href="grayscale-conversion.md">Graustufen-Konvertierungsgenerator enthält weitere Informationen über die Funktionsweise der einzelnen Methoden.</a></td>
  </tr>
  <tr>
    <td><strong>Überblendmodus</strong></td>
    <td>Wählen Sie den zu verwendenden <a href="../../../interface/layer-stack/blending-modes.md">Mischmodus</a> aus.</td>
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
</table>
