---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/painting/dynamic-strokes/dynamic-stroke-performances.html"
breadcrumb-title: ''
description: Erfahren Sie mehr über Überlegungen zur Leistung dynamischer Pinselstriche in Substance 3D Painter, um das Rendern von Pinselstrichen und die Reaktionsfähigkeit zu optimieren.
helpx_creative_field: ""
helpx_description: Painter > Painting > Dynamic strokes > Dynamic Stroke Performances
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Dynamische Strichleistungen
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '995'
ht-degree: 0%

---


# Dynamische Strichleistungen

Für Dynamische Pinselstriche ist die Performance des Substance-Grafen sehr wichtig, da die Substance in kürzester Zeit mehrfach regeneriert werden kann. Wenn eine Substance-Berechnung zu schwer ist, kann sie Latenz erzeugen und daher beim Malen stottert und friert ein. Das alles kann zu einem schlechten Malerlebnis führen. Auf dieser Seite werden Informationen und Empfehlungen zur Verwendung der Funktion &quot;Dynamische Konturen&quot; neu gruppiert.

## Berechnung der Dynamische Pinselstriche kann groß sein

Es ist auch wichtig zu wissen, dass die Berechnung in verschiedenen Kontexten Auswirkungen haben kann:

* **Beim Malen** : Die dynamische Kontur wird (abhängig von ihren Einstellungen) beim Malen erzeugt. Falsche Konfigurationen können das Malen verlangsamen und verzögern.
* **Beim erneuten Öffnen eines Projekts** : Auch wenn der Malprozess gut gelaufen ist, besteht immer noch die Möglichkeit, dass die Berechnung beim Öffnen eines Projekts hängen bleibt und Projekte viel länger geöffnet werden können als sonst. Der Grund dafür ist, dass der ursprüngliche Malprozess gut gelaufen ist, weil die Berechnung über die Zeit verteilt war. Beim Öffnen eines Projekts passiert das jedoch fast immer gleichzeitig. Dies bedeutet, dass ein Projekt Tausende von eindeutigen Substance generieren lassen könnte, wenn der Dynamic Stroke nicht ordnungsgemäß konfiguriert war.
* **Speicherverbrauch** : Wenn Sie für einen Substance-Graf viele Varianten generieren, kann dies zu großem Arbeitsspeicher führen (da diese Generationen flüchtig sind, da sie spontan erstellt werden).

## Verwenden der Einstellungen für Jitter und Abstand

Während es einfach ist, beeindruckende oder erweiterte Effekte innerhalb der Substance selbst zu implementieren, kann es manchmal vorteilhafter sein, sie einfach zu halten und stattdessen native Einstellungen der Werkzeugparameter von Substance 3D Painter zu verwenden. Diese Einstellungen lassen sich viel schneller für das Malen-Engine berechnen:

* **Jitter** : Mit diesen Parametern können Sie sehr kostengünstig Zufälligkeit erzeugen, indem Sie einige Attribute ändern, ohne den Substance neu zu berechnen (z. B. Winkel, Position und Deckkraft).
* **Abstand** : Je kleiner der Abstand ist, desto mehr Stempel werden beim Malen eines Strichs erstellt. Manchmal ist kein kontinuierlicher Pinselstrich erforderlich, und mit einem großen Abstand können Sie auch besser sehen, wie Alpha/Material verwendet wird.

## Wann und welche Art von Zufallswert verwendet werden soll

Die Zufallsverteilung ist eine großartige Möglichkeit, Einzigartigkeit zu erzeugen. Das Problem ist, dass die Generierung kostspielig sein kann und im Falle der Funktion &quot;Dynamischer Strich&quot; ziemlich oft passieren kann, wenn sie nicht richtig angepasst wird. Es ist wichtig zu verstehen, wann man das Random Seed einsetzt und wann man es vermeiden sollte, und es ist besser, eine alternative Methode zu wählen, um den besten Kompromiss zwischen visuellen Inhalten und Leistung zu erzielen:

* **Zufallsverteilung pro Stempel** : In diesem Fall wird für jeden Stempel eine neue, eindeutige Substance-Generation generiert. Das ist gut, um zum Beispiel einzigartige Nägel auf einer Holzdiele zu kreieren, aber nicht, wenn du Tinte-/Malen-Trails kreierst.
* **Zufallsverteilung pro Kontur** : Für den aktuellen Pinselstrich wird eine eindeutige Zufallsverteilung erstellt. Das ist nützlich, wenn es nur wenige Stempel gibt, aber bei jedem Strich einen neuen Satz von Variationen benötigt wird (z. B. ein Sprüheffekt).
* **Statische Zufallsverteilung** : Die Substance wird einmal erstellt und ändert sich nie. Optimal für Aufführungen, aber je nach Bedarf vielleicht zu restriktiv.

