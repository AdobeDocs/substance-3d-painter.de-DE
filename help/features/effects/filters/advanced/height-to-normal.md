---
title: Height auf Normal
description: Erfahren Sie, wie Sie den Substance 3D Painter-Filter "Height zur Normalität" verwenden.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '142'
ht-degree: 2%
---

# Height auf Normal

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![Symbol &quot;Height in Normal&quot;](./Resources/icon_height_to_normal.png "Symbol &quot;Height in Normal&quot;")

<b>In:</b> Effekte/

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Beschreibung

Der Height-zu-Normal-Filter generiert exakte Normaldaten auf der Grundlage des Height-Kanals.

Sie wird auf einer Textur-Ebene verwendet, um Height-Informationen in normale Daten zu konvertieren.

</td>
</tr>
</table>

<a name="parameters"></a>

## Parameter

| Parametername | Beschreibung |
| --- | --- |
| <b>Vorhandene Normalwerte überschreiben:</b> | Überschreiben der vorhandenen normalen Daten aktivieren/deaktivieren. |
| <b>Welteinheiten verwenden:</b> | Umschalten der Verwendung von Welteinheiten für die Konvertierung. |
| <b>Normalintensität:</b> | Wenn **World Units** verwenden **False** ist, passen Sie mit dieser Option die Intensität der generierten Normaldaten an. |
| <b>Oberflächengröße (cm):</b> | Wenn **Weltmaßeinheiten verwenden** **Wahr** ist, verwenden Sie diese Option, um die Breite oder das Height der dargestellten Fläche anzupassen, je nachdem, welcher Wert größer ist. |
| <b>Height Tiefe (cm):</b> | Wenn **World Units** verwenden **True** ist, passen Sie mit dieser Option den maximalen Height-Bereich der Oberfläche an. |
