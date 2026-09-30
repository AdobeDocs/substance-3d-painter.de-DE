---
title: Richtungsabstand
description: Erfahren Sie, wie Sie den Richtungsabstand-Filter in Substance 3D Painter verwenden.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '326'
ht-degree: 1%
---

# Richtungsabstand

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="./Resources/icon_directional_distance.png" alt="Richtungsabstand-Symbol" title="Richtungsabstand"/><br><strong>In:</strong> Effekte/Farbe, Abstand, Richtung, Leck, Regen</td>
    <td style="border: 0;" valign="top">Beschreibung<br>Der Richtungsabstand-Filter erstellt einen Abstandsverlauf, der sich in die gewählte Richtung bewegt.<br>Er wird auf einer Textur-Ebene verwendet, um Richtungsstreifen, Lecks und andere entfernungsbasierte Effekte zu erstellen. Du kannst den Kanalfilter auch als Richtungsabstand für den Height-Kanal verwenden, um dem normalen Kanal mehr Tiefe zu verleihen.</td>
  </tr>
</table>

## Eingaben

| Eingabename | Beschreibung |
| --- | --- |
| **Abstands-Map:** Graustufen | Verwenden einer benutzerdefinierten Textur oder eines Ankerpunkts. |

## Parameter

| Parametername | Beschreibung |
| --- | --- |
| **Entfernung:** | Passen Sie die zurückgelegte Entfernung des Abstandsverlaufs im normalisierten Bildbereich an, wobei 1 der Länge der Bildschmalseite entspricht. |
| **Winkel:** | Passen Sie die Richtung des Abstandsverlaufs in Windungen an, wobei 0 horizontal nach rechts oder entlang eines (1,0) Vektors zeigt. |
| **Kontrast:** | Passen Sie den Kontrast oder den Tonfall des Ergebnisses an. |
| **Abstands-Map-Multiplikator:** | Passen Sie an, wie stark der Abstands-Map die maximale Entfernung beeinflusst. Dieser Parameter hat keine Auswirkungen, wenn der Abstands-Map-Eingang nicht angeschlossen ist. |

## Beispiele

Im folgenden Beispiel verwenden wir den Generatorfilter, um den Richtungsabstand &quot;Zellen 2&quot; dreidimensional erscheinen zu lassen.

![](../../../../assets/filters/directional-distance/3d.png)

Dies wird erreicht, indem eine Füllebene mit aktiviertem Height-Kanal erstellt wird, der auf den Wert 1 gesetzt wird.

Füge dann eine schwarze Maske zur Füllebene hinzu. Füge in der Maske eine Fläche mit der Graustufenfarbe **Zellen 2** hinzu. Dadurch wird die folgende Maske erstellt.

>[!NOTE]
>
> Sie können die Maske im **Viewport** anzeigen, indem Sie die Alt-Taste gedrückt halten und auf das Maskensymbol klicken, oder verwenden Sie bei ausgewählter Füllebene das Dropdown-Menü für den Kanal im **Viewport**, um **Maske** auszuwählen.

![](../../../../assets/filters/directional-distance/cells2.png)

Füge einen Richtungsabstand zur Maske hinzu. Wähle den Maskenfilter aus.

Passen Sie die Filtereinstellungen für das gewünschte Ergebnis an, aber die Maske sollte ungefähr so aussehen wie im Beispiel unten.

![](../../../../assets/filters/directional-distance/result.png)

Wechseln Sie zurück zur Material-Ansicht, um die Auswirkungen im Viewport zu sehen.
