---
title: 3D-Abstand
description: Erfahren Sie, wie Sie den 3D-Distanzgenerator von Substance 3D Painter verwenden.
source-git-commit: b095b9b437f75bbb3a3b85ee84a6850026c3bf98
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 1%

---


# 3D-Abstand

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_3d_distance.webp" alt=""/><br><strong>In:</strong>-Maske, Generator</td>
    <td style="border: 0;" valign="top"><strong>Beschreibung</strong><br>Der 3D-Abstandsgenerator definiert einen Punkt im 3D-Raum (Quellpunkt) und zeigt den Abstand zu diesem Punkt mit einem monochromen Farbverlauf an. Bereiche auf der Gitteroberfläche, die näher am Punkt liegen, sind dunkler und Bereiche, die weiter entfernt liegen, sind heller (standardmäßig).<br><br>Als Bildeingabe ist eine vorgefertigte Positionszuordnung erforderlich. <a href="../../../baking/baking.md">Weitere Informationen zum Backen hier</a>.<br><br>Die 3D-Entfernung gibt eine monochrome (schwarz-weiß) Textur aus. Das ist nützlich, wenn du Masken generieren willst, die einen Verlauf weg von einer bestimmten Position erzeugen.<br><br></td>
  </tr>
</table>

## Eingaben

| Eingabename | Beschreibung |
| --- | --- |
| **Position** | Berechnen Sie die Entfernung mithilfe der Positionskarte. |

## Parameter

| Parametername | Beschreibung |
| --- | --- |
| **Umkehren** | Verlauf umkehren. |
| **Position X** | Transformieren Sie den Quellpunkt entlang der x-Achse. |
| **Position Y** | Transformieren Sie den Quellpunkt entlang der y-Achse. |
| **Position Z** | Transformieren Sie den Quellpunkt entlang der z-Achse. |
| **Radius** | Passen Sie die Größe des Abstands an. |
| **Offset** | Verschieben Sie die Start- und Endposition des Verlaufs zum oder vom Quellpunkt weg. Wenn Sie den Abstand vom Quellpunkt verschieben (den Versatz erhöhen), wird der dunkle Bereich in der Nähe des Quellpunkts vergrößert. Wenn Sie näher an den Quellpunkt heranrücken, wird der Verlauf aufgehellt und möglicherweise vollständig entfernt, wenn **Offset** auf 0 gesetzt ist. |
| **Kontrast** | Passen Sie den Kontrast des sphärischen Farbverlaufs an. |
