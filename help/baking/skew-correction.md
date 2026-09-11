---
title: Verzerrungskorrektur
description: Erfahren Sie, wie Sie mit Verzerrungskorrektur Baking führend Artefakte in Substance 3D Painter beheben können, wenn Sie einen Poly-Arbeitsablauf mit hohem bis niedrigem Wert verwenden.
source-git-commit: db1c8daa33389f21699c53b0d6555c153fbc66d6
workflow-type: tm+mt
source-wordcount: '1027'
ht-degree: 0%

---


# Verzerrungskorrektur

<table>
  <tr style="border: 0;">
    <td style="border: 0; width: 35%" valign="top"><img src="../assets/baking/skew-correction-example.png" alt=""/></td>
    <td style="border: 0; width: 65%" valign="top">Manchmal ist es beim Backen auf Low-Poly von einem High-Poly-Modell möglich, dass Details verzerrt oder verzerrt erscheinen. Dies geschieht in der Regel, wenn die Käfig- und Flächennormalen nicht gut übereinstimmen. Automatisches Backen projiziert das High-Poly auf das Low-Poly basierend auf diesen Normalwerten. Wenn sie also falsch sind, führt das Backen zu schlechten Ergebnissen.<br>Zum Glück ist eine Neigungskorrektur (oder Neigungszuordnung) verfügbar, um diesen Artefakttyp zu beheben.Mit <br>Verzerrungskorrektur können Sie Werte direkt auf den Mesh mit niedriger Poly-Malen, um die beim Baking verwendete Projektion umzuleiten, ohne einen benutzerdefinierten Käfig erstellen zu müssen.</td>
  </tr>
</table>

>[!NOTE]
>
> Die Verzerrungskorrektur wird im **Baking-Modus** gemalt und pro Textursatz gespeichert.

## Malen von Verzerrungskorrekturen

Mit Verzerrungskorrektur Painting können Sie die Oberflächennormalen Ihres Meshs speziell für das Baking manuell anpassen. Sie können zwar Verzerrungskorrekturen ohne Baking Malen, aber es kann helfen, [Ihre Mesh-Map zuerst Baking führen](how-to-bake-mesh-maps.md).

![](../assets/baking/mode_select_buttons.png)

*Wechseln Sie in den Baking-Modus, um auf die Einstellungen für die Verzerrungskorrektur zuzugreifen.*

>[!IMPORTANT]
>
> Zum Malen von Verzerrungskorrekturen sind die folgenden Einstellungen erforderlich:
>
> * Es muss eine hohe Poly-Szene ausgewählt werden. Skew-Painting ist nur beim Baking führ von hohen zu niedrigen Poly-Werten verfügbar. Wenn **Low-Poly-Mesh als High-Poly-Mesh** verwenden aktiviert ist, ist das Zeichnen von Verzerrungskorrekturen **nicht** verfügbar.
> * **Käfig** muss auf **Entfernungsbasiert** festgelegt sein.
> * **Durchschnittliche Normale** müssen überprüft werden.

Mit den oben genannten Einstellungen können Sie im **Bedienfeld für allgemeine Einstellungen** auf **Malen-Verzerrungskorrektur** klicken, um mit dem Malen zu beginnen. Wenn Sie zum ersten Mal den Verzerrungskorrektur-Malmodus aufrufen, wird **Auto-Rebake** automatisch für den normalen Kanal aktiviert. Falls gewünscht, können Sie **Auto-Rebake** deaktivieren oder den ausgewählten Kanal im [**Mesh-Map-Baker-Bedienfeld**](../interface/baking-panels/mesh-map-bakers.md) ändern.

![](../assets/baking/skew-correction-menu.png)

### Malwerkzeuge

Beim Malen von Verzerrungskorrekturen können Sie viele der Tools und Tastaturbefehle verwenden, die Sie vom Malmodus gewohnt sind, einschließlich der Tools **Radiergummi** und **Polygonfüllung**.

* Sie können von der Symbolleiste aus zwischen **Pinsel**, **Radiergummi** und **Polygonfüllung** wechseln oder den standardmäßigen [Tastatur-Tastaturbefehl](../interface/settings/shortcuts.md) aus dem Malmodus verwenden.
* Bei Verwendung der Pinsel- oder Radiergummi-Werkzeuge können Sie die Pinselgröße, den Fluss, die Deckkraft und den Abstand mit den Parametern oben im **Viewport** anpassen. Sie können auch den entsprechenden [Tastatur-Tastaturbefehl](../interface/settings/shortcuts.md) verwenden, sofern verfügbar.

### Kantenschutz

Beim Kantenschutz wird die gestrichelte Verzerrungskorrektur in der Nähe der Kanten ignoriert, um einen gleichmäßigen Verlauf der Flächennormalen beizubehalten. Sie können den **Kantenschutz** im Abschnitt **Verzerrungskorrektur** umschalten. Wenn **Kantenkorrektur** aktiviert ist, können Sie den Kantenabstand und den Kantenkontrast anpassen, um optimale Ergebnisse zu erzielen.

* Kantenabstand: Lege fest, wie weit der Kantenschutz vom Rand entfernt ist.
* Kantenkontrast: Steuern Sie den Kantenschutzverlauf. Ein niedriger Kontrast erzeugt einen glatteren Verlauf.

