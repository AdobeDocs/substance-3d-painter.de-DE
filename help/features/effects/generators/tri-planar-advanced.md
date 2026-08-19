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
    <td style="border: 0;" valign="top"><strong>Beschreibung</strong><br>Der Tri-Planar Advanced-Generator ist eine eigenständige Version des triplanaren Mischmodus mit manuellen Steuerungen für die vollständige Projektion, einschließlich der Steuerung aller Drehungs- und Versatzwerte für jede separate Achse. Im Vergleich zur nativen Füllprojektion verwendet der Tri-Planar Advanced-Generator Weltraum-Normalen, um die drei Projektionsachsen zu überblenden, während die native Implementierung nur auf einer Low-Poly-Geometrie basiert. Dies führt zu mehr Kontrolle und genaueren Ergebnissen.<br><br>Der Tri-Planar Advanced-Generator gibt eine monochrome (schwarz-weiß) Textur aus. Das ist nützlich, um eine dreiflächige Überblendung von einer benutzerdefinierten Maske oder einem Ankerpunkt zu erstellen, die als Maske verwendet werden soll.<br><br>Als Bildeingabe sind eine gepufferte Position und eine Normalmap für den Weltraum erforderlich. <a href="../../../baking/baking.md">Weitere Informationen zum Backen</a>.</td>
  </tr>
</table>

## Eingaben

| Eingabename | Beschreibung |
| --- | --- |
| **Normaler Weltraum** Farbe | Verwenden Sie die gebackene Weltraumnormalkarte. |
| **Position** Farbe | Verwenden Sie die Positionskarte. |
| **mask** Graustufen | Verwenden einer benutzerdefinierten Struktur oder eines Ankerpunkts. |

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
    <td>Wählen Sie die Füllmethode aus, um die Überblendung achsübergreifend durchzuführen.<br><ul><li><strong>Linear</strong>: Bei der linearen Füllmethode ist die Füllübergangslinie gerade.</li><li><strong>Erweitert</strong>: Im Modus "Erweiterte Füllmethode" werden die Achsen basierend auf dem Maximalwert zwischen den 3 Achsen und dem Normalwinkel an der angegebenen Position vermischt.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Überblendkontrast</strong></td>
    <td>Passen Sie an, wie stark die Überblendungslinie verwischt wird.</td>
  </tr>
  <tr>
    <td><strong>Struktur wiederholen</strong></td>
    <td>Passen Sie die Unterteilung der Maskenstruktur an.</td>
  </tr>
</table>

### X-Achse

| Parametername | Beschreibung |
| --- | --- |
| **Drehung X** | Drehe die Texturprojektion &quot;X-Achse&quot;. |
| **Versatz X X** | Verschieben Sie die Texturprojektion &quot;X-Achse&quot; nach links oder rechts. |
| **Versatz X Y** | Verschieben Sie die Texturprojektion &quot;X-Achse&quot; nach oben oder unten. |

### Y-Achse

| Parametername | Beschreibung |
| --- | --- |
| **Drehung X** | Drehe die Texturprojektion &quot;Y-Achse&quot;. |
| **Versatz Y X** | Verschieben Sie die Texturprojektion &quot;Y-Achse&quot; nach links oder rechts. |
| **Versatz Y J** | Verschieben Sie die Texturprojektion der Y-Achse nach oben oder unten. |

### Achse Z

| Parametername | Beschreibung |
| --- | --- |
| **Drehung X** | Drehe die Texturprojektion auf der Z-Achse. |
| **Versatz Z X** | Verschieben Sie die Texturprojektion &quot;Z-Achse&quot; nach links oder rechts. |
| **Versatz Z Y** | Verschieben Sie die Texturprojektion auf der Z-Achse nach oben oder unten. |
