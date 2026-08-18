---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/subsurface-scattering/subsurface-parameters.html"
breadcrumb-title: ''
description: Lerne, wie du in Substance 3D Painter die Parameter für die Volumenstreuung von Untergründen konfigurieren kannst, um realistische, durchsichtige Materialien zu erstellen.
helpx_creative_field: ""
helpx_description: Painter > Features > Subsurface Scattering > Subsurface Parameters
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Parameter des Untergrunds
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 0%

---


# Parameter des Untergrunds

Die Echtzeit-Subsurface-Implementierung von Substance 3D Painter ist ein Subsurface-Scattering-Effekt für den Bildschirmbereich. Die Parameter zur Steuerung werden auf dieser Seite erläutert.\
Die aktuelle Implementierung basiert auf der von PIXAR](http://graphics.pixar.com/library/ApproxBSSRDF/) veröffentlichten Methode &quot;[&quot; &quot;Approximate Reflectances Profiles for Efficient Subsurface Scattering&quot; (Ungefähre Reflexionsprofile für effiziente Untergrundstreuung).

Beispiele für Materialien, die auf diesen Parametern basieren, finden Sie unter: [Materialtyp Untergrund](subsurface-material-type.md).

## Shader/MDL-Parameter

![](../../assets/shader-parameters.png)

Verfügbar im Fenster [Shader settings](../../interface/shader-settings/shader-settings.md).

| *Einstellung* | *Beschreibung* |
| --- | --- |
| **Aktivieren** | Aktivieren oder deaktivieren Sie den Effekt &quot;Unterflächliche Streuung&quot; für diese Shader/mdl-Instanz.  Kann verwendet werden, um den SSS-Effekt auf Material zu deaktivieren, das ihn nicht benötigt. |
| **Streuungstyp** | Definiert das Verhalten der leichten Absorption im Material:<ul data-preserve-html="true"><li data-preserve-html="true"><strong> lichtdurchlässig</strong>: geeignet für generische Materialien wie Jade oder Marmor, bei denen Licht tief in ein Objekt eindringen kann.</li><li data-preserve-html="true"><strong> Skin</strong>: geeignet für organische Haut, bei der das Licht schnell absorbiert wird und nur oberflächliche Streuung.</li><li data-preserve-html="true"><strong>Red Shift/Rayleigh</strong>: präziser als die Hauteinstellung, um die Haut der Oberfläche von Menschen oder Kreaturen zu simulieren.</li></ul> |
| **Skalierung** | Steuert den Radius/die Tiefe der leichten Absorption im Material. Dieses Parameterverhalten ändert sich je nach Größe des Gitters in der Szene.Vergleich zwischen einer Skala von 0,0, 0,2 und 1,0 bei einem menschlichen Kopf:   <div><img data-preserve-html="true" src="../../assets/scale-sss.jpg" width="650"/></div> |
| **Farbe** | Die Farbe des Lichts, wenn es vom Material absorbiert wird.Drei Farben im Vergleich :   <div><img data-preserve-html="true" src="../../assets/color-sss.jpg" width="650"/></div> |

### Parameter für Anzeigeeinstellungen

![](../../assets/display-settings-1.png)

Verfügbar im Fenster &quot;[Anzeigeeinstellungen](../../interface/display-settings/display-settings.md)&quot;.

>[!NOTE]
>
> Dieser Parameter **betrifft nur** die **Echtzeit**-Version des unterirdischen Streueffekts.

| *Einstellung* | *Beschreibung* |
| --- | --- |
| **Beispielanzahl** | Steuert die Anzahl der Samples, die zum Generieren der Unschärfe unter der Oberfläche im Bildschirmbereich ausgeführt werden. Mehr Samples bedeuten weniger Rauschen, wirken sich aber auf die Leistung aus.Vergleich zwischen 8, 32 und 64 Proben bei der Annäherung an eine Oberfläche:   <div><img data-preserve-html="true" src="../../assets/samples-sss-v2.jpg" width="650"/></div>  **Hinweis:** Das Rauschen kann auch reduziert werden, indem [Kameraeinstellungen](../../interface/display-settings/camera-settings.md) aktiviert werden, ohne die Anzahl der Samples zu erhöhen. |
