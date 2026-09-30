---
title: Height anpassen
description: Erfahren Sie, wie Sie den Substance 3D Painter-Filter "Height anpassen" verwenden.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '159'
ht-degree: 1%
---

# Height anpassen

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![Symbol zur Height-Anpassung](./Resources/icon_height_adjust.png "Symbol zur Height-Anpassung")

<b>In:</b> Effekte/Anpassungen, Skalierung, Offset, Invertierung

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Beschreibung

Der Filter &quot;Height Adjust&quot; invertiert, verschiebt oder multipliziert den Height-Kanal mit einem ausgewählten Wert.

Sie wird auf einer Maskenebene oder innerhalb einer Textur (Schwarzweißausgabe) verwendet, um Height-Informationen nicht-destruktiv anzupassen.

</td>
</tr>
</table>

<a name="parameters"></a>

## Parameter

| Parametername | Beschreibung |
| --- | --- |
| <b>Umkehren:</b> | Kehrt die Umkehrung des Ergebnisses um. |
| <b>Offset:</b> | Passen Sie den Wert des Heights an, indem Sie den angegebenen Wert addieren oder subtrahieren. |
| <b>Multiplizieren:</b> | Multiplizieren Sie die Height-Werte mit diesem Wert. Als Multiplikator führt dies zu höheren und niedrigeren Bereichen. |

>[!NOTE]
>
> Der Stapel **Multiply** und **Offset** mit dem Versatz wird zuerst angewendet. Wenn das Offset zu einem Nullpunkt im Height führt, wird die Multiplikation mit Null multipliziert, d. h., sie wird an diesem Punkt nicht verändert. Um die multiplizierten Werte zu multiplizieren und dann einen Offset anzuwenden, können Sie einen zweiten Filter zur Height-Anpassung hinzufügen.
