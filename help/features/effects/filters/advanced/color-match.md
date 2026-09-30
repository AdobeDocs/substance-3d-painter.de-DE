---
title: Farbabgleich
description: Erfahren Sie, wie Sie den Farbabgleich-Filter in Substance 3D Painter verwenden.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 1%
---

# Farbabgleich

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="./Resources/icon_color_match.png" alt="Symbol &quot;Farbabgleich&quot;" title="Farbabgleich"/><br><strong>In:</strong> Effekte/Anpassungen</td>
    <td style="border: 0;" valign="top">Beschreibung<br>Der Farbabgleich-Filter stimmt einen definierten Quellfarbbereich mit einem Zielfarbbereich überein, wobei Eingabeschlitze zum Definieren von Quell- und Zielwerten unterstützt werden. Mit dem Farbabgleich können Sie Details beibehalten, während Sie die Farbe einer Oberfläche ändern, wobei Sie steuern können, wie Farbton, Chrominanz und Luminanz behandelt werden.<br>Farbabgleich wird für eine Füllebene verwendet, um Feinfarbanpassungen vorzunehmen.</td>
  </tr>
</table>

## Eingaben

| Eingabename | Beschreibung |
| --- | --- |
| **Quellfarbe:** | Eingabeschacht für die Quellfarbe. Verwenden einer benutzerdefinierten Farbzuordnung oder eines Ankerpunkts. |
| **Zielfarbe:** | Eingabebereich für die Zielfarbe. Verwenden einer benutzerdefinierten Farbzuordnung oder eines Ankerpunkts. |

## Parameter

<table>
  <tr>
    <th>Parametername</th>
    <th>Beschreibung</th>
  </tr>
  <tr>
    <td><strong>Quellfarbmodus:</strong></td>
    <td>Wählen Sie die Quelle der Quellfarbe aus.<br><ul><li><strong>Durchschnitt</strong>: Verwenden Sie die vorhandene Farbe des Materials als Quellfarbe. Beachten Sie, dass der Mischmodus für Ebenen auf <strong>Passthrough</strong> festgelegt werden muss.</li><li><strong>Parameter</strong>: Legen Sie die Quellfarbe mithilfe eines Parameters fest.</li><li><strong>Eingabe</strong>: Legen Sie die Quellfarbe mithilfe einer Bildeingabe fest.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Quellfarbe:</strong></td>
    <td>Passen Sie die Quellfarbe an, wenn <strong>Quellfarbmodus</strong> auf <strong>Parameter</strong> festgelegt ist.</td>
  </tr>
  <tr>
    <td><strong>Zielfarbmodus:</strong></td>
    <td>Wählen Sie die Quelle der Zielfarbe aus.<br><ul><li><strong>Parameter</strong>: Legen Sie die Zielfarbe mithilfe eines Parameters fest.</li><li><strong>Eingabe</strong>: Legen Sie die Zielfarbe mithilfe einer Bildeingabe fest.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Zielfarbe:</strong></td>
    <td>Passen Sie die Zielfarbe an, wenn <strong>Zielfarbmodus</strong> auf <strong>Parameter</strong> festgelegt ist.</td>
  </tr>
  <tr>
    <td><strong>Benutzerdefinierte Farbvariationen:</strong></td>
    <td>Mit den Steuerungen für Farbton, Chroma und Luminanz lässt sich die Farbgebung gezielt anpassen.</td>
  </tr>
  <tr>
    <td><strong>Farbton:</strong></td>
    <td>Passen Sie die auf das Ergebnis angewendete Farbtonvariation an.</td>
  </tr>
  <tr>
    <td><strong>Chroma:</strong></td>
    <td>Passen Sie die Chroma-Variation des Ergebnisses an.</td>
  </tr>
  <tr>
    <td><strong>Luminanz:</strong></td>
    <td>Passen Sie die Luminanzvariation an, die auf das Ergebnis angewendet wird.</td>
  </tr>
</table>