---
description: Erfahren Sie, wie Sie den Substance 3D Painter-Generator "World Space Normals" verwenden.
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
    <td style="border: 0;" valign="top"><strong>Beschreibung</strong><br>Der Generator "World Space Normal" verwendet die gebackene Weltraum-Normalmap, um Ihr Modell einzufärben oder Effekte anzuwenden, die auf der Richtung basieren, in die jede Oberfläche im 3D-Raum zeigt. Zum Beispiel von oben nach unten.<br><br>Der Generator "World Space Normals" gibt eine monochrome (schwarz-weiß) Textur aus. Aus diesem Grund eignet sie sich gut zum Generieren von Masken, um verschiedene Effekte wie Dirt, Dust, Schnee oder Rost basierend auf den Gesichtsrichtungen anzuwenden.<br><br>Als Bildeingabe sind eine gepufferte Position und eine Normalmap für den Weltraum erforderlich. <a href="../../../baking/baking.md">Weitere Informationen zum Backen</a>.</td>
  </tr>
</table>

## Eingaben

| Eingabename | Beschreibung |
| --- | --- |
| **Textur** Farbe | Verwenden einer benutzerdefinierten Struktur oder eines Ankerpunkts. |
| **Normale im Weltraum** Farbe | Verwenden Sie die gebackene Weltraumnormalkarte. |
| **Positionsverlauf** Farbe | Verwenden Sie die Positionskarte. |

## Parameter

| Parametername | Beschreibung |
| --- | --- |
| **Globale Umkehr** | Kehrt das Endergebnis um, nachdem alle Effekte kombiniert wurden. |
| **Globaler Weichzeichner** | Wende eine gleichmäßige Weichzeichnung der finalen Maske an, nachdem alle Effekte kombiniert wurden. |
| **Globaler Saldo** | Verschiebe den Wert der letzten Maske, nachdem alle Effekte wie eine Helligkeitsanpassung zwischen Schwarz und Weiß kombiniert wurden. |
| **Globaler Kontrast** | Passen Sie den Kontrast der letzten Maske an, nachdem alle Effekte kombiniert wurden. |
| **Textur verwenden** | Schaltet die Verwendung einer benutzerdefinierten Texturmap ein oder aus. |

### Raum-Normale

| Parametername | Beschreibung |
| --- | --- |
| **Umkehren** | Kehre nur die Weltraum-Normalen um. |
| **Weichzeichnen** | Glätten Sie nur die Weltraum-Normalen. |
| **Saldo** | Passe nur die Balance der Weltraum-Normalen an und verschiebe den Mittelpunkt in Richtung Schwarz oder Weiß, wie bei einer Helligkeitsregelung. |
| **Kontrast** | Passen Sie nur den Kontrast/Abfall von Normalen im Weltraum an. |
| **Helligkeit** | Passe die Luminanz der Weltraum-Normalen an. |
| **Rechts nach links** | Passen Sie an, wie der Effekt von links nach rechts über das Gitter angewendet wird. |
| **Von oben nach unten** | Passen Sie an, wie der Effekt über das Gitter hinweg von oben nach unten angewendet wird. |
| **Von vorne nach hinten** | Passen Sie an, wie der Effekt über das Gitter hinweg von vorne nach hinten angewendet wird. |

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
    <td>Nur die eigene Textur umkehren.</td>
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
    <td>Passen Sie an, wie glatt eine Textur übergeht, wenn sie mithilfe von triplanarer Zuordnung projiziert wird. Dadurch wird die Weichheit der Überblendung zwischen den Vorsprüngen aus jeder Richtung eingestellt.</td>
  </tr>
</table>
