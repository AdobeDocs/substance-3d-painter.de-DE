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

Für Dynamische Pinselstriche ist die Performance des Substance-Graphen sehr wichtig, da die Substance in kürzester Zeit mehrfach regeneriert werden kann. Wenn eine Substance-Berechnung zu schwer ist, kann sie zu Latenz führen und daher beim Malen stottert und friert ein. Das alles kann zu einem schlechten Malerlebnis führen. Auf dieser Seite werden Informationen und Empfehlungen zur Verwendung der Funktion &quot;Dynamische Konturen&quot; neu gruppiert.

## Berechnungen mit Dynamischen Pinselstrichen können aufwändig sein

Es ist auch wichtig zu wissen, dass die Berechnung Auswirkungen in verschiedenen Kontexten haben kann:

* **Beim Malen** : Die dynamische Kontur wird (abhängig von ihren Einstellungen) beim Malen erzeugt. Falsche Konfigurationen können das Malen verlangsamen und verzögern.
* **Beim erneuten Öffnen eines Projekts** : Selbst wenn der Malprozess gut verlaufen ist, besteht immer noch die Möglichkeit, dass die Berechnung beim Öffnen eines Projekts zum Stillstand kommt, wodurch die Öffnung von Projekten viel länger dauert als sonst. Das liegt daran, dass der erste Malvorgang gut verlaufen ist, weil die Berechnung über die Zeit verteilt war. Beim Öffnen eines Projekts geschieht dies jedoch fast immer gleichzeitig. Dies bedeutet, dass ein Projekt Tausende von eindeutigen Substance generieren lassen könnte, wenn der Dynamic Stroke nicht ordnungsgemäß konfiguriert war.
* **Speicherverbrauch** : Wenn Sie für ein Substance-Diagramm viele Variationen generieren, kann dies sehr viel Speicher beanspruchen (da diese Generationen flüchtig sind, da sie spontan erstellt werden).

## Verwenden von Jitter- und Abstandseinstellungen

Während es einfach ist, beeindruckende oder erweiterte Effekte innerhalb der Substance selbst zu implementieren, kann es manchmal vorteilhafter sein, sie einfach zu halten und stattdessen native Einstellungen der Werkzeugparameter von Substance 3D Painter zu verwenden. Diese Einstellungen lassen sich viel schneller für die Mal-Engine berechnen:

* **Jitter** : Mit diesen Parametern können Sie sehr kostengünstig Zufälligkeit erzeugen, indem Sie einige Attribute ändern, ohne den Substance neu zu berechnen (z. B. Winkel, Position und Deckkraft).
* **Abstand** : Je kleiner der Abstand ist, desto mehr Stempel werden beim Malen eines Strichs erstellt. Manchmal ist kein kontinuierlicher Pinselstrich erforderlich, und mit einem großen Abstand können Sie auch das verwendete Alpha/Material besser sehen.

## Wann und welche Art von Zufallswert verwendet werden soll

Die Zufallsverteilung ist eine großartige Möglichkeit, Einzigartigkeit zu erzeugen. Das Problem ist, dass die Generierung kostspielig sein kann und im Falle der Funktion &quot;Dynamischer Strich&quot; ziemlich oft passieren kann, wenn sie nicht richtig angepasst wird. Es ist wichtig zu verstehen, wann man das Random Seed einsetzt und wann man es vermeiden sollte, und es ist besser, eine alternative Methode zu wählen, um den besten Kompromiss zwischen visuellen Inhalten und Leistung zu erzielen:

