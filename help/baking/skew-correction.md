---
title: Verzerrungskorrektur
description: Erfahren Sie, wie Sie die Neigungskorrektur verwenden, um Backartefakte zu beheben, wenn Sie einen hohen bis niedrigen Poly-Arbeitsablauf in Substance 3D Painter verwenden.
source-git-commit: db1c8daa33389f21699c53b0d6555c153fbc66d6
workflow-type: tm+mt
source-wordcount: '1027'
ht-degree: 0%

---


# Verzerrungskorrektur

<table>
  <tr style="border: 0;">
    <td style="border: 0; width: 35%" valign="top"><img src="../assets/baking/skew-correction-example.png" alt=""/></td>
    <td style="border: 0; width: 65%" valign="top">Manchmal ist es beim Backen auf Low-Poly von einem High-Poly-Modell möglich, dass Details verzerrt oder verzerrt erscheinen. Dies geschieht in der Regel, wenn die Käfig- und Flächennormalen nicht gut übereinstimmen. Automatisches Backen projiziert das High-Poly auf das Low-Poly basierend auf diesen Normalwerten. Wenn sie also falsch sind, führt das Backen zu schlechten Ergebnissen.<br>Zum Glück ist eine Neigungskorrektur (oder Neigungszuordnung) verfügbar, um diesen Artefakttyp zu beheben.<br>Die Neigungskorrektur ermöglicht es Ihnen, Werte direkt auf das Gitter mit geringer Poly-Polung zu malen, um die beim Backen verwendete Projektion umzuleiten, ohne einen benutzerdefinierten Käfig erstellen zu müssen.</td>
  </tr>
</table>

>[!NOTE]
>
> Die Neigungskorrektur wird im **Backmodus** gemalt und pro Textursatz gespeichert.

## Malen von Verzerrungskorrekturen

Mit der Neigungskorrektur können Sie die Oberflächennormalen Ihres Gitters manuell anpassen, insbesondere für das Backen. Sie können zwar Schrägverzerrungskorrekturen ohne Backen zeichnen, aber Sie können dabei helfen, [zuerst Ihre Gitterzuordnungen zu backen](how-to-bake-mesh-maps.md).

![](../assets/baking/mode_select_buttons.png)

*Wechseln Sie in den Backmodus, um auf die Skew-Korrektureinstellungen zuzugreifen.*

>[!IMPORTANT]
>
> Das Zeichnen mit Neigungskorrektur erfordert die folgenden Einstellungen:
>
> * Es muss eine High-Poly-Szene ausgewählt werden. Skew-Malerei ist nur beim Backen von hohem bis niedrigem Poly verfügbar; Wenn **Niedriges Poly-Gitter als hohes Poly-Gitter verwenden** aktiviert ist, ist das Verzerrungskorrekturmalen **nicht** verfügbar.
> * **Der Käfig** muss auf **Entfernungsbasiert** festgelegt sein.
> * **Durchschnittliche Normale** müssen überprüft werden.

Mit den oben genannten Einstellungen können Sie im **Bedienfeld für allgemeine Einstellungen** auf **Korrektur der Farbneigung** klicken, um mit dem Malen zu beginnen. Wenn Sie den Zeichnungsmodus für die Neigungskorrektur zum ersten Mal aufrufen, wird **Auto-Rebake** automatisch für den normalen Kanal aktiviert. Falls gewünscht, können Sie **Auto-Reframe** deaktivieren oder den ausgewählten Kanal im Fenster [**Gitterzuordnungs-Bäcker**](../interface/baking-panels/mesh-map-bakers.md) ändern.

![](../assets/baking/skew-correction-menu.png)

### Malwerkzeuge

Beim Malen von Neigungskorrekturen können Sie viele der Werkzeuge und Verknüpfungen verwenden, die Sie vom Malmodus gewohnt sind, einschließlich der **Radiergummi**- und **Polygonfüllung**-Werkzeuge.

* Sie können von der Symbolleiste aus zwischen **Pinsel**, **Radiergummi** und **Polygonfüllung** wechseln oder den standardmäßigen [Tastaturbefehl](../interface/settings/shortcuts.md) aus dem Malmodus verwenden.
* Bei Verwendung des Pinsel- oder Radiergummis können Sie die Pinselgröße, den Fluss, die Deckkraft und den Abstand mit den Parametern oben im **Viewport** anpassen. Sofern verfügbar, können Sie auch den entsprechenden [Tastaturbefehl](../interface/settings/shortcuts.md) verwenden.

### Kantenschutz

Beim Kantenschutz wird die Korrektur der gestrichenen Schrägstellung in der Nähe von Kanten ignoriert, um einen glatten Verlauf der Flächennormalen beizubehalten. Sie können den **Kantenschutz** im Abschnitt **Neigungskorrektur** umschalten. Wenn **Kantenkorrektur** aktiviert ist, können Sie den Kantenabstand und den Kantenkontrast anpassen, um optimale Ergebnisse zu erzielen.

* Kantenabstand: Lege fest, wie weit der Kantenschutz vom Rand entfernt ist.
* Kantenkontrast: Steuern Sie den Kantenschutzverlauf. Ein niedriger Kontrast erzeugt einen glatteren Verlauf.

