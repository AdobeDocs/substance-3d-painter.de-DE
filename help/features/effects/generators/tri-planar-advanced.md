---
title: Dreiplanar Fortgeschrittene
description: Erfahren Sie, wie Sie den Tri-Planar Advanced-Generator von Substance 3D Painter verwenden.
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 5%

---


# Dreiplanar Fortgeschrittene

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_tri_planar_advanced.png" alt=""/><br><strong>In:</strong>-Maske, Generator</td>
    <td style="border: 0;" valign="top"><strong>Beschreibung</strong><br>Der Tri-Planar Advanced-Generator ist eine eigenständige Version des Triplanar-Mischmodus mit manuellen Steuerungen für die volle Projektion, einschließlich der Steuerung aller Drehungs- und Versatzwerte für jede separate Achse. Im Vergleich zur nativen Füllgeometrie verwendet der Tri-Planar Advanced-Projektion Weltraum-Normale, um die drei Geometriedarstellungen zu überblenden, während die native Implementierung nur auf einer Low-Poly-Achse basiert. Dies führt zu mehr Kontrolle und genaueren Ergebnissen.<br><br>Der Tri-Planar Advanced-Generator gibt eine Schwarzweiß-Textur aus. Das ist nützlich, um eine planare Überblendung von einer benutzerdefinierten Maske oder einem Ankerpunkt zu erzeugen, die als Maske verwendet werden soll.<br><br> Baking geführt Positions- und Welt-Raum-Normale-Maps sind als Bildeingaben erforderlich. <a href="../../../baking/baking.md">Weitere Informationen zum Baking</a>.</td>
  </tr>
</table>

## Eingaben

| Eingabename | Beschreibung |
| --- | --- |
| **Welt-Raum-Normale** Farbe | Verwenden Sie die gebackene Weltraumnormalkarte. |
| **Position** Farbe | Verwenden Sie die Baking geführt Positionszuordnung. |
| **mask** Graustufen | Verwenden einer benutzerdefinierten Textur oder eines Ankerpunkts. |

## Parameter

<table>
  <tr>
    <th>Parametername</th>
    <th>Beschreibung</th>
  </tr>
  <tr>
    <td><strong>Projektion</strong></td>
    <td>Wählen Sie aus, ob alle Achsen oder nur eine einzelne Achse projiziert werden sollen.</td>
  </tr>
  <tr>
    <td><strong>Überblendmodus</strong></td>
    <td>Wähle die Füllmethode aus, um einen Übergang zwischen den Achsen zu erzeugen.<br><ul><li><strong>Linear</strong>: Bei der linearen Füllmethode ist die Füllübergangslinie gerade.</li><li><strong>Erweitert</strong>: Im Modus "Erweitert" werden Achsen auf der Grundlage des Maximalwerts zwischen den 3 Achsen und dem Normalwinkel an der angegebenen Position vermischt.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Überblendkontrast</strong></td>
    <td>Passen Sie an, wie stark die Überblendungslinie verwischt wird.</td>
  </tr>
  <tr>
    <td><strong>Struktur wiederholen</strong></td>
    <td>Passen Sie die Kachelung der Textur an.</td>
  </tr>
</table>

### X-Achse

| Parametername | Beschreibung |
| --- | --- |
| **Drehung X** | Drehe die X-Achsen-Texturen-Projektion. |
| **Versatz X X** | Bewegen Sie die Projektion der X-Achsen-Textur nach links oder rechts. |
| **Versatz X Y** | Verschiebe die Projektion der Textur der X-Achse nach oben oder unten. |

### Y-Achse

| Parametername | Beschreibung |
| --- | --- |
| **Drehung X** | Drehen Sie die Projektion der Textur der Y-Achse. |
| **Versatz Y X** | Bewegen Sie die Projektion der Textur der Y-Achse nach links oder rechts. |
| **Versatz Y J** | Verschiebe die Projektion der Textur der Y-Achse nach oben oder unten. |

### Achse Z

| Parametername | Beschreibung |
| --- | --- |
| **Drehung X** | Drehen Sie die Z-Achse Textur Projektion. |
| **Versatz Z X** | Verschieben Sie die Projektion der Z-Achse-Textur nach links oder rechts. |
| **Versatz Z Y** | Bewegen Sie die Projektion der Z-Achse-Textur nach oben oder unten. |
