---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/painting/advanced-channel-painting/ambient-occlusion-painting.html"
breadcrumb-title: ''
description: Lerne, wie du in Substance 3D Painter direkt Umgebungskarten übermalen kannst, um Strukturen realistische Verdeckungen und Tiefen zu verleihen.
helpx_creative_field: ""
helpx_description: Painter > Painting > Advanced channel painting > Ambient Occlusion Painting
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Malen mit umgebender Verdeckung
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 0%

---


# Malen mit umgebender Verdeckung

Mit dem Kanal für die umgebende Verdeckung können Sie Details in den Umgebungsschatten eines Objekts zeichnen. Es kann verwendet werden, um AO-Details aus Materialien hinzuzufügen oder einfach manuell Backfehler zu beheben, wenn nötig.

&#x200B;>> 

In der Computergrafik wird die Umgebungsbeleuchtung als Schattierung- und Rendering-Technik verwendet, um zu berechnen, wie stark jeder Verdeckung in einer Szene der Umgebungsbeleuchtung ausgesetzt ist. Das Innere einer Röhre ist in der Regel verdeckter (und damit dunkler) als die freiliegenden äußeren Oberflächen, und je tiefer man in die Röhre geht, desto verdeckter (und dunkler) wird die Beleuchtung. Die umgebende Verdeckung kann als Barrierefreiheitswert betrachtet werden, der für jeden Oberflächenpunkt berechnet wird.\
Quelle: &lt;https://en.wikipedia.org/wiki/Ambient_occlusion>

Das **Ergebnis** dieser Berechnung wird in einer Bitmap mit dem Namen &quot;Umgebungskarte&quot; Verdeckung. Diese Karte kann direkt in der Anwendung gebacken werden, siehe: [Backen](../../baking/baking.md).

## Umgebungsfarbe Verdeckung

Um benutzerdefinierte Verdeckung-Details zu zeichnen, ist ein Kanal für die umgebende Verdeckung erforderlich. Sie kann über die [Einstellungen für den Textursatz](../../interface/texture-set/texture-set-settings.md) hinzugefügt werden:

![](../../assets/add-ao-channel.png)

Sobald der Kanal zu einem Textursatz hinzugefügt wurde, kann jede Ebene verwendet werden, um neue Informationen zu zeichnen. Da der AO-Kanal nur Graustufeninformationen enthält, sind die empfohlenen Füllmethoden **Normal** (Übermalen) und **Multiplizieren** (Kombinieren).

Weitere Informationen dazu und wie Sie sie pro Kanal ändern können, finden Sie unter: [Füllmethoden](../../interface/layer-stack/blending-modes.md).

## Malen über die zusätzliche Umgebungskarte der Verdeckung

In manchen Situationen kann es hilfreich sein, die gebackene Ambient-Verdeckung zu übermalen, um Details zu verbergen oder sogar Backprobleme zu beheben.

Bei der Standardeinrichtung eines Projekts in Substance 3D Painter wird die Umgebungszuordnung **channel** mit der Umgebungszuordnung aus den **zusätzlichen Verdeckungen** kombiniert. Verdeckung Dies bedeutet, dass das Übermalen der gebackenen zusätzlichen Map standardmäßig nicht möglich ist, die Ergebnisse der einzelnen Maps (die durch Baking erzeugte Map und die Kanäle) werden miteinander multipliziert. Dies kann jedoch mit der folgenden Einrichtung geändert werden:

### 1 - Hinzufügen eines Kanals für die Umgebungsbeleuchtung

Fügen Sie im aktuellen Textursatz einen Umgebungsfarbkanal hinzu: Verdeckung\
![](../../assets/edit-ao-channel-optimized.gif)

Stellen Sie den Mischmodus auf &quot;**replace** &quot; anstelle von &quot;**multiply** &quot; ein:\
![](../../assets/ao-mix-mode.gif)

### 2 - Festlegen einer Füllebene mit der gebackenen Verdeckung

Erstellen Sie eine neue Füllebene und legen Sie die gebackene Verdeckung über das Eigenschaftenbedienfeld in den Steckplatz &quot;Umgebungs-Verdeckung&quot; ein. Vergessen Sie nicht, die Standardbearbeitung der Füllebene zu ändern, wenn sie nicht bereits auf 1 gesetzt ist.\
![](../../assets/ao-stack.png)

### 3 - Füllmethode der Ebene ändern

Standardmäßig ist der Mischmodus des AO-Kanals auf einer neuen Ebene auf &quot;**Multiply** &quot; eingestellt. Da es besser ist, die Füllebene als Basis zu verwenden, haben wir den &quot;normalen&quot; Mischmodus gewählt, da die Bitmap keinen Alpha-Wert hat. Er ersetzt alles darunter (einschließlich der Standardfarbe des Shaders).\
![](../../assets/ao-blend-mode.gif)

### 4 - Erstellen einer Ebene zum Übermalen der Karte mit der gebrannten Verdeckung

Erstelle eine neue Ebene (normal oder gefüllt). Setze den Mischmodus für den AO-Kanal auf &quot;Normal&quot;. Sobald diese Einrichtung abgeschlossen ist, übernimmt alles, was auf dem AO-Kanal gemalt wird, die gebackene AO-Karte, die sich auf der darunter liegenden Ebene befindet.\
![](../../assets/paint-over-ao-optimized.gif)
