---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/release-notes/old-versions/version-2-4.html"
breadcrumb-title: ''
description: Lesen Sie die Versionshinweise für Substance 3D Painter 2.4, um mehr über neue Funktionen, Verbesserungen und Fehlerbehebungen zu erfahren.
helpx_creative_field: ""
helpx_description: Painter > Release notes > Old versions > Version 2.4
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Version 2.4
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '631'
ht-degree: 0%

---


# Version 2.4

**Substance Painter 2.4** konzentriert sich auf die Verbesserung des Regal-Fensters sowie der Verwaltung von Ressourcen.

Freigabedatum : *27. Oktober 2016*

## Wichtigste Funktionen

### Neues Regal mit erweiterter Filterung

![](../../assets/new-shelf-240.jpg)

Das neue Regal-Fenster bietet eine **bessere Organisation** von Ressourcen neben **neuen Möglichkeiten zur Filterung von Inhalten**. Wir haben die Möglichkeit hinzugefügt, **benutzerdefinierte Vorgaben** zu erstellen, wobei jede Vorgabe über eigene Filterungen verfügt (sodass schnell zwischen verschiedenen Abfragen gewechselt werden kann). Diese Vorgaben können auch in ein neues Regal isoliert werden **, sodass** mehrere Ansichten **des Fensters möglich sind und nicht nur eine wie zuvor.** Die Filterungen bieten außerdem die Möglichkeit, **die Ordnerhierarchie auf der Festplatte zu durchsuchen**, was nützlich ist, wenn eine allgemeinere Abfrage verfeinert wird. Wir haben auch das **Kontextmenü** (beim Rechtsklick auf eine Ressource) verbessert, um **weitere nützliche Informationen** bereitzustellen.

Informationen zum Erstellen erweiterter Abfragen finden Sie im entsprechenden Teil der Dokumentation : [Erweiterte Suchabfragen](../../interface/assets/advanced-search-queries.md)

### Neues Importressourcenfenster

![](../../assets/import-window-240.png)

Mit der Nachbearbeitung des Regals **haben wir auch das Ressourcenimportfenster** verbessert. Das Fenster ist jetzt konsistenter und kann **auf drei verschiedene Arten aufgerufen werden** : über das Dateimenü, über die Schaltfläche im Regal-Fenster oder wie zuvor durch Ziehen und Ablegen einer Ressource in das Regal-Fenster. Mit dem neuen Fenster können **schnell die Verwendung** für **mehrere Ressourcen** gleichzeitig festlegen. Das bedeutet, dass Sie die Ressourcen nicht mehr zuerst an den richtigen Ort ziehen und ablegen müssen. Wir haben außerdem die Möglichkeit hinzugefügt, **einen benutzerdefinierten Pfad anzugeben**, um Unterordner zu erstellen, um die Vorteile der neuen Strukturansicht zu nutzen.

Weitere Informationen finden Sie im entsprechenden Teil der Dokumentation : [Ressourcen werden über das Importfenster hinzugefügt](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/adding-content-via-the-import-window-151584824.html)

### Neue Partikelvorgaben

![](../../assets/particle-240.png)

Die vorherige **Partikelvorgabe** wurde **überarbeitet**, um einsatzbereiter zu sein (insbesondere die **Regen**-Vorgabe). Wir haben diese Gelegenheit auch genutzt, um **neue Vorgaben** mit neuen Verhalten hinzuzufügen: Sehen Sie sich **Elektrische Schaltung, elektrische Leitungen, Rokoko und Adern klein** an!

## Tutorial

Die neuen Funktionen und die Verwendung von Regalen werden in unserem neuesten Tutorial beschrieben:

## Versionshinweise

### 2.4.1

(Release 28. Oktober 2016)

**Fest:**

* Absturz beim Erstellen eines Projekts mit einer Vorlage
* Absturz beim Schließen des Exportdialogfelds während eines Exports
* [Mac] Fehler beim Speichern des Projekts (Speichern der Exportvorgabe nicht möglich)
* [Regal] Beim Erstellen einer neuen Vorgabe wird diese zweimal angezeigt
* [Regal] Vorgaben können ohne Administratorrechte nicht im schreibgeschützten Modus geladen werden

### 2.4.0

(Release 27. Oktober 2016)

**Hinzugefügt:**

* [Regal] Neue Benutzeroberfläche zum Durchsuchen von Ressourcen (Strukturansicht, Filter usw.)
* [Regal] Speichern einer Suche als Vorgabe zulassen
* [Regal] Erstellen eines neuen Fensters aus einer Vorgabe zulassen
* [Regal] Neue Benutzeroberfläche für den Import von Ressourcen
* [Regal] Kopieren Sie kein standardmäßiges allegorisches Regal im Ordner &quot;Dokumente&quot;
* [Regal] Neue Partikeln-Vorgaben : Stromkreis, elektrische Leitungen, Rokoko, Kleinvenen
* [Regal] Verbesserte Vorgaben für ältere Partikeln, die einfacher zu verwenden sind (z. B. &quot;Rain&quot;)
* [Regal] Neue Informationen zum Kontextmenü der Ressource hinzufügen
* [Viewport] Verbessern der Leistung beim Laden von Umgebungs-Map
* [Viewport] Unterstützung für Umgebungs-Map hinzufügen, die nicht die Macht von zwei sind

**Fest:**

* Absturz beim Entfernen einer Maske
* Absturz beim Malen nach dem Speichern einer Vorgabe
* Absturz mit Umgebungsunschärfe bei einigen GPUs
* Absturz beim Zuweisen einer falschen Ressource zum Mini-Regal
* [Regal] Bereinigen + Speichern: Entfernen Sie Tags und Metadaten für Ressourcen im Projekt.
* [Regal] Beim Importieren einer Vorgabe werden die Ressourcen im Regal angezeigt
* [Exportieren] Normalen-Map, die aus dem Height-Kanal generiert wird, hat eine geringe Intensität.
* [Exportieren] Normal aus Mesh ist in der endgültigen Normalen-Map nicht immer vorhanden
* [Exportieren] Ausdehnung mit Transparenz kann manchmal ohne Transparenz erfolgen
* [Scripting] &quot;alg.plugin\_root\_directory&quot; kann einen abgeschnittenen Netzwerkpfad zurückgeben
* [TextureSet] Sperrschaltfläche ist aktiviert, wenn nicht quadratische Projekte erneut geöffnet werden
