---
title: Anisotropes Kuwahara
description: Erfahren Sie, wie Sie den anisotropen Kuwahara-Filter von Substance 3D Painter verwenden.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 1%
---

# Anisotropes Kuwahara

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![Anisotropes Kuwahara-Symbol](./Resources/icon_anisotropic_kuwahara.png "Anisotropes Kuwahara")

<b>In:</b> Effekte/Graustufen, Kuwahara, anisotropisch, stilisiert

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Beschreibung

Der anisotrope Kuwahara-Filter erzeugt malerische Stilisierungseffekte, während starke Richtungsmerkmale beibehalten werden.

Es wird auf einer Maskenebene oder innerhalb einer Textur (Schwarzweißausgabe) verwendet, um einen stilisierten Look für ganze Materials, Rauschen und Masken zu erstellen.

</td>
</tr>
</table>

## Eingaben

| Eingabename | Beschreibung |
| --- | --- |
| <b>Radiuszuordnung:</b> Graustufen | Verwenden einer benutzerdefinierten Textur oder eines Ankerpunkts. |
| <b>Benutzerdefinierte Eingabe:</b> Farbe | Verwenden einer benutzerdefinierten Textur oder eines Ankerpunkts. |

<a name="parameters"></a>

## Parameter

| Parametername | Beschreibung |
| --- | --- |
| <b>Richtung extrahieren:</b> | Wählen Sie aus, wie der Filter die Weichzeichnungsrichtung ableitet. |
| <b>Radius:</b> | Passen Sie den Weichzeichnungsradius an. Höhere Werte erzeugen einen stärkeren Unschärfe-Effekt. Der Höchstwert ist 32. |
| <b>Smoothness:</b> | Passen Sie an, wie viele Farben in der berechneten Richtung ineinander übergehen. Bei 0 werden die Farben meistens in diese Richtung verschoben, ohne dass eine Überblendung stattfindet. |
| <b>Schärfe:</b> | Passe den Kontrast in unscharfen Bereichen an, um sie flacher und klarer zu definieren. |
| <b>Tensor-Smoothness:</b> | Passen Sie den Weichzeichnungsgrad an, der auf die aus dem Bild berechnete und auf der Richtungs-Map gespeicherte Richtung angewendet wird. Höhere Werte führen zu einem weicheren Ergebnis, wenn das Bild viele hochfrequente Details enthält. |
| <b>Anisotropie:</b> | Passen Sie an, wie stark der Richtungs-Map den Weichzeichner beeinflusst. Die Richtungs-Map und ihre Modifizierer beeinflussen das Ergebnis auch dann noch, wenn dieser Wert 0 ist, da die Map im Kuwahara-Filterkernel verwendet wird. |
| <b>Anisotropy angle:</b> | Passen Sie die Drehung an, die auf den Richtungs-Map in Windungen angewendet wird. Diese Drehung wird dem Wert aus der Anisotropy angle Map-Eingabe hinzugefügt. |