* **Zufallsverteilung pro Stempel** : In diesem Fall wird für jeden Stempel eine neue, eindeutige Substance-Generation generiert. Das ist gut, um zum Beispiel einzigartige Nägel auf einer Holzdiele zu kreieren, aber nicht, wenn du Tinte-/Malspuren kreierst.
* **Zufallsverteilung pro Kontur** : Für den aktuellen Pinselstrich wird eine eindeutige Zufallsverteilung erstellt. Das ist nützlich, wenn es nur wenige Stempel gibt, aber bei jedem Strich einen neuen Satz von Variationen benötigt wird (z. B. ein Sprüheffekt).
* **Statische Zufallsverteilung** : Die Substance wird einmal erstellt und ändert sich nie. Optimal für Aufführungen, aber je nach Bedarf vielleicht zu restriktiv.

Was ist mit **Zeit** ($Zeit) ?\
Die Zeit mag praktisch sein, um einige sehr spezifische Looks zu erstellen, aber sie ist tatsächlich eine der teuersten Variablen, die in einem Substance-Graphen verwendet werden kann. Der Grund dafür ist, dass es sehr schwierig ist, ähnliche Werte von einem Pinselstrich zum anderen zu erhalten, sodass die Pinselmaschine wahrscheinlich immer neue Variationen erzeugen wird. Vermeiden Sie es, wenn Sie können, verwenden Sie stattdessen den Abstand und den Stempelindex, was zusammen zu ähnlichen Ergebnissen führen kann.

## Verwendung von StampIndex und StampCycleCount

**StampIndex** ist die ID eines einzelnen Stempels innerhalb eines Pinselstrichs. Standardmäßig beginnt er bei 0 und erhöht sich für jeden neuen Stempel um 1. **StampCycleCount** ist eine Möglichkeit, die Anzahl eindeutiger Indizes zu begrenzen, und weist Substance 3D Painter an, die bereits generierten Substance-Graphen zu recyceln/wiederzuverwenden. Wenn die aktuelle ID den Grenzwert erreicht, startet Substance 3D Painter wieder von 0, wodurch eine Schleife erstellt wird.

Die beste Lösung, um Zufälligkeit zu haben und gleichzeitig gute Leistungen zu erhalten, besteht daher darin, die Zyklusanzahl mit den folgenden Optionen zu nutzen:

* **StampIndex als RandomSeed** : Beim Erstellen eines Substance-Graphen kann die Zufallsverteilung als &quot;Absolut&quot; eingestellt werden. Auf diese Weise können Sie ihm einen benutzerdefinierten Wert zuweisen, der der Stempelindex sein kann. Damit erstellst du für jeden Stempel in deinem Strich eine eigene Substance-Diagrammversion.
* **In Kombination mit StampCycleCount** : können Sie eine begrenzte Anzahl neuer Varianten erstellen und diese dann wiederverwenden.
* **Zufallsstart** : Wenn der Zykluszähler so festgelegt ist, dass er von einem zufälligen Wert statt von 0 startet, bedeutet dies, dass zu Beginn für jeden Strich innerhalb des Pools bereits generierter Substance eine andere Zyklusversion verwendet wird.

## Deaktivieren der Berechnung auf der Grundlage von Parameterwerten

Substance 3D Painter kann beim Anpassen eines Parameters nicht bestimmen, dass dies zur gleichen Ausgabe führen kann, nur weil die Berechnung im Substance-Graphen ausgeblendet ist. Das ist im Grunde eine Blackbox.

Um die Leistung beim Anpassen von Parametern und beim Malen mit Dynamischen Pinselstrichen zu verbessern, können Sie angeben, wann neue Diagramminstanzen generiert werden sollen, indem Sie bedingte Werte in den Benutzerdatenfeldern des Substance-Diagramms verwenden.

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


In diesem Fall wird der Zufallswert nur geändert, wenn der Diagrammparameter (Bezeichner) **Rundheit\_Jitter** größer als 0 ist oder wenn der boolesche Wert **flip\_x\_jitter** oder **flip\_y\_jitter** aktiviert ist. Wenn die Bedingung nicht erfüllt ist, wird das Diagramm nicht neu generiert. Den Diagrammparametern muss &quot;**input.**&quot; vorangestellt werden.  &quot; zu erkennen.
