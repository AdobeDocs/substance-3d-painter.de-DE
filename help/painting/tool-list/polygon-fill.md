---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/painting/tool-list/polygon-fill.html"
breadcrumb-title: ''
description: Mit dem Polygon-Füllwerkzeug in Substance 3D Painter können Sie ausgewählte Polygone mit Farbe füllen, um effizient Strukturen zu zeichnen.
helpx_creative_field: ""
helpx_description: Painter > Painting > Tool list > Polygon fill
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Polygon-Füllen
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '251'
ht-degree: 1%

---


# Polygon-Füllen

Mit dem Werkzeug **Polygonfüllung** (![](../../assets/image2018-6-12-18-15-12.png)) können Sie schnell Masken zeichnen, indem Sie ausgewählte Polygone in eine Pixelmaske umwandeln. Es mag wie ein 3D-Auswahlwerkzeug aus anderen 3D-CC-Anwendungen aussehen, aber eigentlich ist es ein Füllwerkzeug, das Pixeldaten erzeugt. Das bedeutet, dass Sie mit dieser Option weiß oder schwarz malen können.

Das Polygon-Füllwerkzeug funktioniert auf [Paint Layers,](../../interface/layer-stack/layer-stack.md), ist jedoch auf die Grundfarbe beschränkt und nicht für diesen Zweck vorgesehen. [Verwenden Sie es nur für Masken](../../interface/layer-stack/masking-and-effects.md).

Es gibt vier Auswahlmodi:

* ![](../../assets/image2020-9-30-11-31-53.png) **Dreiecksfüllung** - füllt einzelne Gittertrias.
* ![](../../assets/image2020-9-30-11-32-12.png) **Polygonfüllung** - Füllt ganze Polygone. Unterscheidet sich nicht von der Option &quot;Dreiecksfüllung&quot;, wenn das Gitter beim Export bereits dreieckig ist.
* **![](../../assets/image2020-9-30-11-32-42.png)Gitterfüllung** - Fült alle verbundenen Teilgitter. Wie der Modus &quot;Unter-Objekt&quot; in 3D-Anwendungen füllt auch dieser Modus jedes Polygon, das mit dem angeklickten Polygon verbunden ist.
* **![](../../assets/image2020-9-30-11-32-54.png)UV-Chunk-Füllung** - Füllt den gesamten UV-Chunk oder &quot;Insel&quot;. Funktioniert wie die Mesh-Füllung, aber durch Betrachtung der Polygone, die im UV-Raum verbunden sind. Füllstopps an UV-Rändern.

![](../../assets/polygon-fill.gif)

Diese 4 Modi können kombiniert und umgeschaltet werden, was bedeutet, dass Sie mit einer intelligenten Nutzung Abschnitte in einer Maske mithilfe des Gitter- und UV-Chunk-Modus schnell markieren und die Markierung aufheben können.

Die (Standard-)Hotkeys, die mit dem Werkzeug Polygonfüllung verknüpft sind, sind:

* *Numerische Taste 4* - Wählt das Polygon-Füllwerkzeug aus.
* *X* - Kehrt die aktuelle Farbe beim Malen von Masken um. Tauscht Schwarz gegen Weiß aus. Im Material-Malmodus hat dieser Hotkey keine Wirkung.
