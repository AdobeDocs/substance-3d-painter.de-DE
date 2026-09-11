---
title: Hell
description: Erfahren Sie, wie Sie den Lichtgenerator von Substance 3D Painter verwenden.
source-git-commit: b095b9b437f75bbb3a3b85ee84a6850026c3bf98
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 3%

---


# Licht

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_light.webp" alt=""/><br><strong>In:</strong>-Maske, Generator</td>
    <td style="border: 0;" valign="top"><strong>Beschreibung</strong><br>Der Lichtgenerator simuliert ein auf Ihren Mesh leuchtendes Richtlicht anhand der Welt-Raum-Normale- und Positionsabbildungen.<br><br>Der Lichtgenerator kann auf einer Füllebene oder als Maske verwendet werden. Bei Verwendung in einer Füllebene gibt der Generator Farbkanäle, Metalitätskanäle, Specular-Rauheit, Normal- und Height-Kanäle aus, die in verschiedenen Kombinationen verwendet werden können, um verschiedene Effekte zu erzeugen. Es wird empfohlen, die Kanalansichten im Viewport zu durchlaufen, um zu verstehen, wie sich der Lichtgenerator auf jeden Kanal auswirkt.<br><br> Baking geführt Positions- und Welt-Raum-Normale-Maps sind als Bildeingaben erforderlich. <a href="../../../baking/baking.md">Weitere Informationen zum Baking</a>.</td>
  </tr>
</table>

## Eingaben

| Eingabename | Beschreibung |
| --- | --- |
| **Welt-Raum-Normale** Farbe | Verwenden Sie die gebackene Weltraumnormalkarte. |
| **Position** Farbe | Verwenden Sie die Baking geführt Positionszuordnung. |

## Parameter

| Parametername | Beschreibung |
| --- | --- |
| **Umkehren** | Umkehren der Ausgabefarbzuordnung. |
| **Horizontaler Winkel** | Stellen Sie den horizontalen Winkel des gefälschten Lichts ein. |
| **Vertikaler Winkel** | Legen Sie den vertikalen Winkel des gefälschten Lichts fest. |
| **Glanzlichter hervorheben** | Passen Sie die Abstandsverteilung des markierten Bereichs an. |
| **Ebene hervorheben** | Passen Sie den Kontrast der Glanzlichter an. |
| **Lichtdämpfung** | Passe den Lichtabfall an. |
