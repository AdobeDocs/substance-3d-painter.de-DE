---
title: Reduzieren von Ebenen
description: ''
helpx_description: "Substance 3D Painter"
helpx_url: "https://helpx.adobe.com/substance-3d-painter/interface/layer-stack/flatten-layers.html"
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '883'
ht-degree: 1%

---


# Reduzieren von Ebenen

![](../../assets/v12_banner_flatten.jpg)

## Reduzieren von Ebenen

Durch Reduzieren von Ebenen können Sie die sichtbaren Strukturdaten einer ausgewählten Gruppe in einer einzigen Ebene verdichten. Dies kann dazu beitragen, den Ebenen stapel zu vereinfachen, die Leistung zu verbessern und Ihre Projekte einfacher zu verwalten.

>[!NOTE]
>
> Wenn Sie die Funktion &quot;Reduzieren&quot; verwenden, wird eine neue Ebene erstellt, aber die ursprüngliche Gruppe von Ebenen wird nicht gelöscht. Stattdessen ist die Quellgruppe deaktiviert, sodass Sie sie entweder löschen oder alternativ als Smart-Material für die spätere Bearbeitung speichern können.

## Ebenen reduzieren

So reduzieren Sie eine Reihe von Ebenen:

1. Wählen Sie die gewünschten Ebenen aus.
1. Verwenden Sie <b>STRG + G (CMD + G) </b>zum Gruppieren der Auswahl.
1. Verwenden Sie <b>STRG + M (CMD + M)</b>, um die Auswahl zusammenzuführen.

Statt der Verwendung von Tastaturbefehlen können Sie auch über das Kontextmenü auf diese Optionen zugreifen.

![](../../assets/v12_flatten_menu.jpg)

Wenn Ebenen reduziert werden, wird eine neue Füllebene mit reduzierten Texturen erstellt und die Quellgruppe ist deaktiviert.

## Bestimmte Kanäle reduzieren

* Deaktivieren Sie auf einer Füllebene im Bedienfeld &quot;Eigenschaften&quot; die Kanäle, die Sie nicht reduzieren möchten. Informationen gehen nicht verloren, wenn Kanäle deaktiviert sind. Nachdem Sie die Ebene reduziert haben, können Sie die Kanäle wieder aktivieren, und die Daten sind weiterhin vorhanden
* Bei Gruppen oder Malebenen können Sie Füllmethoden verwenden, um Kanäle zu deaktivieren:
  * Wählen Sie oben im Ebenenstapel den Kanal aus, der deaktiviert werden soll.
  * Ändern Sie die Füllmethode der gewünschten Ebene in &quot;Deaktiviert&quot;.
  * Du kannst denselben Mischmodus auf alle Kanäle einer Ebene anwenden, indem du mit der rechten Maustaste bzw. bei gedrückter Ctrl-Taste auf den Mischmodus klickst und &quot;Auf alle Kanäle anwenden&quot; auswählst.

## Exportieren von reduzierten Maps aus dem Ebenenstapel

Verwenden Sie <b>Reduzierte Gruppe in Dateien exportieren</b> aus dem Kontextmenü im Ebenenstapel, um Texturen schnell zu exportieren. Diese Option ist verfügbar, wenn eine Ebene oder Gruppe ausgewählt ist. Wenn mehrere Ebenen oder Gruppen ausgewählt sind, werden sie als Stapel behandelt - so als ob Sie jede Ebene einzeln exportiert hätten.

>[!NOTE]
>
> Wie bei der <b>Funktion Gruppe reduzieren </b> werden keine leeren oder deaktivierten Kanäle und Ebenen exportiert. Wenn eine Geometriemaske verwendet wird, werden nur UV-Kacheln exportiert, die innerhalb der Geometriemaske aktiviert sind.

### Dateiverwaltung

Wenn Sie <b>Reduzierte Gruppe in Dateien exportieren</b> auswählen, haben Sie die Möglichkeit, einen Ordnerspeicherort für die exportierten Dateien auszuwählen.

Exportierte Dateien werden nach dem Muster im Feld &quot;Dateiname&quot; benannt. Das Standardmuster ist:

* <b>$textureSet\_$layerName\_$srcMap(.$udim)</b>

