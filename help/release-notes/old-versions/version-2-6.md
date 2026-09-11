---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/release-notes/old-versions/version-2-6.html"
breadcrumb-title: ''
description: Lesen Sie die Versionshinweise für Substance 3D Painter 2.6, um mehr über neue Funktionen, Verbesserungen und Fehlerbehebungen zu erfahren.
helpx_creative_field: ""
helpx_description: Painter > Release notes > Old versions > Version 2.6
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Version 2.6
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '1055'
ht-degree: 0%

---


# Version 2.6

Mit **Substance Painter 2.6** wollten wir eine Möglichkeit bieten, die Textursatz direkt im Substance Painter zu verwalten, ohne ein neues Projekt erstellen oder Ihren Mesh mit aktualisierten Material-Namen erneut importieren zu müssen. Wir wollten auch eine Möglichkeit bieten, die in Projekten verwendeten Ressourcen zu aktualisieren, was in der Vergangenheit oft gefordert wurde.

Freigabedatum: *27. April 2017*

## Wichtigste Funktionen

### Neues Beispielprojekt &quot;Meet Mat&quot;

![](../../assets/meetmat-render.jpg)

Dieses neue Beispielprojekt bietet ein neues glänzendes und liebenswertes Zeichen mit dem Namen &quot;**Mat**&quot;. Es enthält drei Textursätze, auf denen man malen kann.\
Nehmen Sie am **Meet Mat**-Wettbewerb teil, um einige wirklich coole Preise zu gewinnen: 2<https://www.allegorithmic.com/contest/meet-mat-2017-substance-3d-painting-contest>

### Neue Scripting-API mit der Möglichkeit, Ressourcen in Projekten zu aktualisieren

![](../../assets/resources-updater-ui.jpg)

Die Skripting-API von Substance Painter wurde verbessert, um neue Funktionen hinzuzufügen, mit denen **Ressourcen** im Projekt durch andere Versionen ersetzt werden können. Um diese neue Funktion zu demonstrieren, wurde ein neues **Plugin** hinzugefügt, das mit der Skript-API erstellt wurde und das Durchsuchen aller Ressourcen in einem bestimmten Projekt ermöglicht. Als rot markierte Ressourcen werden als &quot;veraltet&quot; erkannt und können automatisch ersetzt werden. Diese Funktion ist nicht auf &quot;veraltete&quot; Ressourcen beschränkt, sondern kann durch etwas Anderes ersetzt werden. Dies bietet eine Menge neuer Möglichkeiten und zeigt noch mehr, wie Substance Painter ein **nicht-destruktives Malwerkzeug ist** !

Das **Plug-in** ist auf GitHub verfügbar. Zögern Sie nicht, Ihnen zu helfen, wenn Sie potenzielle Verbesserungen sehen: 2<https://github.com/AllegorithmicSAS/painter-plugin-resources-updater>

![](../../assets/resource-update-demo.gif)

### Neue Möglichkeit zum Umbenennen und Neuzuweisen von Textursätzen

![](../../assets/texture-set-rename-description.png)

