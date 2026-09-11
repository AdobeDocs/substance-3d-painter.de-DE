---
title: Tropfender Rost
description: Erfahren Sie, wie Sie den Dripping Rost-Generator von Substance 3D Painter verwenden.
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 8%

---


# Tropfender Rost

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_dripping_rust.webp" alt=""/><br><strong>In:</strong> Generator, Graustufen, Farbe</td>
    <td style="border: 0;" valign="top"><strong>Beschreibung</strong><br>Der Rost-Tropfgenerator erzeugt nach unten fließende Streifen von Rost, die die Korrosion durch Schwerkraft und Wasserablauf simulieren.<br><br>Der Rost-Generator "Dripping" gibt eine monochrome (Schwarz-Weiß) Textur aus. Daher eignet sie sich gut zum Generieren von Masken, um einen tropfenden Rost-Effekt zu erzeugen.<br><br> Baking geführt Position, Krümmung und ambient occlusion sind als Bildeingaben erforderlich. <a href="../../../baking/baking.md">Weitere Informationen zum Baking</a>.</td>
  </tr>
</table>

## Eingaben

| Eingabename | Beschreibung |
| --- | --- |
| **Krümmung** Graustufen | Verwenden Sie die Baking geführt Krümmungs-Map. |
| **Ambient occlusion** Graustufen | Verwenden Sie die Baking geführt Ambient occlusion-Map. |
| **Position** Farbe | Verwenden Sie die Baking geführt Positionszuordnung. |

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
    <td><strong>Invertieren</strong></td>
    <td>Invertieren Sie bestimmte interne Maps (z. B. Krümmung, AO), bevor sie zur endgültigen Maske kombiniert werden.</td>
  </tr>
  <tr>
    <td><strong>Rostausbreitung</strong></td>
    <td>Passen Sie die Verstärkung des Effekts "Tropfender Rost" an.</td>
  </tr>
  <tr>
    <td><strong>Rostkontrast</strong></td>
    <td>Passen Sie den Kontrast des Effekts "Tropfender Rost" an.</td>
  </tr>
  <tr>
    <td><strong>Glättung ausbreiten</strong></td>
    <td>Passen Sie die Weichzeichnung des tropfenden Rosts an.</td>
  </tr>
  <tr>
    <td><strong>Tropfenstärke</strong></td>
    <td>Passen Sie die Dauer des Effekts "Tropfender Rost" an.</td>
  </tr>
  <tr>
    <td><strong>Tropfenglättung</strong></td>
    <td>Passen Sie die Weichheit des Effekts "Tropfender Rost" an.</td>
  </tr>
  <tr>
    <td><strong>Tropfenprobenmenge</strong></td>
    <td>Passen Sie die Qualität des Effekts an (mehr Samples für eine bessere Qualität).</td>
  </tr>
  <tr>
    <td><strong>Achsenposition</strong></td>
    <td>Wechseln Sie zwischen dem Y-Grün-, X-Rot- und B-Blau-Kanal, um die Richtung des Effekts "Tropfender Rost" zu ändern.</td>
  </tr>
</table>
