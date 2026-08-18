---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/painting/advanced-channel-painting/height-map-painting.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie Heights direkt in Substance 3D Painter malen, um Versatz- und Oberflächenhöheneffekte zu erzeugen.
helpx_creative_field: ""
helpx_description: Painter > Painting > Advanced channel painting > Height Map Painting
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Height Map Painting
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 0%

---


# Height Map Painting

## Allgemeine Idee

Die Arbeit an einer Höhenkarte anstatt direkt an einer normalen bietet zahlreiche Vorteile wie bessere Qualität, bessere Kontrolle, Flexibilität und bessere Konsistenz zwischen Assets.

Der Vorgang läuft wie folgt ab:

* Auf dem Gitter mit niedrigem Poly wird eine normale Karte geladen, die aus einem Gitter mit hohem Poly gebacken wird.
* Sie werden weitere Details auf dem höhtmap-Kanal malen.
* Das Height, das Sie malen, wird über alle Ebenen verteilt, in Echtzeit in eine Normalmap umgewandelt und schließlich mit der Normalansicht des Polygonnetzes vermischt.

Du brauchst dir nur um das Malen des Heights zu sorgen, alles andere wird automatisch gemalt.

### Height HDR-Format

Der Height-Kanal verwendet ein **HDR**-Farbformat, mit dem im Gegensatz zu herkömmlichen Height-Maps, die zwischen 0 und 255 sättigt werden, positive und negative Werte gemalt werden können, ohne jemals eine Helligkeitsgrenze zu erreichen.

* Beim Malen mit einer Bitmap oder einem Stoff auf einem Height wird diese Quelle von ihrem ursprünglichen [0,255]-Bereich auf einen [-1,1]-Bereich neu zugeordnet.

Ein Mittelgrau wird 0 zugeordnet. Daher werden Werte unter 127 **von der Höhenkarte subtrahiert**, während Werte über 127 **hinzufügen**, wenn der für die Height-Maps festgelegte Standardfüllmodus verwendet wird: **Linear Abwedeln (Hinzufügen)**.

* Beim Malen mit Normalfarbe können Sie direkt Werte zwischen -1 und 1 auswählen.

### Visualisierung von Heights

Bei der Visualisierung der Height-Map im Solomodus zeigt die Standardvorschau nur positive Werte an, mit starker schwarzer Sättigung für negative Werte.

Mit der Einstellung &quot;**+/- color**&quot; kann der gesamte Bereich mit einer anderen Farbe für die positiven und negativen Werte angezeigt werden.

Mit der Einstellung **Skalierung** können Sie den sichtbaren Bereich dieser HDR-Map ändern, falls Sie mehr als den standardmäßigen [-1,1]-Bereich hinzugefügt oder entfernt haben.

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../assets/height1.png)

</td>
<td style="border: 0;" valign="top">

![](../../assets/height2.png)

</td>
</tr>
</table>
