---
title: Käfig-Malerei
description: Erfahren Sie, wie Sie mit dem Käfig-Malen in Substance 3D Painter Artefakte vermeiden und den Käfig während des Bakings anpassen können.
hold: true
source-git-commit: eb0b1c111b0c96a87283785cf702def7305f0aa9
workflow-type: tm+mt
source-wordcount: '1040'
ht-degree: 0%
---

# Käfig-Malerei

Mit **Käfig-Painting** können Sie Bereiche Malen, um den Baking führend Käfig weiter weg zu schieben oder näher an die Oberfläche mit geringer Polung heranzuführen. Mit dem Käfig-Painting können Sie Artefakte während des Bakings verhindern, während Sie gleichzeitig alle polyvalenten Details Ihres Meshs erfassen.

## Einrichten des Käfig-Malens

Damit **Käfig-Painting** verfügbar ist, muss das Projekt über mindestens eine Datei mit hoher Szene verfügen, von der aus Baking geführt werden kann, und der Käfig-Typ muss auf **entfernungsbasiert** festgelegt sein.

>[!NOTE]
>
> Unterstützung für **Käfig-Malerei** wird in einer zukünftigen Version für den **automatischen Käfig-Typ** hinzugefügt.

Das Anpassen von **Käfig**-Parametern nach dem Malen mit dem Käfig kann die gemalten Bereiche verändern, was möglicherweise eine Nachbearbeitung erfordert oder sogar einen Neustart des Käfig-Malvorgangs erfordert. Daher ist es besser, diese Parameter zuerst anzupassen.

**Der maximale Abstand nach vorn** und **Der maximale Abstand nach hinten** steuern den Basisabstand zwischen dem Käfig und der Oberfläche des Meshs mit niedriger Poly-Auflösung. Beim Malen mit dem Käfig werden diese Werte als Grenzen verwendet, um festzulegen, wie stark der Käfig geändert werden soll. Große Anpassungen dieser Werte nach dem Malen des Käfigs können zu unerwarteten Schnittpunkten führen.

**Relativ zum Begrenzungsrahmen** steuert die Einheiten, die zum Definieren der Größe des Käfigs verwendet werden. Wenn Sie diesen Parameter ändern, kann sich die Größe des Käfigs drastisch ändern. Daher müssen alle bemalten Bereiche wahrscheinlich neu bemalt werden, um die neuen Werte zu korrigieren.

>[!TIP]
>
> Wenn Sie das Käfig-Malen von Grund auf neu beginnen möchten, können Sie die Käfig-Malparameter, die Käfig-Malstriche oder alle Baking-Einstellungen zurücksetzen.
>
> ![](../assets/baking/cage-painting/resetcage.png)

## Käfig malen

So beginnen Sie mit dem Käfig-Malen:

1. Wechseln Sie in den [**Baking-Modus**](baking.md).
1. Stellen Sie sicher, dass Sie mindestens eine **Datei mit hoher Poly-Szene** ausgewählt haben, von der Baking geführt werden soll.
1. Navigieren Sie im Bereich **Allgemeine Einstellungen** **Bereich** zum Abschnitt **Käfig**.
1. Legen Sie den **Käfig type** auf **Distance-based** fest.
1. Klicken Sie auf **Malen Käfig**.

>[!NOTE]
>
> Standardmäßig ist **Quick Baking** für den normalen Kanal aktiviert, wenn Sie zum ersten Mal **Käfig Malerei** eingeben. Dies bedeutet, dass der Normalen-Map bei jeder Änderung des Käfigs automatisch neu gestartet wird. Wenn Sie dies bevorzugen, können Sie im [**Mesh-Map-Baker-Bedienfeld**](../interface/baking-panels/mesh-map-bakers.md) das **Quick Baking** deaktivieren.

Sobald Sie den Käfig-Malmodus aufrufen, zeigt die Standardvisualisierung in **Viewport** Folgendes an:

* Der Käfig um den Mesh in Beige.
* Bereiche, in denen die hohe Poly den Käfig in leuchtendem Rot schneidet.
* Käfig bemalte grüne Bereiche auf der Oberfläche von Meshs mit niedrigem Poly-Anteil.

Im Käfig-Malmodus können Sie das [**Elementvisualisierungsmenü**](baking-visualization-settings.md) im **Viewport** verwenden, um die Visualisierungsfarbe und -deckkraft für jedes Baking zu ändern, oder die Visualisierung für bestimmte Elemente aktivieren bzw. deaktivieren.

>[!NOTE]
>
> Die leuchtend rote Visualisierung von Kreuzungen mit dem Käfig ist eine ungefähre Vorschau und stimmt nicht genau mit den endgültigen Baking-Ergebnissen überein. In den meisten Fällen ist die Visualisierung recht präzise, aber bei Meshs mit geringem Poly-Wert und langen, schmalen Polygonen kann sie ungenau sein, und es ist besser, das Baking geführt Ergebnis zu sehen.

## Käfig-Malwerkzeuge

Beim Malen des Käfigs können Sie viele der Tools und Tastaturbefehle verwenden, die Sie vom **Malmodus** gewohnt sind, einschließlich der **Pinsel**, **Radiergummi** und **Polygonfüllung**.