Mit diesem Muster haben Maps den Textursatznamen, den Ebenennamen, den Kanalnamen und, wenn es sich um ein UV-Kachelprojekt handelt, die UDIM-Nummer.

Wenn Sie das Muster ändern, wird es beim nächsten Öffnen des Fensters wieder verfügbar sein.

### Eigenschaften exportierter Dateien

Die Eigenschaften der exportierten Dateien basieren zum Zeitpunkt des Exports auf den folgenden Werten:

* Die Auflösung basiert auf der Auflösung des Textursatzes.
* Die Bittiefe basiert auf der Bittiefe des Kanals in den Einstellungen für den Textursatz.

Die folgenden Eigenschaften sind fest codiert und können nicht geändert werden:

* Die Auffüllung ist auf 1 px festgelegt.
* Das Dateiformat hängt vom zu exportierenden Kanal ab. Karten wie Height und Normal benötigen in der Regel mehr Bittiefe und werden als EXR exportiert, während andere Kanäle als PNG exportiert werden.
* Wenn nur eine Maske exportiert wird, können Sie das Exportformat auswählen.

## Wie wird die abgeflachte Ebene generiert?

Die Funktion &quot;Reduzieren&quot; erstellt eine Bitmap pro aktiviertem Kanal in einer neuen Füllebene. Die Auflösung basiert auf der Auflösung des Textursatzes, die Bittiefe wird durch die Einstellungen des Textursatzes bestimmt.

&quot;Reduzieren&quot; funktioniert, wenn Texturdaten in einem bestimmten Kanal vorhanden sind. Das Reduzieren funktioniert nicht auf einer leeren Malebene und sendet eine Fehlermeldung an das Protokoll, wenn keine Daten in der Auswahl vorhanden sind.

Nur sichtbare Ebenen und Effekte können reduziert werden. Wenn einige Ebenen in der Gruppe beim Reduzieren der Gruppe deaktiviert sind, werden die Effekte dieser Ebenen nicht in das Reduzierungsergebnis einbezogen.

### Deaktivierte Ebenen

Nur sichtbare Ebenen und Effekte können reduziert werden. Wenn einige Ebenen in der Gruppe beim Reduzieren der Gruppe deaktiviert sind, werden die Effekte dieser Ebenen nicht in das Reduzierungsergebnis einbezogen.

### Ebenenmasken und Geometrie-Masken

Masken werden getrennt von den Texturdaten abgeflacht. Wenn Sie also eine Gruppe mit einer Maske reduzieren, werden sowohl eine abgeflachte Füllung als auch eine abgeflachte Maske generiert.

Wenn bei Verwendung einer Geometriemaske nur einige UV-Kacheln innerhalb der Geometriemaske ausgewählt sind, behält die abgeflachte Ebene diese Auswahl bei. UV-Kacheln, die nicht in der Geometriemaske ausgewählt wurden, werden als leer angesehen und ihre Texturierung wird daher nicht im abgeflachten Ergebnis beibehalten.

## Verwalten von reduziertem Inhalt

>[!NOTE]
>
> Reduzierte Bilder werden in der Projektdatei (.SPP) gespeichert. Das bedeutet, dass sie sich auf die Größe der Projektdatei auswirken.

Reduzierte Bilder werden automatisch mit dem Tag &quot;Reduziert&quot; versehen, sodass Sie im Bedienfeld &quot;Elemente&quot; einfach nach ihnen suchen können. Sie werden auch automatisch in der Kategorie &quot;Gespeicherte Suchen&quot; gespeichert.

### Nicht verwendete Bilder bereinigen

Wenn du nicht verwendete Bilder aus deiner Projektdatei entfernst, kannst du die Größe deines Projekts aufhellen. Im Bedienfeld &quot;Elemente&quot; können Sie Bilder aus dem Kontextmenü löschen. Zum Entfernen aller nicht verwendeten Bilder verwenden Sie <b>Datei > Nicht verwendete Ressourcen entfernen</b>. Beachten Sie, dass dadurch nicht nur reduzierte Bilder gelöscht werden, sondern auch alle Ressourcen, die nicht im Ebenenstapel, in gesicherten Karten-Slots oder an anderen Stellen in der Benutzeroberfläche verwendet werden.