Es ist jetzt möglich, den Namen eines Textursatzes direkt im Substance Painter zu ändern. Das Umbenennen eines Textursatzes wirkt sich auf den Namen der Texturen aus, die auf die Festplatte exportiert werden (abhängig von der verwendeten Exportvorgabe).\
Um einen Textursatz umzubenennen, doppelklicken Sie einfach auf seinen Namen, um ihn zu ändern, oder öffnen Sie das Kontextmenü mit der rechten Maustaste. Es ist auch möglich, benutzerdefinierte Beschreibungen hinzuzufügen, um weitere Informationen darüber zu erhalten, was Textursatz tun. Dies kann sehr hilfreich sein, wenn Sie an einem [UDIM-Projekt &#x200B;](https://helpx.adobe.com/de/substance-3d/unlisted/documentation/spdoc/uv-tile-udim-legacy-144310352.html) arbeiten. Verwenden Sie die Schaltfläche &quot;**settings**&quot;, um die Anzeige von Beschreibungen in der Liste zu konfigurieren.

![](../../assets/reasign-texture-set.png)

Textursatz können jetzt verschiedenen Mesh-Materialien zugewiesen werden. Dies bedeutet, dass **Textursatz wiederherstellen**, die zuvor deaktiviert wurden (weil sie auf dem Mesh fehlten), oder sogar **austauschen** können. Klicken Sie einfach auf die neue Schaltfläche &quot;**settings**&quot; im Fenster &quot;Textursatz-Liste&quot; und klicken Sie auf den Eintrag &quot;**Textursatz neu zuweisen**&quot;. Es wird ein neues Fenster geöffnet, das sich mit der Verwaltung der Textursatz und der Art und Weise, wie sie mit den Mesh-Materialien verknüpft sind, befasst. Die Verwaltung kann durch **Ziehen und Ablegen** eines Textursatzes an der gewünschten Position erfolgen.

## Tutorial

Die wichtigsten neuen Funktionen werden in unserem neuesten Video-Tutorial erläutert:

## Versionshinweise

### 2.6.2

(Release 20. Oktober 2017)

**Hinzugefügt:**

* [Textursatz] Löschen deaktivierter Textursatz zulassen
* [Regal] Mehrere Benutzer können im selben Regal-Ordner schreiben
* [Scripting] Ordner &quot;Plug-ins&quot; neu laden können
* [Scripting] Fügen Sie eine erforderliche minimale API-Version in den Plug-in-Metadaten hinzu, um die Kompatibilität zu gewährleisten
* [Iray] Verbesserungen im Dialogfeld &quot;Bild exportieren&quot;

**Fest:**

* [Engine] Problem mit verschwundenen Strichen beim Ändern der Auflösung (4K>2K)
* [Baker] ID-Map-Baking schlägt fehl, wenn &quot;Nach Name abgleichen&quot; aktiviert ist
* [Baker] Fehlermeldungen sind nicht explizit genug.
* [3D-Ansicht] Tangente-Speicherplatz wird nicht mit Bakern synchronisiert
* [Werkzeug] Schwarze Artefakte bei Verwendung des Verwischen-Werkzeugs
* [Shader] Nicht-PBR-Shader funktioniert nicht mehr
* [Shader] &quot;pbr-coated&quot; ist gebrochen
* [Shader] Die Rauheit von &quot;pbr-beschichtetem&quot; Shader hat keine Auswirkungen mehr
* [Shader] Spec Gloss Shader stimmt nicht mit Iray und SD überein
* [Regal] Absturz beim Laden zweier Dateien mit demselben Namen, aber unterschiedlichen Dateinamenerweiterungen
* [Regal] Vorgabe kann in den Regale nicht mehr bearbeitet werden
* [Regal] Für im Regal importierte Elemente kann keine benutzerdefinierte Vorschau festgelegt werden
* Aus dem Cache geladene Ressourcen verlieren ihre Nutzung
* Beim Speichern eines Projekts vor dem Erstellen einer Vorlage werden Schreibberechtigungsfehler zurückgegeben.
* Falsches Speichern des Projekts, wenn Dateiname zwei Punkte enthält
* Importieren von Dateien mit mehreren Punkten (.) im Dateinamen führt zu Problemen

### 2.6.1

(Release 12. Mai 2017)

**Hinzugefügt:**

* [TextureSet] Weisen Sie Mesh-Materialien kein Objekt zu.

**Fest:**

* Absturz beim Wechseln von TextureSet nach dem Ersetzen von durch Baking erzeugte Map
* Absturz beim Rückgängigmachen und Wiederholen nach dem Ändern der Füllmethode der Ebene
* Absturz oder Einfrieren bei Verwendung des Effekts &quot;Farbauswahl&quot; mit großem ID-Map
* [Export] Umbenannte Textursatz werden im Exportfenster nicht alphabetisch sortiert.
* [TextureSet] Beim Zurücksetzen auf den Standardnamen wird keine Eindeutigkeit überprüft.
* [TextureSet] Umbenannter Textursatz wird nach dem erneuten Öffnen des Projekts deaktiviert
* [Regal] Fehlender Standardvorlageninhalt
* [Regal] Nicht quadratische Texturen werden als Quadrat angezeigt
* [Shader] Sobald ein Textursatz deaktiviert wurde, wird der zugehörige Shader zerstört.
* [Scripting] alg.Baking.setTextureSetBakingParameters() funktioniert nicht mehr
* [Scripting] Tippfehler in Websocket-Tutorial
* [Scripting] Verschiedene Probleme in AlgWidgets
* [Log] Falsche Erkennung des verfügbaren virtuellen Arbeitsspeichers in einigen Fällen

### 2.6.0

(Release 27. April 2017)

**Hinzugefügt** :

* Neues Beispielprojekt &quot;Meet Mat&quot; hinzufügen
* [Plug-In] Neues Plug-In &quot;Resources Updater&quot;
* [TextureSet] Ermöglicht das Umbenennen und Hinzufügen einer Beschreibung zu Textursätzen
* [TextureSet] Neuzuweisen von Materialien zulassen
* [TextureSet] Hinzufügen einer Einstellungsschaltfläche im Fenster &quot;Textursatz-Liste&quot;
* [TextureSet] &quot;Deaktivierte&quot; Textursatz am Ende der Liste anzeigen
* [Substance] Verwenden Sie bei der aktuellen Textursatz-Auflösung zusätzliche Maps, um die Leistung zu verbessern
* [Scripting] Aktualisieren einer Ressource, die in einem Projekt verwendet wird (Material, Generator usw.)
* [Scripting] Hinzufügen einer Möglichkeit zum Hinzufügen/Entfernen eines Regals
* [Scripting] Ermöglicht das Abfragen von Informationen aus einer Ressource in Projekten.
* [Skripterstellung] Liste der verfügbaren Shelfs abrufen
* [Scripting] Tutorial zur Verbesserung der AlgWidget-Miniaturansicht
* [Exportieren] Deaktivieren/Aktivieren der Bittiefe je nach Dateiformatunterstützung
* [Log] Plug-In-Namen zum Drucken in der Konsole hinzufügen
* [Protokoll] Fehler zu ausgeblendeten Textursätzen entfernen
* &quot;Begrüßungsbildschirm&quot; mit neuen Symbolen und Text für Beispiele aktualisieren

**Fest** :

* Absturz beim Aktualisieren eines Gitters in bestimmten Projekten
* [Viewport] Die innere Symmetrieebene ist nicht mehr sichtbar.
* [Viewport] Einige Nachbearbeitungseffekte sind aktiviert, wenn die Einzelansicht verwendet wird
* [Shaders] Überblendung mit &quot;\_premult&quot; funktioniert nicht richtig
* [Shaders] Warnung zum Alpha-Test mit dem Standard-Shader
* [Shelf] Falsches Analysieren von Tags aus Substance
* [Shelf] MatFX Rost Weathering funktioniert nicht richtig
* [Shelf] HSL-Filter ist standardmäßig für falsche Kanäle aktiviert
* [Shelf] Der Scharfzeichner ist standardmäßig für den Height-/Normalkanal aktiviert
* [Exportieren] Verschiedene Exportvorgaben verwenden keine OpenGL-Normalmap
* [Tool] Ungenauigkeitsprobleme mit dem Klonen-/Verwischen-Werkzeug erzeugen Artefakte
