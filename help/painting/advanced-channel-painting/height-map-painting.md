---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/painting/advanced-channel-painting/height-map-painting.html"
breadcrumb-title: ''
description: Lerne, wie du in Substance 3D Painter Höhen-Map direkt auf die Malen von Fotos aufnimmst, um Versatz- und Oberflächeneffekte zu erzeugen.
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

* Eine von einer High-Poly-Mesh Baking geführt Normalen-Map wird auf den Low-Poly-Mesh geladen.
* Sie werden zusätzliche Details auf dem höhtmap-Kanal Malen.
* Das von Ihnen Malen Height wird über alle Ebenen hinweg zusammengestellt, in Echtzeit in eine Normalen-Map konvertiert und schließlich mit dem normalen Bild aus der High-Poly-Mesh überblendet.

Du brauchst dir nur um das Malen des Heights zu sorgen, alles andere wird automatisch gemalt.

### Height HDR. Format

Der Height-Kanal verwendet ein **HDR.**-Farbformat, mit dem positive und negative Werte Malen werden können, ohne jemals eine Helligkeitsgrenze zu erreichen. Im Gegensatz dazu werden bei herkömmlichen Höhen-Map-Kanälen zwischen 0 und 255 Farbsättigungen erreicht.

* Beim Malen mit einer Bitmap oder einem Stoff auf einem Height wird diese Quelle von ihrem ursprünglichen [0,255]-Bereich auf einen [-1,1]-Bereich neu zugeordnet.

Ein Mittelgrau wird 0 zugeordnet. Werte unter 127 ziehen daher **von der Höhenkarte ab**, während Werte über 127 bei Verwendung des für die Höhen-Map festgelegten Standardmischmodus **Linear abwedeln (Hinzufügen)** **Hinzufügen** bewirken.

* Beim Malen mit Normalfarbe können Sie direkt Werte zwischen -1 und 1 auswählen.

### Visualisierung von Heights

Bei der Visualisierung des Höhen-Map im Solomodus zeigt die Standardvorschau nur positive Werte an, mit starker schwarzer Sättigung für negative Werte.

Mit der Einstellung &quot;**+/- color**&quot; kann der gesamte Bereich mit einer anderen Farbe für die positiven und negativen Werte angezeigt werden.

Mit der Einstellung **Skalierung** können Sie den sichtbaren Bereich dieser HDR ändern, falls Sie mehr als den standardmäßigen [-1,1] Bereich hinzugefügt oder entfernt haben.

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
