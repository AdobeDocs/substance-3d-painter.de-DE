---
title: Aufblasen von Schrumpffolie
description: Erfahren Sie, wie Sie den aufgeblasenen Schrumpffoliengenerator von Substance 3D Painter verwenden.
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 3%

---


# Aufblasen von Schrumpffolie

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_inflate_shrinkwrap.webp" alt=""/><br><strong>In:</strong> Shrinkwrap, inflate, generator, randomseed</td>
    <td style="border: 0;" valign="top"><strong>Beschreibung</strong><br>Der Generator zum Aufblasen von Schrumpffolien fügt Falten hinzu, die den Effekt eines dünnen Materials nachahmen, das über die Oberfläche Ihres Gitters gestreckt wird.<br><br>Der Generator "Inflate Shrinkwrap" gibt eine monochrome (schwarz-weiß) Textur aus. Daher eignet sie sich gut zum Generieren von Masken, die den Schrumpfumbrucheffekt erzeugen. Es kann jedoch auch direkt auf einer Füllebene platziert werden, um Falten zum Height und zu den Normalkanälen hinzuzufügen.<br><br>Eine gebackene Krümmungskarte ist als Bildeingabe erforderlich. <a href="../../../baking/baking.md">Weitere Informationen zum Backen</a>.</td>
  </tr>
</table>

## Eingaben

| Eingabename | Beschreibung |
| --- | --- |
| **Krümmung** Graustufen | Verwenden Sie die Kurvenzeichner-Map. |

## Parameter

<table>
  <tr>
    <th>Parametername</th>
    <th>Beschreibung</th>
  </tr>
  <tr>
    <td><strong>Vorgabe</strong></td>
    <td>Wechseln Sie zwischen den Vorgaben Aufgeblasen, Vakuum gezogen und Eng.</td>
  </tr>
  <tr>
    <td><strong>Zufalls-Startwert</strong></td>
    <td>Legen Sie den Startwert fest, der zum Generieren der Textur des Dirts verwendet wird. <br><ul><li>Klicken Sie auf "Zufällig", um zu einer anderen Zufallsverteilung zu wechseln.</li><li>Klicken Sie auf den Stift, um den aktuellen Wert für das Seed anzuzeigen, und geben Sie bei Bedarf einen bestimmten Wert ein.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Aufblasen oder Einpassen</strong></td>
    <td>Wechseln Sie zwischen den Modi "Aufblasen" und "Einpassen".</td>
  </tr>
  <tr>
    <td><strong>Nahtintensität</strong></td>
    <td>Passen Sie die Kantenstärke an.</td>
  </tr>
  <tr>
    <td><strong>Erhöhte Kantenbreite</strong></td>
    <td>Passen Sie an, wie stark die aufgeblähten Kanten zusammenziehen.</td>
  </tr>
  <tr>
    <td><strong>Intensität erhöhter Kanten</strong></td>
    <td>Passen Sie die Stärke des Effekts "Überhöhte Kanten" an.</td>
  </tr>
  <tr>
    <td><strong>Faltendichte</strong></td>
    <td>Passe die Anzahl der Falten an.</td>
  </tr>
  <tr>
    <td><strong>Faltenfestigkeit</strong></td>
    <td>Passen Sie an, wie eng Falten an den UV-Rändern zusammengezogen werden.</td>
  </tr>
  <tr>
    <td><strong>Faltenbereich</strong></td>
    <td>Passen Sie an, wie weit die Falten von den UV-Rändern reichen.</td>
  </tr>
  <tr>
    <td><strong>Faltenskala</strong></td>
    <td>Passe die Größe der Falten an.</td>
  </tr>
</table>

### Technische Parameter

| Parametername | Beschreibung |
| --- | --- |
| **Height-Bereich** | Legen Sie den Bereich des Heights fest. |
| **Height-Position** | Passen Sie das Height in Richtung Schwarz (0) oder Weiß (1) an. |
| **Oberflächengröße (cm)** | Legen Sie die Physische Größe der Fläche fest. |
| **Tiefe der Oberfläche (cm)** | Stellen Sie die physische Tiefe der Oberfläche ein. |
