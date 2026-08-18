---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/dynamic-material-layering.html"
breadcrumb-title: ''
description: Lerne, wie du in Substance 3D Painter mithilfe von dynamische Materialüberlagerung Materialien mithilfe von Verfahrensmasken verblendest und kombinierst.
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

**Dynamische Materialüberlagerung** ist ein bestimmter Arbeitsablauf, bei dem generische Materialien in einem Shader anstatt in einer einzigen Textur zusammengemischt werden. Der Hauptvorteil dieses Workflows besteht darin, dass die Füllmethode dynamisch ist und es ermöglicht, ein bestimmtes Qualitätsniveau zu kontrollieren und zu erhalten, indem generische Materialien innerhalb des Shaders bearbeitet werden. Materialien sind zwar generisch, aber die Masken, die zum Mischen der Materialien verwendet werden, sind netzspezifisch und wiederholen sich daher nicht.

![](../assets/tilling-mat-layer.gif){width="400px"}

Um den Arbeitsablauf für die Materialschichtung zu aktivieren, ist ein bestimmter Shader erforderlich.\
Der Shader &quot;**pbr-material-layering** &quot;, der standardmäßig mit Substance 3D Painter geliefert wird, ermöglicht das Mischen von 4 Materialien mit 3 Masken.

## Unterebenenstapel

In diesem Shader können Substacks definiert und direkt vom Shader abgetastet werden. Beispiel mit dem Shader &quot;pbr-material-layering&quot;, der im Lieferumfang von Substance 3D Painter enthalten ist:

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


![](../assets/sub-stacks.png) In diesem Beispiel erstellt der Shader drei Unterstapel für einen bestimmten Textursatz mit jeweils einem &quot;Deckkraftkanal&quot;. Auf Unterstapel kann im TextureSet -Listenfenster zugegriffen werden:

Da die **Kanäle** der Unterebenenstapel **im Shader** definiert sind, ist es nicht möglich, neue Kanäle in den Textursatzeinstellungen hinzuzufügen. Um einen Kanal hinzuzufügen oder zu entfernen, muss die Shader-Datei aktualisiert werden.

Die Anzahl der maximal unterstützten Kanäle wird durch die Anzahl der Sampler definiert, die insgesamt von der Hardware unterstützt werden.\
Während Substance 3D Painter bindungslose Texturen (und damit unbegrenzte Anzahl an Texturen) für Materialien unterstützt, die als Parameter geladen werden, sind die Kanäle, die von der Engine für die Ebenenstapel bereitgestellt werden, auf 32 beschränkt (unter Windows). Dieser Grenzwert gilt auch für andere Texturen wie die Verdeckung &quot;Normal&quot; oder &quot;Umgebung&quot;, die auf dem Gitter des Projekts basieren.

## Materialeingaben

Während es möglich ist, Unterstapel einzurichten, um Materialien zusätzlich zu Masken zu definieren, ist es oft praktischer, einfach Materialeingaben im Shader zu definieren und Materialien aus dem Regal direkt zu verwenden. Meist existieren diese Materialien auch in der endgültigen Anwendung wie Unity oder der Unreal Engine 4. Die Benennungskonvention zum Deklarieren von Materialien sieht im Shader &quot;pbr-material-layering&quot; folgendermaßen aus:

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


![](../assets/materials.png) Dies ist das Ergebnis, wenn einige Materialien (Substance-Materialien oder Materialvorgaben) geladen wurden:

Die Materialauflösung kann mit dem Parameter &quot;Größe&quot; definiert werden. Es ist auch möglich, Materialien standardmäßig zu laden, wenn der Shader mit dem Parameter &quot;default&quot; erstellt wird (unter Verwendung des Namens/Labels der Ressource, die geladen werden muss).

Um auf die Materialien und die Maske im Shader selbst zuzugreifen, verbinden Sie sie einfach mit dem Stichwort &quot;param auto&quot; :

```
//: param auto Material1.channel_basecolor 

uniform sampler2D color1; 

 

//: param auto Mask.channel_opacity 

uniform sampler2D mask;
```


In diesem speziellen Arbeitsablauf sind die Masken- und die Shader-Parameter der wichtigste Teil. Daher wird empfohlen, im Exportfenster von Substance 3D Painter die Einstellung &quot;**Exportschattierungsparameter**&quot; zu aktivieren. Dadurch wird eine **JSON**-Datei auf dem Datenträger neben den Texturen erstellt, die Informationen über die Einrichtung der Unterstapel, die verwendeten Materialien und die Shader sowie deren Parameter enthält. Parameter > Exportieren und Importieren

Derzeit wird das Packing von Masken in eine einzelne Textur während des Exports nicht unterstützt. Eine einfache Problemumgehung wäre jedoch, die Skriptfunktionen zu verwenden und die Substance-Batch-Tools aufzurufen, um das Packing stattdessen mit einer Substance auszuführen.

![](../assets/export-window-shader.png)

Diese JSON-Datei kann dann zum Einrichten der Ebenenstapel und Shader eines Projekts verwendet werden.\
So können Sie problemlos zwischen mehreren Anwendungen hin- und herwechseln, indem Sie gemeinsame Parameter verwenden.

![](../assets/import-jsons.png)
