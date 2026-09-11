---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/features/dynamic-material-layering.html"
breadcrumb-title: ''
description: Lerne, wie du mit dynamische Materialüberlagerung in Substance 3D Painter Materialien mithilfe prozeduraler Masken verblendest und kombinierst.
helpx_creative_field: ""
helpx_description: Painter > Features > Dynamic Material Layering
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Dynamische Materialüberlagerung
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 0%

---


# Dynamische Materialüberlagerung

![](../assets/dynamic-material-blending-materials.jpg){width="450px"}

**Dynamische Materialüberlagerung** ist ein bestimmter Workflow, bei dem generische Material in einem Shader anstatt in einer einzigen Textur zusammengemischt werden. Der Hauptvorteil dieses Workflows besteht darin, dass die Füllmethode dynamisch ist und es ermöglicht, ein bestimmtes Qualitätsniveau zu kontrollieren und zu erhalten, indem generische Material innerhalb des Shader bearbeitet werden. Materialien sind zwar generisch, aber die Masken, die zum Überblenden der Materialien verwendet werden, sind spezifisch für Mesh und werden daher nicht wiederholt.

![](../assets/tilling-mat-layer.gif){width="400px"}

Um den Arbeitsablauf für die Material-Ebenen zu aktivieren, ist ein bestimmter Shader erforderlich.\
Der Shader &quot;**pbr-Material-Layer** &quot;, der standardmäßig mit Substance 3D Painter geliefert wird, ermöglicht das Mischen von 4 Materialien mit 3 Masken.

## Sub-Ebenenstapel

In diesem Shader können Sub-Stapel definiert und direkt vom Shader abgetastet werden. Beispiel mit dem Shader &quot;pbr-Material-layering&quot;, der im Lieferumfang von Substance 3D Painter enthalten ist:

```
//: stacks [ 

//:   { 

//:     "id": "Mask", 

//:     "channels": [ 

//:   {"id": "opacity"} 

//:  ] 

//:   }, 

[...] 

//: ]
```


![](../assets/sub-stacks.png) In diesem Beispiel erstellt der Shader drei Unterkanäle auf einem bestimmten Textursatz mit jeweils einem Stapel mit &quot;Deckkraft&quot;. Auf die Sub-Stapel kann im TextureSet-Listenfenster zugegriffen werden:

Da die **Ebenenstapel** der Unterkanäle **im Shader** definiert sind, ist es nicht möglich, in den Kanaleinstellungen neue Textursätze hinzuzufügen. Zum Hinzufügen oder Entfernen eines Kanals ist eine Aktualisierung der Shader-Datei erforderlich.

Die Anzahl der maximal unterstützten Kanäle wird durch die Anzahl der Sampler definiert, die insgesamt von der Hardware unterstützt werden.\
Während Substance 3D Painter für Material, die als Parameter geladen werden, bindungslose Texturen (und damit eine unbegrenzte Anzahl von Texturen) unterstützt, sind die vom Engine für die Ebenenstapel bereitgestellten Kanäle auf 32 (unter Windows) beschränkt. Dieser Grenzwert umfasst auch andere Texturen wie die Normale und die Ambient occlusion, die auf dem Mesh des Projekts Baking geführt werden.

## Materialien-Eingaben

Während es möglich ist, Untermasken einzurichten, um Materialien zusätzlich zu Stapel zu definieren, ist es oft praktischer, einfach Material-Eingaben im Shader zu definieren und Materialien aus dem Regal direkt zu verwenden. Meist sind diese Material auch in der endgültigen Anwendung vorhanden, z. B. Unity oder das Unreal-Engine 4. Die Namenskonvention zum Deklarieren von Materialien sieht im Shader &quot;pbr-Material-layering&quot; folgendermaßen aus:

```
//: materials [ 

//:   { 

//:      "id": "Material1", 

//:      "label": "Material 1", 

//:      "default": "", 

//:      "size": 1024, 

//:      "default_color": [0.5, 0.5, 0.5] 

//:   }, 

[...] 

//: ]
```


![](../assets/materials.png) Dies ist das Ergebnis, wenn einige Material (Substance-Material oder Materialvorgaben) geladen wurden:

Die Auflösung des Materials kann mit dem Parameter &quot;size&quot; definiert werden. Es ist auch möglich, Materialien standardmäßig zu laden, wenn der Shader mit dem Parameter &quot;default&quot; erstellt wird (indem der Name/die Bezeichnung der Ressource verwendet wird, die geladen werden muss).

Um auf die Materialien zuzugreifen und sie im Shader selbst zu maskieren, verbinden Sie sie einfach mit dem Schlüsselwort &quot;param auto&quot; :

```
//: param auto Material1.channel_basecolor 

uniform sampler2D color1; 

 

//: param auto Mask.channel_opacity 

uniform sampler2D mask;
```


In diesem speziellen Arbeitsablauf sind die Maskenparameter und die Shader-Parameter am wichtigsten. Daher wird empfohlen, im Exportfenster von Substance 3D Painter die Einstellung &quot;**Exportschattierungsparameter**&quot; zu aktivieren. Dadurch wird auf dem Datenträger neben den Texturen eine **JSON**-Datei erstellt, die Informationen über die Einrichtung der Unterparameter, die verwendeten Material und die Shader sowie deren Stapel enthält. Parameter > Exportieren und Importieren

Derzeit wird das Packing von Masken in eine einzige Textur während des Exports nicht unterstützt. Eine einfache Problemumgehung wäre jedoch, die Skriptfunktionen zu verwenden und die Substance-Batch-Tools aufzurufen, um das Packing stattdessen mit einer Substance auszuführen.

![](../assets/export-window-shader.png)

Diese JSON-Datei kann dann verwendet werden, um die Ebenenstapel und Shader eines Projekts einzurichten.\
So können Sie problemlos zwischen mehreren Anwendungen hin- und herwechseln, indem Sie gemeinsame Parameter verwenden.

![](../assets/import-jsons.png)
