---
title: UV-Texeldichte
description: Erfahren Sie, wie Sie den UV Texel Density-Generator von Substance 3D Painter verwenden.
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '204'
ht-degree: 0%

---


# UV-Texeldichte

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_uv_texel_density.png" alt=""/><br><strong>In:</strong> uv, size, utility</td>
    <td style="border: 0;" valign="top"><strong>Beschreibung</strong><br>Der UV Texel Density-Generator visualisiert die Texeldichte eines Meshs, indem er einen farbigen Verlauf von niedrig nach hoch anwendet.<br>Der UV Texel Density Generator gibt eine vollfarbige Textur aus und wird am besten auf einer Füllebene verwendet, um eine inkonsistente UV-Skalierung zu identifizieren und eine einheitliche Textur im gesamten Modell sicherzustellen.</td>
  </tr>
</table>

>[!NOTE]
>
> Die Texeldichte bezieht sich auf die Anzahl der Texel (Textur) in einem bestimmten Oberflächenbereich Ihres Modells. Eine hohe Texeldichte bedeutet, dass du viel Detail in einen kleinen Bereich deines Modells packen kannst, wo eine niedrige Texeldichte die Detailgenauigkeit reduzieren, aber die Leistung verbessern kann. Im Allgemeinen empfiehlt es sich, unabhängig von der Auflösung deines Materials eine konsistente Texeldichte über deinen Mesh hinweg beizubehalten, da große Unterschiede in der Texeldichte oft den Betrachtern auffallen und dazu führen können, dass sich ein Element von geringerer Qualität oder weniger realistisch anfühlt.

## Parameter

| Parametername | Beschreibung |
| --- | --- |
| **Farbtiefe** | Legen Sie die Farbe fest, die für Bereiche mit **niedriger** Texeldichte verwendet wird. |
| **Farbmedium** | Legen Sie die Farbe fest, die für Bereiche mit **mittlerer** Texeldichte verwendet wird. |
| **Farbintensiv** | Legen Sie die Farbe fest, die für Bereiche mit **hoher** Texeldichte verwendet wird. |
