---
title: Automatische Zusammenführung
description: Erfahren Sie, wie Sie den automatischen Stitcher-Generator von Substance 3D Painter verwenden.
source-git-commit: b095b9b437f75bbb3a3b85ee84a6850026c3bf98
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 1%

---


# Automatische Zusammenführung

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_auto_stitcher.png" alt=""/><br><strong>In:</strong> Masche, Maschen</td>
    <td style="border: 0;" valign="top"><strong>Beschreibung</strong><br>Der automatische Stitcher-Generator erstellt automatisch einen Hefteffekt entlang prozedural generierter Pfade. Diese Pfade können auf der Grundlage von UV, Krümmungen oder einer benutzerdefinierten Eingabe-Map generiert werden.<br><br>Der automatische Stitcher-Generator gibt eine monochrome (schwarz-weiß) Textur aus. Daher eignet sie sich gut zum Generieren von Masken, um Fügeeffekte anzuwenden.<br><br>Um den Maskierungsmodus der Krümmung zu verwenden, ist eine Baking geführt Krümmungs-Map erforderlich. <a href="../../../baking/baking.md">Weitere Informationen zum Baking</a>.</td>
  </tr>
</table>

## Eingaben

<table>
  <tr>
    <th>Eingabename</th>
    <th>Beschreibung</th>
  </tr>
  <tr>
    <td><strong>Krümmung</strong> Graustufen</td>
    <td>Wählen Sie aus, wie die Heftpfade generiert werden:<br><ul><li><strong>UV-Maske</strong> generiert die Pfade entlang UV-Nähte.</li><li><strong>Krümmung </strong> erzeugt Pfade in der Nähe von Kanten.</li><li>Mit <strong>Benutzerdefinierte Eingabe</strong> können Sie steuern, wo Pfade mithilfe einer Map generiert werden.<br>Bei Verwendung von <strong>Benutzerdefinierter Eingabe</strong> werden Pfade in kontrastreichen Bereichen generiert.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Benutzerdefinierte Eingabe</strong> Graustufen</td>
    <td>Verwenden einer benutzerdefinierten Textur oder eines Ankerpunkts.</td>
  </tr>
</table>

## Parameter

<table>
  <tr>
    <th>Parametername</th>
    <th>Beschreibung</th>
  </tr>
  <tr>
    <td><strong>Maskenmodus</strong></td>
    <td>Wähle den Maskierungsmodus aus.<br><ul><li>UV-Maske: Masken auf Basis von UV-Inseln.</li><li>Krümmung: Masken auf Basis des Krümmungs-Map.</li><li>Benutzerdefinierte Eingabe: Masken, die auf einer benutzerdefinierten Eingabe-Textur basieren.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Path-Smoothness</strong></td>
    <td>Weichen Sie den Pfad, auf dem die Maschen angewendet werden, auf.</td>
  </tr>
  <tr>
    <td><strong>Pfadposition</strong></td>
    <td>Versatz der Pfadposition.</td>
  </tr>
  <tr>
    <td><strong>Maschengröße</strong></td>
    <td>Passen Sie die Stärke der Maschen an.</td>
  </tr>
  <tr>
    <td><strong>Maschenweite</strong></td>
    <td>Die Breite der Maschen anpassen.</td>
  </tr>
  <tr>
    <td><strong>Maschenlänge</strong></td>
    <td>Länge der Maschen anpassen.</td>
  </tr>
  <tr>
    <td><strong>Rundheit zusammenfügen</strong></td>
    <td>Richten Sie die Rundheit der Maschen ein.</td>
  </tr>
  <tr>
    <td><strong>Jitter</strong></td>
    <td>Passen Sie den Jitter in die Fließrichtung der Maschen an.</td>
  </tr>
</table>

## Beispiele

<table>
  <tr>
    <td><img src="../../../assets/generators/examples/auto-stitcher/custom-input2.png" alt=""/></td>
    <td>Dieses Beispiel zeigt, wie benutzerdefinierte Eingaben Heftpfade erstellen. <br><ul><li>Die Schwarz-Weiß-Grundfarbe zeigt die Rauschen-Texturen an, die wir als benutzerdefinierte Eingabe für den Autostitcher-Generator verwenden.</li><li>Der Autostitcher-Generator maskiert die rote Ebene und lässt die rot zusammengefügten Pfade sichtbar.</li><li>Beachten Sie, dass die rot zusammengefügten Pfade in ausreichend große schwarze oder weiße Bereiche der benutzerdefinierten Rauschen-Textur passen. Die rote Naht verläuft nie von weiß nach schwarz oder von schwarz nach weiß.</li></ul><br>Die Abbildung unten zeigt die einfache Ebenenkonfiguration, mit der dieses Beispiel erstellt wurde.<br><br><img src="../../../assets/generators/examples/auto-stitcher/custom-input-layer-stack.png" alt=""/></td>
  </tr>
</table>
