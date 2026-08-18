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

Mit **Substance Painter 2.6** wollten wir eine Möglichkeit bieten, die Textursätze direkt in Substance Painter zu verwalten, ohne ein neues Projekt erstellen oder Ihr Gitter mit aktualisierten Materialnamen erneut importieren zu müssen. Wir wollten auch eine Möglichkeit bieten, die in Projekten verwendeten Ressourcen zu aktualisieren, was in der Vergangenheit oft gefordert wurde.

Freigabedatum: *27. April 2017*

## Wichtigste Funktionen

### Neues Beispielprojekt &quot;Meet Mat&quot;

![](../../assets/meetmat-render.jpg)

Dieses neue Beispielprojekt bietet ein neues glänzendes und liebenswertes Zeichen mit dem Namen &quot;**Mat**&quot;. Es enthält drei Textursets, auf denen gemalt werden kann.\
Nehmen Sie am **Meet Mat**-Wettbewerb teil, um einige wirklich coole Preise zu gewinnen: 2<https://www.allegorithmic.com/contest/meet-mat-2017-substance-3d-painting-contest>

### Neue Scripting-API mit der Möglichkeit, Ressourcen in Projekten zu aktualisieren

![](../../assets/resources-updater-ui.jpg)

Die Skripting-API von Substance Painter wurde verbessert, um neue Funktionen hinzuzufügen, mit denen **Ressourcen** im Projekt durch andere Versionen ersetzt werden können. Um diese neue Funktion zu demonstrieren, wurde ein neues **Plugin** hinzugefügt, das mit der Skript-API erstellt wurde und das Durchsuchen aller Ressourcen in einem bestimmten Projekt ermöglicht. Als rot markierte Ressourcen werden als &quot;veraltet&quot; erkannt und können automatisch ersetzt werden. Diese Funktion ist nicht auf &quot;veraltete&quot; Ressourcen beschränkt, sondern kann durch etwas Anderes ersetzt werden. Dies bietet eine Menge neuer Möglichkeiten und zeigt noch mehr, wie Substance Painter ein **nicht-destruktives Malwerkzeug ist** !

Das **Plug-in** ist auf GitHub verfügbar. Zögern Sie nicht, Ihnen zu helfen, wenn Sie potenzielle Verbesserungen sehen: 2<https://github.com/AllegorithmicSAS/painter-plugin-resources-updater>

![](../../assets/resource-update-demo.gif)

### Neue Möglichkeit zum Umbenennen und Neuzuweisen von Textursätzen

![](../../assets/texture-set-rename-description.png)

