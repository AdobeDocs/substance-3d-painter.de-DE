---
title: Baker für Mesh-Maps
description: Erfahren Sie, wie Sie mit dem Bedienfeld für Gittermaskenbaker steuern, welche Gittermappen über Textursätze hinweg gebacken werden.
source-git-commit: 987b94e15c1dbe4ddf392ea7878126ecdf989423
workflow-type: tm+mt
source-wordcount: '716'
ht-degree: 0%

---


# Fenster &quot;Gittermaskenbäcker&quot;

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../assets/baking/mesh-map-bakers-panel.png" alt=""/></td>
    <td style="border: 0;" valign="top">Im Bereich "<strong>Mesh Map Baker"</strong> können Sie auswählen, welche Maps gebacken werden sollen, und auf die Einstellungen für jeden Map-Typ zugreifen.</td>
  </tr>
</table>

## Steuerelemente pro Karte

Für jede Karte in der Liste der Gitterzuordnungen steht eine Reihe von Steuerelementen zur Verfügung:

![](../../assets/baking/mesh-map-controls.png)

1. **Überprüfen** oder **Deaktivieren** für die Zuordnung.
1. **Die Karte im Ansichtsfenster visualisieren**.
1. **Schnellbake** nur diese Karte.
1. Aktivieren Sie **Automatische Wiederherstellung** für die ausgewählte Netzzuordnung. **Automatisch gebrochene** Maps werden automatisch wiederhergestellt, wenn Änderungen an den Backparametern oder der Neigungskorrektur vorgenommen werden.
1. **Synchronisieren Sie** Einstellungen für diesen Zuordnungstyp über Textursätze hinweg. Deaktivieren Sie diese Option, um die Backeinstellungen für einzelne Maps anzupassen.

## Verwalten von Einstellungen für Mesh-Maps

Es gibt mehrere Möglichkeiten, Ihr Projekt so zu verwalten, dass Backeinstellungen in Gitterkarten oder Texturensätzen gemeinsam verwendet werden. Bei komplexen Projekten hilft es, den Backvorgang zu vereinfachen, wenn Sie wissen, wie Einstellungen freigegeben werden.

Es gibt zwei Arten von Einstellungen, die Sie für verschiedene Textursätze freigeben können:

* Backeinstellungen: Dies sind Parameter, die Sie in den Einstellungsfenstern **Allgemeine Einstellungen** und **Mesh Map ändern können**.
* Status überprüfen: Verwenden Sie diese, um das Backen für bestimmte Gitterzuordnungen zu aktivieren oder zu deaktivieren.

### Synchronisieren von Backeinstellungen über Textursätze hinweg

Wenn Ihr Projekt über mehrere Textursätze verfügt, werden die Optionen zum Synchronisieren zwischen den Textursätzen im Bedienfeld &quot;**Gittermapbakers&quot; angezeigt**.

![](../../assets/baking/synchronize-texture-sets.png)

Wenn Sie die Schaltfläche **Einstellungen synchronisieren** oben im Bereich **Gitterzuordnungs-Bäcker** auswählen, wird das Synchronisierungsfenster für **Allgemeine Einstellungen** geöffnet.

![](../../assets/baking/synchronize-common-settings.png)

In diesem Fenster können Sie auswählen, welche Textursätze für die Synchronisierung allgemeiner Einstellungen verwendet werden sollen. Wenn alle Textursätze ausgewählt sind, werden sie durch Ändern der allgemeinen Einstellungen in allen anderen Textursätzen geändert.

Wenn Sie die Schaltfläche **Einstellungen synchronisieren** neben einer einzelnen Netzzuordnung verwenden, können Sie in ähnlicher Weise Textursätze auswählen, um die für die Netzzuordnung spezifischen Einstellungen freizugeben.

![](../../assets/baking/synchronize-ao-settings.png)

#### Einstellungen für nicht synchronisierte Texturensätze freigeben

Manchmal möchten Sie vielleicht Netzzuordnungen über Textursätze hinweg nicht synchronisieren, aber dennoch die Backeinstellungen von einem Textursatz in einen anderen kopieren.

Um allgemeine Einstellungen in bestimmte Textursätze zu kopieren, ohne sie zu synchronisieren, wählen Sie **Alle Einstellungen mit weiteren Textursätzen synchronisieren...** aus dem Dropdown-Menü **Gittermapbaker**.

Sie können auch **Alle Einstellungen mit allen Textursätzen synchronisieren** verwenden, um die Einstellungen in alle Textursätze im Projekt zu kopieren.

![](../../assets/baking/copy-common-baking-settings.png)

Wenn Sie die Einstellungen für eine einzelne Gitterzuordnung in bestimmte Texturensätze kopieren möchten:

1. Klicken Sie mit der rechten Maustaste auf die Gitterzuordnung.
1. Wählen Sie **Einstellungen für &lt;Mesh Map> auf weitere Textursätze anwenden...**

![](../../assets/baking/copy-ao-settings.gif)

*Im obigen Beispiel beginnt jeder Textursatz mit unterschiedlichen Einstellungen für AO. Ohne die zu synchronisierende AO-Gitterzuordnung verwenden wir **Umgebungseinstellungseinstellungen auf weitere Textursätze anwenden...**, damit wir die AO-Einstellungen für den neuen Textursatz von derselben Grundlinie aus ändern können.*

### Verwalten des Überprüfungsstatus für Netzzuordnungen

Der Überprüfungsstatus bestimmt, ob eine bestimmte Karte enthalten ist, wenn Sie Gitterkarten backen. Es gibt viele Möglichkeiten, den Überprüfungsstatus für den aktuellen Textursatz zu verwalten:

* Aktivieren oder deaktivieren Sie einzelne Karten.
* Verwenden Sie **Alle überprüfen** oder **Alle deaktivieren**, um alle Netzzuordnungen zu überprüfen oder zu deaktivieren.
* Verwenden Sie **Überprüfte Gitterzuordnungen umkehren** aus dem Dropdown-Menü **Gitterzuordnungs-Bäcker**, um den Überprüfungsstatus aller Zuordnungen zu ändern.

![](../../assets/baking/click-drag-check.gif)

>[!TIP]
>
> Sie können auf ein Kontrollkästchen klicken und es ziehen, um mehrere Maps schnell zu aktivieren bzw. zu deaktivieren (siehe Animation oben).

![](../../assets/baking/invert-checked.gif)

*Im obigen Beispiel verwenden wir **Überprüfte Gitterzuordnungen umkehren**, um schnell zwischen der Auswahl zu wechseln, und backen dann Gitterzuordnungen, die noch nicht gebacken wurden.*

Wenn Sie mit mehreren Textursätzen arbeiten, können Sie auch den Überprüfungsstatus von Maps auf andere Textursätze kopieren, indem Sie **Auf weitere Textursätze anwenden...** aktivieren oder den Überprüfungsstatus auf alle Textursätze kopieren, wobei **Auf alle Textursätze anwenden aktiviert ist**.

![](../../assets/baking/copy-checked-status.gif)

*Im obigen Beispiel haben wir das Height, die gebogenen Normalen oder die Deckkraft im Textursatz **Material.001**noch nicht gebacken. Diese Netzzuordnungen sind bereits im **Material**-Textursatz ausgewählt. Daher verwenden wir **Auf weitere Textursätze anwenden...**und wählen **Material.001**, um den Überprüfungsstatus zu kopieren. Anschließend backen wir die Maps zusammen - beachten Sie, dass die Visualisierung die Gittermaps zweimal durchläuft, während die Maps gebacken werden - da sie für beide Textursätze gebacken werden.*