Was ist mit **Zeit** ($Zeit) ?\
Die Zeit ist vielleicht praktisch, um einige sehr spezifische Looks zu erstellen, aber sie ist tatsächlich eine der teuersten Variablen, die in einem Substance-Graf verwendet werden kann. Der Grund dafür ist, dass es sehr schwierig ist, ähnliche Werte von einem Pinselstrich zum anderen zu erhalten, sodass das Pinsel-Engine wahrscheinlich immer neue Variationen erzeugen wird. Vermeiden Sie es, wenn Sie können, verwenden Sie stattdessen den Abstand und den Stempelindex, die kombiniert zu ähnlichen Ergebnissen führen können.

## Verwendung von StampIndex und StampCycleCount

**StampIndex** ist die ID eines einzelnen Stempels innerhalb eines Pinselstrichs. Standardmäßig beginnt er bei 0 und erhöht sich für jeden neuen Stempel um 1. Mit **StampCycleCount** können Sie die Anzahl eindeutiger Indizes begrenzen und Substance 3D Painter anweisen, die bereits generierten Substance-Graf zu recyceln/wiederzuverwenden. Wenn die aktuelle ID den Grenzwert erreicht, startet Substance 3D Painter wieder von 0, wodurch eine Schleife erstellt wird.

Die beste Lösung, um Zufälligkeit zu haben und gleichzeitig gute Leistungen zu erhalten, besteht daher darin, die Zyklusanzahl mit den folgenden Optionen zu nutzen:

* **StampIndex als RandomSeed** : Beim Erstellen eines Substance-Grafen kann die Zufallsverteilung als &quot;Absolut&quot; eingestellt werden. Auf diese Weise können Sie ihm einen benutzerdefinierten Wert zuweisen, der der Stempelindex sein kann. Dadurch wird für jeden Graf innerhalb der Kontur eine eigene Stempelversion erstellt.
* **In Kombination mit StampCycleCount** : können Sie eine begrenzte Anzahl neuer Varianten erstellen und diese dann wiederverwenden.
* **Zufallsstart** : Wenn die Zyklusanzahl so festgelegt ist, dass sie von einem zufälligen Wert statt von 0 startet, bedeutet dies, dass zu Beginn für jeden Strich innerhalb des Pools bereits generierter Graf eine andere Substance-Version verwendet wird.

## Deaktivieren der Berechnung auf der Grundlage von Parameterwerten

Substance 3D Painter kann beim Anpassen eines Parameters nicht bestimmen, dass dies zur gleichen Ausgabe führen kann, nur weil die Berechnung im Substance-Graf ausgeblendet ist. Das ist im Grunde eine Blackbox.

Um die Leistung beim Anpassen von Parametern und beim Malen mit Dynamischen Pinselstrichen zu verbessern, können Sie angeben, wann neue Grapheninstanzen generiert werden sollen, indem Sie bedingte Werte in den Benutzerdatenfeldern des Substance-Grafen verwenden.

Mögliche Werte sind:

| *Variable* | *Nutzung* |
| --- | --- |
| **IsStampIndexActive** | Legt fest, ob sich der Stempelindex beim Malen ändern soll. |
| **IsRandomSeedActive** | Wird verwendet, um festzulegen, ob sich das Zufallsverteilung-Seed während des Malens ändern soll. |
| **IsTimeActive** | Legt fest, ob die Zeit ($time) während des Malens inkrementiert werden soll. |

Beispiel:

```
IsRandomSeedActive=input.roundness_jitter>0 || input.flip_x_jitter || input.flip_y_jitter
```


In diesem Fall wird der Zufallswert nur geändert, wenn der Graf-Parameter (Identifizierung) **Rundheit\_Jitter** größer als 0 ist oder wenn der boolesche **Flip\_x\_Jitter** oder **Flip\_y\_Jitter** aktiviert sind. Wenn die Bedingung nicht erfüllt ist, wird der Graf nicht neu generiert. Graf-Parameter müssen durch die Eingabe &quot;**&quot; vorangestellt werden.**  &quot; zu erkennen.
