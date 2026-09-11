---
title: 3D Linear gradient
description: Erfahren Sie, wie Sie den 3D Linear gradient-Generator von Substance 3D Painter verwenden.
source-git-commit: b095b9b437f75bbb3a3b85ee84a6850026c3bf98
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 1%

---


# 3D Linear gradient

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_3d_linear_gradient.webp" alt=""/><br><strong>In:</strong> Farbverlauf, Graustufen</td>
    <td style="border: 0;" valign="top"><strong>Beschreibung</strong><br>Der Positionsgenerator verwendet die Positionszuordnung, um einen Verlauf zwischen zwei 3D Linear gradient auf dem Mesh zu erstellen. <br><br>3D Linear gradient gibt eine Schwarzweiß-Textur aus. Daher ist es zum Generieren von Masken nützlich, einen linearen Verlauf in einem bestimmten Bereich zu platzieren.<br><br>Eine Baking geführt Positionszuordnung ist als Bildeingabe erforderlich. <a href="../../../baking/baking.md">Weitere Informationen zum Baking</a>.<br><br>Die Positionszuordnung weist jedem Punkt auf dem Mesh eine Farbe zu, die seiner Position zwischen 0 und 1 entlang der X-, Y- und Z-Achse entspricht. Das bedeutet, dass jeder Punkt auf dem Mesh eine eindeutige Farbe hat. Sie können Start- und Endpunkte für den linearen Verlauf festlegen, indem Sie die Positionszuordnungsfarbe an den Start- und Endpositionen auswählen.</td>
  </tr>
</table>

## Eingaben

| Eingabename | Beschreibung |
| --- | --- |
| **Position** | Verwenden Sie die Baking geführt Positionszuordnung. |

## Parameter

| Parametername | Beschreibung |
| --- | --- |
| **Umkehren** | Linearen Verlauf umkehren. |
| **Saldo** | Verschieben Sie die Mittelpunktposition des linearen Farbverlaufs. |
| **Kontrast** | Passen Sie den Kontrast des linearen Farbverlaufs an. |
| **3D-Positionsstart** | Legen Sie den Startpunkt des Verlaufs basierend auf den Farben der Positionskarte fest. Um den Ausgangspunkt einfach zu definieren, zeigen Sie die Positionszuordnung auf dem Bildschirm im Viewport an und wählen Sie den Ausgangspunkt mithilfe des Farbwählers aus. |
| **3D-Positionsende** | Legen Sie den Endpunkt des Verlaufs basierend auf den Farben der Positionskarte fest. Um den Endpunkt einfach zu definieren, zeigen Sie die Positionszuordnung auf dem Bildschirm im Viewport an und verwenden Sie den Farbwähler, um den Endpunkt auszuwählen. |