Es ist jetzt möglich, den Namen eines Textursatzes direkt im Substance Painter zu ändern. Das Umbenennen eines Textursatzes wirkt sich auf den Namen der Texturen aus, die auf der Festplatte exportiert werden (abhängig von der verwendeten Exportvorgabe).\
Um einen Textursatz umzubenennen, doppelklicken Sie einfach auf seinen Namen, um ihn zu ändern, oder öffnen Sie das Kontextmenü mit der rechten Maustaste. Es ist auch möglich, benutzerdefinierte Beschreibungen hinzuzufügen, um weitere Informationen darüber zu geben, was Textursätze tun. Dies kann sehr hilfreich sein, wenn Sie an einem [UDIM-Projekt](https://helpx.adobe.com/de/substance-3d/unlisted/documentation/spdoc/uv-tile-udim-legacy-144310352.html) arbeiten. Verwenden Sie die Schaltfläche &quot;**settings**&quot;, um die Anzeige von Beschreibungen in der Liste zu konfigurieren.

![](../../assets/reasign-texture-set.png)

Textursätze können nun unterschiedlichen Mesh-Materialien zugewiesen werden. Dies bedeutet, dass es möglich ist, **Textursätze wiederherzustellen**, die zuvor deaktiviert wurden (weil sie im Gitter fehlten), oder sie sogar **auszutauschen**. Klicken Sie einfach auf die neue Schaltfläche &quot;**Einstellungen**&quot; im Fenster Textursatzliste und klicken Sie auf den Eintrag &quot;**Textursätze neu zuweisen**&quot;. Es öffnet ein neues Fenster, in dem die Textursätze verwaltet werden und wie sie mit den Gittermaterialien verknüpft werden. Die Verwaltung kann durch **Ziehen und Ablegen** eines Texturensatznamens an die gewünschte Stelle erfolgen.

## Tutorial

Die wichtigsten neuen Funktionen werden in unserem neuesten Video-Tutorial erläutert:

## Versionshinweise

### 2.6.2

(Release 20. Oktober 2017)

**Hinzugefügt:**

* [Textursatz] Deaktivierte Textursätze können gelöscht werden
* [Shelf] Mehrere Benutzer können innerhalb desselben Shelf-Ordners schreiben
* [Scripting] Ordner &quot;Plug-ins&quot; neu laden können
* [Scripting] Fügen Sie eine erforderliche minimale API-Version in den Plug-in-Metadaten hinzu, um die Kompatibilität zu gewährleisten
* [IRay] Verbesserungen im Dialogfeld &quot;Bild exportieren&quot;

**Fest:**

* [Engine] Problem mit verschwindenden Strichen beim Ändern der Auflösung (4K>2K)
* [Bäcker] ID-Zuordnungssicherung schlägt fehl, wenn &quot;Mit Namen abgleichen&quot; aktiviert ist
* [Bäcker] Fehlermeldungen sind nicht explizit genug.
* [3D-Ansicht] Tangentialraum wird nicht mit Bäckereien synchronisiert
* [Werkzeug] Schwarze Artefakte bei Verwendung des Verwischen-Werkzeugs
* [Shader] Nicht-PBR-Shader funktioniert nicht mehr
* [Shader] &quot;pbr-coated&quot; is broken
* [Shader] Die Raueit des &quot;pbr-coated&quot; Shaders hat keine Auswirkungen mehr
* [Shader] Spec Gloss Shader stimmt nicht mit Iray und SD überein
* [Shelf] Absturz beim Laden von zwei Dateien mit demselben Namen, aber unterschiedlichen Erweiterungen
* [Shelf] Vorgabe kann in den Shelfs nicht mehr bearbeitet werden
* [Shelf] Es kann keine benutzerdefinierte Vorschau für in das Shelf importierte Elemente festgelegt werden.
* Aus dem Cache geladene Ressourcen verlieren ihre Nutzung
* Beim Speichern eines Projekts vor dem Erstellen einer Vorlage werden Schreibberechtigungsfehler zurückgegeben.
* Falsches Speichern des Projekts, wenn Dateiname zwei Punkte enthält
* Importieren von Dateien mit mehreren Punkten (.) im Dateinamen führt zu Problemen

### 2.6.1

(Release 12. Mai 2017)

**Hinzugefügt:**

* [TextureSet] Lassen Sie die Neuzuweisung von Gittermaterialien zu nichts zu

**Fest:**

* Absturz beim Wechseln von TextureSet nach dem Ersetzen von durch Baking erzeugte Map
* Absturz beim Rückgängigmachen und Wiederholen nach dem Ändern des Füllmodus der Ebene
* Absturz oder Einfrieren bei Verwendung des Effekts &quot;Farbauswahl&quot; mit großer ID-Map
* [Export] Umbenannte Textursätze werden im Exportfenster nicht alphabetisch sortiert
* [TextureSet] Beim Zurücksetzen auf den Standardnamen wird keine Eindeutigkeit überprüft.
* [TextureSet] Umbenannte Texturgruppe wird nach dem erneuten Öffnen des Projekts deaktiviert
* [Shelf] Fehlender Standardvorlageninhalt
* [Shelf] Nicht quadratische Texturen werden als Quadrat angezeigt
* [Shader] Wenn ein Textursatz deaktiviert wurde, wird der zugehörige Shader gelöscht.
* [Scripting] alg.baking.setTextureSetBakingParameters() funktioniert nicht mehr
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
* [TextureSet] Einstellungsschaltfläche im Fenster der Texturensatzliste hinzufügen
* [TextureSet] &quot;Deaktivierte&quot; Textursätze am Ende der Liste anzeigen
* [Substance] Verwenden Sie zusätzliche Maps bei der aktuellen Textursatzauflösung, um die Leistung zu verbessern
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