>[!TIP]
>
> Die Werte für **Kantenabstand** und **Kantenkontrast** basieren auf der Größe des Meshs. Bei Meshs mit sehr kleinen Details im Vergleich zur Größe des Meshs ist es möglicherweise einfacher, kleine Werte manuell einzugeben, als die Schieberegler zu verwenden.

>[!NOTE]
>
> Der Kantenschutz basiert auf der Mesh-Map **Harte Kanten**, die mit der Geometrie des Meshs verknüpft ist, nicht mit den UV-Rändern.

### Skew-Vektorvisualisierung

Wenn Sie mit dem Malen von Verzerrungskorrekturen beginnen, werden die Flächennormalen des Meshs in **Viewport** standardmäßig als Rot-, Gelb- und Grünlinien angezeigt. Sie können die Darstellung dieser Zeilen ändern oder sie im Abschnitt **Skew-Vektoren** des Menüs **Visualisierungen**, das im Viewport **angezeigt wird, vollständig deaktivieren.**

![](../assets/baking/visualizations_menu.png)

* **Vektorlänge**: Passen Sie die Zeilenlänge im Viewport an. Mit längeren Linien fällt es leichter, die Richtung des Vektors zu verstehen.
* **UV-Vektordichte**: Ändern Sie die Anzahl der Linien auf der Fläche des Meshs. Vektorgrafiken werden im UV-Raum platziert. Wenn der Mesh eine inkonsistente Texeldichte hat, variiert die Anzahl der Vektorgrafiken pro Flächeneinheit entsprechend der Polygongröße in der UV-Map.
* **Vektordeckkraft**: Mache die Vektoren mehr oder weniger transparent.

Die Vektorfarbe gibt den Grad der Verzerrungskorrektur an, der an jeder Vektorposition angewendet wird.

* Rote Vektoren zeigen keine Verzerrungskorrektur an - die Standardoberflächennormale werden verwendet.
* Grüne Vektoren zeigen an, dass die Oberflächennormalen vollständig korrigiert und direkt senkrecht zur Oberfläche verlaufen.

![](../assets/baking/skew-correction-painting.gif)*Das Malen mit einem niedrigen Flusswert ermöglicht eine Feinsteuerung der Stärke der Verzerrungskorrektur.*

## Optimieren der Leistung

### Organisieren von UVs

**Auto-Rebake** ist optimiert, um beim Malen von Verzerrungskorrekturen das Rebake auf den Bereich zu beschränken, der von jedem Pinselstrich betroffen ist. Wenn Sie einen Strich Malen haben, zeichnet **Auto-rebake** einen Begrenzungsrahmen um den Strich im UV-Raum und ändert alles im Rahmen neu. Das bedeutet, wenn Ihr Strich nur einen kleinen Teil des UV-Platzes bedeckt, wird nur ein kleiner Bereich umgebrochen, was den Vorgang sehr effizient macht.

Wenn der Strich jedoch zwei UV-Inseln auf gegenüberliegenden Seiten des UV-Raums kreuzt, muss möglicherweise schon ein kleiner Strich die gesamte Textur zurückgebogen und die Optimierung negiert werden.

Daher empfehlen wir, Mesh-UVs so zu organisieren, dass UV-Inseln, die im 3D-Raum nahe beieinander liegen, auch im UV-Raum nahe beieinander liegen. Dadurch wird die Leistung von **Auto-Rebake** verbessert.

### Ausrichtung auf UV festlegen

Im Allgemeinen ist das Malen von Verzerrungskorrekturen, bei denen **Projektion > Ausrichtung** auf UV festgelegt ist, leistungsfähiger. So ändern Sie die **Ausrichtung**:

1. Wählen Sie **Malen-Verzerrungskorrektur** und statten Sie entweder den **Pinsel** oder den **Radiergummi** aus.
1. Klicken Sie mit der rechten Maustaste in den **Viewport**, um das **Pinseleinstellungsbedienfeld** zu öffnen.
1. Scrollen Sie nach unten zu **Projektion**.
1. Legen Sie **Ausrichtung** auf **UV** fest.

Da **Alignment** auf **UV** festgelegt ist, ist es schwieriger, glatte Konturen über UV-Insel-Nähte hinweg zu Malen. Dies ist jedoch beim Malen von Verzerrungskorrekturen im Allgemeinen weniger wichtig als beim Texturieren Ihres Meshs.

>[!NOTE]
>
> Die Parameter für **Brush** und **Radiergummi** werden separat gespeichert. Um die Leistung für beide Tools zu maximieren, müssen Sie **Alignment** für jedes Werkzeug einzeln festlegen.

## Verzerrungskorrekturen und der Stapel &quot;Rückgängig&quot;

Backen und Malen haben einen einzigen Verlauf, der rückgängig gemacht wird. Der Wechsel zwischen dem Backmodus und dem Malmodus kann rückgängig gemacht werden. Das Aktivieren oder Deaktivieren der Neigungskorrektur kann ebenfalls rückgängig gemacht werden. Wenn Sie einen Baking führend Vorgang rückgängig machen, während Sie sich im Malen-Modus befinden, wird der Baking führend Modus automatisch erneut geöffnet, bevor diese Schritte rückgängig gemacht werden. Eine Aktion wird daher außerhalb des Modus, in dem sie ausgeführt wurde, nie rückgängig gemacht.