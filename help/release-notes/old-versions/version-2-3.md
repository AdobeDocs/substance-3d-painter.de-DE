---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/release-notes/old-versions/version-2-3.html"
breadcrumb-title: ''
description: Lesen Sie die Versionshinweise für Substance 3D Painter 2.3, um mehr über neue Funktionen, Verbesserungen und Fehlerbehebungen zu erfahren.
helpx_creative_field: ""
helpx_description: Painter > Release notes > Old versions > Version 2.3
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Version 2.3
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 0%

---


# Version 2.3

**Substance Painter 2.3** verbessert die Skript-API, um ihr erstes offizielles Plug-in zu veröffentlichen: einem Photoshop-Export mit dem vollständigen Ebenenstapel verfügbar.

Freigabedatum : *15. September 2016*

## Wichtigste Funktionen

### Neues Photoshop-Export-Plug-in

![](../../assets/ps-230.jpg)

Mit dieser Version haben wir uns darauf konzentriert, neue Möglichkeiten in der Skript-API hinzuzufügen, um **einen erweiterten Exporteur für Photoshop** zu implementieren. Um auf diesen neuen Export zuzugreifen, klicken Sie einfach auf das Photoshop-Symbol in der Hauptsymbolleiste (wenn das Plug-in aktiviert ist, was standardmäßig der Fall ist). Mit diesem Plug-in kannst du den gesamten Ebenen-Stapel aus einem Texturensatz exportieren und eine ähnliche Struktur innerhalb einer PSD-Datei erstellen. Für diese Funktion **muss Photoshop auf dem Computer installiert sein**, damit die PSD-Datei generiert werden kann.

Einige Optionen sind über die Schaltfläche &quot;Konfigurieren&quot; im Plug-in-Menü verfügbar:

![](../../assets/configure-ps.png)

## Tutorial

Unser neuestes Tutorial erklärt den Exportvorgang mit dem neuen Plug-in :

## Versionshinweise

### 2.3.1

(Release 7. Oktober 2016)

**Hinzugefügt:**

* [Plugin][Photoshop] Geben Sie an, welches Material/welcher Stapel/welche Kanäle exportiert werden sollen.
* [Scripting] Funktionsnamen weisen einige Inkonsistenzen auf.

**Fest:**

* [Exportieren] Alpha kann in benutzerdefinierten Exportvorgaben verworfen werden
* [Exportieren] Alpha erhält falsche Gamma-Konvertierung auf sRGB-Kanälen
* [Exportieren] Nicht quadratische Dokumente werden als quadratisch exportiert
* [Exportieren] Zusätzliche Karten können nicht exportiert werden, wenn eine fehlt
* [Iray] Einige Parameter (wie die emittierende Intensität) haben keine Auswirkungen
* [NVIDIA] Absturz beim Start mit NVIDIA Quadro K2200/GTX 750/760
* [AMD] Falscher Farbsatz für Miniaturen und Vorschauen
* [AMD] Einfrieren und Treiberfehler beim Öffnen neuer Dateien und Dateien
* [Log] &quot;software-version&quot; fehlt in der Protokolldatei

### 2.3.0

(Release 15. September 2016)

**Hinzugefügt:**

* [Zusatzmodul] Neues Zusatzmodul &quot;Nach Photoshop exportieren&quot; (vollständiger Ebenenstapel exportieren)
* [Exportieren] Geben Sie die Breite der Auffüllung an (in Pixel oder unendlich).
* [Exportieren] Festlegen des Hintergrundtyps außerhalb der UVs zulassen
* [Regal] Neuer Material-Ebenen-Shader zum Mischen von 10 Materialien
* [Shelf] Neuer Tonschattierer zur Anzeige von Details mit dem Height-/Normalkanal
* [Shelf] Neuer gebackener Lichtfilter mit Umgebungseingabe
* [Shelf] Einige Maskengeneratoren wurden aktualisiert, um nicht quadratische Transformationen hinzuzufügen.
* [Viewport] Hinzufügen einer zusammengesetzten Normalmap (Normal+Height+Backen) zum Solomodus
* [Skripterstellung] Exportieren zusätzlicher Maps zulassen
* [Skripterstellung] Verfügbare zusätzliche Karten pro Textursatz abfragen
* [Scripting] Kanalformat kann abgerufen werden.
* [Scripting] Fügen Sie Beispiele in der Backing-Dokumentation hinzu
* [Scripting] Ermöglicht das Abfragen der Sichtbarkeit einer Ebene.
* [Skripterstellung] Ermöglicht das Abfragen der Füllmethode und Deckkraft der Ebene
* [Skripterstellung] Exportieren konvertierter Maps (endgültige Normalmaps, gemischte AO usw.)
* [Substance] Benutzerdefinierte Verwendungen lesen und verbinden
* [Shortcuts] Zusatztaste (SHIFT) hinzufügen, um Solo-Modus rückwärts zu durchlaufen
* [Exportieren] Standardvorgabe für den Export wurde aktualisiert, um Alpha zu deaktivieren
* [UI] Miniaturen werden jetzt nur berechnet, wenn die Engine verfügbar ist
* [UI] Anzeigen einer Erwähnung bei der Berechnung von Miniaturansichten

**Fest:**

* Absturz mit einigen alten Projekten beim Öffnen
* Absturz mit beschädigtem Texturkanal-Cache
* Absturz beim Mischen von mehr als 4 Materialien mit dem Arbeitsablauf &quot;Materialebenen&quot;
* [UI] Tastenkombinationen funktionieren nicht, wenn die Symbolleiste ausgeblendet ist
* [UI] Die Iris-Symbolleiste ist im Menü &quot;Ansicht&quot; mit &quot;Unbenannt&quot; gekennzeichnet
* [UI] Plug-in-Symbolleisten werden im Menü &quot;Ansicht&quot; als &quot;Nicht geneigt&quot; bezeichnet
* [Baker] Durch Drücken der Eingabetaste beim Bearbeiten einer Backeinstellung wird der Backvorgang gestartet.
* [Baker] Falsche Bereiche für einige Parameter
* [Importieren] OBJ-Gitter können aufgrund sehr großer Zahlen nicht importiert werden.
* [Importieren] Einige OBJ-Dateien werden mit zu vielen Unterobjekten importiert
* [Export] Kanalhintergrund wird beim Export mit Schwarz anstelle der Standardfarbe gefüllt
* [Tool] Partikel funktionieren nicht ordnungsgemäß, wenn der FOV-Wert zu niedrig ist
* [Werkzeug] Die Pinselvorschaufarbe ist bei Masken in Unterstapeln falsch
* [Viewport] Wenn der Pinsel in leere Bereiche in der 2D-Ansicht geht, wird er gigantisch
* [Viewport] Leere Pinselvorschau beim Malen normaler Texturen
* [Skripterstellung] Falsche Dokumentation : &quot;ao&quot; anstelle von &quot;ambientocclusion&quot; aufgeführt
* [Skripterstellung] Der mit subprocess() begonnene Prozess wird beim Schließen von Painter beendet
* [Shelf] Gebackener Beleuchtungsfilter verwenden falsche AO-Eingabe
* [MacOS] Entferntes Fire Hydrant-Projekt (inkompatibel)
* Standardprojekt wird beim Laden einer \*.spt-Datei geöffnet (anstelle von \*.spp).
