---
title: UV-Random-Farbe
description: Erfahren Sie, wie Sie den UV-Zufallsfarbengenerator von Substance 3D Painter verwenden.
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '182'
ht-degree: 2%

---


# UV-Random-Farbe

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_uv_random_color.png" alt=""/><br><strong>Im:</strong>-Dienstprogramm, Maske</td>
    <td style="border: 0;" valign="top"><strong>Beschreibung</strong><br>Der UV-Zufallsfarbengenerator weist jeder UV-Insel eindeutige Farbflächen zu. Dies ist oft nützlich als Diagnosewerkzeug mit komplexen Netzen.<br><br>UV Random color kann entweder zum Erstellen einer Maske (Schwarzweißausgabe) oder direkt als Füllebene verwendet werden, um basierend auf UV-Inseln Farbvariationen auf Ihr Gitter anzuwenden, z. B. um jede Planke eines Holzbodens randomisieren zu lassen.</td>
  </tr>
</table>

## Eingaben

| Eingabename | Beschreibung |
| --- | --- |
| **Benutzerdefinierter Verlauf** | Verwenden Sie eine Verlaufsumsetzung, um den Farbbereich zu definieren. |

## Parameter

<table>
  <tr>
    <th>Parametername</th>
    <th>Beschreibung</th>
  </tr>
  <tr>
    <td><strong>Zufalls-Startwert</strong></td>
    <td>Legen Sie den Startwert fest, der zum Generieren der Textur des Dirts verwendet wird. <br><ul><li>Klicken Sie auf "Zufällig", um zu einer anderen Zufallsverteilung zu wechseln.</li><li>Klicken Sie auf den Stift, um den aktuellen Wert für das Seed anzuzeigen, und geben Sie bei Bedarf einen bestimmten Wert ein.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Farbquellenmodus</strong></td>
    <td>Legt den verwendeten Farbquellenmodus fest. <br><ul><li><strong>Zufällig</strong>: Im Zufallsmodus werden die Farben nach dem Zufallsprinzip definiert und zugewiesen.</li><li><strong>Benutzerdefinierter Verlauf</strong>: Im Modus "Benutzerdefinierter Verlauf" steht Ihnen eine zusätzliche Eingabe zur Verfügung, um eine benutzerdefinierte Verlaufsumsetzung hinzuzufügen, aus der die Farben ausgewählt werden.</li></ul></td>
  </tr>
</table>