* Sie können von der Symbolleiste aus zwischen **Pinsel**, **Radiergummi** und **Polygonfüllung** wechseln oder die standardmäßigen [Tastaturbefehle](../interface/settings/shortcuts.md) im Malmodus verwenden.
* Bei Verwendung der Tools **Paintbrush** oder **Radiergummi** können Sie die Größe, den Fluss, die Deckkraft und den Abstand des Tools mithilfe der Parameter oben im **Viewport** anpassen. Sofern verfügbar, können Sie auch die entsprechenden [Tastaturbefehle](../interface/settings/shortcuts.md) verwenden.

### Pinsel

Die Verwendung des **Pinsels** in voller **Stärke**, **Fluss** und **Deckkraft** hat einen großen Einfluss auf die Oberfläche des Käfigs. Es wird empfohlen, einen sehr niedrigen Wert für **Stärke** festzulegen und die Parameter &quot;Fluss&quot; und &quot;Deckkraft&quot; zu verwenden, um die Stärke des Pinsels zu steuern.

TODO: Animation/Video, die den Unterschied in der Stärke zeigt

>[!NOTE]
>
> Standardmäßig verwendet das Pinselwerkzeug beim Malen mit Käfigen den Mischmodus **Linear abwedeln (Hinzufügen)**. Bei dieser Füllmethode wird durch nachfolgende Striche im selben Bereich die Stärke des Effekts konsistent aufgebaut, sodass Sie die Käfig-Oberfläche mit konsistenten Ergebnissen formen können. Die standardmäßigen **Maximalen (Aufhellen)**- und **Normalen**-Mischmodi sind weiterhin verfügbar:
>
> 1. Klicken Sie mit der rechten Maustaste, um die Pinseleigenschaften zu öffnen.
> 1. Scrollen Sie nach unten zu **Alpha > Erweiterte Füllmethode**.
> 1. Wählen Sie den Modus &quot;**Stempelmischung**&quot; aus.

### Radiergummi

Mit dem Radiergummi-Werkzeug können Sie Malen aus dem Käfig entfernen und gelöschte Bereiche effektiv auf die Standardgröße des Käfigs zurücksetzen.

### Polygon-Füllen

Im **Käfig-Malen** **Modus** verfügt das Polygon-Füllwerkzeug über eine zusätzliche Funktion. Nach der Auswahl von Polygonen wird im Viewport ein **Stärke-Schieberegler** angezeigt, mit dem Sie die Stärke für die ausgewählten Polygone anpassen können. Dies kann die Feinabstimmung der Stärke des Effekts erleichtern, ohne dass Polygone ständig neu ausgewählt werden müssen.

>[!NOTE]
>
> Diese Funktion wiederholt den letzten Vorgang (Anwenden der Polygonfüllung) mit einer anderen Stärke. Wenn Sie einen anderen Vorgang ausführen oder Werkzeuge ändern, verschwindet der Schieberegler.

Es kann oft sinnvoll sein, den gleichen Polygon-Füllwert auf mehrere Bereiche des Meshs anzuwenden. Gehen Sie folgendermaßen vor:

1. Wählen Sie den ersten Polygonsatz aus.
1. Verwenden Sie den Regler **Käfig Stärke**, um die Stärke des Effekts anzupassen.
1. Kopieren Sie den Wert **Käfig Stärke** aus dem temporären Schieberegler in **Viewport**.
1. Fügen Sie den Wert in den Schieberegler **Stärke** oben im **Viewport** ein.
1. Wählen Sie die nachfolgenden Sätze von Polygonen mit der gleichen Stärke aus, die auf sie angewendet werden soll.

Im folgenden Video wird dieser Arbeitsablauf in Aktion gezeigt. Dabei wird die **Polygonfüllung** **Werkzeug** mit **Mesh-Füllung** ausgewählt.

TODO: VIDEO

### Überblendung

Standardmäßig wird für das Pinsel- und das Polygon-Füllwerkzeug der Mischmodus &quot;**Linear abwedeln&quot; (Hinzufügen)**&quot; verwendet, Sie können jedoch auch die Mischmodi &quot;**Normal**&quot; und &quot;**Aufhellen&quot; (Max)&quot;** verwenden.

* **Linear abwedeln (hinzufügen)**: Mit jeder Kontur/jedem Stempel wird der angegebene Wert für die Stärke zum vorhandenen Wert hinzugefügt oder vom vorhandenen Wert abgezogen. Dieser Mischmodus funktioniert ähnlich wie bei 3D-Modellierungsanwendungen, bei denen jeder von Ihnen Malen Strich zur Mesh-Oberfläche hinzufügt.
* **Normal**: Jeder Strich/Stempel legt den Wert auf die angegebene Stärke fest und überschreibt den vorhandenen Wert. Dieser Mischmodus verhält sich wie der Standard-Pinsel im Malmodus, sodass Sie die vorhandene Oberfläche mit einem anderen Wert abdecken können.
* **Aufhellen (max.)**: Jede Kontur/jeder Stempel wählt den Maximalwert zwischen der Stärke und dem vorhandenen Wert aus. Bei dieser Füllmethode dauert es länger, bis die Kanten des Pinsels auf den nachfolgenden Strichen aufbauen, was einen fließenderen Übergang ermöglicht.