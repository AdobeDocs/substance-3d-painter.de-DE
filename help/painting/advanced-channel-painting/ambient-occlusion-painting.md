---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/painting/advanced-channel-painting/ambient-occlusion-painting.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie ambient occlusion-Maps direkt in Substance 3D Painter Malen, um Texturen realistische Schatten und Tiefe zu verleihen.
helpx_creative_field: ""
helpx_description: Painter > Painting > Advanced channel painting > Ambient Occlusion Painting
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Ambient occlusion Painting
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 0%

---


# Ambient occlusion Painting

Der ambient occlusion-Kanal ermöglicht das Malen von Details in den Umgebungsschatten eines Objekts. Es kann verwendet werden, um AO-Details aus Materialien hinzuzufügen oder einfach manuell Baking geführt Fehler zu beheben, wenn nötig.

&#x200B;>> 

In der Computergrafik ist das ambient occlusion eine Schattierung- und Rendering-Technik, mit der berechnet wird, wie gelegt jeder Punkt in einer Szene von der Umgebungsbeleuchtung ist. Das Innere eines Röhrchens ist in der Regel verdeckter (und damit dunkler) als die gelegt Außenflächen, und je tiefer man in das Innere des Röhrchens geht, desto verdeckter (und dunkler) wird die Beleuchtung. Ambient occlusion kann als Barrierefreiheitswert betrachtet werden, der für jeden Oberflächenpunkt berechnet wird.\
Quelle: &lt;https://en.wikipedia.org/wiki/Ambient_occlusion>

Das **Ergebnis** dieser Berechnung wird in einer Bitmap mit dem Namen &quot;Ambient occlusion&quot; gespeichert. Diese Map kann direkt in der Anwendung Baking geführt werden. Weitere Informationen finden Sie unter: [Baking](../../baking/baking.md).

## Ambient occlusion malen

Zum Malen benutzerdefinierter Verdeckung-Details ist ein Ambient occlusion-Kanal erforderlich. Sie kann über die [Textursatz-Einstellungen](../../interface/texture-set/texture-set-settings.md) hinzugefügt werden:

![](../../assets/add-ao-channel.png)

Nachdem der Kanal einem Textursatz hinzugefügt wurde, kann jede Ebene zum Malen neuer Informationen verwendet werden. Da der AO-Kanal nur Graustufeninformationen enthält, wird der Mischmodus &quot;**Normal**&quot; (Malen Over) und &quot;**Multiply**&quot; (Kombinieren) empfohlen.

Weitere Informationen dazu und wie Sie sie pro Kanal ändern können, finden Sie unter: [Füllmethoden](../../interface/layer-stack/blending-modes.md).

## Malen über die zusätzliche Ambient occlusion-Map

In manchen Situationen kann es hilfreich sein, über die Baking geführt Ambient occlusion zu Malen, um Details auszublenden oder sogar Baking führend Probleme zu beheben.

Beim Standardsetup eines Projekts in Substance 3D Painter wird die Ambient occlusion **channel** mit der Ambient occlusion-Map aus den **zusätzlichen Maps** kombiniert. Dies bedeutet, dass das Übermalen der Baking geführt zusätzlichen Map standardmäßig nicht möglich ist, die Ergebnisse der einzelnen Maps (die durch Baking erzeugte Map und die Kanäle) werden miteinander multipliziert. Dies kann jedoch mit der folgenden Einrichtung geändert werden:

### 1 - Hinzufügen eines Ambient occlusion-Kanals

Hinzufügen eines ambient occlusion-Kanals im aktuellen Textursatz :\
![](../../assets/edit-ao-channel-optimized.gif)

Stellen Sie den Mischmodus auf &quot;**replace** &quot; anstelle von &quot;**multiply** &quot; ein:\
![](../../assets/ao-mix-mode.gif)

### 2 - Festlegen einer Füllebene mit dem Baking geführt ambient occlusion

Erstellen Sie eine neue Füllebene und legen Sie die Baking geführt ambient occlusion über das Eigenschaftenbedienfeld in den Steckplatz &quot;ambient occlusion&quot;. Vergessen Sie nicht, die Standardbearbeitung der Füllebene zu ändern, wenn sie nicht bereits auf 1 gesetzt ist.\
![](../../assets/ao-stack.png)

### 3 - Ändern der Füllmethode der Füllebene

Standardmäßig ist der Mischmodus des AO-Kanals auf einer neuen Ebene auf &quot;**Multiply** &quot; eingestellt. Da es besser ist, die Füllebene als Grundlage zu verwenden, haben wir den &quot;normalen&quot; Mischmodus gewählt, da die Bitmap keinen Alpha-Wert hat. Alles darunter (einschließlich der Standardfarbe des Shader) wird ersetzt.\
![](../../assets/ao-blend-mode.gif)

### 4 - Erstellen einer Ebene zum Malen über der Baking geführt ambient occlusion Map

Erstelle eine neue Ebene (normal oder gefüllt). Setze den Mischmodus für den AO-Kanal auf &quot;Normal&quot;. Sobald diese Einrichtung abgeschlossen ist, übernimmt alles, was auf dem AO-Kanal gemalt wird, die Baking geführt AO-Map, die sich auf der darunter liegenden Ebene befindet.\
![](../../assets/paint-over-ao-optimized.gif)