>[!TIP]
>
> Die Werte für **Kantenabstand** und **Kantenkontrast** basieren auf der Größe des Gitters. Bei Maschen mit sehr kleinen Details im Vergleich zur Maschengröße ist es möglicherweise einfacher, kleine Werte manuell einzugeben, anstatt die Schieberegler zu verwenden.

>[!NOTE]
>
> Der Kantenschutz basiert auf der Gittermaske **Harte Kanten**, die an die Geometrie des Gitters gebunden ist, nicht an die UV-Grenzen.

### Skew-Vektorvisualisierung

Wenn Sie mit dem Zeichnen von Neigungskorrekturen beginnen, werden die Netzflächennormalen im **Viewport** standardmäßig als rote, gelbe und grüne Linien angezeigt. Sie können die Darstellung dieser Zeilen ändern oder sie im Abschnitt **Skew-Vektoren** des Menüs **Visualisierungen**, das im **Viewport** angezeigt wird, vollständig deaktivieren.

![](../assets/baking/visualizations_menu.png)

* **Vektorlänge**: Passen Sie die Länge der Linien im Darstellungsfenster an. Mit längeren Linien fällt es leichter, die Richtung des Vektors zu verstehen.
* **UV-Dichte von Vektoren**: Ändern Sie die Anzahl der Linien auf der Oberfläche des Gitters. Vektoren werden im UV-Raum platziert. Wenn das Gitter also eine inkonsistente Texeldichte hat, variiert die Anzahl der Vektoren pro Flächeneinheit mit der Polygongröße in der UV-Karte.
* **Vektordeckkraft**: Mache die Vektoren mehr oder weniger transparent.

Die Farbe der Vektoren gibt den Umfang der Neigungskorrektur an, die an jeder Vektorposition angewendet wird.

* Rote Vektoren zeigen keine Neigungskorrektur an - die Standardoberflächennormale werden verwendet.
* Grüne Vektoren zeigen an, dass die Oberflächennormalen vollständig korrigiert und direkt senkrecht zur Oberfläche verlaufen.

![](../assets/baking/skew-correction-painting.gif)*Das Malen mit einem niedrigen Flusswert gibt eine feine Kontrolle über die Stärke der Neigungskorrektur.*

## Optimieren der Leistung

### Organisieren von UVs

**Auto-Rebake** ist optimiert, um beim Malen von Verzerrungskorrekturen das Nachzeichnen auf den Bereich zu beschränken, der von jedem Pinselstrich betroffen ist. Wenn Sie einen Strich zeichnen, zeichnet **Auto-rebake** einen Begrenzungsrahmen um den Strich im UV-Raum und ändert alles im Rahmen neu. Das bedeutet, wenn Ihr Strich nur einen kleinen Teil des UV-Raumes bedeckt, wird nur ein kleiner Bereich umgebrochen, was den Vorgang sehr effizient macht.

Wenn der Strich jedoch zwei UV-Inseln auf gegenüberliegenden Seiten des UV-Raums kreuzt, muss möglicherweise schon ein kleiner Strich die gesamte Textur zurückgenommen und die Optimierung negiert werden.

Daher empfehlen wir, die Gitter-UVs so zu organisieren, dass UV-Inseln, die im 3D-Raum nahe beieinander liegen, auch im UV-Raum nahe beieinander liegen. Dadurch wird die Leistung von **Auto-Rebake** verbessert.

### Ausrichtung auf UV festlegen

Im Allgemeinen ist das Malen von Neigungskorrekturen mit **Projektion > Ausrichtung** auf UV leistungsfähiger. So ändern Sie die **Ausrichtung**:

1. Wählen Sie &quot;**Paint skew correction**&quot; aus und statten Sie entweder den **Pinsel** oder den **Radiergummi** aus.
1. Klicken Sie mit der rechten Maustaste in den **Viewport**, um das **Bedienfeld für Pinseleinstellungen** zu öffnen.
1. Scrollen Sie nach unten zu **Projektion**.
1. Legen Sie **Ausrichtung** auf **UV** fest.

Da **Alignment** auf **UV** festgelegt ist, ist es schwieriger, glatte Konturen über UV-Insel-Nähte zu malen. Dies ist jedoch im Allgemeinen beim Malen von Neigungskorrekturen weniger wichtig als beim Texturieren des Gitters.

>[!NOTE]
>
> Die Parameter für den **Pinsel** und den **Radiergummi** werden separat gespeichert. Um die Leistung für beide Tools zu maximieren, müssen Sie **Alignment** für jedes Werkzeug einzeln festlegen.

## Neigungskorrekturen und Rückgängigmachen des Stapels

Backen und Malen haben einen einzigen Verlauf, der rückgängig gemacht wird. Der Wechsel zwischen dem Backmodus und dem Malmodus kann rückgängig gemacht werden. Das Aktivieren oder Deaktivieren der Neigungskorrektur kann ebenfalls rückgängig gemacht werden. Wenn Sie eine Backaktion im Malmodus rückgängig machen, wird der Backmodus automatisch erneut geöffnet, bevor diese Schritte rückgängig gemacht werden. Eine Aktion wird also außerhalb des Modus, in dem sie ausgeführt wurde, nie rückgängig gemacht.