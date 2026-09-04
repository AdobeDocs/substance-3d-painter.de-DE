---
helpx_url: 'https://helpx.adobe.com/substance-3d-painter/release-notes/all-changes.html'
breadcrumb-title: ''
description: Prüfe alle Änderungen und Updates in den verschiedenen Substance 3D Painter-Versionen, um den Funktionsverlauf und Verbesserungen im Laufe der Zeit nachzuverfolgen.
helpx_creative_field: ''
helpx_description: Painter > Release notes > All Changes
helpx_experience_level: ''
helpx_learn_topic: ''
helpx_tags: ''
title: Alle Änderungen
user-guide-description: ''
user-guide-title: ''
hold: false
source-git-commit: fc154cd38e23b0e598c15bfbfee8a263d5770592
workflow-type: tm+mt
source-wordcount: '34015'
ht-degree: 0%

---


# Alle Änderungen

Diese Seite enthält Versionshinweise für alle früheren Versionen von Substance 3D Painter, sortiert nach aktuellster bis ältester Version.

>[!NOTE]
>
> Informationen zum Anzeigen bekannter Probleme, die sich auf Painter auswirken können, finden Sie auf der [Seite zur dedizierten Dokumentation](known-issues.md).

## Version 12

### 12.1.4

Freigabedatum: **2026/09/04**

Zusammenfassung: **Nebenversion**

**Fest:**

- \[Absturz\] Absturz beim Importieren oder Exportieren von Dateien, deren Dateinamen Nicht-ASCII-Zeichen enthalten

### 12.1.3

Freigabedatum: **2026/08/26**

Zusammenfassung: **Nebenversion**

**Hinzugefügt:**

&#x200B;* Substance Engine auf Version 9.4.6 aktualisieren

**Fest:**

&#x200B;* [Graustufenwähler] Die Auswahl bleibt nach dem Ändern des Tools geöffnet
&#x200B;* [Baking verzerren] Verzerrungskorrektur wird beim Malen und Rückgängigmachen unterbrochen
&#x200B;* Die Interaktion mit dem [Projektion-Tool]-Viewport wird vom Projektion-Tool blockiert.
&#x200B;* [Dynamische Kontur] Fehlende dynamische Konturparameter in den Pinseleigenschaften
&#x200B;* Export in ein Netzwerk funktioniert nicht mehr

### 12.1.2

Freigabedatum: **2026/08/03**

Zusammenfassung: **Nebenversion**

**Fest:**

&#x200B;* \[Absturz\] Einige Substance können beim Rendern zu einem Absturz führen
&#x200B;* \[Absturz\] Mesh beim Baking erneut importieren
&#x200B;* \[Absturz\] Fehler beim Initialisieren der Grafikanzeige kann zu einem Absturz führen.
&#x200B;* \[Absturz\] Exportieren von Texturen kann in einigen Fällen abstürzen, während das Protokoll aktualisiert wird
&#x200B;* \[Absturz\] Absturz im Backing-Modus in einigen Fällen beim Laden/Aktualisieren der Umgebungszuordnung
&#x200B;* \[Backen\] Das erneute Starten des Backens nach dem Ändern einer hohen Poly-Datei kann zu einem Einfrieren führen
&#x200B;* \[An Photoshop senden\] Fehler beim Exportieren der Ebenenmaske
&#x200B;* \[Engine\] Das Ergebnis des Ankerpunkts wird nicht zwischen einer Maske und einem Farbkanal gerendert

### 12.1.1

Freigabedatum: <b>2026/07/09</b>

Zusammenfassung: Nebenversion

Hinzugefügt:

&#x200B;* [Skew-Baking] Gelegt: Normaler Neigungsbasismodus: Mesh oder pro Dreieck
&#x200B;* [Eigenschaften] einheitliche Farben immer auf den Standardwert ihres Kanals zurücksetzen lassen
&#x200B;* [OpenPBR] Kanäle nach Kategorien im Fenster &quot;Texturen exportieren&quot; für die Erstellung von Ausgabevorlagen neu gruppieren
&#x200B;* Substance Engine auf Version 9.4.5 aktualisieren

Fest:

&#x200B;* [Projekt] Das Öffnen und Speichern einiger Projekte kann länger als gewöhnlich dauern
&#x200B;* [Absturz] Das erneute Laden mehrerer Meshes kann zu einem Absturz führen
&#x200B;* [Absturz] Das Löschen eines Kanals im Maskenansichtsmodus führt zu einem Absturz
&#x200B;* [Absturz] Einige Substance können beim Rendern zu einem Absturz führen
&#x200B;* [Neigung malen] Das ausgewählte Werkzeug in der Neigung bleibt nach dem Wechsel in den Malmodus ausgewählt
&#x200B;* [Allgemeine Einstellungen sichern] Einstellungen für die Käfigentfernung aktualisieren die Drahtgitter- und Shader-Visualisierung für Käfige nicht
&#x200B;* [Engine] UV-Auffüllmodus &quot;3D Space Neighbor&quot; funktioniert nicht gut bei dünnen Dreiecken
&#x200B;* Das Ergebnis des [Engine]-Ankerpunkts wird nicht zwischen einer Maske und einem Farbkanal gerendert

### 12.1.0

Freigabedatum: <b>2026/06/23</b>

Zusammenfassung: <b>Dieses Update ist eine Hauptversion. Es enthält Verbesserungen an Bakern mit dem Standardzustand &quot;Neues Baking&quot;, der Zeichnungs-Skew-Map, dem automatischen Reake, einer neuen Option für den automatischen entpack von UV für Mesh und OpenPBR mit fester Oberfläche. Weitere Informationen finden Sie in den vollständigen Versionshinweisen.</b>

<b>Hinzugefügt</b>:

&#x200B;* [Baking Neigen] Malwerkzeuge Neigen
&#x200B;* [Skew Baking] Hinzufügen von Skew Preview Shader und Skew Direction Vektorgrafiken beim Malen von Skew Map
&#x200B;* [Skew-Backing] Option &quot;Kantenschutz hinzufügen&quot;
&#x200B;* [Backen mit Neigung] Automatische Wiederherstellung
&#x200B;* [Skew Backing] Benutzeroberfläche der Gitterzuordnungs-Liste überarbeiten
&#x200B;* [Skew Baking] Gitterzuordnung teilen/Allgemeine Backeinstellungen + Allgemeine Einstellungen aus Gitterzuordnungsliste verschieben (nur Grundfarbe oder Maske)
&#x200B;* [Skew Backing] Symbolleistenschaltflächen für Ansichtsfenster ändern
&#x200B;* [Schrägbacken] Symmetrie-Schalter für Pinsel in der oberen Symbolleiste anzeigen
&#x200B;* [Skew Backing] Umbenennungsoptionen im Menü &quot;Listensynchronisation&quot; der Gitterzuordnung
&#x200B;* [Skew Backing] Dialogfelder &quot;Synchronisation aktualisieren&quot; und &quot;Überwachter Status&quot;
&#x200B;* [Backen mit Neigung] Erstellen einer Graustufen-Farbwählervariante
&#x200B;* [Skew Backing] Symbol für Aktualisierungsbackmodus
&#x200B;* [Automatisch entpacken] Option &quot;Harte Oberfläche integrieren&quot;
&#x200B;* [OpenPBR] Unterstützung für OpenPBR 1.1 hinzufügen
&#x200B;* [OpenPBR] OpenPBR zum Standard-Workflow und -Shader machen
&#x200B;* [OpenPBR] Importieren von OpenPBR-Materialien und -Texturen über USD
&#x200B;* [OpenPBR] Exportieren von OpenPBR-Materialien und -Texturen über USD
&#x200B;* [OpenPBR] Fenster &quot;Export Textures&quot; aktualisieren, um die OpenPBR-Benennungskonvention anzuzeigen
&#x200B;* [OpenPBR] Hinzufügen von Dokumentationen zu Änderungen an der Support-OpenPBR
&#x200B;* [OpenPBR]&#x200B;[Iray] Fügen Sie eine neue MDL hinzu, um OpenPBR 1.1 in Iray zu unterstützen
&#x200B;* Mehrere geringfügige Verbesserungen bei den USD-Exporten
&#x200B;* [UI] Fügen Sie eine Warnung im Viewport hinzu, wenn Sie versuchen, auf einem anderen Textursatz zu malen
&#x200B;* [Reduzieren] Reduzieren aller instanzierten Ebenen über Textursätze hinweg zulassen
&#x200B;* [Einstellungen für Textursatz] Mehrere Kanäle gleichzeitig über ein neues Fenster auswählen
&#x200B;* [Verlauf] &quot;Wert&quot; aktualisieren Eintragsformulierung rückgängig machen, um den Parameternamen wiederzugeben
&#x200B;* [Ebenenstapel] Fülleffekte in Masken standardmäßig auf Weiß einstellen (1.0)
&#x200B;* [Substance] Neue &quot;mesh_hard_edges_triangle&quot;-Engine-Zuordnungseingabe hinzufügen
&#x200B;* [Substance] Neue Eingabe für die Engine &quot;mesh_hard_edges&quot; hinzufügen
&#x200B;* [Shader] Verhindern, dass Shader-Instanzen dieselben Namen haben
&#x200B;* [Shader] Verwenden Sie den Shader aus der Projektvorlage beim Importieren einer USD- oder GLTF-Datei.
&#x200B;* Adobe Color Engine auf Version 7.0 aktualisieren
&#x200B;* Aktualisieren der MacOSX-Mindestversion auf 13.0 (Ventura)
&#x200B;* [Inhalt] Neue Projektvorlagen für OpenPBR
&#x200B;* [Inhalt] Aktualisieren von Beispielprojekten, um den neuen OpenPBR Shader zu verwenden
&#x200B;* [Python] Erweitern Sie die Geometrie-Masken-API, um Einschluss- und Ausschlussmodi wie in der Benutzeroberfläche zu ermöglichen.

<b>Fest</b>:

&#x200B;* [Absturz]&#x200B;[Einstellungen für Gitterzuordnungen] Anwenden von Einstellungen auf andere Textursätze
&#x200B;* [Absturz] Wenn die Krümmung von der Karte ohne den Weltraum normal gebacken wird
&#x200B;* [Absturz]&#x200B;[Backen] Backen mit aktiviertem benutzerdefiniertem Käfig, aber ohne Dateiauswahl stürzt ab
&#x200B;* [Absturz] Abbrechen des AO-Backens
&#x200B;* [Auto-Cage] Unendliche Belastung, wenn der hohe Poly-Dateipfad ungültig ist
&#x200B;* [Linux]&#x200B;[Windows] Der Farbwähler kann manchmal ganz schwarz sein oder nicht angezeigt werden.
&#x200B;* [Polygon-Füllwerkzeug] Das Werkzeug funktioniert nicht mit Nicht-PBR
&#x200B;* &lbrack;[Malen] Löschen des Kanals für die Grundfarbe löscht keine zuvor gemalte Farbe
&#x200B;* [USD] Shader-Instanzen werden nicht alle korrekt erkannt.
&#x200B;* [Substance] Es wird nur die erste Verwendung eines Eingabe-/Ausgabeknotens berücksichtigt
&#x200B;* [Shader] Umgebungsbelichtung wird zweimal mit Textur-Sets unter Verwendung verschiedener Mischmethoden angewendet.
&#x200B;* [Engine] Normale Texturen mit leerem blauen Kanal (schwarz) können zu falschen Angleichungsergebnissen führen
&#x200B;* [GLTF Import] Alpha-Überblendung ist für jeden Textursatz aktiviert
&#x200B;* [GLTF-Export] Die Alpha-Füllmethode ist beim Export immer aktiviert
&#x200B;* [Export] Doppelseitige Geometrie ist beim Importieren einer GLTF-Datei immer deaktiviert
&#x200B;* [Javascript] Das Ändern von Shader-Einstellungen trägt nicht zum Rückgängigmachen des Verlaufs bei
&#x200B;* [Samples] Die Volumenstreuung ist in den Anzeigeeinstellungen für die Meet Mat nicht aktiviert.

### 12.0.3

Freigabedatum: **2026/05/05**

Zusammenfassung: **Nebenversion**

**Hinzugefügt:**

&#x200B;* Update Baker auf Version 3.22.2
&#x200B;* Aktualisieren der Substance-Engine auf Version 9.4.3
&#x200B;* \[Python\] Speichern Sie ein intelligentes Material an einem bestimmten Speicherort

**Fest:**

&#x200B;* \[Ubuntu\] Absturz beim Auswählen von Material
&#x200B;* \[Mac\] Wiederkehrendes Popupfenster fordert den Zugriff auf Daten anderer Anwendungen an
&#x200B;* \[Backen\] Artefakte können auf der Krümmungskarte angezeigt werden.
&#x200B;* \[Backen\] Das Backen ist in einigen Fällen langsamer
&#x200B;* \[Verformen zu Geometrie\] Verformen zu Geometrie wird in einigen Fällen deaktiviert
&#x200B;* \[UV-Kachel\] Alpha des extrahierten Ankerpunkts wird von anderen Kacheln ignoriert
&#x200B;* \[Python\]\[Mac\] Ausnahmen in der Python-Konsole mit SSL
&#x200B;* \[Python\] Painter stürzt beim Beenden mit Qt-Widgets ab

### 12.0.2

Freigabedatum: **2026/04/07**

Zusammenfassung: **Nebenversion**

**Hinzugefügt:**

&#x200B;* [Farbmanagement] Fügen Sie ein neues OCIO hinzu, um den Standardfarbraum des Farbwählers anzugeben.
&#x200B;* [Python] Stellen Sie die Einstellungen für das automatische Ausgliedern in der Python-API bereit.

**Fest:**

&#x200B;* [Absturz] Das Speichern mit zu wenig Speicherplatz kann zu einem Absturz oder einer Beschädigung von Projekten führen
&#x200B;* [Absturz] [Menüband] Verwenden des Menübands kann zu Abstürzen bei einigen Projekten führen
&#x200B;* [Absturz] [Backen] Absturz, wenn .assbin-Datei nicht in den Ordner geschrieben werden kann
&#x200B;* [Import] OBJ-Gitter aus Stager können bei der Projekterstellung fehlschlagen
&#x200B;* [Import] OBJ hat in einigen Fällen ein fehlendes Gesicht
&#x200B;* [Import] USD-Gitter ohne zugewiesenes Material können beim Import abstürzen
&#x200B;* [Ausgefüllter Pfad] Nicht von Symmetrie betroffen
&#x200B;* [Schablone] Die Vorschau hat eine geringere Auflösung als das gemalte Ergebnis
&#x200B;* [UI] &quot;uv island&quot; wird weiterhin in der QuickInfo zur ID-Map-Farbquelle erwähnt
&#x200B;* [Anzeige] Schatten erscheinen invertiert
&#x200B;* [Viewport] Transformation der Verkrümmungsprojektion bleibt nach dem Wechsel in den Backmodus erhalten
&#x200B;* [Verkrümmen] Raster verschwindet, wenn die Skalierung auf der Z-Achse auf 0 eingestellt ist und &quot;Auf Geometrie verkrümmen&quot; aktiviert ist
&#x200B;* [Python] Unerwarteter Fehler beim Hinzufügen eines Kanals mit umfangreichen Änderungen

### 12.0.1

Freigabedatum: **2026/03/18**

Zusammenfassung: **Nebenversion**

**Fest:**

&#x200B;* \[Absturz\]\[Einfrieren\] Export aus bestimmten Projekten

### 12.0.0

Freigabedatum: <b>2026/03/09</b>
Zusammenfassung: <b>Dies ist eine Hauptversion. Diese Version enthält die Funktionen zum Reduzieren von Ebenen, Verformen auf Geometrie, neue Post-Effekte, Verbesserung des neuen Projektfensters und andere Verbesserungen.</b>

<b>Hinzugefügt</b>:

&#x200B;* [Ebenen reduzieren] Ebenen innerhalb des Ebenenstapels reduzieren
&#x200B;* [Ebenen reduzieren] Exportieren reduzierter Ebenen auf die Festplatte
&#x200B;* [Verformen zu Geometrie] Hinzufügen neuer automatischer Verkrümmungsfunktionen zu Verkrümmen-Projektionen
&#x200B;* [Post-Effekte] Ersetzen Sie Post-Effekte durch neue
&#x200B;* [Post-Effects] Aktualisieren der Tonzuordnung
&#x200B;* [Post-Effects] Neue Verwendung für Post-Effects-Assets hinzufügen
&#x200B;* [Inhalt]&#x200B;[Nacheffekte] Integrieren von Standard-Nacheffekt-Assets in die Bibliothek
&#x200B;* [Neues Projekt] Verbessern der Benutzeroberfläche für die Projekterstellung
&#x200B;* [Neues Projekt] Änderungen an der Funktion zum erneuten Importieren des Gitters
&#x200B;* [Neues Projekt] Öffnen von \*.geo.usd-Dateien zulassen
&#x200B;* [Projektkonfiguration] Verbessern der Benutzeroberfläche für die Projektkonfiguration
&#x200B;* Aktualisieren der USD-Bibliothek auf Version 25.05
&#x200B;* Substance Engine auf Version 9.3.4 aktualisieren
&#x200B;* Erhöhen der Mindesttreiber auf 25.3.1/25.Q2 für AMD-GPUs
&#x200B;* Update Qt auf 6.8.6
&#x200B;* [Scripting] JavaScript-API auf Version 1.1.20 aktualisieren
&#x200B;* Aktualisieren von Python auf 3.13

<b>Fest:</b>

&#x200B;* [Absturz] Das Ändern der Materialkanalausgabe in einer Maske kann abstürzen
&#x200B;* [Import] EXR-Texturen werden beim Importieren von USD-Dateien in sRGB anstelle von linear erzwungen
&#x200B;* [UV-Kacheln] Bildsequenz mit einem einzelnen Bild füllt auch andere UV-Kacheln
&#x200B;* [Backen] AO unterscheidet sich zwischen CPU- und GPU-Backen
&#x200B;* [Farbmanagement]&#x200B;[MacOS] Viewport BaseColor stimmt nicht mit dem Farbwähler überein
&#x200B;* [USD] Einheitliche Werte werden in einigen Fällen nicht importiert

## Version 11

### 11.1.3

Freigabedatum: <b>2026/02/12</b>
Zusammenfassung: <b>Nebenversion</b>

<b>Fest</b>:

&#x200B;* [Malen] Schablone und Symmetrie funktionieren in einigen Fällen nicht
&#x200B;* [Pfad] Keine Aktualisierung beim Ändern des Deckkraftreglers für Verwischungsstrich
&#x200B;* [Projekt] Auf einer Geometrie kann nicht gemalt werden.
&#x200B;* [Menüband] Instantiierter Pfad verschwindet, wenn die Auflösung des Textursatzes geändert wird
&#x200B;* [UI] Farbwähler kann in einigen Fällen schrumpfen und verschwinden

### 11.1.2

Freigabedatum: <b>2026/01/13</b>
Zusammenfassung: <b>Nebenversion</b>

<b>Hinzugefügt</b>:

&#x200B;* [Backen] Verbessern der Backzeit für UV-Kacheln-Projekt mit asynchroner Speicherung
&#x200B;* [Shaders] Erwähnung in Shader-API Changelog ändert sich nach Vulkan migration
&#x200B;* Update OpenEXR auf Version 3.4.4

<b>Fest</b>:

&#x200B;* [Absturz] Absturz beim Start der Nvidia GTX 10xx-Serie
&#x200B;* [Absturz] Die Verwendung des Farbwählers auf verschiedenen Textursätzen kann beim Beenden der Anwendung zu einem Absturz führen
&#x200B;* [Leistung] Leistungsproblem beim Malen im Projekt mit vielen Ebenen
&#x200B;* [Leistung] Verzögerung beim Malen mit dem Grafiktablett-Stift
&#x200B;* [UI] Kameraeinstellungen bleiben im Rendermodus deaktiviert (Iray)
&#x200B;* [Menüband] Pfad kann sich in einigen Fällen nach einer Ecke unerwartet überlappen
&#x200B;* [Menüband] Leistungsproblem mit UV-Kacheln
&#x200B;* [Substance]&#x200B;[UI] Bildeingaben verschwinden, wenn sie ausgeblendet werden
&#x200B;* [Substance]&#x200B;[UI] Verschachtelte Gruppen können auch dann erhalten bleiben, wenn &quot;Sichtbar&quot; sie ausblendet.
&#x200B;* [Backen]&#x200B;[UI] Der Krümmungs-Sampling-Radius kann nicht über 0,01 hinaus festgelegt werden
&#x200B;* [Backen]&#x200B;[Benutzeroberfläche] Die maximale Okklusionsentfernung kann nicht auf mehr als 1 festgelegt werden.
&#x200B;* [Backen] Die AO-Einstellung &quot;Selbstverdeckung&quot; wird bei mehreren Textursätzen ignoriert, bei &quot;Niedrig&quot; ist der Backvorgang hoch.
&#x200B;* [Backen] ID-Map backt keine Scheitelpunktfarben von FBX im Modus &quot;Niedrig bis Hoch&quot;
&#x200B;* [Inhalt] Hochpassfilter führt zu ausgewaschenen Farben in farbverwalteten Kanälen

### 11.1.1

Freigabedatum: <b>2025/12/09</b>
Zusammenfassung: <b>Nebenversion</b>

<b>Hinzugefügt</b>:

&#x200B;* [Leistung] Verbessern der Leistung von UV-Kacheln beim Berechnen von Teiltexturen
&#x200B;* [Bakers] Update auf Version 3.15.4

<b>Fest</b>:

&#x200B;* [Absturz]&#x200B;[MacOS] Speichern eines Projekts aus einer früheren Version stürzt immer ab
&#x200B;* [Absturz] Das Schließen eines Projekts kann manchmal zu einem Absturz führen
&#x200B;* [Project] Fehler &quot;Die Mitgliederanzahl stimmt nicht überein&quot; beim Öffnen des in der vorherigen Version erstellten Projekts.
&#x200B;* [Backen] UV-Kacheln werden nicht mit vorherigen Backergebnissen kombiniert, sofern vorhanden
&#x200B;* [Backen] Gerät verloren, auch wenn Raytracing auf Nvidia GTX 10XX deaktiviert ist
&#x200B;* [Backen] AO mit Normal weist an Kanten Artefakte auf, da keine Auffüllung erfolgt.
&#x200B;* [Backen] Die AO-Einstellung &quot;Selbstverdeckung&quot; wird ignoriert, wenn mehrere Textursätze und &quot;Namensübereinstimmung&quot; aktiviert sind
&#x200B;* [Backen] ID-Map ist vollständig schwarz, wenn hohe Poly-Meshes keine Scheitelpunktfarben aufweisen.
&#x200B;* [Menüband] QuickInfo für den Alpha-Mischmodus nennt den Bildschirm-Mischmodus anstelle des linearen Abwedlers
&#x200B;* [Pfad] Tangenten erzeugen eine unerwartete Schleife, wenn der Punkt eng an die Pfadenden verschoben wird
&#x200B;* [Werkzeug] Die Materialvorschau funktioniert nicht, wenn die Projektion in einer Maske verwendet wird
&#x200B;* [Engine] Das Malen kleiner Pinselstriche kann zu blockartigen Artefakten führen
&#x200B;* [Shader] Beim Rückgängigmachen der Erstellung der Shader-Instanz wird diese nicht ordnungsgemäß entfernt.
&#x200B;* [Exportieren] Der Alpha-Modus für den GLTF-Export ist immer auf MASK festgelegt.
&#x200B;* [Python] Unerwarteter Fehler beim Bearbeiten des Ebenenstapels außerhalb des umfangreichen Änderungsblocks

<b>Bekannte Probleme</b>:

&#x200B;* [Menüband] Leistungsproblem mit UV-Kacheln
&#x200B;* [Menüband] Pfad kann sich in einigen Fällen nach einer Ecke unerwartet überlappen
&#x200B;* [Absturz]&#x200B;[Menüband] Erstellen sehr langer Texte in Menüband kann abstürzen
&#x200B;* [Farbmanagement] HDR-Farbraumkonvertierungen mit ACE unter Linux erzeugen festgeklemmte Farben
&#x200B;* [Regression]&#x200B;[UI] Kontextmenü auf HD-Bildschirmen ist zu klein
&#x200B;* [Crash]&#x200B;[Python] USD-Export, ausgelöst durch TextureStateEvent
&#x200B;* [Engine] Malen mit dem Kopierwerkzeug in normalen Kanalverschiebungsfarben falsch
&#x200B;* [Python] Das Ghost-Widget wird durch das noch funktionierende Skript gelöscht.

### 11.1.0

Freigabedatum: <b>2025/11/18</b>
Zusammenfassung: <b>Dieses Update ist eine Hauptversion. Es enthält das neue Tool für die Multifunktionsleiste mit eigenem neuen Inhalt, Unterstützung der Symmetrie für Füllebenen, Leistungsparameter für Versatz, verbesserte Physische Größe durch die aktualisierten Baker, vollständige Vulkan-Unterstützung für Windows und Linux und weitere Verbesserungen.</b>

<b>Hinzugefügt</b>:

&#x200B;* Neues Bandwerkzeug
&#x200B;* [Tool] Neues Werkzeug für die Multifunktionsleiste hinzufügen, um nahtlose Pfade zu erstellen
&#x200B;* [Menüband] Tastenkombinationen für die Menübandvorgabe im Eigenschaftenfenster hinzufügen
&#x200B;* [Menüband] Ermöglicht das Ändern der Deckkraft des Menübands pro Scheitelpunkt des Pfads.
&#x200B;* [Menüband] Ermöglicht das Ändern der Größe des Menübands pro Scheitelpunkt des Pfades.
&#x200B;* [Menüband] Entfernen von Anfang/Ende, definiert auf einer Substance, wenn Pfade geschlossen sind
&#x200B;* [Menüband] Entfernen der Pfad-/Materialvorschau im Eigenschaftenfenster für Pfade-Werkzeuge zum Malen, Radieren und Verwischen
&#x200B;* [Menüband] Hinzufügen von Füllmethoden für Alpha und einige Kanäle bei selbstüberlappender Anordnung
&#x200B;* Symmetrie füllen
&#x200B;* [Füllen] Unterstützung für Symmetrie auf Füllebenen und Effekten hinzufügen
&#x200B;* [Füllung]&#x200B;[UI] Belichten von Symmetrie-Einstellungen im Eigenschaftenfenster für Füllebene und Effekte
&#x200B;* [Fill] Benutzeroberfläche für Einstellungen für &quot;Symmetrie nachbearbeiten&quot; im Menü &quot;Viewport&quot; und im Eigenschaftenfenster
&#x200B;* [Füllen] Ordentliche Texturen bei Projektion im Verkrümmungsmodus korrekt neu ausrichten
&#x200B;* Physische Größe Versatz
&#x200B;* [Versatz] Physische Größe als Versatz verwenden
&#x200B;* Leistungssteigerung
&#x200B;* [Leistung] Verbessern der Darstellung kleiner Pinselstriche auf großen Dreiecken
&#x200B;* [Performance] Verbessern der Shader-Kompilierungszeit
&#x200B;* [Performance] Volle Vulkan-Unterstützung für Windows und Linux
&#x200B;* [Leistung] Aktualisierte Baker mit schnellerem GPU-Rendering und Unterstützung von AMD-Raytracing
&#x200B;* [UI] Ordnen Sie Werkzeugeigenschaften neu in Gruppen an und reduzieren Sie einige standardmäßig
&#x200B;* [Engine] Update-Substance Engine auf Version 9.2.5
&#x200B;* [Substance] Außerkraftsetzung der Auflösung für Substance-Ressourcen in Tools und Füllungen
&#x200B;* [Exportieren] Aktualisieren der Exportvoreinstellung für Mesh Maps zum Exportieren von Graustufen-Texturen
&#x200B;* Python
&#x200B;* [Backen]&#x200B;[Python] Anzeige in Änderungslog-Umbruchänderungen nach Aktualisierung des Bäckers
&#x200B;* [Python] Verfügbarmachen von Einstellungen für Füllsymmetrie in Python
&#x200B;* Content und neue Inhalte.
&#x200B;* [Inhalt] Hinzufügen von 75 neuen Werkzeugvorgaben für das Menüband-Werkzeug
&#x200B;* [Inhalt] Aktualisieren der Verlaufsgenerator-Ressource, um mit dem Menüband kompatibel zu sein

<b>Fest</b>:

&#x200B;* [Absturz] Das Laden eines anderen Projekts, während die Pfadausrichtung aktiviert ist, kann abstürzen
&#x200B;* [Absturz] Ein Rechtsklick im Pfadfenster mit Informationen aus einer anderen Sitzung in der Zwischenablage kann abstürzen
&#x200B;* [UI] Die Benutzeroberfläche scrollt in den Werkzeugeigenschaften nach oben, wenn ein Pfad erstellt wird
&#x200B;* [UI] Maus-Cursor verschwindet, wenn die Pfadansichtsport-Visualisierung ausgeblendet ist
&#x200B;* [Pfad] Das Kopieren/Einfügen verschiedener Werkzeugeigenschaften im Bedienfeld &quot;Pfad&quot; führt zu instabilen Eigenschaften
&#x200B;* [Werkzeug] Radierer- und Verwischen-Werkzeugvorgaben aktualisieren nicht immer die Kanalauswahl
&#x200B;* [Tool] Gemalter Wert ist grau, aber Benutzeroberfläche zeigt Weiß nach dem Laden der farbigen Werkzeugvorgabe in der Maske an
&#x200B;* [Tool] Die aus der Maske erstellte Voreinstellung behält Kanalwerte bei, die aus einer anderen Voreinstellung geladen wurden
&#x200B;* [Substance] Die im Diagramm definierte normale Farbraumübersteuerung wird nicht berücksichtigt
&#x200B;* [Inhalt] Die Standard-Pinselformressource verwendet eine veraltete Substance.

<b>Bekannte Probleme</b>:

&#x200B;* Der Verlauf der Shader-Instanz wurde nicht ordnungsgemäß verfolgt
&#x200B;* [Menüband] Leistungsproblem mit UV-Kacheln
&#x200B;* [Menüband] Pfad kann sich in einigen Fällen nach einer Ecke unerwartet überlappen
&#x200B;* [Menüband] Tangenten erzeugen eine unerwünschte Schleife, wenn der Punkt eng an die Pfadenden verschoben wird
&#x200B;* [Absturz]&#x200B;[Menüband] Erstellen sehr langer Texte in Menüband kann abstürzen
&#x200B;* [Werkzeug] Die Materialvorschau funktioniert nicht, wenn die Projektion in einer Maske verwendet wird
&#x200B;* [Backen] Die AO-Einstellung &quot;Selbstverdeckung&quot; wird bei mehreren Textursätzen ignoriert und &quot;Namensübereinstimmung&quot; ist aktiviert.
&#x200B;* [Backen] AO mit Normal weist an Kanten Artefakte auf, da die Auffüllung fehlt
&#x200B;* [Farbmanagement] HDR-Farbraumkonvertierungen mit ACE unter Linux erzeugen festgeklemmte Farben
&#x200B;* [Regression]&#x200B;[UI] Kontextmenü auf HD-Bildschirmen ist zu klein
&#x200B;* [Crash]&#x200B;[Python] USD-Export, ausgelöst durch TextureStateEvent
&#x200B;* [Engine] Malen mit dem Kopierwerkzeug in normalen Kanalverschiebungsfarben falsch
&#x200B;* [Python] Das Ghost-Widget wird durch das noch funktionierende Skript gelöscht.

### 11.0.3

Freigabedatum: <b>2025/08/05</b>
Zusammenfassung: <b>Nebenversion</b>

<b>Hinzugefügt</b>:

&#x200B;* [Substance 3D Assets] Hinzufügen eines Benachrichtigungspunkts zum Bedienfeld &quot;3D-Elemente&quot;
&#x200B;* [VFX Platform 2025] ACES 2.0-Konfiguration in den Farbmanagementeinstellungen hinzufügen
&#x200B;* [VFX Platform 2025] Update OCIO auf Version 2.4.2
&#x200B;* Update Iray auf Version 2024.10
&#x200B;* [Engine] Update auf Substance Engine v.9.2.3
&#x200B;* [Nvidia] Erhöhung der Nvidia-Mindesttreiberversion auf 572.60 (Win) und 570.169 (Linux)

<b>Fest</b>:

&#x200B;* [Python] Bereichsänderung wird nicht im Verlaufsfenster angezeigt

<b>Bekannte Probleme</b>:

&#x200B;* [Farbmanagement] HDR-Farbraumkonvertierungen mit ACE unter Linux erzeugen festgeklemmte Farben
&#x200B;* [Regression]&#x200B;[UI] Kontextmenü auf HD-Bildschirmen ist zu klein
&#x200B;* [Crash]&#x200B;[Python] USD-Export, ausgelöst durch TextureStateEvent
&#x200B;* [Engine] Malen mit dem Kopierwerkzeug in normalen Kanalverschiebungsfarben falsch
&#x200B;* [Python] Das Ghost-Widget wird durch das noch funktionierende Skript gelöscht.

### 11.0.2

Freigabedatum: <b>2025/06/10</b>
Zusammenfassung: <b>Nebenversion</b>

<b>Hinzugefügt</b>:

&#x200B;* [Mac] Fügen Sie Warnungen zu bestimmten Betriebssystemversionen hinzu, die zu Artefakten führen
&#x200B;* [Automatische Aktualisierung] Kleine UX-Verbesserungen im Fehlerprotokoll &quot;Assets&quot;
&#x200B;* [Automatisches Ausgliedern] Update auf Version 1.3.2 mit Verbesserter Nahtfunktion
&#x200B;* [USD]&#x200B;[FBX] Unterstützung für mehrere UV-Sets mit geringen Datenmengen hinzufügen
&#x200B;* [Export] Bei als FBX exportierten Meshes fehlen die zusätzlichen UV-Sets, wenn beim Import vorhanden

<b>Fest</b>:

&#x200B;* [MacOS]&#x200B;[Linux] Absturz beim Speichern auf dem Netzlaufwerk
&#x200B;* [Win]&#x200B;[Tablet] Flackern beim Schwenken
&#x200B;* [SpaceMouse] Problem bei der Arbeit mit dem Pfadwerkzeug
&#x200B;* [Auto-Cage] Nach erneuter Netzlast kann nicht gebacken werden
&#x200B;* [Automatische Aktualisierung] Bildsequenz wird nicht neu geladen, wenn die erste Kachel fehlt
&#x200B;* [Pfad] Benutzerdefinierte Tangente kann andere Tangente beeinflussen
&#x200B;* [Pfad] Pfad wird im Textursatz nicht angezeigt, wenn sich der erste Punkt in einem anderen Textursatz befindet
&#x200B;* [UI] Einige Menüs sind nach dem Öffnen eines Projekts immer deaktiviert (z. B.: Symmetrie)
&#x200B;* [Eigenschaften] Werkzeugvorgaben mit ausgefülltem Pfadwerkzeug können nicht verwendet/geladen werden
&#x200B;* [USD] Mehrere UV-Sätze werden in benutzerdefiniertem Shader nicht erkannt, wenn USD-Dateien verwendet werden
&#x200B;* [USD] Kameras mit den gleichen Namen werden überschrieben
&#x200B;* [Exportieren] &quot;An Photoshop senden&quot; führt zu einem falschen Farbraum für Farb- und Graustufenergebnisse
&#x200B;* [Exportieren] Graustufen-Kanäle mit Alpha werden als Farbe anstatt als Graustufen mit PNG-Format exportiert
&#x200B;* [Exportieren] Exportieren des Graustufenkanals als PSD führt zu einer ungültigen/verkürzten Datei
&#x200B;* [Inhalt] Verkrümmungsfilter im Mehrrichtungsmodus funktioniert nicht
&#x200B;* [Python] Fehler beim Zuweisen der Liste beim Crawlen von Ebenenstapelknoten nicht möglich

<b>Bekannte Probleme</b>:

&#x200B;* [Farbmanagement] HDR-Farbraumkonvertierungen mit ACE unter Linux erzeugen festgeklemmte Farben
&#x200B;* [Regression]&#x200B;[UI] Kontextmenü auf HD-Bildschirmen ist zu klein
&#x200B;* [Crash]&#x200B;[Python] USD-Export, ausgelöst durch TextureStateEvent
&#x200B;* [Engine] Malen mit dem Kopierwerkzeug in normalen Kanalverschiebungsfarben falsch
&#x200B;* [Python] Das Ghost-Widget wird durch das noch funktionierende Skript gelöscht.

### 11.0.1

Freigabedatum: <b>2025/04/10</b>
Zusammenfassung: <b>Nebenversion</b>

Hinweis: <b>Die Linux CCD-Version wird auf den 29. April verschoben.</b>

<b>Hinzugefügt:</b>

&#x200B;* Update auf Qt 6.5.8
&#x200B;* [Substance] Fügen Sie eine Protokollmeldung für Filter hinzu, wenn mehrere Bildeingaben dieselbe Verwendung haben.
&#x200B;* [Nvidia] Warnung über die neuesten Nvidia-Treiber hinzufügen (572.47)

<b>Fest:</b>

&#x200B;* [Absturz] Wenn Sie einen SBSAR mit einer Verwendung in einem einzelnen Kanalsteckplatz ziehen und ablegen
&#x200B;* [Absturz]&#x200B;[Pfad] Die Option &quot;Pfadtyp ändern&quot; ist nicht ausgegraut, wenn Sie nicht auf einen bestimmten Pfad klicken.
&#x200B;* [Füllpfad] Sollte nicht in der Lage sein, Substance-Material auszuwählen
&#x200B;* [Engine] Artefakte an Pinselstrichen
&#x200B;* [Engine] Pfade können mit bestimmten Einstellungen unterbrochen werden.
&#x200B;* Problem mit der Dropdown-Liste für den Pipetten-Farbraum
&#x200B;* [Automatische Aktualisierung] [Python] Falsche Fehlermeldung bei Verwendung von ResourceID ohne Version
&#x200B;* [Shader] Absturz beim Öffnen einiger Projekte

<b>Bekannte Probleme:</b>

&#x200B;* [SpaceMouse] Problem bei der Arbeit mit dem Pfadwerkzeug
&#x200B;* [Farbmanagement] HDR-Farbraumkonvertierungen mit ACE unter Linux erzeugen festgeklemmte Farben
&#x200B;* [Regression]&#x200B;[UI] Kontextmenü auf HD-Bildschirmen ist zu klein
&#x200B;* [Crash]&#x200B;[Python] USD-Export, ausgelöst durch TextureStateEvent
&#x200B;* [Engine] Malen mit dem Kopierwerkzeug in normalen Kanalverschiebungsfarben falsch
&#x200B;* [Python] Das Ghost-Widget wird durch das noch funktionierende Skript gelöscht.

### 11.0.0

Freigabedatum: <b>2025/03/11</b>
Zusammenfassung: <b>Hauptversion, neue Funktion zur automatischen Aktualisierung, Tool für gefüllte Pfade und andere Pfadverbesserungen sowie neue Filter und eine experimentelle Generierung von automatischen Käfigen für Backvorgänge</b>

<b>Hinzugefügt</b>:

&#x200B;* Automatische Aktualisierung
&#x200B;* [Automatische Aktualisierung] Automatische Aktualisierung geänderter Elemente im Bedienfeld &quot;Elemente&quot;
&#x200B;* [Automatische Aktualisierung] Automatische Aktualisierung geänderter Elemente im gesamten Projekt
&#x200B;* [Automatische Aktualisierung] Automatische Aktualisierung standardmäßig deaktiviert lassen
&#x200B;* [Automatische Aktualisierung] Optionale Aktualisierung, wenn die Ressourcenparameter nicht übereinstimmen (.sbsar, .glsl, .ai, .svg)
&#x200B;* [Automatische Aktualisierung] Umgebungsvariable hinzufügen, um die automatische Aktualisierung zu deaktivieren
&#x200B;* [Automatische Aktualisierung]&#x200B;[SBSAR] Optionale Aktualisierung, wenn die Ressourcenparameter nicht übereinstimmen
&#x200B;* Ausgefüllter Pfad
&#x200B;* [Pfad]&#x200B;[Füllen] Fügen Sie ein neues Werkzeug hinzu, um gefüllte Pfade zu erstellen.
&#x200B;* Verbesserungen an Pfaden
&#x200B;* [Pfad] Erstellen von Pfaden, die an Polygonen ausgerichtet werden
&#x200B;* [Pfad] Wechsel der Pfadtypen zulassen
&#x200B;* [Pfad] Kopieren und Einfügen von Pfadscheitelpunktdaten zwischen Inhalt und Maske zulassen
&#x200B;* [Pfad] Winkel beim Erstellen eines neuen Punkts einschränken
&#x200B;* [Path] Erlaubt das Beschränken der Punkterstellung auf eine Linie.
&#x200B;* [Pfad] Form mit einem Klick schließen
&#x200B;* [Pfad] Anzeigen von Pfadinformationen
&#x200B;* [Pfad] Skalieren und Drehen von Pfadscheitelpunkten zulassen
&#x200B;* [Pfad]&#x200B;[UX] Einfacherer Zugriff auf Transformations-Gizmos
&#x200B;* [Pfad] Pfadvorschau hinzufügen
&#x200B;* [Pfad] Deaktivieren der Pfadvorschau mit Umschalt + P
&#x200B;* [Pfad] Verbesserung der Tangentenausgabe in der Seitenansicht
&#x200B;* [Pfad] Fokus auf einen 3D-Pfad festlegen.
&#x200B;* [Pfad] Scheitelpunkte sollten den Auswahlstatus beibehalten, wenn die Benutzeroberfläche aus- und wieder aktiviert wird
&#x200B;* [Path] Löschen von Pfaden mit Rücktaste zulassen
&#x200B;* [Pfad] Die Pfadliste offen halten, wenn der Benutzer sie erweitert
&#x200B;* [Pfad]&#x200B;[Ebenenstapel] Duplikate beim Kopieren/Einfügen richtig umbenennen
&#x200B;* Verbesserungen an der Benutzeroberfläche und der QuickInfo [Path]
&#x200B;* Leistung
&#x200B;* [Leistung] Verbessern der Viewport-Leistung bei Verwendung einer hohen Tesselierungsstufe
&#x200B;* [Leistung] Nur den ersten Kanal auf neuen Füllebenen/Effekten aktivieren
&#x200B;* [Leistung] Parallelisierung der Pinselstrichberechnung
&#x200B;* Baking
&#x200B;* [Backen] Neue vollautomatische Käfigerzeugungsoption zum Backen mit High-Poly-Netzen hinzufügen (experimentell)
&#x200B;* Inhalt
&#x200B;* [Inhalt] Fügen Sie 6 neue Filter hinzu: stilisierung, quantisieren, anisotropic kuwahara, weiche Abschrägung, Richtungsabstand, Graustufen konvertierung
&#x200B;* [Inhalt] Aktualisieren von Rauschen und Grunges auf die neueste Version von Designer (mit der neuen 2D-Voronoi)
&#x200B;* [Inhalt] 3 neue Texturgeneratoren hinzufügen (Kachelzufall, Triangle Grid, Scratches-Generator)
&#x200B;* [Inhalt] Unreal Engine-Vorlage umbenennen und Vorgaben exportieren
&#x200B;* Python
&#x200B;* [Shelf]&#x200B;[Python] Speichern Sie Smart-Material oder Smart-Maske von Python auf der Festplatte.
&#x200B;* [Python] Hinzufügen des automatischen Käfigs zum Python-API
&#x200B;* [Python] Bearbeiten von Namen und Beschreibungen von Textursätzen/UV-Kacheln zulassen
&#x200B;* [Python] Freigeben von Auflösungseinstellungen für Vektor- und Schriftartenquellen
&#x200B;* [Automatische Aktualisierung]&#x200B;[Python] Stellen Sie die Funktionen zur automatischen Aktualisierung von Projekten in Python bereit.
&#x200B;* Verschiedenes
&#x200B;* [Exportieren] Erleichtern Sie den Zugriff auf die Optionen für Senden an mit einem neuen Fenster
&#x200B;* [Nvidia] Warnung über die neuesten Nvidia-Treiber hinzufügen (572.16)
&#x200B;* Die Winkelausrichtung sollte durch die Objekt-/Welt-Raumauswahl beeinflusst werden.
&#x200B;* [Liste der Textursätze] Benutzerdefinierten Namen zu UV-Kacheln hinzufügen und diese beim Export verwenden
&#x200B;* Mac
&#x200B;* [Mac] Verwenden von Metal anstelle von OpenGL für das Grafik-Rendering
&#x200B;* [Mac] Mac Intel-Support entfernen

<b>Fest</b>:

&#x200B;* [Absturz] Löschen der Bildeingabe
&#x200B;* Smart-Matte kann nicht über die Ebenenstapelschaltfläche hinzugefügt werden
&#x200B;* [Python] Effekte auf GroupLayerNode können nicht gefunden werden

<b>Bekannte Probleme</b>:

&#x200B;* [Farbmanagement] HDR-Farbraumkonvertierungen mit ACE unter Linux erzeugen festgeklemmte Farben
&#x200B;* [Regression]&#x200B;[UI] Kontextmenü auf HD-Bildschirmen ist zu klein
&#x200B;* [Crash]&#x200B;[Python] USD-Export, ausgelöst durch TextureStateEvent
&#x200B;* [MacOS Intel] Absturz beim Importieren einiger Vorgaben
&#x200B;* [Engine] Malen mit dem Kopierwerkzeug in normalen Kanalverschiebungsfarben falsch
&#x200B;* [Python] Das Ghost-Widget wird durch das noch funktionierende Skript gelöscht.
&#x200B;* [RedHat] Probleme mit dem Farbwähler

## Version 10

### 10.1.2

Freigabedatum: <b>2024/12/3</b>
Zusammenfassung: <b>Nebenversion, Fehlerbehebungen</b>

<b>Fest</b>:

&#x200B;* [Absturz] Löschen der Bildeingabe
&#x200B;* Smart-Matte kann nicht über die Ebenenstapelschaltfläche hinzugefügt werden
&#x200B;* [Python] Effekte auf GroupLayerNode können nicht gefunden werden

<b>Bekannte Probleme</b>:

&#x200B;* [Farbmanagement] HDR-Farbraumkonvertierungen mit ACE unter Linux erzeugen festgeklemmte Farben
&#x200B;* [Regression]&#x200B;[UI] Kontextmenü auf HD-Bildschirmen ist zu klein
&#x200B;* [Crash]&#x200B;[Python] USD-Export, ausgelöst durch TextureStateEvent
&#x200B;* [MacOS Intel] Absturz beim Importieren einiger Vorgaben
&#x200B;* [Engine] Malen mit dem Kopierwerkzeug in normalen Kanalverschiebungsfarben falsch
&#x200B;* [Python] Das Ghost-Widget wird durch das noch funktionierende Skript gelöscht.
&#x200B;* [RedHat] Probleme mit dem Farbwähler

### 10.1.1

Freigabedatum: <b>2024/11/5</b>
Zusammenfassung: <b>Nebenversion, Fehlerbehebungen</b>

<b>Hinzugefügt</b>:

&#x200B;* [Projekt] Aktuelles Projekt bleibt geöffnet, bis die neue Projektauswahl validiert wurde
&#x200B;* [Automatisches Ausgliedern] Texeldichte ermöglicht ein besseres Aufteilen von UV-Inseln in UDIMs
&#x200B;* [Backen] Mehrdeutige Kopie im Kontextmenü von Mesh Maps beheben
&#x200B;* [Verformen] Skalierung im Ansichtsfenster für Z-Achse (Tiefe) entfernen
&#x200B;* [Importieren/Exportieren] Unterstützung nicht verwendeter Bilddateiformate entfernen
&#x200B;* Update Substance Engine auf 9.1.4

<b>Fest</b>:

&#x200B;* [Absturz] Nach dem Verschieben der Ressource in &quot;Assets&quot; und dem Speichern des Projekts
&#x200B;* [Absturz] Probleme mit der Serverbibliothek
&#x200B;* [Absturz] Absturz des Illustrator-Servers in einigen seltenen Fällen
&#x200B;* [Absturz] Beim Beenden der Anwendung in seltenen Fällen
&#x200B;* Absturzberichte können auf einigen Computern nicht gesendet werden
&#x200B;* [Backen] Die Scheitelpunktfarbe wird nicht richtig gelesen
&#x200B;* [UI] Position von Fenstern und Neue Funktionen beim Start wurde verschoben
&#x200B;* [Assimp] Maya&#39;s StandardSurface wird beim ID-Backen nicht erkannt
&#x200B;* [Python] Fehlende SSL-Bibliothek gibt einen Fehler aus
&#x200B;* [Python]&#x200B;[Win] Fehler beim Aufrufen von QColorConstants.Transparent
&#x200B;* [Python] Ebenen-Miniaturansichten, die über Python erstellt wurden, werden erst aktualisiert, wenn Sie in den Ebenenstapel klicken
&#x200B;* [Shader] Fehlerhafte Verknüpfung im Shader-API-Changelog
&#x200B;* [3D-Elemente] OS-Proxy-Einstellungen für den Zugriff auf 3D-Elemente verwenden

<b>Bekannte Probleme</b>:

&#x200B;* [Farbmanagement] HDR-Farbraumkonvertierungen mit ACE unter Linux erzeugen festgeklemmte Farben
&#x200B;* [Regression]&#x200B;[UI] Kontextmenü auf HD-Bildschirmen ist zu klein
&#x200B;* [Crash]&#x200B;[Python] USD-Export, ausgelöst durch TextureStateEvent
&#x200B;* [MacOS Intel] Absturz beim Importieren einiger Vorgaben
&#x200B;* [Engine] Malen mit dem Kopierwerkzeug in normalen Kanalverschiebungsfarben falsch
&#x200B;* [Python] Widget, das über ein noch funktionierendes Skript gelöscht scheint
&#x200B;* [RedHat] Probleme mit dem Farbwähler

### 10.1.0

Freigabedatum: <b>2024/09/17</b>
Zusammenfassung: <b>Hauptversion, neuer Inhalt: Füllbereichsmaske/Farbfilter, Stickereiaufklebefilter und sechs generische Substance-Filter, Import von USD mit Material- und Shader-Eigenschaften, Leistungsverbesserung, VFX-Plattform 2024-kompatibel und Migration auf Linux RedHat</b>

<b>Hinzugefügt</b>:

&#x200B;* [Inhalt] Neue Füllbereichsmaske/Farbfilter hinzufügen
&#x200B;* [Inhalt] Neuen Stickerei Decal Filter hinzufügen
&#x200B;* [Inhalt] Fügen Sie 6 neue generische Substance-Filter hinzu (FXAA, Vergröberungsfilter, Hochpass, Posterisierung, Glättungsschritt, Schwellenwert).
&#x200B;* [USD] Exportieren der USD-Ebene mit einem definierten ASM-Material
&#x200B;* [USD] Importieren von USD mit Material- und Shader-Eigenschaften
&#x200B;* [Leistung] Aktivieren Sie standardmäßig optimierte Ebenenstapel-Miniaturansichten
&#x200B;* [Leistung] Reduzieren der Öffnungszeit von Projektdateien und des Speicherverbrauchs (Datendecodierung)
&#x200B;* VFX-Plattform 2024-kompatibel
&#x200B;* [VFX Platform 2024] Update auf Python 3.11
&#x200B;* [VFX Platform 2024] Update auf OpenEXR 3.2
&#x200B;* [VFX Platform 2024] [USD] Update OpenSubdiv 3.6.0
&#x200B;* [VFX Platform 2024]&#x200B;[Color Management] Update auf OCIO 2.3.2
&#x200B;* [Linux] Migration zu Linux RedHat
&#x200B;* [Linux] Aktualisieren Sie den Nvidia-Treiber auf Version 535.171.04
&#x200B;* [Importieren] Fügen Sie eine Option hinzu, um die normale Map beim Importieren eines GLTF-Gitters zu spiegeln.
&#x200B;* [UI] Standardwert des Betriebssystems für die Entfernung der Erkennung von Ziehereignissen verwenden
&#x200B;* [Substance Engine] Fügen Sie eine Aufrufstreifenfunktion hinzu, um die Symbole aus der ausführbaren Datei zu entfernen.
&#x200B;* [Begrüßungsbildschirm] Update auf neues Begrüßungsbildschirmformat
&#x200B;* Substance Engine auf Version 9.1.3 aktualisieren
&#x200B;* [Python] Link zu Beispielen im Dokumentationsmenü des Ebenenstapels anzeigen
&#x200B;* [JavaScript] Verschieben von JavaScript-Plugins in den Unterordner &quot;javascript/plugins&quot;

<b>Fest</b>:

&#x200B;* [Illustrator] Absturz beim Exportieren einer UV-Kachel mit .ai-Grafik in bestimmten Fällen
&#x200B;* [Dynamische Pinselstriche]&#x200B;[Pfad] Zufällig pro Strich funktioniert nicht auf einem Pfad
&#x200B;* [UI]&#x200B;[Eigenschaften] Sperre ist aktiviert, wenn die Unterteilung nicht einheitlich ist
&#x200B;* Debug TXT-Datei wird erstellt, wenn Sie auf ein Painter-Projekt doppelklicken
&#x200B;* [USD]&#x200B;[Export] Möglicherweise fehlen einige Texturen.
&#x200B;* [ASM] Beim Streufarbkanal werden metallische
&#x200B;* [Inhalt] Weichzeichnungsfilter funktioniert nicht im &quot;funktionierenden&quot; Farbraum
&#x200B;* [Inhalt] Height Der Filter &quot;Anpassen&quot; ändert auch das Alpha der Ebene.

<b>Bekannte Probleme</b>:

&#x200B;* [Farbmanagement] HDR-Farbraumkonvertierungen mit ACE unter Linux erzeugen festgeklemmte Farben
&#x200B;* [Win]&#x200B;[Absturz] [ACE] sRGB ICE-Farbraum wird für die Bildschirmtransformation nicht verwendet.
&#x200B;* [Regression]&#x200B;[UI] Kontextmenü auf HD-Bildschirmen ist zu klein
&#x200B;* [Crash]&#x200B;[Python] USD-Export, ausgelöst durch TextureStateEvent
&#x200B;* [MacOS Intel] Absturz beim Importieren einiger Vorgaben
&#x200B;* [Absturz] Ressource verschieben und Projekt speichern
&#x200B;* [Engine] Malen mit dem Kopierwerkzeug in normalen Kanalverschiebungsfarben falsch
&#x200B;* [Python] Das Ghost-Widget wird durch das noch funktionierende Skript gelöscht.
&#x200B;* [RedHat] Probleme mit dem Farbwähler

### 10.0.1

Freigabedatum: <b>2024/06/11</b>
Zusammenfassung: <b>Nebenversion, Fehlerbehebungen</b>

<b>Hinzugefügt:</b>

&#x200B;* [Library] Konvertieren von Substance-Schriftarten in normale Schriftdateien
&#x200B;* [Illustrator]&#x200B;[SVG] Miniaturansichten in der Bereichsauswahl einen hellgrauen Hintergrund geben
&#x200B;* [Python] Hinzufügen einer Funktion in der Bitmapquelle, um verfügbare Farbräume aufzulisten

<b>Fest</b>:

&#x200B;* [Ebenenstapel] Ordner immer geschlossen, wenn er in andere Ordner verschoben oder aus anderen Ordnern verschoben wird
&#x200B;* [Speichern] Projektdatei geht verloren, wenn &quot;Speichern als Kopie&quot; oder automatisches Speichern in bestimmten Fällen fehlschlägt
&#x200B;* [Importieren] Assets mit demselben Namen, aber unterschiedlichen Erweiterungen werden überschrieben
&#x200B;* [Eigenschaften] Einstellungen fehlen, wenn Ankerpunkt in Bildeingaben verwendet wird
&#x200B;* [Illustrator] Illustrator-Dateien können nach Serverabsturz nicht importiert werden, ohne Painter neu zu starten
&#x200B;* [Python] Übergeordnete Instanz kann nicht mit Typ &quot;Eigenschaften&quot; festgelegt werden
&#x200B;* [Python] Das Festlegen des hohen Poly als Backparameter lädt das hohe Poly nicht
&#x200B;* [Python] Fehlermeldung für set\_color\_space() ist zu allgemein
&#x200B;* [Python] Referenzquellen ermöglichen das Erstellen von Zyklen

<b>Bekannte Probleme</b>:

&#x200B;* [Farbmanagement] HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen festgeklemmte Farben
&#x200B;* [Regression]&#x200B;[UI] Kontextmenü auf HD-Bildschirmen ist zu klein
&#x200B;* [Absturz]&#x200B;[Python] USD durch TextureStateEvent ausgelöst
&#x200B;* [MacOS Intel] Absturz beim Importieren einiger Vorgaben
&#x200B;* [Illustrator] Absturz beim Exportieren einer UV-Kachel mit .ai-Grafik in bestimmten Fällen
&#x200B;* [Dynamische Pinselstriche]&#x200B;[Pfad] Zufällig pro Strich funktioniert nicht auf einem Pfad

### 10.0.0

Freigabedatum: <b>2024/05/16</b>
Zusammenfassung: <b>Hauptversion, Edition des Ebenenstapels mit Python-API, Lesen nativer Illustrator-Dateien, Integration von 3D-Assets und neuer Textressource</b>

<b>Hinzugefügt</b>:

&#x200B;* [Illustrator] Verwenden von Illustrator-Dateien mit Zeichenflächen in Painter
&#x200B;* [Illustrator]&#x200B;[SVG] Hinzufügen von Vorschauen in der Bereichsauswahl
&#x200B;* [Substance 3D Assets] Durchsuchen, Auswählen und Herunterladen von 3D-Assets direkt in Painter
&#x200B;* [Substance 3D Assets]&#x200B;[UI] Neues Bedienfeld
&#x200B;* [Substance 3D Assets] Unterstützung für Umgebungs-Map und Materials
&#x200B;* [Substance 3D Assets] Ermöglicht das erneute Laden und Navigieren im Speicherortordner und das Öffnen im neuen Bedienfeld &quot;Substance 3D Assets&quot;.
&#x200B;* [Substance 3D Assets] Hinzufügen eines Download-Managers
&#x200B;* [Textressource] Einbettbare Schriftarten verwenden
&#x200B;* [Textressource] Erlaubt das Rendern einer Schriftart/eines Texts auf einem Mesh.
&#x200B;* [Textressource] Anzeigen von Schriftarten von Benutzer- und anderen freigegebenen Pfaden im Bedienfeld &quot;Elemente&quot; mit einer neuen Kategorie
&#x200B;* [Textressource]&#x200B;[Eigenschaften] Unterstützung für erweiterte Schriftarteigenschaften hinzufügen
&#x200B;* [Textressource] Ermöglicht das Suchen/Anzeigen von Schriftarten in Mini-Regalen
&#x200B;* [Textressource] Fehlermeldung/Dialogfeld hinzufügen, wenn eine inkompatible Schriftart importiert wird
&#x200B;* Sonstiges
&#x200B;* [Projektion füllen] Verbessern Sie das Verhalten des Manipulators Skalierung bei Verwendung kleiner Werte
&#x200B;* [Manipulator] Hinzufügen eines neuen präzisen Modus beim Drücken von STRG-Tastaturbefehl
&#x200B;* [Manipulator] Verbessern der Stabilität des Manipulators auf der Oberfläche beim Kamera beweg
&#x200B;* [Exportieren] Hinzufügen eines Farbraumnamens in SBSAR-Ausgaben
&#x200B;* [Performance] Verbessern der Erkennungszeit von Elementen auf der Festplatte in Bibliotheken
&#x200B;* [Substance] Update auf Substance Engine Version 9.1.2
&#x200B;* [Drag &amp; Drop] Ausrichten der Aufkleberdrehung an der Kamera beim Ablegen im Viewport
&#x200B;* [Python] Edition des Ebenenstapels
&#x200B;* [Python] Auswahl von Ebene, Effekt, Maske und Geomaske in der Benutzeroberfläche zulassen
&#x200B;* [Python] Abrufen/Festlegen von Mischmodi für Ebenen
&#x200B;* [Python] Einstellungen für die Füllebene-Projektion abrufen/festlegen
&#x200B;* [Python] Abfrage der Substance-Material-Farbe aus einer Füllebene zulassen
&#x200B;* [Python] Abfragen und Festlegen von einheitliche Farben und Ressourcen in Ebenen und Effekten zulassen
&#x200B;* [Python] Erstellen und Bearbeiten von Textressourcen im Ebenenstapel zulassen
&#x200B;* [Python] Bearbeiten aktiver Kanäle für Ebenen und Effekte zulassen
&#x200B;* [Python] Batch-Aktionen können nur einmal rückgängig gemacht/wiederholt werden.
&#x200B;* [Python] Laden/Bearbeiten von vektoriellen Quellparametern zulassen
&#x200B;* [Python] Bearbeiten von Ebenen- und Effektfarbeneigenschaften mit Farbmanagement zulassen
&#x200B;* [Python] Abfragen und Erstellen instanzierter Ebenen zulassen
&#x200B;* [Python] Hinzufügen des Effekts &quot;Farbauswahl&quot; zulassen
&#x200B;* [Python] Steuern des Farbmanagements für Bitmapbilder
&#x200B;* [Python] Engine anhalten/fortsetzen
&#x200B;* [Python] Navigation zu gleichrangigen und übergeordneten Knoten zulassen
&#x200B;* [Python] Erstellen eines Filter-/Generatoreffekts zulassen
&#x200B;* [Python] Hinzufügen des Ebeneneffekts zulassen
&#x200B;* [Python] Hinzufügen von intelligente Maske zu einer Ebene zulassen
&#x200B;* [Python] Erstellen/Bearbeiten von Ankerpunkten zulassen
&#x200B;* [Python] Maske für Ebenen abrufen/festlegen
&#x200B;* [Python] Erstellen des Effekts &quot;Maske vergleichen&quot; zulassen
&#x200B;* [Python] Zulassen, dass Vorgaben aus Substance-Ressourcen abgefragt und verwendet werden
&#x200B;* [Python] Erlaubt das Auflisten von Vorgaben und ihren Werten über die interne \_properties-Funktion für Substance-Ressourcen.
&#x200B;* [Python] Liste vordefinierter Exportvorgaben zulassen
&#x200B;* [Python] Auflisten der in der Bibliothek verfügbaren Exportvorgaben
&#x200B;* [Python] Abrufen des Inhalts von Exportvorgaben zulassen

<b>Fest</b>:

&#x200B;* [Absturz] Rückgängigmachen von &quot;Shader-Instanz entfernen&quot; mit Strg+Z
&#x200B;* [Absturz] Erstellen einer Ebene auf leerem Stapel, wenn die letzte Auswahl ein Effekt war
&#x200B;* [SVG] Problem mit benutzerdefiniertem Wert für den zugeschnittenen Bereich
&#x200B;* [Automatisches Entpacken] Die Neuberechnung nur des Packings ohne Änderung der Ausrichtung der UV führt zu einem Absturz
&#x200B;* [Drag &amp; Drop] Verzögerung aufgrund externer Ressourcen wird mehrmals vorgeladen
&#x200B;* [UI] Miniaturansicht der Ressource per Drag &amp; Drop kann Warnmeldung im Ebenenstapel ausblenden
&#x200B;* [Performance] Maskierte UV-Kacheln werden noch berechnet
&#x200B;* [USD] Falsche Markierung für die Bereichsauswahl
&#x200B;* [Ressource] Bitmapbild wird beschädigt, nachdem im normalen Kanal gemalt und das Projekt gespeichert wurde
&#x200B;* [USD] Unterstützung für die Bestellung von Meshs für den linkshändigen Scheitelpunkt
&#x200B;* [Substance] Auf die Standardeinstellung zurücksetzen, um immer auf null für Winkel-Widget zurückzusetzen
&#x200B;* [Engine] Das Malen mit einem SVG in einer Schablone funktioniert nicht
&#x200B;* [Engine] Normalen-Map-Pinselstriche brechen nach einem Rückgängigmachen
&#x200B;* [Inhalt] Grafik zu Materialfilter hat falsche Alpha-Überblendung und falschen Farbraum
&#x200B;* [Inhalt] Füllmethoden auf dem Tile Generator funktionieren nicht
&#x200B;* [Inhalt] Histogramm-Scanfilter erzeugt in einigen Fällen Streifenbildung
&#x200B;* [Inhalt] Baking geführt stilisierte Beleuchtung berücksichtigt kein gemaltes Height
&#x200B;* [Python] Unerwarteter Fehler beim Abrufen instanzierter Ebeneninformationen nach Shader-Änderung
&#x200B;* [Speichern] Projektdatei geht verloren, wenn &quot;Speichern unter&quot; in bestimmten Fällen fehlschlägt

<b>Bekannte Probleme</b>:

&#x200B;* [Farbmanagement] HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen festgeklemmte Farben
&#x200B;* [Absturz]&#x200B;[Linux]&#x200B;[AMD] Ziehen und Ablegen von Ressourcen im Ebenenstapel unter Wayland OS
&#x200B;* [Regression]&#x200B;[UI] Kontextmenü auf HD-Bildschirmen ist zu klein
&#x200B;* [Absturz]&#x200B;[Python] USD durch TextureStateEvent ausgelöst
&#x200B;* [Speichern] Spp-Projektdatei geht verloren, wenn &quot;Als Kopie speichern&quot; in bestimmten Fällen fehlschlägt
&#x200B;* [MacOS Intel] Absturz beim Importieren einiger Vorgaben
&#x200B;* [Illustrator] Ai-Dateien können nach dem Server-Absturz nicht importiert werden, ohne Painter neu zu starten
&#x200B;* [Importieren] Assets mit demselben Namen, aber unterschiedlichen Erweiterungen werden überschrieben

## Version 9

### 9.1.2

Freigabedatum: <b>2024/01/30</b>
Zusammenfassung: <b>Nebenversion, Fehlerbehebungen</b>

<b>Hinzugefügt</b>:

&#x200B;* [Performance] Verbessern der Erstellungszeit der ersten Füllebene in neuen Projekten
&#x200B;* [Performance] Verkürzung der Ladezeit schwerer Umgebungs-Map
&#x200B;* [Substance] Speichern/Schließen von Projekten zulassen, selbst wenn Miniaturansichten generiert werden

<b>Fest</b>:

&#x200B;* Speichern schlägt in Projekten früherer Versionen fehl, wenn der Viewport geändert wird
&#x200B;* [Absturz] Mesh wird bei Verwendung von benutzerdefiniertem AO und Farbmanagement erneut importiert
&#x200B;* [Projektion füllen] Beim Klicken auf den Manipulator &quot;Skalieren&quot; wird die Meldung &quot;nicht bemalbar&quot; angezeigt.
&#x200B;* [Pinsel] Malen mit UV-Ausrichtung verursacht Artefakte
&#x200B;* [Ebenenstapel] Das Umbenennen der Ebene ist langsam, wenn der Stapel sehr lang ist
&#x200B;* [Ebenenstapel] Falsche Fehlermeldung bei Verwendung eines inkompatiblen Filters in der Maske
&#x200B;* [Ebenenstapel] Die Auswahl wechselt nach dem Löschen zurück zur obersten Ebene
&#x200B;* [Exportieren] Generierte normale Textur befindet sich immer im 3D-Modus &quot;Abstand: Nachbar&quot;.
&#x200B;* [Export] Textur-Alpha wird nicht mit der Exportvorgabe der 2D-Ansicht generiert
&#x200B;* [Export] Beim SBSAR-Export werden falsche Verwendungsmöglichkeiten mit konvertierten Karten verwendet.
&#x200B;* [Shader] Shader-API-Changelog ist nicht auf dem neuesten Stand bei ASM-Änderungen

<b>Bekannte Probleme</b>:

&#x200B;* [Farbmanagement] HDR-Farbraumkonvertierungen mit ACE unter Linux erzeugen festgeklemmte Farben
&#x200B;* [Absturz]&#x200B;[Linux]&#x200B;[AMD] Ziehen und Ablegen von Ressourcen im Ebenenstapel unter Wayland OS
&#x200B;* [Regression]&#x200B;[UI] Kontextmenü auf HD-Bildschirmen ist zu klein
&#x200B;* [Crash]&#x200B;[Python] USD-Export, ausgelöst durch TextureStateEvent

### 9.1.1

Freigabedatum: <b>2023/12/05</b>
Zusammenfassung: <b>Nebenversion, Fehlerbehebungen und Senden an After Effects-Funktionen</b>

<b>Hinzugefügt:</b>

&#x200B;* [Interop] Senden eines strukturierten Gitters an After Effects zulassen (Ae 24.1)

<b>Fest:</b>

&#x200B;* [Füllung] UV-Set auf UV-Set-Projektion liest nicht mehr als 2 UV-Sets
&#x200B;* [Absturz] Verwenden der 16.000-KB-Umgebungszuordnung
&#x200B;* [Absturz] Exr als Bildeingabe verwendet
&#x200B;* [Absturz] Kopieren und Einfügen von Pfaden über Projekte hinweg
&#x200B;* [QoL] Ziehen und Ablegen von Alpha-Ressourcen im Aufklebermodus erzeugt UV-Projektion in der Maske
&#x200B;* [Pfad] Beim Kopieren von Pfadscheitelpunkten wird der Zielpfad auch beim erneuten Öffnen des Projekts umbenannt.
&#x200B;* [Linux] Die Farbauswahl kann mit mehreren Bildschirmen unterbrochen werden
&#x200B;* [Automatisches Ausgliedern] UI-Problem für Texeldichtesteuerung
&#x200B;* [Farbmanagement] UI-Feedback ist sinnvoll, aber Engine ist nicht
&#x200B;* [Farbmanagement] Falsche Farbraumauswahl in der Maske mit Überschreibung von Benutzerdaten

<b>Bekannte Probleme:</b>

&#x200B;* [Farbmanagement] HDR-Farbraumkonvertierungen mit ACE unter Linux erzeugen festgeklemmte Farben
&#x200B;* [Absturz]&#x200B;[Linux] mit Linux Wayland auf AMD beim Ziehen und Ablegen von Ressourcen im Ebenenstapel
&#x200B;* [Absturz]&#x200B;[Mac] Ändern des anisotropen Filterwerts unter Monterey OS
&#x200B;* [Regression]&#x200B;[UI] Kontextmenü auf HD-Bildschirm ist zu klein
&#x200B;* [Python] Absturz beim Exportieren von USD, ausgelöst durch TextureStateEvent

### 9.1.0

Freigabedatum: <b>2023.11.07</b>
Zusammenfassung: <b>Hauptversion mit SVG- und Transparenzunterstützung sowie Verbesserungen an Drag-and-Drop- und Pfad-Tools</b>

<b>Hinzugefügt:</b>

&#x200B;* [SVG] Importieren von Vektordateien zulassen (SVG)
&#x200B;* [SVG]&#x200B;[UI] Unterstützung für SVG-spezifische Eigenschaften hinzufügen
&#x200B;* [SVG] Fügen Sie eine Option hinzu, um die ursprünglichen Bildproportionen einfach beizubehalten
&#x200B;* [SVG] Automatisches Verwenden von Alpha von SVG mit Transparenz zulassen
&#x200B;* [Interop] Senden eines strukturierten Gitters an After Effects zulassen (Ae 24.1 Beta)
&#x200B;* [Interop] Hinzufügen von Einstellungen für &quot;An After Effects senden&quot;
&#x200B;* [QoL]&#x200B;[Assets]&#x200B;[UI] Automatisches Importieren von Assets beim Ziehen und Ablegen in einen Steckplatz der Benutzeroberfläche
&#x200B;* [QoL] Zulassen, dass externe Assets in den Ebenenstapel gezogen und abgelegt werden
&#x200B;* [QoL]&#x200B;[Ebenenstapel] Ziehen Sie Texturen aus dem Bedienfeld &quot;Elemente&quot; in den Ebenenstapel
&#x200B;* [QoL]&#x200B;[Viewport] Generator ziehen und ablegen, Filter auf dem Gitter
&#x200B;* [QoL]&#x200B;[Viewport] Zulassen, dass externe Elemente im Gitter abgelegt werden.
&#x200B;* [QoL]&#x200B;[Projektion] Hinzufügen eines neuen UV-Satzes zum UV-Satzprojektionsmodus
&#x200B;* [QoL] Ziehen und Ablegen von Smart-Masken als neue Ebenen im Ansichtsfenster und im Ebenenstapel
&#x200B;* [QoL] Hinzufügen eines Selektors für Generatoren mit mehreren Ausgaben, wenn er in der Maske verwendet wird
&#x200B;* [QoL] Einkanalbilder können über einen Fülleffekt gezogen und abgelegt werden.
&#x200B;* [QoL]&#x200B;[Ebenenstapel] Verwenden Sie STRG/ALT-Modifizierer mit Drag &amp; Drop, um anzugeben, wo/wie Effekte/Ebenen erstellt werden sollen
&#x200B;* [Pfad] Umschalten der Pfadsichtbarkeit einzeln im Pfadbedienfeld
&#x200B;* [Path] Verwenden von Transformations-Manipulatoren für Pfadpunkte zulassen
&#x200B;* [Path] Tangenten pro Scheitelpunkt manuell steuern
&#x200B;* [Pfad] Kopieren/Einfügen von Pfadeigenschaften
&#x200B;* [Pfad] Schaltfläche &quot;Leerer Tastaturbefehl für Pausen-Tangente einführen&quot;
&#x200B;* [Shader] Unterstützung für Deckkraft und Translucency in ASM-Shader hinzufügen
&#x200B;* [Shader] Unterstützung für Absorptionsfarbe Channel mit ASM Shader hinzufügen
&#x200B;* [Shader] ASM-Shader-Parameter verbessern - QuickInfos
&#x200B;* [Shader] Ändern der Standardfarbe des Translucency-Kanals in Schwarz
&#x200B;* [Anzeigeeinstellungen] Temporale Anti-Aliasing standardmäßig aktivieren
&#x200B;* [Anzeigeeinstellungen] Aktivieren Sie standardmäßig die Einstellung für die Teilflächenstreuung.
&#x200B;* [Substance] Hinzufügen von Unterstützung für die ColorSpace-Eigenschaft von der Eingabe/Ausgabe des Grafen
&#x200B;* [Substance] Substance-Engine auf Version 9.0.3 aktualisieren
&#x200B;* [UI] Zugriff auf die Schaltfläche der kontextbezogenen Symbolleiste, auch wenn das App-Fenster klein ist
&#x200B;* [Automatisch Entpackt] Steuernummer für UV-Kacheln mit Texeldichte
&#x200B;* [Baking] Deaktivieren von GPU-Raytracing auf AMD-GPUs standardmäßig
&#x200B;* [Leistung] Anwendung der verlustfreien Komprimierung auf 16-Bit-Bilder, um den Projektbedarf zu reduzieren
&#x200B;* [Python] Bearbeiten der standardmäßigen Kamera in der 3D-Ansicht zulassen
&#x200B;* [Python] Möglichkeit zum Exportieren von Mesh über Skripterstellung Gelegt
&#x200B;* [Inhalt]&#x200B;[Beispiele] Neues Beispielprojekt hinzufügen &quot;Französische Restauranttabelle&quot;
&#x200B;* [Inhalt] Aktualisieren des Alpha-Substance-Logos auf die neue Version
&#x200B;* [Inhalt] Fügen Sie drei Material-Filter mit SVG hinzu (Benutzerdefinierter Aufkleber, Benutzerdefiniertes Sprühen und Grafik zu Material).

<b>Fest:</b>

&#x200B;* [Absturz] Ändern der Größe von Manipulator, wenn das Werkzeug &quot;Symmetrie&quot; nicht verwendet wird
&#x200B;* [Absturz] [Ebenenstapel] Erstellen einer Ebene, wenn nichts ausgewählt ist
&#x200B;* [Project] Mesh-Map können nach dem Entfernen nicht verwendeter Ressourcen beschädigt werden.
&#x200B;* [Projekt] Ressourcenbeschädigung nach dem erneuten Importieren oder Baking des Images
&#x200B;* [Assets] Durch erneutes Laden eines Assets wird es aus den Favoriten entfernt
&#x200B;* [Importieren] Ressourcen können nicht importiert werden, wenn im Bedienfeld &quot;Asset&quot; &quot;Kein Ergebnis gefunden&quot; angezeigt wird
&#x200B;* [UI] Der kontextbezogene Symbolleistenpfeil wird in einigen Fällen nicht angezeigt
&#x200B;* [Substance] Schaltfläche &quot;Nebeneinander&quot; für boolesche Werte wird nicht unterstützt
&#x200B;* [Level] Falsche Kanalbeschriftung bei Verwendung in Maske
&#x200B;* [Exportieren]&#x200B;[glTF] glTF/GLB-Dateien, die aus Painter exportiert werden, haben keine Physische Größe
&#x200B;* [Inhalt] Intensität des Weichzeichnungsfilters ist auf 16 eingestellt
&#x200B;* [Inhalt] Farbabstimmungsfilter &quot;Zielfarbe&quot; Bildeingabe ist nicht sichtbar

<b>Bekannte Probleme:</b>

&#x200B;* [Farbmanagement] HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen festgeklemmte Farben
&#x200B;* [Absturz]&#x200B;[Linux] mit Linux Wayland auf AMD beim Ziehen und Ablegen von Ressourcen im Ebenenstapel
&#x200B;* [Absturz]&#x200B;[Mac] Ändern des Werts für anisotrope Filterungen unter Monterey OS
&#x200B;* [Absturz] Exr als Bildeingabe verwendet
&#x200B;* [Absturz] Verwenden von 16.000 Umgebungs-Map
&#x200B;* [Automatisch Entpackt] UI-Problem für Texeldichtesteuerung
&#x200B;* [Regression]&#x200B;[UI] Kontextmenü auf HD-Bildschirm ist zu klein
&#x200B;* [Python] Absturz exportieren USD ausgelöst durch TextureStateEvent
&#x200B;* [QoL] Ziehen und Ablegen von Alpha-Ressourcen im Aufklebermodus erzeugt UV-Projektion in der Maske

### 9.0.1

Freigabedatum: <b>2023/09/19</b>
Zusammenfassung: <b>Geringfügige Fehlerbehebungsversion mit mehreren Verbesserungen</b>

<b>Hinzugefügt:</b>

&#x200B;* [Import] Festlegen des Standard-Importspeicherorts im Importfenster
&#x200B;* [Baking-Modus] Parameter auf ihre Standardwerte zurücksetzen
&#x200B;* [Baking] Legen Sie beim Erstellen eines Projekts die Baking-Auflösung auf Malen fest.
&#x200B;* [Symmetrie] Binden Sie Symmetrie-spezifischen Manipulator von Tastaturbefehl Q ab.
&#x200B;* [Menü] Option &quot;Protokoll anzeigen&quot; im Hilfemenü hinzufügen
&#x200B;* [Viewport] Verbessern der Schatten-Rendering-Geschwindigkeit
&#x200B;* [Substance] Engine auf Version 9.0.1 aktualisieren
&#x200B;* [Farbmanagement] OCIO Konfigurationsdatei kann einen beliebigen Erweiterungstyp haben
&#x200B;* [Assets] Sbsar-Ressource mit der Verwendung von Aufklebern sollte automatisch auf Verkrümmungs-Projektion gesetzt werden.
&#x200B;* [Pfad] Meldung anzeigen, wenn versucht wird, mit dem Pfad-Werkzeug zu interagieren, während UI und Gizmos ausgeblendet sind

<b>Fest:</b>

&#x200B;* [Absturz] Alt + Ziehen im Pfadbedienfeld
&#x200B;* [Ressourcen importieren] Zufälliger Absturz beim Entfernen der zu importierenden Ressourcen
&#x200B;* Absturz beim Importieren einer komprimierten GLB-Datei
&#x200B;* Problem beim Malen auf Meshs, die UVs gemeinsam nutzen
&#x200B;* Mesh blinkt schwarz, wenn der Cache neu berechnet oder geladen wird
&#x200B;* [Eigenschaften] Kontextmenü zum Zurücksetzen von Parametern wird in Dropdown-Listen nicht angezeigt
&#x200B;* [Level] Eingangsregler durch vorherige Ebene gesperrt
&#x200B;* [AMD]&#x200B;[Weniger] SVT-Option, wenn aktiviert, erzeugt Artefakte
&#x200B;* [Projektion]&#x200B;[Verformen] Absturz beim Doppelklicken auf Scheitelpunkt
&#x200B;* Benutzeroberfläche und Pfad von [Pfad] im Baking-Modus
&#x200B;* [AMD] Textur verloren, wenn mit Sichtbarkeit gespielt wird
&#x200B;* [Gering] Die Auflösung ist zu niedrig, wenn Sie den Mesh umdrehen.

<b>Bekannte Probleme:</b>

&#x200B;* [Farbmanagement] HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen festgeklemmte Farben

### 9.0.0

Freigabedatum: <b>2023/06/20</b>
Zusammenfassung: <b>Hauptversion mit &quot;Paint along path&quot;, die 3D-Kurven, neue Basismaterialien und das Reinigen älterer Materialien sowie neue Vorgaben für 3D-Kurven ermöglicht</b>

<b>Hinzugefügt:</b>

&#x200B;* [Pfad] Neues Werkzeug &quot;entlang Pfad malen&quot; hinzufügen
&#x200B;* [Pfad] Hinzufügen eines leeren Tastaturbefehls für das Pfadwerkzeug
&#x200B;* [Pfad] Hinzufügen neuer Punkte zu einem vorhandenen Pfad zulassen
&#x200B;* [Pfad] Verknüpfung zum Beenden der aktuellen Pfaderstellung hinzufügen
&#x200B;* [Pfad] Bearbeiten der Pinseleigenschaften für Pfade zulassen
&#x200B;* [Pfad] Automatische Anpassung von Tangenten beim Platzieren eines Punkts
&#x200B;* [Pfad] Tangenten beim Verschieben eines Punkts neu berechnen
&#x200B;* [Pfad] Ausrichten neu erstellter Punkte an der Oberfläche eines Gitters
&#x200B;* [Pfad] Bearbeiten des Drucks pro Scheitelpunkt zulassen
&#x200B;* [Pfad] Anpassen des Drucks des neu erstellten Punkts von benachbarten Punkten
&#x200B;* [Pfad] Umwandeln von Punkten in Übergang/Ecke zulassen (Tangentenumbruch)
&#x200B;* [Pfad] Sofort einen neu hinzugefügten Punkt verschieben
&#x200B;* [Pfad] Punkte aus vorhandenem Pfad entfernen
&#x200B;* [Pfad] Umkehren der Richtung eines Pfads zulassen
&#x200B;* [Pfad] Auswahl eines Pfads im Darstellungsfenster zulassen
&#x200B;* [Pfad] Auswählen von Pfadpunkten mit dem Auswahlrechteck zulassen
&#x200B;* [Pfad] Einführung von STRG+A-Tastaturbefehlen zum Auswählen aller Punkte eines Pfads
&#x200B;* [Pfad] Schließen des Pfads zulassen
&#x200B;* [Pfad] Geben Sie unter &quot;Eigenschaften&quot; den Pfad um die Achse nach oben an.
&#x200B;* [Path] Hinzufügen eines Scheitelpunkt-Steuerungsmenüs zur kontextabhängigen Symbolleiste
&#x200B;* [Pfad] Hinzufügen von Mal-, Lösch- und Verwischen-Modi zum Pfadwerkzeug
&#x200B;* [Pfad] Erstellen von visuellem Feedback für Pfade im Viewport
&#x200B;* [Pfad] Hinzufügen eines visuellen Indikators für die Pfadrichtung
&#x200B;* [Path] Hinzufügen der Thickness zu den Anzeigeeinstellungen des Pfads
&#x200B;* [Path] Pfade ausblenden - Benutzeroberfläche
&#x200B;* [Pfad] Bedienfeld &quot;Pfad hinzufügen&quot; zur Liste der Pfade der aktuell ausgewählten Ebene
&#x200B;* [Pfad] Fügen Sie visuelles Feedback hinzu, wenn Sie den Mauszeiger über einen Pfad im Pfadbedienfeld bewegen
&#x200B;* [Pfad] Pfadbedienfeld anzeigen, wenn das Pfadwerkzeug ausgewählt ist
&#x200B;* [Pfad] Umbenennen, Löschen, Kopieren, Ausschneiden und Duplizieren von Pfaden im Bedienfeld &quot;Pfad&quot; zulassen
&#x200B;* [Pfad] Meldung anzeigen, wenn versucht wird, im 2D-Viewport mit dem Pfad-Werkzeug zu interagieren
&#x200B;* [Library] Integrieren neuer Inhalte (Pfad-Tools und -Basismaterial)
&#x200B;* [Dynamische Pinselstriche] Eigenschaft &quot;Abstand&quot; für Dynamische Pinselstriche hinzufügen
&#x200B;* [Dynamische Pinselstriche] Hinzufügen von Größen- und Abstand-Eigenschaften zu Dynamischen Pinselstrichen
&#x200B;* [Dynamische Pinselstriche] Hinzufügen der Eigenschaft &quot;Anfang&quot;, &quot;Mitte&quot; und &quot;Ende&quot; für Dynamische Pinselstriche
&#x200B;* [Python]&#x200B;[USD] Gelegt Projektkonfigurationsparameter für das USD
&#x200B;* [Python]&#x200B;[USD] Gelegt Projekterstellungsparameter für das USD
&#x200B;* [Exportieren]&#x200B;[USD] Fügen Sie Projektpfadinformationen innerhalb der exportierten USD hinzu
&#x200B;* [GLTF] Aktualisieren von Texturen in der Bibliothek beim erneuten Laden einer GLTF-Datei
&#x200B;* [Shader] Reduzieren von Artefakten in der Naht für UV-Inseln mit unterschiedlicher Ausrichtung
&#x200B;* [Engine] Update auf Substance Engine Version 9.0

<b>Fest:</b>

&#x200B;* [Importieren] Einige GLB mit Texturen erhalten keine Texturen in Painter
&#x200B;* [AMD] Artefakte an Rändern für alle 3D-Projektion-Flächen
&#x200B;* [Engine] Texturen brechen beim Umschalten der Ebenensichtbarkeit ab
&#x200B;* [Engine] Texturen sind an einigen Stellen leer, wenn der Mischmodus geändert wird
&#x200B;* [Engine] Textur/Projektion ist in einigen Fällen leerer Verkrümmungsmodus
&#x200B;* [Iray] Iteration wird beim Speichern des Renderings auf 0 zurückgesetzt
&#x200B;* [Log] USD Fehlermeldung beim Ausführen von Datei > Neu

<b>Bekannte Probleme:</b>

&#x200B;* [Farbmanagement] HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen festgeklemmte Farben
&#x200B;* [Ebenenstapel] Eingabequelle nicht pro Ebene gespeichert

## Version 8

### 8.3.1

Freigabedatum: <b>2023/04/27</b>

<b>Hinzugefügt:</b>

&#x200B;* [Baking-Modus] Hinzufügen (leeren) Tastaturbefehl, um den Viewport anzuzeigen/auszublenden
&#x200B;* [Baking führend Modus] Bei Verwendung der Schaltfläche &quot;Baking führend Mesh ausblenden&quot; immer niedrige Poly-Werte anzeigen
&#x200B;* [Baking Mode] Suffix für &quot;Matching By Name&quot; basierend auf aktuellem Textursatz anzeigen
&#x200B;* [Import] Unterstützung für GLTF-Binärdateien (glb) hinzufügen
&#x200B;* [Liste der Textursatz] Menü &quot;Hinzufügen&quot;, um Shader-Instanzen auszuwählen oder zu erstellen
&#x200B;* [Liste der Textursatz] Schnelles Ändern der Auflösung von Textursatz und UV-Kachel
&#x200B;* [Physische Größe] Verbessern des Manipulator-Verhaltens bei Verwendung von Physische Größe in UV-Projektion
&#x200B;* [UI] &quot;Speichern unter&quot; wieder im Hauptmenü &quot;Datei&quot; anzeigen
&#x200B;* [UI] Speichern der Ansichtsauswahl (nur 2D, nur 3D, beide) im UI-Layout
&#x200B;* [USD] Weniger vage Fehlermeldung bei der Projekterstellung mit nicht unterstützten USD
&#x200B;* [Python] Hinzufügen von Baking führend Ereignissen, um dem Fortschritt des Bakings zu folgen
&#x200B;* [Python] Abbrechen eines Baking zulassen
&#x200B;* [Python] Leg &quot;Basierend auf Ausgabevorlage&quot; für Dateityp und Bittiefe beim Export
&#x200B;* [Python] Gelegt Aktualisierungszeit für TextureStateEvent.Update

<b>Fest:</b>

&#x200B;* [Absturz] Seltener Absturz beim Schließen eines Projekts
&#x200B;* [Absturz] [Baking] Aktivieren der Mesh-Map-Synchronisierung mit dem Height oder der Krümmung für ein bestimmtes Projekt
&#x200B;* [Absturz]&#x200B;[Skripterstellung] Absturz beim Hinzufügen eines Materials nach der Erstellung einer Shader-Instanz
&#x200B;* [Baking Mode] AO-Intensität im neutralen Material hat keine Auswirkung
&#x200B;* [Baking-Modus] Absturz beim Wechseln in den Baking-Modus vor dem Laden des Modells
&#x200B;* [Baking führend Modus] Fehlende Fehlermeldung auf der Registerkarte &quot;Baking führend Prozess&quot;
&#x200B;* [Baking-Modus] Einstellungen für neutrale Material haben nach dem erneuten Importieren eines Meshs keine Auswirkungen
&#x200B;* [Modustrennzeichen] Viewport-Trennzeichen werden global und nicht pro Baking gespeichert.
&#x200B;* [Baking führend Modus] Visualisierungsproblem: Durchschnittliche Normale verändert die Oberfläche des Käfigs nicht
&#x200B;* [Farbmanagement] Die Einstellung &quot;Farbraum automatisch erkennen&quot; ist deaktiviert, wenn OCIO env var vorhanden ist
&#x200B;* [Inhalt] Der Maskenkonturfilter weist ein Artefakt mit Height-Eingabe auf.
&#x200B;* [Inhalt] Regler für die Intensität des Steigung-Weichzeichnungsfilters ist bei 1,0 eingeklemmt
&#x200B;* [Interop] Projekt mit GLTF kann nicht aus Sampler erstellt werden
&#x200B;* [Ebenenstapel] Der Wert für die Kachelung der Projektion wird nicht korrekt mit dem Manipulator aktualisiert.
&#x200B;* [Linux] Versatz zwischen Grafiktablett-Stift und Cursor mit einem HDPI von mehr als 100 %
&#x200B;* [Python] Absturz beim erneuten Importieren eines Meshs nach dem Erstellen eines Projekts
&#x200B;* [Substance] 3D-Rauschen werden nach dem erneuten Importieren eines Meshs beschädigt
&#x200B;* [UV-Kacheln] Offset für UV-Projektion auf 1 geklemmt
&#x200B;* [Viewport] Visuelles Feedback für gerade Linien ist nicht mehr sichtbar
&#x200B;* [WhatsNew] Falscher Zeilenumbruch bei Funktionstiteln

<b>Bekannte Probleme:</b>

&#x200B;* [Importieren] Einige GLB mit Texturen erhalten keine Texturen in Painter

### 8.3.0

*(Freigegeben: 10. Januar 2023)*
Zusammenfassung: <b>Hauptversion mit neuem Importmodus, neuem Baking und Export von USD und Physische Größe-Unterstützung für UV-Projektion</b>

<b>Hinzugefügt:</b>

&#x200B;* [Baking führend Modus] Neuer Baking führend Modus, der dem Baking führend Prozess gewidmet ist
&#x200B;* [Baking-Modus] Stellen Sie den Tastaturbefehl so ein, dass er in den Baking-Modus auf F8 wechselt.
&#x200B;* [Baking-Modus] Hinzufügen der Schaltfläche &quot;Start&quot; und &quot;Baking abbrechen&quot; im Viewport
&#x200B;* [Baking führend Modus] Hinzufügen einer Baking führend Auswahl zur Liste der Textursatz
&#x200B;* [Backmodus] Neues Fenster &quot;Gitterzuordnungs-Bäcker&quot; hinzufügen, um Bäcker auszuwählen
&#x200B;* [Backing-Modus] Neues Fenster &quot;Gitterzuordnungs-Einstellungen&quot; hinzufügen, um Backing-Einstellungen zu bearbeiten
&#x200B;* [Backing Mode] Neues Backing Log-Fenster hinzufügen, um Backing-Prozess zu verfolgen
&#x200B;* [Backing Mode] Backing-Parameter hinzufügen und Aktionen im Verlaufsfenster rückgängig machen
&#x200B;* [Backing-Modus] Hinzufügen von Breadcrumbs in den Mesh-Map-Einstellungen
&#x200B;* [Backmodus] Hinzufügen von Mesh Maps-Miniaturansichten im Fenster &quot;Gitter-Map-Bäcker&quot;
&#x200B;* [Backmodus] Menü &quot;Visualisierungseinstellungen reduzierbar&quot; im 3D-Viewport hinzufügen
&#x200B;* [Backmodus] Fügen Sie eine Visualisierungseinstellung hinzu, um das High-Poly-Gitter ein- oder auszublenden
&#x200B;* [Backmodus] Visualisierungseinstellung hinzufügen, um das Gitter und das Drahtgitter des Käfigs ein- bzw. auszublenden
&#x200B;* [Backmodus] Fügen Sie eine Visualisierungseinstellung hinzu, um das Gitter mit der niedrigen Poly-Intensität ein- oder auszublenden.
&#x200B;* [Backmodus] Hinzufügen einer Visualisierungseinstellung, um harte Kanten ohne UV-Nähte als Fehler anzuzeigen
&#x200B;* [Backing Mode] Informieren Sie im Viewport über Gitter- und Backing-Fehler, wenn das Backing-Protokoll nicht sichtbar ist
&#x200B;* [Backmodus] Aktion hinzufügen, um die Backeinstellungen für alle Textursätze zu synchronisieren

  Im Fenster &quot;Gitter-Map-Bäcker&quot; kann jeder Bäcker (sowie die allgemeinen Einstellungen) über Textursätze hinweg synchronisiert werden, indem Sie auf das Verknüpfungssymbol neben seinem Namen klicken. Durch diese Aktion wird ein Fenster geöffnet, in dem Sie auswählen können, welche Textursätze dieselben Parameter verwenden sollen.

&#x200B;* [Backmodus] Hinzufügen von Aktionen zum Kopieren und Einfügen von Backereinstellungen

  Im Fenster &quot;Gitterzuordnungs-Bäcker&quot; stehen Aktionen zum Kopieren und Übergehen der einzelnen Bäckereinstellungen über Textursätze entweder über das spezielle Menü oben im Fenster oder das Kontextmenü mit der rechten Maustaste zur Verfügung.

&#x200B;* [Backing Mode] Schaltfläche Hinzufügen im Backing Log, um von Fehler zu den richtigen Einstellungen zu springen

  Wenn ein Bäcker ausfällt oder ein Gitter nicht ordnungsgemäß geladen wird, wird im Backprotokoll eine Fehlermeldung angezeigt. Mit einer Schaltfläche neben der Meldung können Sie das Fenster Gitterzuordnungs-Bäcker und Gitterzuordnungs-Einstellungen ändern, um die zugehörigen Einstellungen anzuzeigen. Dies hilft dabei, die Ursache eines Problems einfacher zu isolieren, um es beheben zu können.

&#x200B;* [Backmodus] Hinzufügen von Menüs zum Verwalten von Textursätzen und Bäcker-Auswahlen

  Sowohl in der &quot;Texture Set-Liste&quot; und &quot;Mesh Map Bakers&quot; Fenster wurden ein kleines Action-Menü hinzugefügt, um zu kopieren, invertieren Auswahlen.

&#x200B;* [Backmodus] Baker-Auswahlliste nach Textursatz teilen
&#x200B;* [Backmodus] Teilen allgemeiner Einstellungen pro Textursatz
&#x200B;* [Backmodus] Laden von High-Poly- und Käfigmaschen ohne Einfrieren der Schnittstelle
&#x200B;* [Backmodus] Verwenden Sie die Viewport-Fortschrittsleiste, um die Gitterbelastung anzuzeigen
&#x200B;* [Backing-Modus] Hinzufügen des Netzladestatus im Backing-Protokoll
&#x200B;* [Backmodus] Umkehren des Gitters im Viewport während des Backens zulassen
&#x200B;* [Backmodus] Backreihenfolge basierend auf der aktuellen Gittersichtweite des Ports festlegen
&#x200B;* [Backmodus] Anzeige des impliziten Backkäfigs im Viewport

  Wenn Sie keine benutzerdefinierte Gitterdatei für den Käfig verwenden, wird ein automatisches Gitter für den Käfig generiert und im Viewport angezeigt. Die Größe basiert auf dem Parameter &quot;Max. Frontalentfernung&quot; der üblichen Backeinstellungen. Das Gitter des Käfigs wird verwendet, um anzuzeigen, wie weit die Anpassung zwischen dem niedrigen und dem hohen Poly gehen wird.

&#x200B;* [Backing-Modus] Übereinstimmende Liste von Gitternamen für &quot;Übereinstimmender Name&quot; im Backing-Protokoll anzeigen
&#x200B;* [Backmodus] Verwenden Sie neutrales Material, um das 3D-Modell im Viewport anzuzeigen.
&#x200B;* [Backing-Modus] Deaktivieren der Engine-Berechnung im Backing-Modus
&#x200B;* [Backmodus] Beim Beenden der App während des Backens wird eine Warnung angezeigt
&#x200B;* [Bäcker] Aktualisieren der Beschriftungen für Anti-Aliasing-Einstellungen

  Die Einstellungswerte für das Anti-Aliasing wurden in &quot;Supersampling&quot; umbenannt und mit einer expliziten Multiplikatornummer versehen, um das Verhalten zu verdeutlichen.

&#x200B;* [Bakers] Aktualisieren Sie Bakers auf Version 2.5.7.
&#x200B;* [USD] Importieren und Exportieren von Universal Scene Description (USD)-Dateien
&#x200B;* [USD] Hinzufügen von USD-Optionen zum Fenster &quot;Neues Projekt&quot;, wenn Sie eine USD-Datei auswählen
&#x200B;* [USD] Neues Auswahlfenster für Umfang und Varianten hinzufügen

  Wenn Sie eine USD-Datei importieren, können Sie durch Klicken auf die Schaltfläche &quot;Ändern&quot; im Fenster &quot;Neues Projekt&quot; oder &quot;Projektkonfiguration&quot; auswählen, welcher Teil und welche Varianten einer USD-Datei importiert werden sollen.

&#x200B;* [USD] Option &quot;Unterteilungsebenen hinzufügen&quot;

  Wenn Sie ein neues Projekt mit einer USD-Gitterdatei erstellen, die Unterteilungen enthält, können Sie die Ebene der Unterteilungen mithilfe eines Schiebereglers auswählen. Das Projekt wird mit dem unterteilten Gitter erstellt. Die Ebene kann über die Projektkonfiguration geändert werden.

&#x200B;* [USD] Importieren von in USD gehäuften Netzen in einem bestimmten Frame

  Wenn Sie ein neues Projekt mit einer USD-Gitterdatei erstellen, die Animationen enthält, können Sie den Frame mit einem Schieberegler auswählen, der die eingebettete Timeline-Sequenz widerspiegelt. Der Frame kann über die Projektkonfiguration geändert werden.

&#x200B;* [USD]&#x200B;[Exportieren] Fügen Sie eine Option zum Exportieren von USD-Dateien hinzu.

  Das neue Kontrollkästchen &quot;USD exportieren&quot; wurde dem Fenster &quot;Texturen exportieren&quot; hinzugefügt. Wenn diese Option aktiviert ist, können Sie USD-Dateien sowie Texturmaps aus beliebigen Vorlagen exportieren.

&#x200B;* [USD]&#x200B;[Exportieren] Fügen Sie dem Gitterexport das USD-Dateiformat hinzu.
&#x200B;* [USD] Benennen Sie die vorhandene Exportvoreinstellung &quot;USD PBR Metal Roughness&quot; um, um ein expliziteres Format zu erhalten

  Die USD-Exportvorlage, die zuvor als &quot;USD PBR Metal Roughness&quot; bekannt war, ist weiterhin über &quot;Texturen exportieren&quot; > &quot;Ausgabevorlage&quot; > &quot;USDz&quot; (Apple AR) verfügbar.

&#x200B;* [Automatisch entpacken] Ausrichtung für Packing sperren hinzufügen

  Neue Option für Einstellungen zum automatischen Ausgliedern, mit der die Ausrichtung vorhandener UV-Inseln beibehalten werden kann, wenn die Funktion &quot;Packing&quot; verwendet wird. Der Zugriff darauf erfolgt über &quot;Neues Projekt&quot; > &quot;Optionen zum automatischen Ausgliedern&quot; > &quot;Ausrichtung der UV-Insel&quot;.

&#x200B;* [Physische Größe] Fügen Sie eine Einstellung hinzu, um die Physische Größe automatisch in Fülleffekt/Ebene zu verwenden.

  Es wurde eine neue Option hinzugefügt, mit der bei Verwendung eines Materials mit eingebetteter Physische Größe automatisch zur Physische Größe-Skala gewechselt werden kann. Sie kann pro Projekt über &quot;Neues Projekt&quot; oder über &quot;Bearbeiten&quot; > &quot;Projektkonfiguration&quot; > &quot;Physische Größe&quot; > &quot;Beim Zuweisen von Materialien Füllebenenskalierung auf Physische Größe umschalten&quot; aktiviert werden.

&#x200B;* [Physische Größe] Physische Größe für UV-Projektion verfügbar machen

  Physische Größe-Skalierung ist jetzt für UV-Projektionen verfügbar - sie ermöglicht die automatische Größenänderung für ein Material basierend auf der Physische Größe eines Gitters. Sie kann über &quot;Skalieren > Physische Größe&quot; in der Füllebene oder im Effekteigenschaftsfenster ausgewählt werden.

&#x200B;* [Scripting]&#x200B;[Python] Abfrage der Anwendungsversion zulassen
&#x200B;* [Scripting]&#x200B;[JavaScript] Update-API für neue Backing-Parameter
&#x200B;* [Scripting]&#x200B;[Python] Backmodul: Backparameter bearbeiten
&#x200B;* [Scripting]&#x200B;[Python] Backmodul: Backen starten/abbrechen
&#x200B;* [Scripting]&#x200B;[Python] Backmodul: Methode der selektierten Krümmung
&#x200B;* [Scripting]&#x200B;[Python] Backmodul: Auswahl an Bäckereien/UV-Fliesen
&#x200B;* [Scripting]&#x200B;[Python] Backmodul: Bäckereinstellungen für alle Textursätze synchronisieren
&#x200B;* [SVT] Aktivieren der Unterstützung für wenig Hardware auf AMD-GPUs

  Die Hardwarebeschleunigung für das Dünn besetzte virtuelle Textur-System kann jetzt mit AMD-GPUs aktiviert werden. Diese Einstellung wird in den allgemeinen Voreinstellungen automatisch aktiviert.

&#x200B;* [Projektion] Parameter für zylindrische Projektion umbenennen

  Der Parameter &quot;Cylinder Cap Culling&quot; wurde in &quot;Rückseiten-Ausblendung&quot; umbenannt, um seine Wirkung besser darzustellen. Die zugehörige QuickInfo wurde entsprechend angepasst.

&#x200B;* [Project] Speichern Sie die Anwendungsversion im Projekt und rufen Sie sie über Skripterstellung ab.

  Seit Version 8.2 wird die Version der Anwendung beim Speichern in der spp-Datei gespeichert.
  Diese Versionsnummer kann mit der Funktion last\_saved\_substance\_painter\_version() im Projektmodul der Python-API abgerufen werden.
  Für Projekte, die vor 8.2 erstellt wurden, ist der zurückgegebene Wert null.

&#x200B;* [Import] Verbessern der allgemeinen Importzeit von 3D-Modellen

  Wir haben die allgemeine Importzeit von Meshs verbessert. Zum Beispiel die Verkürzung der Wartezeit beim Laden von High-Poly-Meshs zum Baking. Diese Optimierung gilt insbesondere für das Laden von OBJ.

<b>Fest:</b>

&#x200B;* [Absturz] Ändern von Kanälen bei Filtern mit bestimmtem Stapel
&#x200B;* [Mac]&#x200B;[M1] Absturz beim Erstellen einer Füllebene und beim Verlassen des Ebenenstapels

  Dieses Problem kann durch Aktualisieren auf Mac OS 13 (Ventura) behoben werden.

&#x200B;* [Scripting]&#x200B;[Python] Absturz bei Verwendung von ui.add\_dock\_widget() mit falschem Typ
&#x200B;* [Baking] Unvollständige Fehlermeldung im Protokoll, wenn ein Baking fehlschlägt
&#x200B;* [Baking] Speicher wird nach Abschluss des Bakings nicht freigegeben
&#x200B;* [Engine] Texturen-Cache wird nicht aktualisiert, wenn die Effektsichtbarkeit geändert wird
&#x200B;* [Exportieren] 2D-Ansicht exportiert zufällig einheitliche Map
&#x200B;* [Projekt] Speicherzuordnungsfehler beim Speichern eines Projekts mit großem Mesh
&#x200B;* [Viewport] TAA verursacht Artefakte beim Malen in einigen Fällen

<b>Bekannte Probleme:</b>

&#x200B;* [Farbmanagement] HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen festgeklemmte Farben
&#x200B;* [Ebenenstapel] Eingabequelle nicht pro Ebene gespeichert

### 8.2.0

*(Freigegeben: 6. Oktober 2022)*
Zusammenfassung: **Hauptversion mit neuen Onboarding-Bedienfeldern (neues Begrüßungs-Bedienfeld und neues Bedienfeld), Export in SBSAR, Effekten für Ordner, mehreren Verbesserungen für die Lebensqualität und Fehlerbehebungen.**

**Hinzugefügt:**

&#x200B;* [Onboarding] Onboarding-Bereich zur Begrüßung neuer Benutzer

  Es wurde ein neuer Begrüßungsbildschirm hinzugefügt, wenn neue CC-Benutzer Painter zum ersten Mal öffnen.

&#x200B;* [Onboarding] Neuerungen im Bedienfeld zur Verbesserung der Auffindbarkeit neuer Funktionen

  Es wurde ein neuer Bildschirm &quot;Neue Funktionen&quot; hinzugefügt, auf dem die wichtigsten neuen Funktionen angezeigt werden. Es wird automatisch angezeigt, wenn Painter nach einem wichtigen Update zum ersten Mal geöffnet wird, und Sie können erneut auf es über Hilfe > Neue Funktionen zugreifen.

&#x200B;* [Onboarding] Alten Begrüßungsbildschirm in &quot;Startseite&quot; umbenennen

  Alter Begrüßungsbildschirm wurde in Startbildschirm umbenannt, um Verwechslungen mit dem neuen Begrüßungsbildschirm zu vermeiden.

&#x200B;* [UI] Beheben von Skalierungsproblemen für Bildschirme mit hoher DPI

  Verbesserte Anpassung der Painter-Benutzeroberfläche auf HD-Bildschirmen mit benutzerdefinierter Anzeigeskalierung.

&#x200B;* [UI] Vermeiden Sie persistente Fehlermeldungen in der Benutzeroberfläche

  Fehlermeldungen aus vorherigen Projekten werden jetzt aus der unteren Statusleiste entfernt.

&#x200B;* [UI] Menü zum Speichern von Überarbeitung

  Zusätzliche Speicheroptionen sind jetzt in einem Untermenü gruppiert und einige werden aus Konsistenzgründen umbenannt.

&#x200B;* [UI] Speichern und Exportieren/Freigeben von UI-Layouts

  Im Menü &quot;Fenster&quot; (Window) gibt es neue Aktionen, mit denen Sie das UI-Layout in Dateien speichern und neu laden können. Die Layouts &quot;Malen&quot; und &quot;Rendern&quot; werden separat gespeichert.
  &quot;substance\_painter.ui&quot; wurde um verschiedene Funktionen erweitert, mit denen auch UI-Layouts gespeichert, zurückgesetzt und geladen werden können.

&#x200B;* Hinzufügen von Kopier-/Einfügeaktionen für Mischmodi/Deckkraft einer Ebene

  Es wurde ein neuer Eintrag &quot;Fülloptionen&quot; im Kontextmenü von Ebenen hinzugefügt. Damit können Sie den Mischmodus und die Deckkraft aller Kanäle von einer Ebene in eine andere kopieren und einfügen.

&#x200B;* Mischmodus/Deckkraft auf alle Kanäle einer Ebene anwenden

  Dem Mischmodus und der Deckkraft von Ebenen wurde eine Rechtsklick-Funktion hinzugefügt, mit der die derzeit angeklickte Einrichtung auf alle Kanäle angewendet werden kann.

&#x200B;* Mesh mit einem Tastatur-Tastaturbefehl neu laden (STRG+UMSCHALT+R)

  Es wurde ein bearbeitbarer Tastaturbefehl hinzugefügt, um die Meshdatei mit den zuletzt verfügbaren Einstellungen neu zu laden. Sie können auch über Bearbeiten > Mesh erneut importieren darauf zugreifen.

&#x200B;* Substance-Parameter auf die Standardeinstellungen zurücksetzen

  Es wurde eine neue Schaltfläche in den Eigenschaften am unteren Rand von .sbsar-Ressourcen hinzugefügt, mit der die Ressource auf die Standardeinstellungen zurückgesetzt werden kann.

&#x200B;* Malen-Pinsel auf die Standardeinstellungen zurücksetzen

  Es wurde ein neues Menü zum Abschnitt &quot;Pinsel&quot; in den Eigenschaften hinzugefügt, über das Sie den Standard-Standardpinsel zurücksetzen können.

&#x200B;* Rechtsklick zum Zurücksetzen der einzelnen Substance-Parameter auf die Standardeinstellungen

  Es wurde die Möglichkeit hinzugefügt, einzelne Parameter innerhalb einer .sbsar-Ressource per Rechtsklick zurückzusetzen.

&#x200B;* [Bedienfeld &quot;Elemente&quot;] Favoritenelemente &quot;Nadel&quot; werden oben im Bedienfeld &quot;Elemente&quot; angezeigt

  Es wurde eine neue Option zum Klicken mit der rechten Maustaste hinzugefügt, um Elemente zu bibliothekieren, mit der sie oben im Bedienfeld als Favoriten Nadel werden können. Sie können auch alle Ihre bevorzugten Assets über &quot;Gespeicherte Suchen&quot; anzeigen.

&#x200B;* [Bedienfeld &quot;Elemente&quot;] Elemente löschen, neu laden und umbenennen

  Kontextmenüoptionen zum Löschen, erneuten Laden und Umbenennen von Elementen in der Benutzerbibliothek wurden hinzugefügt. Sie werden direkt aus ihrem Bibliotheksspeicherort auf der Festplatte gelöscht und vom ursprünglichen Speicherort neu geladen. Elemente, die Teil eines Pakets wie .abr oder .sbsar sind, können nicht einzeln bearbeitet werden.

&#x200B;* [Farbauswahl] Füllen des Effekts &quot;Farbauswahl&quot; mit Füllmethoden
&#x200B;* [Ebenenstapel] Hinzufügen von Füllmethode und Deckkraft für Filter
&#x200B;* [Ebenenstapel] Kachelung-Werte größer als 128 für Füllebene/Effekte zulassen
&#x200B;* [Ebenenstapel] Zylinderdeckel für zylindrische Projektion in Füllebene/Wirkung

  Bei der zylindrischen Projektion in den Eigenschaften der Füllebene haben Sie jetzt die Möglichkeit, Zylinderkappen zu entfernen.

&#x200B;* [Protokoll] Fehlermeldung anzeigen, wenn sich ein Mesh-Teil beim Erstellen eines UV-Kachel-Projekts in einem negativen Bereich befindet

  Es wurde eine deutlichere Fehlermeldung hinzugefügt, wenn ein UV-Kachel-Projekt nicht erstellt werden kann, da UV-Teile in Leerzeichen gefunden werden.

&#x200B;* [Project] Geben Sie beim Öffnen eines Projekts die Version in der Fehlermeldung &quot;Daten zu aktuell&quot; an.

  Wenn Sie ein Projekt öffnen, das für die Anwendung zu neu ist, wird in der Fehlermeldung jetzt die Version des Projekts angezeigt, damit Sie die richtige Anwendungsversion leichter erkennen können.

&#x200B;* [Viewport] Lassen Sie den Mesh von unten beleuchten

  Ein neuer Parameter für die Umgebungsausrichtung wurde unter Anzeigeeinstellungen > Kamera > Umgebungseinstellungen hinzugefügt, um die Umgebungs-Map-Beleuchtung an der Kamera auszurichten, wenn sie auf &quot;Lokal&quot; eingestellt ist.

&#x200B;* [Viewport] Anzeigen von R, G, B und Alpha im Viewport (Einzelanzeigemodus)

  Unter Anzeigeeinstellungen > Kanaleinstellungen > Kanalanzeige gibt es eine neue Farbkanaleinstellung, mit der nur die R-, G-, B- oder Kanalkomponente eines Viewports im Einzelanzeigemodus angezeigt werden kann.

&#x200B;* [Shader] Benutzerkanäle als RGBA in Material-Layer-Shadern festlegen

  Bei der Einstellung der Kanalkonfiguration innerhalb eines Shader für die Kanalschichtung ist es nun möglich, das Textursatz des Materials so festzulegen, dass es vom Standardwert abweicht. Auf diese Weise können Benutzer-Farbkanäle anstelle von Graustufen angefordert werden.

&#x200B;* [Exportieren] Exportieren von Texturen als SBSAR zulassen

  Beim Exportieren von Texturen über das Fenster Datei > Texturen exportieren kann das Dateiformat SBSAR (Substance Archive) ausgewählt werden, um sie neu zu gruppieren. Der Inhalt des SBSAR richtet sich nach der verwendeten Ausgabevorlage.
  Das Datenformat kann auch in den Exportvorgaben festgelegt werden. Bei Verwendung einer Hybridkonfiguration (SBSAR + Anderes Format) werden Texturen, die ein SBSAR betreffen, gruppiert, während der Rest parallel exportiert wird.

&#x200B;* [Exportieren] 16-Bit-Option für EXR Dateiformat Gelegt

  Beim Exportieren EXR Textur-Dateien können Sie jetzt im Fenster &quot;Exporteinstellungen&quot; die Texturen 16f Bit (halbe Fließkommazahl) oder 32f Bit (Fließkommazahl) auswählen (sowohl für Exporteinstellungen als auch Exportvorgaben). Alte Projekte und alte Exportvorgaben werden standardmäßig auf 16f Bit gesetzt, um das alte Verhalten widerzuspiegeln.

&#x200B;* [Python] Ereignis hinzufügen, um zu wissen, wann Textursatz geändert werden

  Der neue &quot;substance\_painter.event.TextureStateEvent&quot; gibt Aufschluss darüber, ob ein Textursatz entweder aufgrund eines Malen-Strichs, eines hinzugefügten oder eines entfernten Kanals geändert wurde.

&#x200B;* [Python] Abrufen und Festlegen von Mesh-Map-Ressourcen in den Textursatz-Einstellungen zulassen

  Neue Funktionen wurden im Modul &quot;substance\_painter.project&quot; hinzugefügt, um Mesh-Map-Ressourcen abzurufen und einzurichten. Diese Funktionen können verwendet werden, um die Mesh-Map zu aktualisieren, auf die in den Textursatz-Einstellungen verwiesen wird.

&#x200B;* [Plug-ins] Option entfernen, um andere JS-Plug-ins zu erhalten

  Die Option, JavaScript-Plug-ins abzurufen, wurde entfernt, da sie auf der veralteten Freigabe-Website gehostet wurden.

&#x200B;* [Inhalt] Neue Roblox-Vorlage hinzufügen und Vorgabe exportieren

  Eine neue Roblox-Projektvorlage &quot;Materialvariante&quot; und &quot;Oberflächenerscheinung&quot; sowie eine Exportvorgabe wurden hinzugefügt, um den Export von PBR-Texturen nach Roblox zu erleichtern. Auf die Vorlage kann über das Fenster Datei > Neues Projekt zugegriffen werden.

&#x200B;* Substance Engine auf die neueste Version (8.6.3) aktualisieren
&#x200B;* [Steam] Optimierter Build für Apple Silicon Chipsatz (Apple M1 / M2)

**Fest:**

&#x200B;* Absturz bei Verwendung von 16k exr
&#x200B;* [Absturz] Strg Z Nach dem Löschen einer Shader-Instanz
&#x200B;* [Iray] IoR ist für einige Shader auf 1 blockiert
&#x200B;* [Win]&#x200B;[Backen] Einige High-Poly-Fehler beim Laden
&#x200B;* [Farbmanagement] Falscher Farbraumname in der Benutzeroberfläche mit Filtern
&#x200B;* [Python] Von der Importfunktion zurückgegebene Ressourcenobjekte haben keinen Typ

  Beim Importieren eines Substance-Pakets in Python gab die Funktion das Paket zurück, anstelle der Diagramme. Das Ressourcenmodul stellt nun Funktionen und Parameter bereit, um die Graphen eines Substance-Pakets abzurufen.

**Bekannte Probleme:**

&#x200B;* [Farbmanagement] HDR-Farbraumkonvertierungen mit ACE unter Linux erzeugen festgeklemmte Farben
&#x200B;* [Ebenenstapel] Eingabequelle nicht pro Ebene gespeichert
&#x200B;* [Malen] Zeitweiliges Anti-Aliasing verursacht beim Malen in einigen Fällen Artefakte
&#x200B;* [Exportieren] 2D-Ansicht exportiert zufällig einheitliche Karte

### 8.1.3

*(Freigegeben: 25. August 2022)*
Zusammenfassung: **Geringfügige Fehlerbehebungsversion**

**Hinzugefügt:**

&#x200B;* Update auf Iray SDK 1.6

**Fest:**

&#x200B;* [Shader] Absturz mit altem fehlerhaften Shader
&#x200B;* [Materialebenen] Materialien können beim erneuten Öffnen eines Projekts verschwinden

**Bekannte Probleme:**

&#x200B;* [Farbmanagement] HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen festgeklemmte Farben
&#x200B;* [Ebenenstapel] Eingabequelle nicht pro Ebene gespeichert
&#x200B;* [Absturz] Strg Z Nach dem Löschen einer Shader-Instanz
&#x200B;* [Iray] IoR ist bei einigen Shadern auf 1 blockiert

### 8.1.2

*(Freigegeben: 19. Juli 2022)*
Zusammenfassung: **Geringfügige Fehlerbehebungsversion**

**Hinzugefügt:**

&#x200B;* [Automatisch Entpackt] Neue Option &quot;Für organische Mesh optimieren&quot; zur Auswahl des Segmentierungsalgorithmus
&#x200B;* [Physische Größe] Gelegt Einheitsoptionen in &quot;Neues Projekt&quot; und &quot;Projektkonfiguration&quot;
&#x200B;* [Farbmanagement] Verwenden Sie die Monitoranzeige standardmäßig, wenn Sie ACE
&#x200B;* [Farbmanagement]&#x200B;[Python] Berücksichtigen Sie ACE env-var-Vorgabedatei beim Erstellen von Projekten
&#x200B;* [Farbmanagement] Setzen Sie die Farbmanagement-Einstellungen im Fenster &quot;Neues Projekt&quot; zurück, wenn sich die Konfiguration ändert
&#x200B;* [Farbmanagement] Deaktivieren Sie den Zugriff auf die OCIO, wenn env-var vorhanden ist
&#x200B;* [Farbmanagement] Sicheres Aktualisieren ACE Einstellungen, wenn ein Parameter nicht mehr vorhanden ist
&#x200B;* Substance Engine auf Version 8.6.0 aktualisieren
&#x200B;* [Exportieren] Fügen Sie eine neue GLTF-Exportvorgabe mit Versatz-Unterstützung hinzu
&#x200B;* [Scripting]&#x200B;[Python] Abrufen von Ressourceninformationen (einschließlich benutzerdefinierter Metadaten)
&#x200B;* [Scripting]&#x200B;[Python] Funktion zur Abfrageliste der Mesh pro Textursatz hinzufügen
&#x200B;* [Inhalt] Neue Mischervorlage hinzufügen und Vorgabe exportieren

**Fest:**

&#x200B;* [MacOS] Absturz beim Starten von Iray in einigen Fällen
&#x200B;* [Miniaturansichten] Regal-Miniaturansichten werden nicht richtig geladen
&#x200B;* Mehrere UV-Kanäle werden ignoriert.
&#x200B;* [Automatisch Entpackt] Unnötige Berechnung beim Aufteilen langer Inseln
&#x200B;* [Automatisches Auspacken] Option zur Vermeidung länglicher Inseln, die nicht berücksichtigt werden
&#x200B;* [Automatisches Auspacken] Verlust zusätzlicher Daten (Scheitelpunktfarben) beim Umpacken von UVs
&#x200B;* [UI] Horizontale Bildlaufleiste im Eigenschaftsfenster, wenn Farbmanagement aktiviert ist
&#x200B;* [Farbmanagement] OCIO-Konfigurationen fehlen substance\_3d\_painter\_standard\_srgb
&#x200B;* [Generator] Falsche Verwendung von Benutzerdaten &quot;deaktiviert&quot;
&#x200B;* [Farbmanagement] Dropdown-Liste &quot;Nicht kompatibel&quot; für Farbraum sollte nicht klickbar sein
&#x200B;* [Farbmanagement]&#x200B;[Shader] sRGB override define funktioniert nicht mehr
&#x200B;* [Generator] Falsche Verwendung von Benutzerdaten &quot;deaktivieren&quot;
&#x200B;* [Ebenenstapel] Fehlerhafte Vorschauen mit UV-Kacheln-Projekten
&#x200B;* [Shader] API-Dokumentation ist nicht vollständig auf dem neuesten Stand mit gebogenen Normalen
&#x200B;* [Export]&#x200B;[Interoperabilität] Kann nicht mit Sonderzeichen an Stager gesendet werden.
&#x200B;* [Inhalt] Einige Miniaturen von Pinselvorgaben sind leer oder zu dunkel

**Bekannte Probleme:**

&#x200B;* [Farbmanagement] HDR-Farbraumkonvertierungen mit ACE unter Linux erzeugen festgeklemmte Farben
&#x200B;* [Ebenenstapel] Eingabequellen werden nicht pro Ebene gespeichert
&#x200B;* [Absturz] Strg Z Nach dem Löschen einer Shader-Instanz
&#x200B;* [Iray] IoR ist für einige Shader auf 1 blockiert
&#x200B;* [Shader] Absturz mit altem fehlerhaften Shader

### 8.1.1

*(Freigegeben: 28. Juni 2022)*
Zusammenfassung: **Minor Release-Hotfix**

**Hinzugefügt:**

&#x200B;* [Ebenenstapel] Mit Alt-Klick auf Maske wird die Auswahl von Effekten nicht mehr aufgehoben

**Fest:**

&#x200B;* [Absturz] Öffnen des alten Projekts im Einzelansichtsmodus gespeichert
&#x200B;* [Absturz] Löschen eines Generators in den Eigenschaften
&#x200B;* [Textursatz-Einstellungen] Normale/Ambient occlusion-Abmischung und Height-zu-Normal-Methoden sind fehlerhaft
&#x200B;* [Exportieren] Exportieren von Texturen mit Diffusion-Innenabständen rendert schwarze Maps

**Bekannte Probleme:**

&#x200B;* [MacOS] Absturz beim Starten von Iray auf Monterey
&#x200B;* [Vorschau-Miniaturansicht] Vereinfachte Miniaturansichten werden nicht aktualisiert, wenn ein Anker verwendet wird
&#x200B;* [Farbmanagement] HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen festgeklemmte Farben

### 8.1.0

*(Freigegeben: 7. Juni 2022)*
Zusammenfassung: **Hauptversion mit ICC-Unterstützung, Material-Skalierung auf der Grundlage von Physische Größe-Daten, neue Baker, Verbesserungen an der FarbPipette und eine Reihe zusätzlicher Inhalte**

**Hinzugefügt:**

&#x200B;* [Farbmanagement] Unterstützung für ICC-Profile mit Adobe Color Engine hinzufügen (ACE)
&#x200B;* [Farbmanagement] Unterstützung für &quot;Adobe 98 RGB&quot; als Arbeitsfarbraum für ICC hinzufügen
&#x200B;* [Farbmanagement] Konfigurieren von ACE/ICC-Einstellungen über eine Konfigurationsdatei zulassen
&#x200B;* [Farbmanagement] Zulassen, dass lineare Farbwerte im Farbwähler mit dem Legacy-Modus eingegeben werden
&#x200B;* [Farbmanagement] Geben Sie das Farbprofil an, das für die Farbauswahl außerhalb der Benutzeroberfläche verwendet wird.
&#x200B;* [Farbmanagement] Merken Sie sich den letzten im Viewport ausgewählten Anzeigewert.
&#x200B;* [Farbmanagement]&#x200B;[Substance] Sorgen Sie dafür, dass Generatoren/Filter mit dem Farbmanagement ordnungsgemäß funktionieren.
&#x200B;* [Farbmanagement]&#x200B;[Substance] Fügen Sie neue Schlüsselwörter für die Farbraumüberschreibung $working und $standardsrgb hinzu
&#x200B;* [Physische Größe]&#x200B;[Engine] Extrahieren von Physische Größe-Informationen aus Mesh
&#x200B;* [Physische Größe]&#x200B;[Engine] Physische Größe Berechnung
&#x200B;* [Physische Größe] Leg von Optionen zur Verwendung von Physische Größe in der Benutzeroberfläche
&#x200B;* [Physische Größe] Visuelle Helfer im Viewport hinzufügen
&#x200B;* [Baking] Height-Baker hinzufügen
&#x200B;* [Baking] Bent normals-Baker hinzufügen
&#x200B;* [Baking] Baker für Deckkraft hinzufügen
&#x200B;* [Pipette] Neue Farb-Pipettenvorschau neben der Maus und Farbmanagement
&#x200B;* [Pipette] Das Farbwählerbedienfeld wird wieder an der letzten Position angezeigt, wenn es erneut geöffnet wird
&#x200B;* [Pipette] Ein neues Symbol für die Material-Auswahl
&#x200B;* [Pipette] Farbe verwaltet die Kanalvorschau des Farbwählers
&#x200B;* [Pipette] Fügen Sie der Pipette eine Funktion zum Klicken hinzu, um diese auszuwählen
&#x200B;* [Eye Dropper] Kanalauswahl aktiviert nicht aktive Materialien nicht mehr
&#x200B;* [Pipette] Pipette mit Tastaturbefehl verwenden
&#x200B;* [Pipette] Die Pipette nimmt den relevanten Kanal auf, falls zutreffend.
&#x200B;* [Pipette] Beim Aufrufen des Farbwählermodus werden alle Tastaturbefehle deaktiviert
&#x200B;* [Pipette] Automatische Auswahl des Hexadezimalfelds entfernen
&#x200B;* [Pipette] Schließen Sie das Bedienfeld nicht, wenn Sie die Material-Auswahl verwenden
&#x200B;* [Pipette] Neuer deaktivierter Zustand, wenn der Kanal nicht zur Auswahl verfügbar ist
&#x200B;* [Exportieren] Fügen Sie das Attribut &quot;Tangente&quot; dem glTF-Export hinzu
&#x200B;* Substance Engine auf Version 8.4 aktualisieren
&#x200B;* Update Auto Entpack auf 0.9.0
&#x200B;* Update auf Qt 5.15.8
&#x200B;* Update auf Python 3.9
&#x200B;* [Shader] Unterstützung für Bent normals-Schattierung hinzufügen
&#x200B;* [MacOS] Unterstützung von 3DConnection SpaceMouse
&#x200B;* [Python] Dokumentieren der in der API verwendeten Python-Version
&#x200B;* [Inhalt] Sechs neue 3D-Rauschen mit 105 Vorgaben hinzufügen
&#x200B;* [Inhalt] 20 neue Schmutz Maps und 2 Stofffalten
&#x200B;* [Inhalt] Aktualisieren der Exportvoreinstellung &quot;Mesh-Map&quot;, um neue Baker zu verwenden
&#x200B;* [Inhalt] Weichzeichnungs- und Verkrümmungsfilter hängen von der Steigung des Textursatzes ab
&#x200B;* [Inhalt] Aktualisieren von Beispielprojekten, um die 3 neuen Baker zu verwenden

**Fest:**

&#x200B;* [glTF] glTF kann nicht mit Sonderzeichen geöffnet werden
&#x200B;* [Engine] Artefakte mit deaktivierter Anisotropie und SVT
&#x200B;* [MacOS]&#x200B;[M1] Intelligenten Materials werden nicht korrekt angezeigt
&#x200B;* [Mesh Processing] Mesh können nicht aus Modeler importiert werden.
&#x200B;* [UI] Horizontale Bildlaufleiste in neuem Projektfenster mit aktiviertem Farbmanagement
&#x200B;* [Farbmanagement] Arbeitsfarbraumwert fehlt in der Farbauswahl bei einigen OCIO
&#x200B;* [Farbmanagement] Pinselvorschau im Viewport ist nicht farbverwaltet
&#x200B;* [SpaceMouse] Pivot wird nicht sofort mit Fokusänderung aktualisiert und kann außerhalb des Modells liegen
&#x200B;* [Exportieren]&#x200B;[USD] Exportierte USD haben eine falsche Struktur.
&#x200B;* [USD] Ambient occlusion-Problem beim Exportieren
&#x200B;* [Inhalt] Mesh der Miniaturansicht entsprechend dem Vorschaukugel-Beispielprojekt aktualisieren

**Bekannte Probleme:**

&#x200B;* Texturen mit Innenabständen exportieren macht schwarze Diffusionen.
&#x200B;* Normale/Ambient occlusion-Mischung ist defekt
&#x200B;* [MacOS] Absturz beim Starten von Iray in seltenen Fällen
&#x200B;* [Vorschau-Miniaturansicht] Vereinfachte Miniaturansichten werden nicht aktualisiert, wenn ein Anker verwendet wird
&#x200B;* [Farbmanagement] HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen festgeklemmte Farben

## Version 7

### 7.4.3

*(Freigegeben: 11. April 2022)*
Zusammenfassung: **Bugfix mit Unterstützung von 3D-Verbindung SpaceMouse im 2D-Viewport**

**Hinzugefügt:**

&#x200B;* [SpaceMouse] Unterstützung von 3DConnection SpaceMouse im 2D-Viewport

**Fest:**

&#x200B;* [Farbwähler] Kann nicht in das Hexadezimalfeld geschrieben werden
&#x200B;* [Farbmanagement] Ressourcen, die im Projektion-Modus verwendet werden, werden in der Überlagerung nicht farbverwaltet
&#x200B;* [Farbmanagement] Fehler werden nicht im Protokoll gemeldet.
&#x200B;* [SpaceMouse] Generische Fehlermeldung entfernen, wenn der Benutzer keine SpaceMouse hat
&#x200B;* [SpaceMouse] Beim Laden eines Projekts ist der Drehpunkt immer ausgeblendet.
&#x200B;* [Bäcker] Die Einstellung &quot;Durchschnittliche Normale&quot; hat keine Auswirkungen in UV-Kachelprojekten
&#x200B;* [UV-Kachel] Inaktive UV-Kachelüberlagerungen verschwinden beim erneuten Laden des Gitters mit verschiedenen Kacheln
&#x200B;* [Scripting]&#x200B;[Python] Remote-Scripting ist beschädigt
&#x200B;* [Scripting]&#x200B;[Python] Mehrere Kanäle können nicht von der API abgefragt werden und es wird ein Fehler ausgelöst.
&#x200B;* [Scripting]&#x200B;[Python] Absturz bei Verwendung des ProjectEditionEntered-Ereignisses
&#x200B;* [Scripting]&#x200B;[Python] Absturz beim Aufruf von get\_active\_stack()

**Bekannte Probleme:**

&#x200B;* 3D-Verbindung SpaceMouse wird auf MacOS nicht unterstützt
&#x200B;* [UI] Horizontale Bildlaufleiste mit Farbmanagement, die in einigen Fällen in neuen Projektfenstern angezeigt wird
&#x200B;* [Mac M1] Smart-Materialien werden nicht korrekt angezeigt

### 7.4.2

*(Freigegeben: 8. März 2022)*
Zusammenfassung: **Bugfix mit Unterstützung von Verbesserungen für 3D-Verbindung, SpaceMouse und Farbmanagement (OCIO)**

**Hinzugefügt:**

&#x200B;* [SpaceMouse]&#x200B;[Windows] Unterstützung der 3D-Verbindung von SpaceMouse im 3D-Viewport für die Navigation
&#x200B;* [SpaceMouse]&#x200B;[Windows] Grundlegende Tastaturbefehle/Tasten für Pro- und Enterprise-SpaceMouse-Modelle im 3D-Viewport
&#x200B;* [SpaceMouse]&#x200B;[Windows] Dediziertes Drehmittelsymbol im 3D-Viewport
&#x200B;* [Farbmanagement] Verwenden Sie Rollen aus der OCIO-Konfiguration, um Standardeinstellungen zu ändern
&#x200B;* [Farbmanagement] Farbmanagement des Eigenschaftenfensters für Farb-Widgets
&#x200B;* [Farbmanagement] Farbmanagement des Eigenschaftsfensters für die Materialvorschau
&#x200B;* [Farbmanagement] Farbfelder im Farbwähler verwalten
&#x200B;* [Farbmanagement] Fügen Sie eine Einstellung hinzu, um den standardmäßigen sRGB-Farbraum zu definieren
&#x200B;* [Farbmanagement] Hinzufügen des standardmäßigen sRGB-Farbraums aus der OCIO-Konfiguration in der Farbwähler-Auswahlliste &quot;Anzeige&quot;
&#x200B;* [Farbmanagement] Verbesserungen für das Menü zum Überschreiben des Farbraums
&#x200B;* [Farbmanagement] Überschreiben des Umgebungs-Map-Farbraums in den Anzeigeeinstellungen zulassen
&#x200B;* [Farbmanagement] Zeichnen von Farbwählerverläufen basierend auf der aktuellen Anzeige
&#x200B;* [Farbmanagement] Klemmen von HDR-Werten standardmäßig im Farbeditor
&#x200B;* [Farbmanagement] Passthrough (kein Farbraum) für Filter im Legacy-Modus verwenden
&#x200B;* [Farbmanagement] Anzeige von Farbverläufen im Farbeditor auf Übereinstimmung mit dem Bereich [0-1] beschränken
&#x200B;* [Farbmanagement] Ausblenden der Anzeigeselektor im Farbwähler im Modus &quot;Legacy&quot;
&#x200B;* [Farbmanagement] Hex-Code für Farbwähler immer im sRGB-Farbraum
&#x200B;* [Farbmanagement] Deaktivieren der Farbwähler-Dropdown-Liste &quot;Anzeige&quot; für Datenkanäle
&#x200B;* [Optimierung] Verkrümmungsraster berechnet nur überdeckte UV-Kacheln neu
&#x200B;* [Exportieren] Exportieren von UV-Kachelprojekten für Sketchfab, USD und glTF zulassen
&#x200B;* [Scripting]&#x200B;[Python] Ändern der Tonzuordnungsfunktion zulassen

**Fest:**

&#x200B;* [Sketchfab] Durch die Aktualisierung des vorhandenen Modells wird am Ende ein neues Modell erstellt.
&#x200B;* [Sketchfab] Absturz bei der Suche nach einem zuvor aktualisierten Modell
&#x200B;* Absturz beim Exportieren in USD
&#x200B;* Absturz beim Erstellen einer neuen Shader-Instanz in der Geometriemaske oder wenn die Geometrie ausgeblendet ist
&#x200B;* [Fenster &quot;Element importieren&quot;] Absturz beim Ändern des Typs von importierten Ressourcen
&#x200B;* Normale Mesh-Maps werden bei Verwendung im Ebenenstapel invertiert
&#x200B;* [Substance] Der Benutzerdaten-Mischmodus wird nicht berücksichtigt.
&#x200B;* [Farbmanagement] Bitmaps mit Farbraum im Dateinamen werden als UV-Mustersequenzen importiert
&#x200B;* [Farbmanagement] Farbverwaltete Ausgaben des Substance-Diagramms befinden sich im falschen Farbraum
&#x200B;* [Farbmanagement] Polygon-Füllwerkzeug zeigt die falsche Farbe an
&#x200B;* [Color Management] ACES-Tonabnehmer wird im Solomodus auf Kanäle angewendet
&#x200B;* [Farbmanagement] Die Kugelbeleuchtung der Werkzeugvorschau ist nicht farbverwaltet
&#x200B;* [Farbmanagement]&#x200B;[Exportieren] Konvertierte Karten werden falsch konvertiert.
&#x200B;* [Scripting]&#x200B;[Python]&#x200B;[Farbmanagement] Projekte, die mit Vorlage und OCIO Umgebungsvariablen erstellt wurden, befinden sich im Modus &quot;Veraltet&quot;.
&#x200B;* [Scripting]&#x200B;[Python] Die JavaScript-Evaluierungsfunktion kann beim Start nicht verwendet werden.
&#x200B;* [3D-Adobe-Angebot] Painter kann nicht gestartet werden, wenn regionale Einstellungen mit Sprachen verwendet werden, die nicht standardmäßig unterstützt werden

**Bekannte Probleme:**

&#x200B;* 3D-Verbindung SpaceMouse wird auf MacOS nicht unterstützt
&#x200B;* [UI] Horizontale Bildlaufleiste mit Farbmanagement, die in einigen Fällen in neuen Projektfenstern angezeigt wird
&#x200B;* [Baker] Die Einstellung &quot;Durchschnittliche Normale&quot; hat keine Auswirkungen auf UV-Kachel-Projekte
&#x200B;* [Mac M1] Intelligenten Materials werden nicht korrekt angezeigt
&#x200B;* [Farbmanagement] Ressourcen, die im Projektion-Modus verwendet werden, werden in der Überlagerung nicht farbverwaltet
&#x200B;* [Farbwähler] Kann nicht in das Hexadezimalfeld geschrieben werden

### 7.4.1

*(Freigegeben: 14. Dezember 2021)*
Zusammenfassung: **Bugfix mit Farbmanagement-Verbesserungen**

**Hinzugefügt:**

&#x200B;* [Farbmanagement] Verwenden der Datenrolle in exportierten Dateinamen
&#x200B;* [Farbmanagement] Erweitern Sie den Abschnitt Farbmanagement standardmäßig, wenn OCIO in den Fenstern für neue Projekt- und Projekteinstellungen ausgewählt ist.
&#x200B;* [Farbmanagement] Hinzufügen ACE Tonwertumsetzers im Legacy-Modus
&#x200B;* [Farbmanagement] Standardkonfigurationseinstellungen anpassen
&#x200B;* [Farbmanagement]&#x200B;[Exportieren] Fill $colorSpace in Dateinamen für Datenkanäle
&#x200B;* [Exportieren] Exportieren von UV-Kachel-Projekten in Stager
&#x200B;* [Interoperabilität] Nicht verfügbar für Steam- und Substance-Editionen
&#x200B;* [Interoperabilität] Senden eines UV-Kachel-Projekts an Stager zulassen

**Fest:**

&#x200B;* [MacOS]&#x200B;[Absturz] Painter beginnt nicht mit Catalina
&#x200B;* [Farbmanagement]&#x200B;[Absturz] Zufälliger Absturz bei der Wiedergabe von Datentyp/Farbmanagement auf Benutzerkanal
&#x200B;* [Farbmanagement] Ressourcen, die als Graustufen in Masken verwendet werden, zeigen den Farbraum an Neues Menü
&#x200B;* [Farbmanagement] Benutzerkanal ist im Viewport im Legacy-Modus + Solo-Ansicht dunkler
&#x200B;* [Farbmanagement] Die Env-Map ist immer linear, wenn sie in iRay verwendet wird
&#x200B;* [Farbmanagement] Die Farbauswahl wählt im Legacy-Modus nicht den richtigen Wert für den Datenkanal aus
&#x200B;* [Farbmanagement] Farbwähler in einer Substance im Legacy-Modus funktioniert nicht
&#x200B;* [Farbmanagement] Der Wechsel zwischen Solokanal-Ansichten im Viewport wird bei Verwendung des Dropdown-Menüs nicht mit dem richtigen Farbraum angezeigt
&#x200B;* [Farbmanagement] Beim Export wird die falsche Konvertierung auf farbverwaltete Benutzerkanäle im Legacy-Modus angewendet.
&#x200B;* In der Einzelansichtsmaske erstellte Konturen werden beim Zurückwechseln zur Material-Ansicht nicht angezeigt
&#x200B;* [Exportieren] Konvertierte Karten werden nicht als farbverwaltete Kanäle exportiert
&#x200B;* [Textursatz] QuickInfo mit Originalnamen fehlt auf umbenannten Benutzerkanälen
&#x200B;* [Steam] Dateien fehlen beim Überprüfen der Dateiintegrität mit Steam

**Bekannte Probleme:**

&#x200B;* [Mac M1] Intelligenten Materials werden nicht korrekt angezeigt

### 7.4.0

*(Freigegeben: 24. November 2021)*
Zusammenfassung: **Hauptversion. Einführung der ersten Farbmanagement-Version, Abdocken der 2D- oder 3D-Ansicht, neue Option für den automatischen entpack von UV zum Vermeiden von länglichen Inseln, Aufruf von JavaScript-Funktionen von der Python-API und neuer Inhalt**

**Hinzugefügt:**

&#x200B;* [Farbmanagement] Unterstützung von Farbmanagement OpenColorIO Version 2
&#x200B;* [Farbmanagement] Hinzufügen von Farbmanagementeinstellungen zu Projekteinstellungen
&#x200B;* [Farbmanagement] Warnfenster zu Farbmanagement-Konfigurationsänderungen beim Öffnen eines Projekts
&#x200B;* [Farbmanagement] Zeigt eine Fehlermeldung an, wenn eine ungültige OCIO-Konfigurationsdatei ausgewählt ist
&#x200B;* [Farbmanagement] Überschreiben der Konfiguration mit OCIO Umgebungsvariablen zulassen
&#x200B;* [Farbmanagement] Mehrere OCIO sind standardmäßig in die Anwendung integriert.
&#x200B;* [Farbmanagement] Extrahieren des Farbraumnamens aus dem importierten Bitmap-Dateinamen
&#x200B;* [Farbmanagement] Überschreiben des Farbraums mit einem Farbraum aus der Konfiguration im Eigenschaftenfenster zulassen
&#x200B;* [Farbmanagement] Hinzufügen von Farbmanagementoptionen in den Textursatzeinstellungen
&#x200B;* [Farbmanagement]&#x200B;[Viewport] Ermöglicht das separate Farbmanagement für 2D- und 3D-Ansichten.
&#x200B;* [Farbmanagement] Umgebungszuordnung laden und in den Arbeitsfarbraum konvertieren
&#x200B;* [Farbmanagement] Anpassen des Farbwählers und Editors mit dem aktuellen Farbraum
&#x200B;* [Farbmanagement] Erlauben Sie mit einem neuen Dropdown-Menü die Auswahl des Anzeigetransformationsfarbraums im Viewport.
&#x200B;* [Farbmanagement] Anwenden der Anzeigetransformation mit Iray-Renderingergebnissen
&#x200B;* [Farbmanagement] Exportieren von Texturen mit verschiedenen Farbräumen
&#x200B;* [Farbmanagement]&#x200B;[Python] Anwenden von Farbmanagementeinstellungen der Umgebungsvariablen (OCIO) auf neue Projekte
&#x200B;* [Viewport] Abdocken des 2D- oder 3D-Viewports zulassen
&#x200B;* [Automatisches Ausgliedern] Neue Option zur Vermeidung länglicher Inseln
&#x200B;* [Scripting Python] Aufrufen von JavaScript-Funktionen über die Python-API
&#x200B;* [Neues Projektfenster] Reduzieren des Abschnitts &quot;Importierte Karten&quot;
&#x200B;* [Projektion]&#x200B;[Verkrümmen] Normale als Option in den Verkrümmungseinstellungen können ausgeblendet werden.
&#x200B;* [Content] 11 neue Schmutz-Maps
&#x200B;* [Inhalt] 8 neue Werkzeugvorgaben (Reißverschluss, Spannschnur, Glitter)
&#x200B;* [Inhalt] 8 neue Materialien (Narbe, Tasche, ...)
&#x200B;* [Inhalt] 1 neuer Generator (inflate schrumpfwarp)

**Bekannte Probleme:**

&#x200B;* [Mac M1] Smart-Materialien werden nicht korrekt angezeigt
&#x200B;* [Farbmanagement]&#x200B;[Absturz] Zufälliger Absturz beim Spielen mit Datentyp/Farbmanagement auf Benutzerkanal
&#x200B;* [Farbmanagement] Die Farbauswahl wählt im Legacy-Modus nicht den richtigen Wert für den Datenkanal aus
&#x200B;* [Farbmanagement]&#x200B;[Iray] Das Speichern des Renderings in EXR oder TIFF, während das Farbmanagement im Viewport aktiviert ist, wird immer linear gespeichert
&#x200B;* [Farbmanagement] Ressourcen, die als Graustufen in Masken verwendet werden, zeigen das falsche Farbraummenü an
&#x200B;* [Farbmanagement]&#x200B;[Iray] Die Env-Map ist immer linear, wenn sie in Iray verwendet wird
&#x200B;* [Farbmanagement]&#x200B;[Exportieren] Konvertierte Karten werden nicht als farbverwaltete Kanäle exportiert
&#x200B;* [Farbmanagement]&#x200B;[Exportieren] Der Export ignoriert, wenn der Benutzerkanal farbverwaltet ist oder nicht im Legacy-Modus ausgeführt wird

### 7.3.1

*(Freigegeben: 24. November 2021)*
Zusammenfassung: **Bugfix**

**Hinzugefügt:**

&#x200B;* [Projektion] Skalierung sollte nur im Objektbereich funktionieren

**Fest:**

&#x200B;* [Mac M1] Materialschichtung funktioniert nicht
&#x200B;* [Mac M1]&#x200B;[Projektion] Verkrümmung funktioniert nicht
&#x200B;* Micro-Details werden nicht richtig angezeigt
&#x200B;* [Projektion]&#x200B;[Absturz] Wechseln in den Verkrümmungsmodus mit einer Ebene, die mit einer vorherigen Version erstellt wurde
&#x200B;* [Projektion]&#x200B;[Verkrümmen] Spiegeln funktioniert nicht, wenn die Transformation auf den Weltraum eingestellt ist
&#x200B;* [Projektion]&#x200B;[Verkrümmen] Die Option &quot;Teilen&quot; bleibt nach Abschluss des Teilens ausgewählt.
&#x200B;* [Projektion]&#x200B;[UV] Der Pivot-Punkt wird beim Spiegeln der Projektion zurückgesetzt.
&#x200B;* [Filter] Bake Lighting-Umgebung ändert sich beim erneuten Laden oder Ändern eines Parameters
&#x200B;* [Interoperabilität] Nicht verfügbar für Steam- und Substance-Editionen
&#x200B;* [Interoperabilität] Die Schaltfläche &quot;3D-Assets auf dem Marktplatz durchsuchen&quot; sollte immer CCD auf der Registerkarte &quot;Stock &amp; Marketplace 3D&quot; öffnen.

**Bekannte Probleme:**

&#x200B;* [Mac M1] Smart-Materialien werden nicht korrekt angezeigt

### 7.3.0

*(Freigegeben: 13. Oktober 2021)*
Zusammenfassung: **Hauptversion. Es enthält eine neue 3D-Verkrümmungsprojektion, eine neue zylindrische Projektion, Verbesserungen des Farbwählers, neue Funktionen in der Python-API und Fehlerbehebungen**

**Hinzugefügt:**

&#x200B;* [Projektion]&#x200B;[Verkrümmen] 3D-Verkrümmung als neuen Projektionsmodus verfügbar machen
&#x200B;* [Projektion]&#x200B;[Verkrümmen] Erlauben Sie den Aufklebermodus für Alphas, Texturen und Prozeduralen mit Drag &amp; Drop im Viewport
&#x200B;* [Projektion]&#x200B;[Verformen] Verwenden der Verkrümmungsprojektion mit Aufkleberkürzeln (ALT)
&#x200B;* [Projektion]&#x200B;[Verkrümmen]&#x200B;[Symbolleiste] Transformieren der Verkrümmung als Ganzes oder pro Scheitelpunkt
&#x200B;* [Projektion]&#x200B;[Verkrümmen]&#x200B;[Symbolleiste] Hinzufügen von Rasterpunkten mit geteilten Verkrümmungsoptionen in Querrichtung, horizontal oder vertikal
&#x200B;* [Projektion]&#x200B;[Verkrümmen]&#x200B;[Symbolleiste] Dediziertes Menü für Zurücksetzen-Aktionen
&#x200B;* [Projektion]&#x200B;[Verkrümmen]&#x200B;[Symbolleiste] Option zur automatischen Anpassung der Tangenten beim Verschieben von Punkten
&#x200B;* [Projektion]&#x200B;[Verkrümmung]&#x200B;[Symbolleiste] Spezielles Menü für die Rasterausgabe (Größe, Zurücksetzen, Farbe und Griffgröße)
&#x200B;* [Projektion]&#x200B;[Verformen] Neuer Tastaturbefehl zum Umschalten des Warp-Editionsmodus für ganze Scheitelpunkte (UMSCHALT+V)
&#x200B;* [Projektion]&#x200B;[Verformen] Klicken+Strg ermöglicht den Wechsel zwischen Flächenwerkzeug und anderen Werkzeugen
&#x200B;* [Projektion]&#x200B;[Zylindrisch] Zeigen Sie den zylindrischen Projektionsmodus an.
&#x200B;* [Projektion]&#x200B;[Symbolleiste] Einstellungen für den Gruppenmanipulator (Größe, Rasterschritte, Winkelschritte)
&#x200B;* [Farbwähler] Neue Benutzeroberfläche für Farbwähler
&#x200B;* [Farbwähler] Verwenden von sRGB-Werten in Farbwähler-Widgets
&#x200B;* [Farbwähler] Farbfelder speichern und löschen
&#x200B;* [Farbwähler] Pipette, die über Farbkanäle und normale Slots zugänglich ist
&#x200B;* [Farbwähler] Dynamische Farbe zwischen 0 und 255 Werten bearbeiten
&#x200B;* [Farbwähler] Gemeinsamer HSV-/RGB-Status in der App
&#x200B;* [Farbwähler] Das Fenster &quot;Farbwähler&quot; ist halbpersistent.
&#x200B;* [Farbwähler] Durch Drücken von Esc wird das Farbwählerfenster geschlossen.
&#x200B;* Leistungsverbesserung für UI-Interaktion und beim Malen
&#x200B;* [Engine] Update auf die neue Substance-Engine-Version (8.3.0)
&#x200B;* [Scripting]&#x200B;[Python] Ermöglicht das erneute Laden des Gitters des aktuellen Projekts.
&#x200B;* [Scripting]&#x200B;[Python] Aktualisieren von Ressourcen in Projekten zulassen
&#x200B;* [Scripting]&#x200B;[Python] Festlegen und Abfragen der Auflösung von UV-Kacheln zulassen
&#x200B;* [Interoperabilität] Nicht verfügbar für Steam- und Substance-Editionen
&#x200B;* [Interoperabilität] Empfangen mehrerer Ressourcen von Bridge

**Fest:**

&#x200B;* Der Farbwähler zeigt nicht die richtige Farbe an
&#x200B;* [Backen] Textursatzliste wird nicht korrekt angeordnet
&#x200B;* [FBX-Import] 3ds Max. Gruppen-Pivot-Transformationen werden nicht berücksichtigt
&#x200B;* [Substance Engine] Absturz beim Importieren von beschädigtem SBSAR
&#x200B;* [MacOS] Projektkonfigurationsoption in verschiedenen Sprachen ist nicht vorhanden.
&#x200B;* Automatische Speicherung kann Painter während langer Prozesse einfrieren

**Bekannte Probleme:**

&#x200B;* [Projektion]&#x200B;[Verkrümmen] Die Option &quot;Teilen&quot; bleibt nach Abschluss des Teilens ausgewählt.
&#x200B;* [Projektion]&#x200B;[Verkrümmen] Spiegeln funktioniert nicht, wenn die Transformation auf den Weltraum eingestellt ist
&#x200B;* [Projektion]&#x200B;[Verkrümmen] Artefaktlinien zwischen Patches in seltenen Fällen
&#x200B;* [Projektion]&#x200B;[UV] Der Pivot-Punkt wird beim Spiegeln der Projektion zurückgesetzt.
&#x200B;* [Mac M1] Smart-Materialien werden nicht korrekt angezeigt
&#x200B;* [M1]&#x200B;[Regression] Materialschichtung funktioniert nicht

### 7.2.3

*(Freigegeben: 24. August 2021)*
Zusammenfassung: **Nebenversion, Bugfix**

**Hinzugefügt:**

&#x200B;* [Bibliotheken] Hinzufügen einer Möglichkeit, unerwünschte Dateien vom Durchsuchen auszuschließen

**Fest:**

&#x200B;* [Win] Mehrere Bildschirme und Schlafprobleme
&#x200B;* [MacOS]&#x200B;[Absturz] Wechseln des Shaders bei Verwendung von Effekten
&#x200B;* [Viewport] Im vollständigen Vorschaumodus wird der Pinselcursor nicht mehr ohne Alpha angezeigt.
&#x200B;* [UI] Winkel-Widget schlägt falsch
&#x200B;* [Ebenenstapel] Viele Unterordner erstellen sehr lange Einfrieren
&#x200B;* [Iray] Verschiedene Ansichten in Iray und OpenGL: Sichtbar, wenn nicht funktionierend
&#x200B;* [Iray] Brechungsindex nicht berücksichtigt und erscheint nicht in den Eigenschaften von mdl
&#x200B;* [JavaScript] ShowExportDialog() gibt nie true zurück.
&#x200B;* Kann keine MTL aus Adobe Stock lesen

### 7.2.2

*(Freigegeben: 27. Juli 2021)*
Zusammenfassung: **Nebenversion, Bugfix**

**Hinzugefügt:**

&#x200B;* Aktualisieren Sie die Version der AMD-Treiberanforderungen

**Fest:**

&#x200B;* [Mac M1] Falsche Speichererkennung
&#x200B;* [Exportieren] Sehr lange Pfade werden nicht richtig angezeigt

**Bekannte Probleme:**

&#x200B;* [Inhalt] Veraltete Shader der Samples

### 7.2.1

*(Freigegeben: 2. Juli 2021)*
Zusammenfassung: **Nebenversion, Hotfix**

**Hinzugefügt:**

&#x200B;* [Interop] Fügen Sie eine QuickInfo hinzu, die darüber informiert, dass das Senden von UV-Kachel-Projekten an Stager noch nicht unterstützt wird.
&#x200B;* [Plug-in]&#x200B;[UI] Aktualisierung des LiveLink-Symbols

**Fest:**

&#x200B;* [NVIDIA] Treiberversion ab 30 gilt als veraltet
&#x200B;* [Bibliotheken] Der Status des Bedienfelds &quot;Elemente&quot; wird nur gespeichert, wenn ein Projekt geöffnet ist
&#x200B;* [Bibliotheken] Neue gespeicherte Suche behält Stichwörter aus alter gespeicherter Suche bei
&#x200B;* [Baker]&#x200B;[UVTiles] ID-Map pro MeshID berücksichtigen auch UV-Kacheln
&#x200B;* [Exportieren] gLTF-Dateien importieren keine Scheitelpunkt-Farbe
&#x200B;* [Iray] Einige QuickInfos fehlen
&#x200B;* [Interop] Senden an Stager ist nicht immer deaktiviert, wenn Stager nicht erkannt wird
&#x200B;* [Resource Updater] Photoshop-Pinselmaker kann nicht aktualisiert werden.
&#x200B;* [Inhalt] Glasfaser-Kantenverschleißgenerator ist defekt

### 7.2.0

*(Freigegeben: 23. Juni 2021)*
Zusammenfassung: **Die Hauptversion bietet eine Aktualisierung des Bedienfelds &quot;Elemente&quot;, einen neuen Shader mit Zugriff auf neue Kanäle und Parameter, eine allgemeine Aktualisierung der Benutzeroberfläche, einige dringend angeforderte Leistungsverbesserungen, erweiterte Sprachunterstützung und vieles mehr!**

**Hinzugefügt:**

&#x200B;* [Bibliotheken] Neues Bedienfeld &quot;Elemente&quot;, um das Regal zu ersetzen
&#x200B;* [Bibliotheken]&#x200B;[UI] Neues Bedienfeld &quot;Elemente&quot;
&#x200B;* [Bibliotheken]&#x200B;[UI] Ändern der standardmäßigen Ausrichtung des Bedienfelds &quot;Elemente&quot; und der Benutzeroberfläche
&#x200B;* [Bibliotheken]&#x200B;[Benutzeroberfläche] Einführung einer Listenansichtsoption in die Bibliothek
&#x200B;* [Bibliotheken]&#x200B;[UI] Neue Breadcrumbs-Navigation im Bedienfeld &quot;Elemente&quot;
&#x200B;* [Bibliotheken]&#x200B;[UI] Wählen Sie &quot;Alle Bibliotheken&quot; aus, wenn Sie eine gespeicherte Suche auswählen.
&#x200B;* [Bibliotheken]&#x200B;[UI] Wählen Sie &quot;Alle Bibliotheken&quot;, wenn alle Ordner deaktiviert sind.
&#x200B;* [Bibliotheken]&#x200B;[UI] Neues Tag für Partikelpinsel
&#x200B;* [Bibliotheken]&#x200B;[UI] &quot;Ablage&quot; durch &quot;Alle Bibliotheken&quot; in der gesamten App ersetzt
&#x200B;* [Bibliotheken]&#x200B;[UI] Leere Ordner ausblenden
&#x200B;* [Bibliotheken]&#x200B;[UI] Die Standardbenutzerbibliothek sollte auch dann sichtbar sein, wenn sie leer ist
&#x200B;* [Bibliotheken]&#x200B;[UI] Neue Filtermethode über die Symbole des Elementtyps
&#x200B;* [Bibliotheken] Tastenkombination &quot;STRG&quot; zum Auswählen mehrerer Elementtypen
&#x200B;* [Bibliotheken] Neue Umgebungsvariable zur Steuerung des Speicherbudgets für die Elementvorschau
&#x200B;* [Bibliotheken]&#x200B;[Inhalt] Neue Umgebungszuordnungen
&#x200B;* [Bibliotheken]&#x200B;[Inhalt]&#x200B;[Benutzeroberfläche] Rendern von Versatz auf Standardmaterialien
&#x200B;* [Bibliotheken]&#x200B;[Inhalt] Legen Sie den Adobe Standard Material (ASM)-Shader als Standard für die Vorschauerstellung fest.
&#x200B;* [Bibliotheken]&#x200B;[Inhalt]&#x200B;[ASM] Neue Projektvorlagen für neuen ASM-Shader
&#x200B;* [Bibliotheken]&#x200B;[Miniaturansicht] Neue Studio 6-Umgebungszuordnung verwenden
&#x200B;* [Bibliotheken]&#x200B;[Miniaturansicht] Miniaturansicht in Ressource lesen, anstatt sie zu generieren
&#x200B;* [Bibliotheken]&#x200B;[Miniaturansicht] Versatz zur Miniaturgenerierung hinzufügen
&#x200B;* [Einstellungen für Struktureinstellungen]
&#x200B;* [Einstellungen für Struktureinstellungen]&#x200B;[UI] Neues Height wird einer normalen Konvertierungsmethode zugewiesen.
&#x200B;* [Einstellungen für Textursatz]&#x200B;[UI] Nachbearbeitung der UI-Organisation der Kanäle
&#x200B;* [Einstellungen für Textursatz] Benutzerkanallimit auf 16 Kanäle erhöht
&#x200B;* [Einstellungen für Textursatz]&#x200B;[UI] Geben Sie an, welche Kanäle mit dem aktuell ausgewählten Shader kompatibel sind.
&#x200B;* [Shader]&#x200B;[ASM] Neuer Adobe Standard Material Shader
&#x200B;* [Shader]&#x200B;[ASM] Zusätzliche Unterstützung für Anisotropie, Clear Coat, Subsurface Scattering, Specular edge color und Sheen
&#x200B;* [Shader]&#x200B;[ASM] Ändern der Farbwerte der Standardkanäle
&#x200B;* [Shader]&#x200B;[ASM]&#x200B;[Export] Aktualisierte Exportvorlage Adobe Dimension zu Adobe Substance 3D Stager
&#x200B;* [Shader]&#x200B;[ASM] Beschriftungen und QuickInfos für Shader- und MDL-Parameter hinzugefügt
&#x200B;* [Shader]&#x200B;[ASM] Die Farbfarbe der Streuung in der 2D-Ansicht sichtbar machen, auch wenn SSS nicht unterstützt wird
&#x200B;* [Shader]&#x200B;[ASM]&#x200B;[Iray] Unterstützung des ASM-Shaders in Iray mit neuer MDL
&#x200B;* [Shader]&#x200B;[ASM]&#x200B;[Iray] Aktualisierte Untergrundstreuung in veraltetem PBR-Spezifikationsglanz und beschichtet
&#x200B;* [Shader]&#x200B;[ASM]&#x200B;[Content] Der Standard-SSS-Typ für Samples wurde geändert
&#x200B;* [Shader]&#x200B;[ASM] Hinzugefügte Dokumentation für ASM API
&#x200B;* [Shader]&#x200B;[ASM] Optimieren Sie Shader, um nicht verwendete Kanäle zu ignorieren
&#x200B;* [Shader] Neue Texturset-Kanäle anzeigen
&#x200B;* [Shader] Verbesserte Untergrundstreuung
&#x200B;* [Shader] Neue Shader-Parameter für einige Shader wurden ausgeblendet.
&#x200B;* [Shader] Sichtbar, wenn für Shader-Parameter
&#x200B;* [Leistung]
&#x200B;* [Bibliotheken] Verbesserungen der Ladezeit der Ressourcenvorschau und der Berechnungsleistung
&#x200B;* [Engine] Verbesserungen der Malleistung
&#x200B;* [Automatisches Ausgliedern]
&#x200B;* [Automatisches Ausgliedern] Leistungsverbesserungen bei Packing
&#x200B;* [Automatisch Entpackt] Automatisch entpackt, kompatibel mit dem Workflow der UV-Kachel
&#x200B;* [Automatisches Entpacken] Neue Option zur Positionierung von UVs entsprechend der Ausrichtung des Meshs
&#x200B;* [Sonstige]
&#x200B;* [Einstellungen] Standardzoomrichtung geändert
&#x200B;* [UI] Gesamte Aktualisierung der Benutzeroberfläche
&#x200B;* [UI] Überarbeitung des Hilfemenüs
&#x200B;* [UI] Symbol &quot;Umkehren ersetzen&quot;
&#x200B;* [UI]&#x200B;[Plug-In] Symbol &quot;Ersetzen&quot; für den DCC-Link des Plug-Ins
&#x200B;* [UI]&#x200B;[AMD] Mindest erforderliche Version aktualisieren und Popup-Nachricht
&#x200B;* [Ebenenstapel] Neue Ebene innerhalb des ausgewählten leeren Ordners erstellen
&#x200B;* Python-Dokumentation aktualisieren
&#x200B;* [Branding]
&#x200B;* [Branding]&#x200B;[UI] Der Anwendungsname wurde in Adobe Substance 3D Painter aktualisiert.
&#x200B;* [Branding]&#x200B;[UI] Eigenständige Version auf &quot;Substance Edition&quot; aktualisiert
&#x200B;* [Branding]&#x200B;[UI] Aktualisierter Name der ausführbaren Datei der Anwendung, Installationspfad, Paket und Symbole
&#x200B;* [Branding]&#x200B;[UI] Standardbibliothek und -pfad wurden umbenannt
&#x200B;* [Branding]&#x200B;[UI] Aktualisiert über das Fenster
&#x200B;* [Branding]&#x200B;[UI] Aktualisierter Begrüßungsbildschirm
&#x200B;* [Branding]&#x200B;[UI] Die jährliche Versionsnummer wurde entfernt.
&#x200B;* [Lokalisierung] Neue Übersetzungen in Deutsch, Französisch und vereinfachtem Chinesisch
&#x200B;* [Interoperabilität] Nicht verfügbar für Steam- und Substance-Editionen
&#x200B;* [Interoperabilität] Interoperabilität mit dem Adobe-Ökosystem: Designer, Sampler, Stager und Bridge
&#x200B;* [Interoperabilität]&#x200B;[Benutzeroberfläche] Empfangen und Aktualisieren von Elementen aus Designer
&#x200B;* [Interoperabilität]&#x200B;[Benutzeroberfläche] Empfangen von Elementen aus Sampler
&#x200B;* [Interoperabilität]&#x200B;[UI] Element an Stager senden
&#x200B;* [Interoperabilität]&#x200B;[Benutzeroberfläche] In Adobe Bridge anzeigen
&#x200B;* [Interoperabilität]&#x200B;[UI] Schneller Zugriff auf Adobe 3D-Elemente
&#x200B;* [Interoperabilität] Neue Verwendungs-Tags von sbsar
&#x200B;* [Interoperabilität] Umgang mit empfangenen Elementtypen
&#x200B;* [Interoperabilität] Von Adobe Substance 3D Designer oder Adobe Substance 3D Sampler empfangene Elemente werden in der vom Benutzer standardmäßig ausgewählten Bibliothek gespeichert.
&#x200B;* [Interoperabilität]&#x200B;[Benutzeroberfläche] Neues Symbol in der linken Symbolleiste zum Senden an Stager oder Photoshop

**Fest:**

&#x200B;* [Tablet] Geringe Leistung beim Malen mit Druck
&#x200B;* [Tablet] Problem auf Tablets mit Schiebereglern
&#x200B;* [Absturz] Namenskonflikt zwischen der Liste der Textursatz und dem Exporter
&#x200B;* [Absturz]&#x200B;[Bibliotheken] Doppelklicken Sie auf eine Unterbibliothek.
&#x200B;* [Bibliotheken] Problem beim Durchsuchen von Bibliotheksverzeichnissen
&#x200B;* [Bibliotheken] Befehlszeile zum Erzwingen der Vorschaugenerierung funktioniert nicht wie erwartet
&#x200B;* [Libraries]&#x200B;[Content] Der Baking geführt Lichtumgebungsfilter ist standardmäßig schwarz.
&#x200B;* [Linux]&#x200B;[MacOS]&#x200B;[Mesh exportieren] Kann unter Linux/MacOS erstellte glTF nicht importieren
&#x200B;* [Linux] Das Ziehen und Ablegen einer Datei in das Bedienfeld &quot;Asset&quot; kann zu einem Absturz führen
&#x200B;* [Automatisches Entpacken] Automatisches Entpacken ist auch dann verfügbar, wenn kein Mesh zum erneuten Laden ausgewählt wurde
&#x200B;* [Partikeln] Falsche Partikel mit Schwerkraft
&#x200B;* [Ebenenstapel] Ebenen-Histogramm kann nur Luminanz mit einigen Kanälen verwenden
&#x200B;* [Geometriemaske] Rechtsklick-Menü auf einen Ordner beim Bearbeiten der Geometriemaske funktioniert nicht
&#x200B;* [Projektion] Naht mit sphärische Projektion und bilinearen Filterungen
&#x200B;* [UV-Kacheln] Exportmaske in Datei exportiert nur Kachel 0, 0
&#x200B;* [Mesh exportieren] FBX Mesh-Export ist leer.
&#x200B;* [Iray] Normalen-Map wird beim Rendern in neuen Projekten nicht berücksichtigt
&#x200B;* [Speichern] Speichern von Problemen auf freigegebenen Laufwerken
&#x200B;* [Baking] Beim erneuten Erstellen eines Meshs mit geänderten Parametern wird eine Warnung angezeigt.
&#x200B;* [Baking]&#x200B;[Regression] Falsches Ergebnis, wenn der globale Begrenzungsrahmen des hohen Poly-Meshs den Ursprung der Szene nicht enthält
&#x200B;* [Python] Benutzerdefinierte Benutzerbibliotheken werden nicht berücksichtigt

**Bekannte Probleme:**

&#x200B;* [Bibliotheken] Gespeicherte Suchen werden nicht gespeichert, wenn kein Projekt geöffnet wird
&#x200B;* [NVIDIA] Meldung für veralteten Treiber, selbst wenn der Treiber auf dem neuesten Stand ist

### 7.1.1 (2021.1.1)

*(Freigegeben: 23. März 2021)*
Zusammenfassung: **Nebenversion, Bugfix mit der Möglichkeit, Hexadezimalwerte in den Farbwähler einzugeben**

**Hinzugefügt:**

&#x200B;* [Protokoll] Benutzer über inkompatible AMD-GPU-Treiber warnen
&#x200B;* [Farbwähler] Hexadezimalwerte können eingegeben werden

**Fest:**

&#x200B;* [Baker] Leistungseinbruch
&#x200B;* [Geometriemaske] Alt-Klick auf Mesh-Namen kann zu einem Absturz führen
&#x200B;* [Engine] Beim Malen wird bei Bedarf nicht die gesamte Ansicht aktualisiert
&#x200B;* [Ebenenstapel] Auswahl bleibt nach dem Ändern des Shader hängen
&#x200B;* [MacOS]&#x200B;[Farbwähler] Die Farbe ist etwas anders als die ausgewählte
&#x200B;* [Exportieren] Bei Verwendung des PSD-Dateiformats wird nicht eine Datei pro UV-Kachel generiert.
&#x200B;* [Scripting]&#x200B;[Javascript] alg.mapexport.getPathsExportDocumentMaps() gibt nicht alle Werte zurück.
&#x200B;* [Scripting]&#x200B;[Python] Deaktivierte Plug-ins werden beim erneuten Öffnen von Painter wieder aktiviert

### 7.1.0 (2021.1.0)

*(Freigegeben: 28. Januar 2021)*
Zusammenfassung: **Hauptversion, neue Geometriemaske, mit der Teile der UV-Kachel ausgewählt und Malen werden können, Kopier-/Einfügeeffekte im Ebenenstapel, verbesserte Geometriemaske, Aktualisierung von Iray, Bakern, Substance Engine und neuen Inhalten**

**Hinzugefügt:**

&#x200B;* Neue Geometriemaske und Malen ausgewählter Teile der Geometrie
&#x200B;* [Geometriemaske] Erlaubt das Malen ausgewählter Geometrieteile nach Mesh-Namen.
&#x200B;* [Geometrie-Maske] Rechteckige Auswahl in beiden Ansichten
&#x200B;* [Geometriemaske] Ausgeschlossene Geometrie auf einer Ebene ausblenden/ignorieren
&#x200B;* [Geometriemaske]&#x200B;[Eigenschaften] Schnellauswahl für Kontrollkästchen mit Klicken und Ziehen
&#x200B;* [Geometriemaske]&#x200B;[Eigenschaften]&#x200B;[UI] Alle Elemente mit einer Dropdown-Liste im Eigenschaftenfenster einschließen/ausschließen
&#x200B;* [Geometriemaske]&#x200B;[Eigenschaften] Ermöglicht die schnelle Auswahl eines Elements in einer Liste mit ALT+LINKSKLICK.
&#x200B;* [Geometriemaske]&#x200B;[Eigenschaften] Überlagerung in Viewports, wenn der Mauszeiger über Gitternamen/UV-Kacheln im Eigenschaftenfenster bewegt wird
&#x200B;* [Geometriemaske]&#x200B;[Ebenenstapel] Optionen zum Kopieren/Einfügen zur Geometriemaske hinzufügen
&#x200B;* [Geometriemaske] Neues Symbol für Schaltfläche &quot;Ausgeschlossene Geometrie ausblenden/ignorieren&quot;
&#x200B;* [Geometriemaske] Neue QuickInfo für Ausgeschlossene Geometrie ausblenden/ignorieren
&#x200B;* [Geometriemaske] Tastaturbefehl ALT+H zum Aktivieren/Deaktivieren der Schaltfläche &quot;Ausgeschlossene Geometrie ignorieren&quot;
&#x200B;* [UV-Kacheln]&#x200B;[Ebenenstapel] Neue Kugelvorschau der Füllebene für UV-Kacheln und vereinfachten Modus
&#x200B;* [UV-Kacheln]&#x200B;[Ebenenstapel] Einfaches Beenden der UV-Kachelmaske
&#x200B;* [UV-Kacheln]&#x200B;[Texturset-Liste] Geben Sie eine Beschreibung pro UV-Kachel an.
&#x200B;* [UV-Kacheln]&#x200B;[Einstellungen für Textursatz]&#x200B;[UI] Zwei neue Abschnittstitel im Dropdown-Menü zum Ändern der UV-Kachelauflösung
&#x200B;* [UV-Kacheln]&#x200B;[Viewport] Beenden Sie die UV-Kachelmaske, wenn Sie ein Material in das Viewport ziehen.
&#x200B;* [Ebenenstapel] Optionen zum Kopieren/Einfügen für Effekte hinzufügen
&#x200B;* [Ebenenstapel] Kopieren/Einfügen von Effekten von einem Textursatz in einen anderen zulassen
&#x200B;* [Ebenenstapel] Mehrere Effekte auswählen
&#x200B;* [Ebenenstapel] Optionen zum Kopieren/Einfügen als Tastaturbefehle für Ebeneneffekte hinzufügen
&#x200B;* [Ebenenstapel] Automatisch zwischen Maske und Inhalt wechseln, wenn Effekte auf eine andere Ebene gezogen werden
&#x200B;* [Ebenenstapel] Beim Einfügen einer Maske aus einer anderen Ebene automatisch eine Maske erstellen
&#x200B;* [Ebenenstapel] Fügen Sie im Kontextmenü der Effekte die Aktionen zum Verschieben hinzu.
&#x200B;* [Ebenenstapel] Ziehen und Ablegen von Effekten von einer Ebene auf eine andere zulassen
&#x200B;* [Ebenenstapel] Wenn Elemente in einen Ordner gezogen werden, werden sie oben im Ordner platziert.
&#x200B;* Aktualisieren Sie Iray auf Version 2020.1.0
&#x200B;* [Baker] Update Baker auf Version 2.5.4
&#x200B;* [Bäcker] Anzeigen einzelner UV-Kacheln im Fenster Backfortschritt
&#x200B;* [Bäcker]&#x200B;[UI] Ermöglicht das schnelle Backen des aktuellen Textursatzes mit einer neuen Schaltfläche
&#x200B;* [Bäcker] Benutzer können schnell einen der Bäcker mit ALT+LINKSKLICK auswählen
&#x200B;* Substance Engine auf Version 8.0.8 aktualisieren
&#x200B;* [Substance Engine] Unterstützung der Standardfarbe in neuen .sbsar-Dateien
&#x200B;* [Automatisches Ausgliedern] Leistungsverbesserung
&#x200B;* [Exportieren] Fügen Sie visuelles Feedback hinzu, um anzugeben, welche UV-Kachel-Auflösung von der Standardauflösung des Projekts abweicht
&#x200B;* [Exportieren] Hinzufügen des Szenengrößenfaktors zur exportierten Shader-JSON-Datei
&#x200B;* [Sprache] Japanische Übersetzung hinzufügen
&#x200B;* [UI] Aktualisierung des Fensters mit Versionierung interner Abhängigkeiten
&#x200B;* [Scripting]&#x200B;[Python] Verwaltung von Shelf-Ressourcen zulassen
&#x200B;* [Scripting]&#x200B;[Python] Ermitteln Sie, wann ein Projekt zum Backen und Exportieren bereit ist.
&#x200B;* [Scripting]&#x200B;[Python] Ermitteln Sie, wann ein Shelf das Crawlen von Ressourcen auf der Festplatte abgeschlossen hat.
&#x200B;* [Scripting]&#x200B;[Python] Liste der UV-Kacheln pro Textursatz abfragen
&#x200B;* [Scripting]&#x200B;[Python] Zulassen, dass den Shelf-Ressourcen eine benutzerdefinierte Vorschau zugewiesen wird
&#x200B;* [Scripting]&#x200B;[Python] Verwaltung benutzerdefinierter Ablagen zulassen
&#x200B;* [Scripting]&#x200B;[Python] Hinzufügen eines Methodenindexes in jedem Untermodul in der Dokumentation
&#x200B;* [Scripting]&#x200B;[Python] Neuer Stil für die Dokumentation
&#x200B;* [Scripting]&#x200B;[Python] Verbesserung der Ressourcen und der Dokumentation im Shelf
&#x200B;* [Inhalt] Drei neue Werkzeugvorgaben zum Erstellen von Nähten
&#x200B;* [Shelf] Entfernen Sie vorübergehend &quot;Exportieren auf Substance share&quot;, während Sie zur neuen Substance share-Plattform wechseln.

**Fest:**

&#x200B;* Absturz bei Verwendung von Monitoren mit unterschiedlichen Auflösungen
&#x200B;* Absturz im Substance Engine mit einigen seltenen Projekten
&#x200B;* Die Aktualisierung des Viewports schlägt beim Wechseln von Ebenen mit &quot;Ausgeschlossene Geometrie ausblenden/ignorieren&quot; fehl.
&#x200B;* [2D-Ansicht] Bei einigen Projekten kann 2D-Viewport fehlen
&#x200B;* [Baking] &quot;Übereinstimmung nach Mesh&quot; ignoriert Teile des Objekts
&#x200B;* [Ebenenstapel] Durch Klicken auf einen Ebeneneffekt wird der Ordner geöffnet.
&#x200B;* [Geometriemaske] UV-Kachel wird in der Maske immer noch gezählt, auch wenn der Mesh ohne sie erneut importiert wird
&#x200B;* [Geometriemaske] Das Kontextmenü im Viewport bietet nicht die richtigen Werkzeuge
&#x200B;* [Engine] Schwerwiegende Verzögerungen bei bestimmten Projekten
&#x200B;* [Scripting] Hohe Latenz bei Anforderungen an Remote-JSON-POST unter Windows
&#x200B;* [Linux] Vram-Menge wird bei bestimmten integrierten GPUs nicht richtig erkannt
&#x200B;* [Automatisch Entpackt] Absturz oder lange entpack an einigen Projekten

## Version 6

### 6.2.2 (2020.2.2)

*(Freigegeben: 28. September 2020)*
Zusammenfassung: **Nebenversion, Bugfix mit einigen Funktionen in der Python-API**

**Hinzugefügt:**

&#x200B;* [Leistung] Nicht alle UV-Kacheln bei Verwendung der Farb-ID berechnen
&#x200B;* [Baker]&#x200B;[UI] Textursatz-Beschreibungen anzeigen
&#x200B;* [Baker] Speichern von Baking-Einstellungen zulassen
&#x200B;* [Baker] Hinzufügen aller reduzierten/erweiterter Optionen zur Registerkarte &quot;Auswahl&quot;
&#x200B;* [Liste der Textursatz] Beschreibung ausblenden, wenn leer
&#x200B;* [UV-Kacheln]&#x200B;[Liste der Textursatz] Durch Klicken auf die UV-Kachel sollte die Liste erweitert/reduziert werden.
&#x200B;* [Exportieren]&#x200B;[UI] Horizontales Ändern der Größe des Bedienfelds &quot;Textursatz-Liste&quot; zulassen
&#x200B;* [Exportieren]&#x200B;[UI] Konsistenter QuickInfo-Text für UV-Kacheln und Textursatz-Arbeitsablauf mit nicht ausgewählten Texturen
&#x200B;* [Scripting]&#x200B;[Python] Verwenden von Exportvorgaben zum Exportieren von Texturen zulassen
&#x200B;* [Scripting]&#x200B;[Python] Hinzufügen eines Änderungsprotokolls in der Dokumentation
&#x200B;* [Scripting]&#x200B;[Python] Ermöglicht die Abfrage aller verfügbaren Kanäle auf einem bestimmten Stapel.
&#x200B;* [Scripting]&#x200B;[Python] Verbesserungen der Konsolen-Benutzeroberfläche

**Fest:**

&#x200B;* [AMD] Falsche Erkennung veralteter Treiberversionen
&#x200B;* Absturz beim erneuten Importieren eines Meshs mit unterschiedlichem UV-Kacheln-Layout in einigen Fällen
&#x200B;* Absturz bei der Verwendung von Partikeln mit UDIM auf sehr schweren Meshs
&#x200B;* [UV-Kacheln] Absturz beim Exportieren eines Meshs mit Versatz-Informationen in einigen Fällen
&#x200B;* [Exportieren]&#x200B;[Absturz] Exportieren von 2D-Ansichten im PSD-Format kann einen Absturz verursachen
&#x200B;* Das Importieren von Bildern als Sequenzen beim Erstellen eines Projekts funktioniert nicht
&#x200B;* Engine in einer Endlosschleife
&#x200B;* [Tastaturbefehl] Kamera dreht sich immer im einrasten Modus, wenn die Kurzbefehle für den einrasten Modus geändert werden
&#x200B;* Mesh werden immer automatisch entpackt, wenn sie erneut importiert werden, auch wenn die Option deaktiviert ist
&#x200B;* [Liste der Textursatz] Das Textfeld &quot;Beschreibung&quot; ist in der Edition manchmal nicht vollständig sichtbar.
&#x200B;* [Liste der Textursatz] Dropdown-Menü zum Ein-/Ausblenden von Textursätzen ist nicht vollständig sichtbar
&#x200B;* [Liste der Textursatz] Wenn Sie auf das Augensymbol klicken, sollte nicht der Name &quot;Textursatz bearbeiten&quot; eingegeben werden.
&#x200B;* [Kanaleinstellungen] Beim Entfernen eines Textursatzes wird auch der darunter liegende Kanal entfernt
&#x200B;* [Exportieren] Alle einschließen und Alle zurücksetzen berücksichtigt keine UV-Kacheln
&#x200B;* [Baker] Während des Bakings werden nicht ausgewählte Baker angezeigt.
&#x200B;* Die Behebungsaktualisierung wird bei durch Baking erzeugte Map als Eingabe nicht berücksichtigt
&#x200B;* [UV-Kacheln]&#x200B;[Viewport] 3D-Viewport friert ein, wenn Intelligente Material nach UV-Kachel mit ausgewählter Ordnermaske hinzugefügt wird
&#x200B;* [UV-Kacheln]&#x200B;[Viewport] Drahtgitter ist weiterhin für ausgeblendete Kacheln sichtbar, wenn der Modus &quot;Malen durch&quot; aktiviert ist.
&#x200B;* [Export]&#x200B;[Sketchfab] Probleme mit dem Abonnementtyp &quot;Plus&quot;
&#x200B;* [Sketchfab] Das Kontrollkästchen &quot;Dieses Asset ist privat&quot; wird nach dem Kontowechsel nicht angezeigt
&#x200B;* [Exportieren]&#x200B;[Inhalt] &quot;Verwackelt&quot;-Pinselvorgaben können zu Leistungsproblemen führen
&#x200B;* [Plugin Photoshop] Meldung im Protokoll: nicht kompatibel mit dem UV-Kachel-Workflow
&#x200B;* [Scripting]&#x200B;[Python] PYTHONPATH env var verhindert den Start der Anwendung
&#x200B;* [Scripting]&#x200B;[Python] Typo in der Python-Dokumentation

### 6.2.1 (2020.2.1)

*(Freigegeben: 29. Juli 2020)*
Zusammenfassung: **Nebenversion, Hotfix**

**Hinzugefügt:**

&#x200B;* Umgebungsvariable &quot;SUBSTANCE\_PAINTER\_VRAM\_BUDGET&quot; hinzufügen, um GPU-VRam-Wert zu überschreiben
&#x200B;* [UV-Kacheln]&#x200B;[Leistung] Nicht alle UV-Kacheln bei Verwendung des Polygon-Füllwerkzeugs berechnen

**Fest:**

&#x200B;* [Iray] Beim Speichern des Renderings wird ein Fehler zurückgegeben, der zu einem schwarzen Bild führt
&#x200B;* [Linux] Absturz nach dem Begrüßungsbildschirm unter CentOS 7.3
&#x200B;* [Linux] Vram-Menge wird bei bestimmten Konfigurationen nicht richtig erkannt
&#x200B;* [Absturz] Öffnen eines Projekts mit dem Namen des duplizierten Textursatzes
&#x200B;* [Engine] Cache-Invalidierungsproblem beim Ändern einer Maske
&#x200B;* [Liste der Textursatz] Falscher Schrifteffekt, wenn Textursatz deaktiviert ist

**Bekannte Probleme:**

&#x200B;* [Liste der Textursatz] Die Beschreibung kann nicht ausgeblendet werden.
&#x200B;* [Textursatz List] UI-Probleme
&#x200B;* [Iray] PSD-Rendering wird nicht geöffnet
&#x200B;* [Plug-In Photoshop] Nicht kompatibel mit dem Arbeitsablauf für UV-Kacheln

### 6.2.0 (2020.2.0)

*(Freigegeben: 23. Juli 2020)*
Zusammenfassung: **Hauptversion mit neuem UV-Kacheln-Workflow, Malen über UV-Kacheln hinweg und Leistungsverbesserung**

**Hinzugefügt:**

&#x200B;* UV-Kacheln (UDIM)
&#x200B;* [UV-Kacheln] Malen über UV-Kacheln
&#x200B;* [UV-Kacheln] Auswahl zwischen neuem und veraltetem Arbeitsablauf für UV-Kacheln zulassen
&#x200B;* [UV-Kacheln] Importieren von UDIM/UV-Kachel-Bildsequenzen als Ressource
&#x200B;* [UV-Kacheln] Liste der UV-Kacheln pro Textursatz im Fenster &quot;Liste der Textursatz&quot; hinzufügen
&#x200B;* [UV-Kacheln] Erlauben Sie, die Auflösung mehrerer UV-Kacheln gleichzeitig in den Textursatz-Einstellungen zu bearbeiten.
&#x200B;* [UV-Kacheln]&#x200B;[2D-Ansicht] UV-Kacheln als Raster anzeigen
&#x200B;* [UV-Kacheln]&#x200B;[2D-Ansichten] Neue Viewport-Schaltfläche zum Anzeigen oder Ausblenden von UV-Kacheln-Informationen
&#x200B;* [UV-Kacheln] Wechseln des Malwerkzeugs für UV-Kachel-Projekte standardmäßig zum Ein Kanal
&#x200B;* [UV-Kacheln] Neue Schaltfläche in der kontextabhängigen Symbolleiste, um maskierte UV-Kacheln beim Malen zu ignorieren
&#x200B;* [UV-Kacheln]&#x200B;[Ebenenstapel] Neue Ebenenstapel-Symbole zur Leistungssteigerung
&#x200B;* [UV-Kacheln]&#x200B;[Ebenenstapel] Verbessern der Symbole &quot;Malen und Füllen&quot; in der Symbolleiste
&#x200B;* [UV-Kachel Maske]&#x200B;[2D-Ansicht] Mehrere UV-Kacheln gleichzeitig ein- oder ausschließen (Linksklick, Strg+Linksklick)
&#x200B;* [Ebenenmaske] Neue Ebenenmaske zum Einschließen, Ausschließen von Kacheln pro UV-Kachel mit neuem Symbol
&#x200B;* [UV-Kacheln-Maske]&#x200B;[Ebenenstapel] Zeigt die Anzahl der UV-Kacheln im UV-Kacheln-Maskensymbol an, wenn nicht alle eingeschlossen sind.
&#x200B;* [UV-Kachel-Maske]&#x200B;[2D/3D-Ansicht] Fügen Sie einen Hover-Effekt hinzu, um UV-Kacheln unter dem Cursor darzustellen.
&#x200B;* [UV-Kacheln]&#x200B;[Baker] Auswahl und Baking bestimmter UV-Kacheln zulassen
&#x200B;* [UV-Kacheln]&#x200B;[Baker] Hinzufügen von Auswahloptionen für Textursatz/UV-Kacheln
&#x200B;* [UV-Kacheln]&#x200B;[Baker] Kontextmenüoption zum Auswählen von UV-Kacheln in einem Textursatz
&#x200B;* [UV-Kacheln]&#x200B;[Baker] Ermöglichen Sie eine schnelle Auswahl im Textursatz/in den UV-Kacheln durch Ziehen
&#x200B;* [UV-Kacheln]&#x200B;[Baker] Ersetzen Sie die Schaltflächen &quot;Alle&quot; und &quot;Keine&quot; in Mesh-Map durch explizitere Auswahloptionen.
&#x200B;* [UV-Kacheln]&#x200B;[Baker] Anzahl der zu Baking führend Texturen anzeigen
&#x200B;* [UV-Kacheln]&#x200B;[Exportieren] Auswahl und Export bestimmter UV-Kacheln zulassen
&#x200B;* [UV-Kacheln]&#x200B;[Exportieren] Ermöglicht die schnelle Auswahl von UV-Kacheln durch Ziehen
&#x200B;* [UV-Kacheln]&#x200B;[Exportieren] Dropdown-Menüoptionen für UV-Kacheln hinzufügen
&#x200B;* [UV-Kacheln]&#x200B;[Exportieren] Stellen Sie einige Exportvorgaben nicht zur Verfügung, wenn sie nicht mit UV-Kacheln funktionieren (Adobe Dimension, Sketchfab, glTF, USD)
&#x200B;* [UV-Kacheln]&#x200B;[Inhalt] Aktualisieren Sie die Exportvorgaben, um das neue $udim-Tag zu verwenden
&#x200B;* [UV-Kacheln] Verbessern der Fehlerberichterstattung beim Importieren von Meshs mit überlappenden UV-Inseln
&#x200B;* [UV-Kacheln] In Iray kompatible UV-Kacheln
&#x200B;* [UV-Kacheln]&#x200B;[Skripterstellung] Hinzufügen einer Exportdokumentation für UV-Kacheln zu Python-Dokumenten
&#x200B;* Leistung
&#x200B;* [Leistung] Neue Schaltfläche in der kontextabhängigen Symbolleiste zum Anhalten der Modulberechnung bei der Arbeit (UMSCHALT+ESC)
&#x200B;* [Leistung] Schnellere Projektöffnung durch Verzögerung der Berechnung des Texture Set-Caches
&#x200B;* [Leistung] Warten Sie nicht darauf, dass Gitterzuordnungen beim Öffnen des Projekts geladen werden.
&#x200B;* [Leistung]&#x200B;[2D-/3D-Ansicht] Berechnen Sie den Maskenkanal im Viewport nicht, wenn er nicht verwendet wird.
&#x200B;* [Leistung] Die Anwendung nicht blockieren, wenn in den Viewports angezeigte Gitterzuordnungen geladen werden.
&#x200B;* [Leistung] Verbessern der inkrementellen Speichergeschwindigkeit beim Speichern eines Projekts
&#x200B;* [Performance]&#x200B;[Bäcker] Ändern Sie die Standardeinstellungen für die Erweiterung, um Zeit und Projektgröße zu sparen.
&#x200B;* [Leistung]&#x200B;[Bäcker] Wechseln Sie auf bestimmte Bäcker in Graustufen, um Zeit und Projektgröße zu sparen.
&#x200B;* [Performance]&#x200B;[Export] Verbessern Sie die Engine-Performance, um Texturen schneller zu exportieren.
&#x200B;* [Leistung]&#x200B;[Export] Verbessern Sie die Reaktionsfähigkeit beim Öffnen des Exportdialogs mit vielen Textursätzen
&#x200B;* [Leistung]&#x200B;[Export] Verbessern Sie die Leistung beim Wechsel zur Registerkarte &quot;Exportliste&quot;.
&#x200B;* [Performance]&#x200B;[Iris] Reduzieren der Startzeit von Iris
&#x200B;* Sonstige
&#x200B;* [Bäcker] Hinzufügen von Auswahloptionen für Textursätze
&#x200B;* Shader-Instanzverwaltung in die Textursatzeinstellungen verschieben
&#x200B;* [2D-/3D-Ansicht] Fügen Sie am unteren Rand des Viewports eine Meldung hinzu, die angibt, welcher Maskentyp bearbeitet wurde.
&#x200B;* [Ebenenstapel] Neue Option in den Einstellungen, um zwischen alten und neuen Miniaturansichten zu wechseln
&#x200B;* [Ebenenstapel] Fügen Sie visuelles Feedback hinzu, um den Ladezustand der Miniaturansichten anzuzeigen
&#x200B;* [Proj] Neuer Projektionsmodus &quot;Füllen (Per UV-Kachel abgleichen)&quot; zum Laden von Bildsequenzen
&#x200B;* [Proj] Ändern Sie den Projektionsmodus für Füllebenen in &quot;Füllen (Per UV-Kachel abgleichen)&quot; in bestimmten Fällen.
&#x200B;* [Inhalt] Optimieren Sie die Pinselvorgaben für Kohle, um die Leistung zu verbessern
&#x200B;* Aktualisieren Sie Iray auf Version 2020.0.0
&#x200B;* [Exportieren] Deaktivieren Sie die Registerkarte &quot;Exportliste&quot;, wenn nichts ausgewählt ist
&#x200B;* Automatisches Ausgliedern
&#x200B;* [Automatisch entpacken] Verbessern der Erfolgsrate des automatischen Entpackungsprozesses
&#x200B;* [Automatisch entpacken] Verbesserte Parametrisierung zur Erhöhung der Geschwindigkeit und Stabilität

**Fest:**

&#x200B;* [Alembic] Facesets werden beim Importieren von Dateien ignoriert
&#x200B;* [Alembic] Unendliche Ladezeit mit bestimmten Dateien
&#x200B;* [Importieren] Falsche UDIM-Bildsequenz wird importiert, wenn nur die Dateierweiterung unterschiedlich ist
&#x200B;* [Absturz] Der Versuch, ein durch einen anderen Prozess gesperrtes Projekt zu öffnen, führt zu einem Absturz
&#x200B;* [Projektion] Artefakte am duplizierten Gitter bei Verwendung der triplanaren Projektion
&#x200B;* [Exportieren] Emissive-Kanal wird nicht mit USD exportiert
&#x200B;* [Inhalt] Smart Material &quot;Charcoal&quot; enthält Pinselstriche

**Bekannte Probleme:**

&#x200B;* [Textursatzliste] Beschreibung kann nicht ausgeblendet werden.
&#x200B;* [Texture Set List] UI-Probleme

### 6.1.3 (2020.1.3)

*(Freigegeben: 16. Juni 2020)*
Zusammenfassung: **Bugfix**

**Hinzugefügt:**

&#x200B;* [Exportieren] Hinzufügen von Versatz-Einstellungen in der Shader-Parameter-JSON-Datei

**Fest:**

&#x200B;* [Absturz]&#x200B;[Engine] Absturz beim Versuch, vorhandene Kanäle zu löschen und zu ersetzen
&#x200B;* [Absturz] Ändern des Shaders nach dem Malen einer Maske in der Materialschichtung
&#x200B;* [Absturz]&#x200B;[Engine] Absturz mit einigen umfangreichen Projekten
&#x200B;* [Baker] Zuordnung nach Name funktioniert nicht mit aus zBrush exportierten OBJ
&#x200B;* [Versatz]&#x200B;[SVT] Texturen werden beim Öffnen des Projekts nicht angezeigt, wenn der Versatz aktiviert ist
&#x200B;* [Exportieren] Einige Texturen werden in einheitlichem Grau exportiert.
&#x200B;* [Exportieren] Deaktivierte Textursätze sollten nicht für Dimension- und Sketchfab-Exportvorgaben exportiert werden
&#x200B;* [Scripting]&#x200B;[JavaScript]-Absturz bei der Verwendung der JavaScript-API für den Zugriff auf die Exportkonfiguration im onProjectOpened-Ereignis
&#x200B;* [Skripterstellung]&#x200B;[Javascript] onExportFinished() wird nach einem Export nicht aufgerufen

### 6.1.2 (2020.1.2)

*(Freigegeben: 28. Mai 2020)*
Zusammenfassung: **Bugfix mit Substance Engine- und Baker-Update**

**Hinzugefügt:**

&#x200B;* [Baker] Update auf die neueste Version
&#x200B;* [Baker] Neue Sampling-Methode in den Bakern Ambient occlusion, Krümmung, Thickness
&#x200B;* Aktualisieren Sie auf die neueste Version von Substance Engine
&#x200B;* [Scripting]&#x200B;[Python] Erstellen der ResourceID für Projektressourcen zulassen
&#x200B;* [Scripting]&#x200B;[Python] Abfragen von Kanalinformationen zulassen
&#x200B;* [Scripting]&#x200B;[Python] Fügen Sie Dryrun- und Rückruffunktionen hinzu, um den Export von Texturen zu simulieren

**Fest:**

&#x200B;* [Baker] Falsche Normale im Welt-Raum-Normale-Baker unter Verwendung einer Tangente-Normalen-Map in bestimmten Fällen
&#x200B;* [Baker] Fehler beim Baking von Ambient occlusion mit Optix, wenn kein hohes Poly
&#x200B;* [Dynamische Pinselstriche] Verzögerung beim Laden eines bestimmten Textursatzes
&#x200B;* [Exportieren] Die deaktivierten Textursatz für USD sollten nicht exportiert werden. glTF
&#x200B;* [Skripterstellung]&#x200B;[JavaScript] Die Einstellungen für den neuen Krümmung-Baker können nicht bearbeitet werden.
&#x200B;* [Scripting]&#x200B;[JavaScript] alg.texturesets.addChannel() gibt in einigen Fällen keinen Fehler zurück.
&#x200B;* [Scripting]&#x200B;[JavaScript] Tippfehler in der JavaScript-API-Dokumentation für setProjectExportOptions()
&#x200B;* [Skripterstellung]&#x200B;[JavaScript] Exportiert immer alle Textursatz
&#x200B;* [Scripting]&#x200B;[Python] sys.executable gibt einen Pfad zu python.exe anstelle von Substance Painter zurück
&#x200B;* Textur-Cache nicht kompatibel mit Mac OS und Windows/Linux
&#x200B;* [Livelink UE4] Nur das letzte Material wird für alle Textursatz in einem kombinierten Mesh verwendet.

**Bekannte Probleme:**

&#x200B;* [Exportieren]&#x200B;[Dimension]&#x200B;[Skecthfab] Die deaktivierten Textursatz sollten nicht exportiert werden.
&#x200B;* [Absturz] Ändern des Shaders nach dem Malen einer Maske in der Materialschichtung

### 6.1.1 (2020.1.1)

*(Freigegeben: 5. Mai 2020)*
Zusammenfassung: **Hotfix**

**Hinzugefügt:**

&#x200B;* [Export] Überschriebenes visuelles Feedback zu TextureSet

**Fest:**

&#x200B;* [Export] Exporter-Fenster ist auf einem Monitor mit spezieller Auflösung zu groß und kann nicht skaliert werden
&#x200B;* [Export] Optionen werden nach dem Export nicht gespeichert
&#x200B;* [Export] Absturz oder kann nicht mit der Exportvorgabe &quot;Aus Cache&quot; exportiert werden
&#x200B;* [Export] Wenn Sie den Export abbrechen, wird eine unerwartete zusätzliche leere Map generiert.
&#x200B;* [Exportieren] Virtuelle Exportvoreinstellungen korrigieren
&#x200B;* [Python] PYTHONPATH env var wird nicht berücksichtigt
&#x200B;* [Python]&#x200B;[Export] Wenn Sie den Export über Python abbrechen, wird ein Ausnahmefehler zurückgegeben.
&#x200B;* [Python]&#x200B;[Export] export\_project\_textures falsches Ergebnis mit psd-Dateiformat
&#x200B;* [Bäcker] Absturz unter Linux mit GPU-Raytracing

**Bekannte Probleme:**

&#x200B;* [JavaScript] Neue Curvature-Bäcker-Einstellungen können nicht bearbeitet werden
&#x200B;* [JavaScript]&#x200B;[Export] Exportiert immer alle Textursätze
&#x200B;* [Exportieren]&#x200B;[USD] Die deaktivierten Textursätze sollten nicht exportiert werden.
&#x200B;* [Absturz] Ändern des Shaders nach dem Malen einer Maske in der Materialschichtung

### 6.1.0 (2020.1.0)

*(Freigegeben: 22. April 2020)*
Zusammenfassung: **Hauptversion mit neuem Textur- und Gitterexporteur (mit Versatz und Tesselierung), aktualisiertem UV-Auspacken mit mehr Steuerelementen, neuen Bäckereien, neuer Scripting-Python-API, besserem UX für Decalprojektion und neuem Inhalt**

**Hinzugefügt:**

&#x200B;* Neuer Textur- und Maschenexporteur
&#x200B;* [Export] Benutzeroberfläche für neue Ausführer
&#x200B;* [Exportieren]&#x200B;[Registerkarte &quot;Exportieren&quot;] Ermöglicht die Auswahl der Kartenkanäle, die pro Textursatz exportiert werden.
&#x200B;* [Exportieren]&#x200B;[Registerkarte &quot;Exportieren&quot;] Modifizierung der Größe des Textursatzes für alle Textursatz in einer Aktion zulassen
&#x200B;* [Exportieren]&#x200B;[Registerkarte &quot;Exportieren&quot;] Lassen Sie eine andere Vorlage pro Textursatz zu (außer USD, glTF, Sketchfab und Dimension)
&#x200B;* [Exportieren]&#x200B;[Registerkarte &quot;Exportieren&quot;] Schnelle Aktivierung und Deaktivierung von Karten und Textursätze
&#x200B;* [Exportieren]&#x200B;[Registerkarte &quot;Exportieren&quot;] Die Exportauflösung 8192x8192 ist nicht mehr experimentell
&#x200B;* [Exportieren]&#x200B;[Registerkarte &quot;Exportieren&quot;] Änderung des Dateiformats und der Bittiefe pro Map zulassen
&#x200B;* [Exportieren]&#x200B;[Registerkarte &quot;Exportieren&quot;] Zurücksetzen auf die Werte der Standardparameter zulassen
&#x200B;* [Exportieren]&#x200B;[Registerkarte &quot;Exportieren&quot;] Speichern von Einstellungen ohne Exportieren zulassen
&#x200B;* [Exportieren]&#x200B;[Registerkarte &quot;Ausgabevorlagen&quot;] Benennen Sie die Registerkarte &quot;Konfiguration&quot; in die Registerkarte &quot;Ausgabevorlagen&quot; um
&#x200B;* [Exportieren]&#x200B;[Registerkarte &quot;Ausgabevorlagen&quot;] Definition von Dateiformat und Bittiefe pro voreingestellter Map zulassen
&#x200B;* [Export]&#x200B;[Registerkarte &quot;Liste der Exporte&quot;] Neue Vorschauregisterkarte zum Zusammenfassen und Anzeigen des Exportvorgangs
&#x200B;* [Mesh importieren/exportieren] Optimierung der Performance der Import-/Exportzeit
&#x200B;* [Mesh exportieren] Mesh in FBX exportieren
&#x200B;* [Mesh exportieren] Exportieren von Mesh mit Versatz und Tessellation
&#x200B;* [Mesh exportieren]&#x200B;[UI] Neue Einstellungen für die Neuberechnung des normalen Scheitelpunkts, Anwendung der Triangulation
&#x200B;* [Mesh exportieren] Exportieren der ursprünglichen Mesh-Topologie mit neuen UVs, die durch automatischen entpack generiert werden
&#x200B;* Automatischer entpack mit weiteren Steuerelementen wurde aktualisiert
&#x200B;* [UV Entpackend]&#x200B;[UI] Fügen Sie die Einstellung hinzu, um die automatische UV-entpack in einem neuen Projektfenster zu aktivieren
&#x200B;* [Entpackend UV]&#x200B;[UI] Neue Optionen zum Steuern der entpackend Schritte (Nähte, entpackend Packing)
&#x200B;* [Entpackend UV]&#x200B;[UI] Beibehaltung bestehender entpackend Nähte/entpackend /Packing zulassen
&#x200B;* [UV Entpackend]&#x200B;[UI] Neue Optionen zur vollständigen Neuberechnung entpackend Schritte
&#x200B;* [Entpackend UV]&#x200B;[UI] Neue Option zur Steuerung der Randgröße (keine, kleine, mittlere und große)
&#x200B;* Neue Baker
&#x200B;* [Baker] Alte Krümmung durch neue Krümmung aus Mesh ersetzen
&#x200B;* [Baker] Fügen Sie die Option &quot;Match by Name&quot; hinzu, um die Rückseite im Baker &quot;Ambient occlusion&quot; zu ignorieren
&#x200B;* [Bäcker] Hinzufügen der Option &quot;Grundebene&quot; im Bäcker &quot;Ambient Verdeckung&quot;
&#x200B;* Neue Python-API für die Skripterstellung (3.7.6)
&#x200B;* [Python]&#x200B;[UI] Neues Skriptmenü für Python
&#x200B;* [Python]&#x200B;[UI] Neue Python-Dokumentation im Hilfemenü
&#x200B;* [Python] Substance Painter-Python-Module verfügbar machen: substance\_painter, alg, display, project.setting, project, texturesets, ui
&#x200B;* [Python] Stellen Sie das neue Python-Modul &quot;substance\_painter&quot; bereit
&#x200B;* [Python] Neues Python-Untermodul verfügbar machen: alg, display, log, project, resource, texturesets, ui
&#x200B;* [Python] Listener für Projektänderungen
&#x200B;* [Python] Neue Beispiele in der Python-Dokumentation
&#x200B;* [JavaScript]&#x200B;[UI] Menü &quot;Plug-ins&quot; durch JavaScript ersetzt
&#x200B;* [Viewport] Ermöglicht die Erstellung einer Aufkleberprojektion durch Ziehen/Ablegen + ALT einer Ressource aus dem Regal.
&#x200B;* Neue Inhalte
&#x200B;* [Inhalt] 5 neue Aufklebermaterialien von Substance Source
&#x200B;* [Inhalt] Hinzufügen neuer Projektvorlagen und Exportieren von Vorgaben für den Maxwell-Renderer
&#x200B;* [Inhalt] Hinzufügen einer Projektvorlage für den Keyshot 9-Export
&#x200B;* [Inhalt] Aktualisieren der Keyshot 9-Exportvoreinstellung, um Versatz und Emissionen zu unterstützen
&#x200B;* [Inhalt]&#x200B;[Exporter] Aktualisierung aller Exportvorgaben, um die neuesten Versionen von Game-Engines und Renderern zu berücksichtigen
&#x200B;* [Content]&#x200B;[Exporter] Aktualisieren Sie die Exportvoreinstellungsdateien, um das neue Format und die Dithering-Einstellungen zu verwenden
&#x200B;* [Inhalt] Neue Vorlagen und Shader zur Unterstützung von VRay-Material (VRayMtl)
&#x200B;* [Ebenenstapel] Löschen von Ebeneneffekten mit dem Papierkorbsymbol oder dem Tastaturbefehl Löschen zulassen
&#x200B;* Plug-in-Substance Source entfernen (Launcher mit &quot;Senden an&quot;-Funktion verwenden)
&#x200B;* [Windows] TDR-Warnung nicht auf High-End-GPUs anzeigen

**Fest:**

&#x200B;* Übersetzungsprobleme im Dialogfeld &quot;Neue Projektdatei&quot;
&#x200B;* [Bäcker] Einstellung &quot;Vorverarbeitete Szenendatei speichern&quot; funktioniert nicht mehr
&#x200B;* [Planare Projektion] Projektion funktioniert nicht bei Gittern mit sich wiederholenden UVs
&#x200B;* [Decal] Verhaltensunterschied im normalen Kanal bei Verwendung verschiedener Projektionsmodi für Füllebenen
&#x200B;* [Verwischen]&#x200B;[Klonen] Beim Malen in der Maske kann ein Artefakt angezeigt werden
&#x200B;* [Engine] Absturz mit bestimmtem Ebeneninhalt
&#x200B;* [Engine] Zufälliger Absturz beim Malen in einigen Fällen
&#x200B;* [Ankerpunkt] Der Verweis auf eine leere Maske gibt immer Weiß zurück
&#x200B;* [Export] Ebene wird in bestimmten Stapelkonfigurationen nicht berücksichtigt
&#x200B;* [Exportgitter] Kann nicht mit einem Pfad exportiert werden, der Sonderzeichen enthält
&#x200B;* [Export Mesh] GlTF-Dateien können beim Export aus Linux oder MacOS nicht gelesen werden
&#x200B;* [Mesh importieren] Der erneute Import von DAE, PLY oder glTF funktioniert nicht wie beabsichtigt

**Bekannte Probleme:**

&#x200B;* [Skripterstellung]&#x200B;[JavaScript] Neue Einstellungen für den Kurvenzeichner können nicht bearbeitet werden.
&#x200B;* [Bäcker] Absturz unter Linux mit GPU-Raytracing
&#x200B;* [Exportieren]&#x200B;[USD] Die deaktivierten Textursätze sollten nicht exportiert werden.
&#x200B;* [Absturz] Ändern des Shaders nach dem Malen einer Maske in der Materialschichtung

## Version 5

### 5.3.3 (2019.3.3)

*(Freigegeben: 6. Februar 2020)*
Zusammenfassung: **Bugfix mit Upgrade auf Irak 2019.3**

**Hinzugefügt:**

&#x200B;* Upgrade auf Irak 2019.3
&#x200B;* [Log] Veraltetes BIOS für Ryzen-CPU anzeigen, was während des Bakings zu Abstürzen führt
&#x200B;* [ABR] Extrahieren von ABR-Alphas in das Regal

**Fest:**

&#x200B;* [Baker] Baking schlägt fehl, wenn High-Poly-Mesh keine UVs enthält
&#x200B;* [Linux] Benutzerdefinierte Mauskürzel werden nicht gespeichert
&#x200B;* [Pinsel] Die Kontur verschwindet mit einigen Alpha-Formen
&#x200B;* [Tablet] Fehlerhafte Erkennung beim Verschieben von Schiebereglern
&#x200B;* [Tastaturbefehle] Mit Strg+Alt+Mausklick kann kein Tastaturbefehl eingerichtet werden
&#x200B;* [Regal] Die Ressourcen-QuickInfo wird bei Verwendung eines Stift-Tablets nicht angezeigt
&#x200B;* [2D-Ansicht]&#x200B;[Exportieren] Die voreingestellte 2D-Ansicht berücksichtigt nicht die normalen Informationen
&#x200B;* Einfrieren beim Malen in UV-Ausrichtung mit bestimmten Pinseln
&#x200B;* Malen unter einem Filter erzeugt Artefakt auf dem laufenden Strich
&#x200B;* [Viewport] Falscher Texturen-Cache im Viewport nach dem erneuten Importieren eines Meshs
&#x200B;* [Absturz] Fehler beim Speichern nach dem Export in Photoshop
&#x200B;* [Absturz] Schreiben von Sonderzeichen im Präfix beim Importieren von Ressourcen
&#x200B;* [Absturz] Klicken Sie in den Ankerpunkt-Eigenschaften auf die Referenz.
&#x200B;* [Ankerpunkte] Kanal wird nicht aktualisiert, wenn ein Filter zwischen Ankerpunkt und Referenz vorhanden ist
&#x200B;* Iray-URL-Link im Hilfemenü funktioniert nicht

**Bekannte Probleme:**

&#x200B;* [Entpackend UV] Die Verarbeitung von Meshs mit hohem Poly-Anteil kann lange dauern
&#x200B;* [Entpackend UV] Scheitelpunkt mit genau denselben Koordinaten werden zusammengeführt
&#x200B;* [UV Entpackend] In seltenen Fällen kann die UV-Generierung auf einigen Mesh-Teilen fehlschlagen.
&#x200B;* [UV Entpackend] Ungleichmäßiges oder stark verzerrtes Textilverhältnis in einer einzigen UV-Insel in einigen Fällen
&#x200B;* [UV Entpackend] Ungleichmäßiges Textilverhältnis zwischen Textursätzen
&#x200B;* [UV Entpackend] UV-Insel kann sehr lang sein und passt in manchen Fällen nicht in den UV-Raum
&#x200B;* [UV Entpackend] Flächen mit degenerierten Flächen oder nicht dreieckigem Mesh mit kleinen oder überlappenden Kanten werden möglicherweise nicht in UV entpackt

### 5.3.2 (2019.3.2)

*(Freigegeben: 21. Januar 2020)*
Zusammenfassung: **Bugfix**

**Fest:**

&#x200B;* Beim Öffnen eines Projekts, das im Einzelkanalmodus gespeichert wurde, wird der Mesh nicht angezeigt
&#x200B;* Viewport wird nicht immer aktualisiert, wenn unter einer Ebene mit dem Kopierwerkzeug gemalt wird

**Bekannte Probleme:**

&#x200B;* [Bäcker] Absturz im Zusammenhang mit Multithreading auf Ryzen-CPUs
&#x200B;* [UV-Entpacken] Die Verarbeitung von hochpolaren Netzen kann lange dauern
&#x200B;* [UV-Entpackung] Eckpunkte mit genau denselben Koordinaten werden zusammengeführt
&#x200B;* [UV-Entpackung] Die UV-Generierung kann in seltenen Fällen an einigen Netzteilen fehlschlagen
&#x200B;* [UV-Entpackung] Uneinheitliches oder stark verzerrtes Textilverhältnis in einer einzigen UV-Insel in einigen Fällen
&#x200B;* [UV-Entpackung] Nicht einheitliches Textilverhältnis zwischen Textursätzen
&#x200B;* [UV-Entpackung] erzeugte UV-Insel kann sehr lang sein und passt in einigen Fällen nicht in den UV-Raum.
&#x200B;* [UV-Entpackung] Degenerierte Flächen oder nicht dreieckige Netzflächen mit kleinen oder überlappenden Kanten werden möglicherweise nicht UV-entpackt

### 5.3.1 (2019.3.1)

*(Freigegeben: 20. Dezember 2019)*
Zusammenfassung: **Hotfix**

**Fest:**

&#x200B;* Absturz beim Arbeiten an Netzen mit bestimmten UV-Projektionen
&#x200B;* [ABR] Absturz beim Wechseln zwischen Photoshop-Vorgaben
&#x200B;* [Linux] Substance Painter kann unter CentOS 7.4 aufgrund eines libGLX-Abhängigkeitsproblems nicht gestartet werden
&#x200B;* [Bäcker] Absturz beim Backen nach Verwendung von Datei > Bereinigen
&#x200B;* [Bäcker] Dialogfeld &quot;Backfortschritt&quot; friert nach Abbruch ein
&#x200B;* [Bäcker] Backen von Gittern nach dem Exportieren von Texturen funktioniert nicht
&#x200B;* [Bäcker] Verwenden von &quot;Match By Name&quot; mit schwarzen Mesh Maps
&#x200B;* [Bäcker] Käfig wird nicht berücksichtigt
&#x200B;* [Shelf] Das Importieren von PSD-Dateien führt zu beschädigten Bildern
&#x200B;* [Beispiel] Beispielprojekt &quot;Matte&quot; mit beschädigten Kameras und falscher Exportvorgabe

**Bekannte Probleme:**

&#x200B;* [Bäcker] Absturz im Zusammenhang mit Multithreading auf Ryzen-CPUs
&#x200B;* [Entpackend UV] Die Verarbeitung von Meshs mit hohem Poly-Anteil kann lange dauern
&#x200B;* [Entpackend UV] Scheitelpunkt mit genau denselben Koordinaten werden zusammengeführt
&#x200B;* [UV Entpackend] In seltenen Fällen kann die UV-Generierung auf einigen Mesh-Teilen fehlschlagen.
&#x200B;* [UV Entpackend] Ungleichmäßiges oder stark verzerrtes Textilverhältnis in einer einzigen UV-Insel in einigen Fällen
&#x200B;* [UV Entpackend] Ungleichmäßiges Textilverhältnis zwischen Textursätzen
&#x200B;* [UV Entpackend] UV-Insel kann sehr lang sein und passt in manchen Fällen nicht in den UV-Raum
&#x200B;* [UV Entpackend] Flächen mit degenerierten Flächen oder nicht dreieckigem Mesh mit kleinen oder überlappenden Kanten werden möglicherweise nicht in UV entpackt

### 5.3.0 (2019.3.0)

*(Freigegeben: 17. Dezember 2019)*
Zusammenfassung: **Hauptversion mit Verbesserung der Benutzererfahrung beim Handmalen, Arbeiten mit Tablets, automatischem UV entpack in der Beta-Version (0.3.0) und verschiedenen neuen Inhalten zum Handmalen**

**Hinzugefügt:**

&#x200B;* Integration von Automatic UV entpack 0.3.0 in Substance Painter
&#x200B;* [UV entpackend] Automatische UV entpackend im Substance Painter, wenn keine UVs oder partielle UVs vorhanden sind
&#x200B;* [entpackend UV] Eine globale Einstellung zum Aktivieren und Deaktivieren
&#x200B;* [entpackend UV] In Protokolldatei gemeldete Version
&#x200B;* [entpackend UV]&#x200B;[UI] Anzeige des Fortschritts beim Entpackend UV
&#x200B;* [UI] Neue Einstellungen in der kontextabhängigen Symbolleiste zur Auswahl der Pinselvorschau: Vollständige Vorschau, Pinselkontur und Fadenkreuz
&#x200B;* [Tool] Neuer erweiterter Mischmodus im Alpha-Abschnitt: Aufhellen (Maximal) zusätzlich zu Normal
&#x200B;* [Ebenenstapel] Gammakorrektur-Option pro Ebene für Alpha oder Maske (Kontextmenü)
&#x200B;* [Ebenenstapel]&#x200B;[UI] Fügen Sie das Symbol &quot;i&quot; hinzu, wenn ein Alpha-Layer gamma-korrigiert ist
&#x200B;* [Tablet]&#x200B;[Tool] Gelegt Mindestdruck für Größe und Fluss
&#x200B;* [Tablet]&#x200B;[UI] Neue Einstellung in der kontextabhängigen Symbolleiste zur Auswahl des Kurvendrucks: linear, easy-in, easy-in-out
&#x200B;* [Tablet]&#x200B;[UX] Strg+Alt+Klick zum Scrollen hinzufügen
&#x200B;* Photoshop-Pinselvorgaben importieren (ABR-Format)
&#x200B;* [ABR] Support Shape-Parameter
&#x200B;* [ABR] Unterstützung von Parametern für die Formdynamik
&#x200B;* [ABR] Support Transfer-Parameter
&#x200B;* [ABR] Unterstützung von Streuungsparametern
&#x200B;* [ABR]&#x200B;[Dynamische Pinselstriche] Unterstützung von Rundheit und Spiegelung
&#x200B;* [ABR]&#x200B;[Shelf] Stellen Sie die Pinselordnerstruktur im Filter-Editor bereit.
&#x200B;* [ABR]&#x200B;[Regal] Photoshop-Symbol zu Miniaturansichten hinzufügen
&#x200B;* [ABR]&#x200B;[Regal] Fügen Sie eine Liste nicht unterstützter Parameter zur detaillierten Miniaturansicht von ABR hinzu.
&#x200B;* [Tool]&#x200B;[Dynamische Pinselstriche] Neue dynamische Stricheinstellung zur Steuerung der Anzahl der zu generierenden Zufallszahlen
&#x200B;* [Tool]&#x200B;[UI] Neue Verteilungs- und Achseneinstellungen für &quot;Jitter bei Streuung&quot; hinzufügen
&#x200B;* [Tastaturbefehl] Fügen Sie Strg+Umschalt+B hinzu, um das Backfenster zu öffnen
&#x200B;* [UI]&#x200B;[Menu] Eintrag im Menü &quot;Bearbeiten&quot; hinzufügen, um das Backfenster zu öffnen
&#x200B;* [UI]&#x200B;[Einstellungen] Verbesserte Ausrichtung der Liste der Tastaturbefehle
&#x200B;* [UI] Ersetzen von Drucksteuerelementen (Größe und Fluss) durch Schaltflächen zum Ein- und Ausschalten
&#x200B;* [Viewport] Ermöglicht die separate Fokussierung von 2D- und 3D-Viewport.
&#x200B;* Update auf QT 5.12.5
&#x200B;* [UI] Mesh-Ladefortschritt anzeigen
&#x200B;* [Substance] Zusätzliche Unterstützung für den nicht geklemmten und weichen Bereich mit Schiebereglern
&#x200B;* [Substance] Erhöhung der Präzision der Substance-Parameter auf bis zu 6 Dezimalstellen
&#x200B;* [Substance] Berücksichtigen Sie den durch einen Parameter definierten Schritt.
&#x200B;* [Substance] Optimieren der dynamischen Konturgenerierung mit Unterstützung von Bedingungen in Benutzerdaten
&#x200B;* [Substance] Legen Sie die Diagrammausgabe als Maske für alle Kanäle über Benutzerdaten fest.
&#x200B;* [Inhalt] Aktualisieren des Beispielprojekts &quot;Mat&quot; mit Kameratopologie, neuer ID-Versatz und neuen Kameras
&#x200B;* [Inhalt] Integration von drei neuen Filtern (MatFx): Comic, Aquarell, Ölfarbe (inspiriert von der Arbeit von Emrecan Cubukcu)
&#x200B;* [Inhalt] Integrieren Sie 102 Photoshop-Pinselvorgaben aus den Packs von Kyle T. Webster
&#x200B;* [Inhalt] Integrieren Sie 18 neue Pinselvorgaben: Malrollenpfeil, Malrollenwarntext, Aktivkohle - Fein und vieles mehr
&#x200B;* [Inhalt] Integrieren Sie 9 neue Alphas: Pinselmacher-Paintroller, Pinselmacher Photoshop, Pinselmuster und mehr
&#x200B;* [Inhalt] Integrieren Sie 2 neue Werkzeugvorgaben: Gouache Dense und Gouache Faded
&#x200B;* [Inhalt] 1 neuen Generator integrieren : UV-Checker (UV-Inseln und Nähte hervorheben)
&#x200B;* [Inhalt] Integrieren Sie 2 neue Exportvoreinstellungen: Keyshot 9+ und Spark AR Studio
&#x200B;* [Inhalt] 1 neue Projektvorlage integrieren : Spark AR Studio (Facebook)

**Fest:**

&#x200B;* [Tablet] Das Rückgängigmachen von Stiftstrichen (Strg+Z) verzögert sich mehr als das Rückgängigmachen von Mausstrichen
&#x200B;* [Tablet] Anfangs- und Enddruck werden beim Zeichnen einer Geraden nicht berücksichtigt
&#x200B;* [Tablet] Der erste Stempel wird bei einer geraden Linie zweimal gezeichnet
&#x200B;* [Tablet] Verbessern der Unterstützung für Huion-Tablet-Tastaturbefehle
&#x200B;* [Tablet] Verbesserte Unterstützung für Huion Stift-Buttons
&#x200B;* [Tablet] Abstand zwischen der Pinselvorschau und dem gezeichneten Stempel
&#x200B;* [Tablet] Verknüpfungen zum Ändern von Pinseln mit Stift führen in seltenen Fällen zu geringer Leistung
&#x200B;* [Tablet] Verzögerung beim Malen auf einer bestimmten Ebene
&#x200B;* Unscharfe Texturen können in seltenen Fällen beim Wechseln des Viewport auftreten
&#x200B;* [UI]&#x200B;[Substance] Bildeingaben werden nicht immer angezeigt
&#x200B;* Beim Bereinigen werden keine Vorgaben aus dem Regal entfernt, die in ein Projekt importiert wurden
&#x200B;* [Tool]&#x200B;[Dynamischer Strich] Leistungsproblem beim Anpassen der Stempelzyklusanzahl
&#x200B;* Aktualisierungsprobleme beim Malen im 3D/2D-Viewport in seltenen Fällen
&#x200B;* Wenn Sie einen sehr langen Pinselstrich zeichnen, kann dies zum Einfrieren führen
&#x200B;* [Tool] Leistungsproblem beim Malen mit bestimmten Dynamischen Pinselstrichen
&#x200B;* [UI] Kontextbezogene Symbolleiste zeigt weiterhin Pinseleigenschaften an, wenn ein Ordner ausgewählt wird
&#x200B;* Werte für die Achse der Symmetrie werden nicht zurückgesetzt
&#x200B;* Import von EXR Texturen mit Fließkommawerten sind komplett schwarz
&#x200B;* Alt+Klicken auf einen Kanal zum Isolieren funktioniert nicht für Filter und Generator
&#x200B;* [Exportieren] Spezifische Projekt-Absturz beim Exportieren
&#x200B;* [Substance] Falscher Standardwert im Dropdown, wenn der Parameter von Visible If ausgeblendet wird
&#x200B;* [Shader] Kanäle, die über Materialebenen definiert wurden, werden in der Benutzeroberfläche nicht gleich sortiert
&#x200B;* [Shelf] Voreinstellungsmetadaten werden nicht auf dem Datenträger gespeichert

**Bekannte Probleme:**

&#x200B;* [UV-Entpacken] Die Verarbeitung von hochpolaren Netzen kann lange dauern
&#x200B;* [UV-Entpackung] Eckpunkte mit genau denselben Koordinaten werden zusammengeführt
&#x200B;* [UV-Entpackung] Die UV-Generierung kann in seltenen Fällen an einigen Netzteilen fehlschlagen
&#x200B;* [UV-Entpackung] Uneinheitliches oder stark verzerrtes Textilverhältnis in einer einzigen UV-Insel in einigen Fällen
&#x200B;* [UV-Entpackung] Nicht einheitliches Textilverhältnis zwischen Textursätzen
&#x200B;* [UV-Entpackung] erzeugte UV-Insel kann sehr lang sein und passt in einigen Fällen nicht in den UV-Raum.
&#x200B;* [UV-Entpackung] Degenerierte Flächen oder nicht dreieckige Netzflächen mit kleinen oder überlappenden Kanten werden möglicherweise nicht UV-entpackt
&#x200B;* Das Metamat-Beispiel hat einige Probleme mit importierten Kameras

### 5.2.3 (2019.2.3)

*(Freigegeben: 23. Oktober 2019)*
Zusammenfassung: **Bugfix-Version**

**Hinzugefügt:**

&#x200B;* [Textursatzliste] Schaltfläche &quot;Hinzufügen&quot;, um den Fokusmodus schnell zu aktivieren/deaktivieren
&#x200B;* [Log] Windows 10-Versionsnummer in die Protokolldatei einfügen
&#x200B;* Aktualisieren Sie auf die neueste Version von Substance Engine
&#x200B;* [MacOS] Die Software wurde notariell beglaubigt, um die neuen MacOS Catalina-Verteilungsanforderungen zu befolgen

**Fest:**

&#x200B;* [Plugin] Plugin Source funktioniert nicht
&#x200B;* [MacOS]&#x200B;[Shader] Mac OS 10.14.5 und AMD: Materialschichtung funktioniert nicht wie vorgesehen

**Bekannte Probleme:**

&#x200B;* Alembic-Dateien mit Unterteilungen können nicht importiert werden
&#x200B;* Seltene Abstürze beim Importieren einiger Alembic-Dateien
&#x200B;* Benutzeroberfläche reagiert beim Baking führ mit DXR auf Pascal-GPUs vorübergehend nicht

### 5.2.2 (2019.2.2)

*(Freigegeben: 20. September 2019)*
Zusammenfassung: **Bugfix-Version**

**Fest:**

&#x200B;* Das Importieren von Ressourcen durch Skripterstellung kann zu einem Absturz führen
&#x200B;* [Plugin] Das Herunterladen des Materials von der Quelle kann zu einem Absturz führen

**Bekannte Probleme:**

&#x200B;* Alembic-Dateien mit Unterteilungen können nicht importiert werden
&#x200B;* Seltene Absturz beim Importieren einiger Alembic-Dateien
&#x200B;* Benutzeroberfläche reagiert beim Baking führ mit DXR auf Pascal-GPUs vorübergehend nicht

### 5.2.1 (2019.2.1)

*(Freigegeben: 17. September 2019)*
Zusammenfassung: **Bugfix-Version**

**Fest:**

&#x200B;* [Mac]&#x200B;[USD] Exportierte USDZ-Dateien aus MacOS können nicht geöffnet werden.
&#x200B;* [Textursatz] Es ist nicht möglich, einen Textursatz mit dem ALT-Modifizierer zu isolieren
&#x200B;* [Regal] Vorgaben, Intelligente Materialien und Intelligente Masken werden beim Beenden der Anwendung immer geändert
&#x200B;* [Ebenenstapel] Effekt kann nach dem Löschen eines anderen Effekts nicht ausgewählt werden
&#x200B;* Flackern bei Verwendung eines Schiebereglers im Bedienfeld &quot;Werkzeugeigenschaften&quot;
&#x200B;* Absturz beim Exportieren von Vorgaben in Regal
&#x200B;* Absturz beim Exportieren einer Vorgabe mit zu wenig Speicherplatz
&#x200B;* Absturz beim Erstellen einer Vorgabe mit zu wenig Speicherplatz

**Bekannte Probleme:**

&#x200B;* Alembic-Dateien mit Unterteilungen können nicht importiert werden
&#x200B;* Seltene Absturz beim Importieren einiger Alembic-Dateien
&#x200B;* Benutzeroberfläche reagiert beim Baking führ mit DXR auf Pascal-GPUs vorübergehend nicht

### 5.2.0 (2019.2.0)

*(Freigegeben: 25. Juli 2019)*
Zusammenfassung: **Hauptversion mit Leistungsaktualisierungen der Baker und einem neuen Vorvisualisierungsmodus + neuem Inhalt**

**Hinzugefügt:**

&#x200B;* [Baker] Zusätzliche Unterstützung für GPU-Raytracing mit DXR und OptiX (Ambient occlusion, Thickness)
&#x200B;* [Baker] Optimierungen und Beschleunigungen für CPU-Raytracing
&#x200B;* [Baker]&#x200B;[VIS-Modus]&#x200B;[UI] Neuer Visualisierungsmodus für Baking im Viewport
&#x200B;* [Baker]&#x200B;[Voreinstellungen]&#x200B;[Benutzeroberfläche] Neue Baking-Option zum Aktivieren/Deaktivieren von GPU-Raytracing
&#x200B;* [Baker]&#x200B;[UI] Überarbeitung des Fortschrittsbalken-Dialogfelds
&#x200B;* [Baker] Verbesserung von Warn- und Fehlermeldungen
&#x200B;* [Baker] Responsiveres Abbrechen des Bakings zulassen
&#x200B;* [Baker] Fenster &quot;Baking&quot; nach Klicken auf &quot;Abbrechen&quot; erneut öffnen
&#x200B;* [Proj]&#x200B;[UX] Verbesserte Verwendbarkeit des Rotations-Manipulators
&#x200B;* [Einstellungen] Option zur Leistungssteigerung durch Reduzierung der Viewport-Auflösung für HDPI-Bildschirme
&#x200B;* [Skripterstellung] Ändern der Auflösung von Textursätzen
&#x200B;* [Skripterstellung] Ausgewählten Textursatz abrufen
&#x200B;* [Scripting] Benutzer können einen Textursatz auswählen
&#x200B;* [Skripterstellung] Funktion, um zu erfahren, wann die Auswahl des Textursatzes geändert wurde
&#x200B;* [Regal] Es wurden 40 neue intelligente Materialien hinzugefügt.
&#x200B;* [Regal] 20 neue intelligente Masken hinzugefügt

**Fest:**

&#x200B;* [Ebenenstapel] Einfrieren der Benutzeroberfläche bei Mehrfachauswahl von Ebenen
&#x200B;* [Ebenenstapel] Beim Gruppieren vieler Ebenen wird die Benutzeroberfläche länger als gewöhnlich eingefroren.
&#x200B;* [Ebenenstapel] In einigen Fällen können eine Ebene und ein Effekt gleichzeitig ausgewählt werden
&#x200B;* In Malwerkzeugen verwendete Substance-Graf werden nicht mit der richtigen Auflösung generiert
&#x200B;* [Baker] Schaltfläche &quot;Alle Textursatz Baking geführt&quot; ist nicht deaktiviert, wenn keine Baker ausgewählt sind
&#x200B;* [MacOS] Deaktivieren der Warnmeldung zur Tessellation
&#x200B;* Bei Verwendung mit einer Projektion hat das Maskierungswerkzeug keine Vorschau.
&#x200B;* Absturz und beschädigte Projekte beim Speichern mit zu wenig Speicherplatz
&#x200B;* [Regal] Absturz beim Importieren einer Ressource auf dem Datenträger über ein Regal mit nicht genügend Speicherplatz
&#x200B;* [Regal] Absturz beim Wiederherstellen der Sitzungsvorgabe
&#x200B;* [Regal] Das Importieren einer Vorgabe mit einem Namen, der mit einem Leerzeichen endet, führt zu einem Absturz
&#x200B;* [Regal] Das Importieren einer Ressource mit einem Präfix, das mit einem leeren Leerzeichen endet, führt zu einem Absturz

**Bekannte Probleme:**

&#x200B;* Alembic-Dateien mit Unterteilungen können nicht importiert werden
&#x200B;* Seltene Absturz beim Importieren einiger Alembic-Dateien
&#x200B;* Benutzeroberfläche reagiert beim Baking führ mit DXR auf Pascal-GPUs vorübergehend nicht

### 5.1.3 (2019.1.3)

*(Freigegeben: Juli 2019)*
Zusammenfassung: **Bugfix mit 2 neuen Funktionen**

**Hinzugefügt:**

&#x200B;* Geben Sie das VRam-Budget über eine Befehlszeile (z. B. —vram-budget 4096)
&#x200B;* [QML] Leg von wrapMode- und elide-Eigenschaften von QML-Schaltflächen und -Kontrollkästchen

**Fest:**

&#x200B;* &quot;Pfad folgen&quot; funktioniert nicht immer
&#x200B;* Kanalzuordnung funktioniert nicht mit SBSAR, das in Ein Kanal-Steckplätzen verwendet wird
&#x200B;* [Ebenenstapel] Niedrige Leistung beim Scrollen mit ausgeblendeten Ebenen
&#x200B;* [TextureSet] Absturz beim Klicken zwischen Masken
&#x200B;* [SVT] Versatz wird nicht richtig angezeigt und flackert in einigen Fällen
&#x200B;* [Alembic] Absturz mit Mesh, der Punktnormalen anstelle von Scheitelpunkt-Normalen verwendet
&#x200B;* [Alembic]&#x200B;[Log] Melden Sie einen Fehler im Log, wenn die Alembic-Datei während des Imports nicht unterstützt wird

**Bekannte Probleme:**

&#x200B;* Alembic-Dateien mit Unterteilungen können nicht importiert werden
&#x200B;* Seltene Absturz beim Importieren einiger Alembic-Dateien

### 5.1.2 (2019.1.2)

*(Freigegeben: 21. Mai 2019)*
Zusammenfassung: **Hotfix**

**Fest:**

&#x200B;* Absturz beim Auswählen von zwei Ressourcen mit einer Bildeingabe

### 5.1.1 (2019.1.1)

*(Freigegeben: 20. Mai 2019)*
Zusammenfassung: **Hotfix**

**Hinzugefügt:**

&#x200B;* Aktualisieren Sie auf die neueste Version von Substance Engine mit der letzten Version von Substance Designer 2019.1

**Fest:**

&#x200B;* [Substance] Visible If wird bei Eingabebildern nicht berücksichtigt
&#x200B;* [SVT]&#x200B;[Engine] Das Ändern der Textursatz-Auflösung führt in einigen Fällen zu einem Absturz
&#x200B;* [Engine] In einigen Fällen werden zufällige schwarze Texturen angezeigt
&#x200B;* [Ebenenstapel]&#x200B;[UI] Wenn Sie mit UMSCHALTTASTE eine Maske umschalten, können Sie mehrere Ebenen gleichzeitig auswählen
&#x200B;* [Ebenenstapel] Deckkraft hat keine Auswirkungen auf den Malen-Effekt mit dem Mischmodus &quot;Hindurchwirken&quot;
&#x200B;* [Ebenenstapel] Filtereingabe &quot;Height zu Normal&quot; wird mit dem Pinselstrich des Radiergummis nicht ordnungsgemäß aktualisiert
&#x200B;* Absturz [LayersStack] beim Rückgängigmachen des Ablagevorgangs für eine intelligente Maske
&#x200B;* Flackerndes Drahtgitter mit aktiviertem temporalem Anti-Aliasing
&#x200B;* [Versatz] Verzögerung bei AMD mit einigen schweren Meshs
&#x200B;* [Windows] Absturz beim Öffnen einiger Projekte über den Datei-Explorer
&#x200B;* [Histogramm] Absturz beim Entfernen von Masken mit Ankerpunkt in einigen Fällen
&#x200B;* Absturz bei der Vorschauerstellung in einigen seltenen Fällen
&#x200B;* [Absturz] Ein Projekt kann mit zu vielen Klon- und Verwisch-Tools nicht erneut geöffnet werden
&#x200B;* Nach dem Speichern wird in einigen Fällen kein Mesh im Materialmodi angezeigt
&#x200B;* [Scripting] alg.mapexport.documentStructure() gibt falsche Werte für Ordner zurück

**Bekannte Probleme:**

&#x200B;* Durch Doppelklicken auf den Namen des Textursatzes wird dieser vor dem Umbenennungsmodus ausgewählt

### 5.1.0 (2019.1.0)

*(Freigegeben: 23. April 2019)*
Zusammenfassung: **Dynamischer Pinselstrich mit eigenem neuen Inhalt, Versatz und Tesselierung in Echtzeit und in Irak, Maskenvergleichseffekt, Radialsymmetrie, planar und Sphärische Projektion**

**Hinzugefügt:**

&#x200B;* [Werkzeug] Dynamischer Strich: Substance-Variation entlang eines Pinselstrichs
&#x200B;* [Dynamischer Strich] Stellen Sie einen neuen Stempelindexparameter mit Optionen bereit.
&#x200B;* [Dynamischer Strich] Parameter $time berücksichtigen
&#x200B;* [Dynamischer Strich] Generieren eines neuen $randomseed-Parameters pro Strich und pro Stempel
&#x200B;* [Dynamischer Strich] Starten eines dynamischen Strichindex aus einer zufälligen Zahl
&#x200B;* [Dynamischer Strich]&#x200B;[Ablage] Helfen Sie, eine dynamische Strichressource mit einem neuen Symbol zu finden.
&#x200B;* Versatz und Tesselierung im Echtzeit-Viewport
&#x200B;* Versatz und Tesselierung in Iran
&#x200B;* [Shader settings]&#x200B;[UI] Neue Registerkarte für die Steuerung von Versatz und Tesselierung
&#x200B;* [Ebenenstapel] Neuer Effekt &quot;Maske vergleichen&quot;: durch Vergleich zweier Kanäle eine Maske generieren
&#x200B;* [Ebenenstapel]&#x200B;[UI] Neuer Eintrag im Rechtsklick-Menü &quot;Height mit Maskenkombination hinzufügen&quot;, um einen CompareMask-Effekt einzufügen
&#x200B;* [Symmetrie] Neuer Symmetriemodus: Radialmalerei
&#x200B;* [Symmetrie-Einstellungen] Erweitern Sie beide Abschnitte &quot;Einstellungen&quot; und &quot;Anzeige&quot;.
&#x200B;* [Symmetrie-Einstellungen]&#x200B;[UI] Vorschau für radiales Malen
&#x200B;* Zeigen Sie zwei neue Projektionsmodi an: planar und sphärisch
&#x200B;* [Proj] Neuer Formzuschneidemodus für alle Projektionen
&#x200B;* [Proj] Planarer Modus mit neuem Manipulator: Oberflächenwerkzeug
&#x200B;* [Proj]&#x200B;[Shortcut] Shortcut UMSCHALTTASTE+W für Oberflächenwerkzeug
&#x200B;* [Proj] Planare Projektionsmaskierung mit Tiefe ausblenden- und Rückseitenschälung
&#x200B;* [Manipulator] Verbesserung des Manipulators der Drehung auf allen drei Achsen für triplanare
&#x200B;* [Tool]&#x200B;[UX] Alt-Klick auf einen Kanal fokussiert diesen Kanal (aktiviert ihn oder deaktiviert alle anderen)
&#x200B;* [Engine] Update auf die neueste Version von Substance Engine
&#x200B;* [Textursatz] Mehrfachauswahl und Auflösungsänderung
&#x200B;* [Textursatz] Schnelle Aktivierung und Deaktivierung der Textursatz
&#x200B;* [Textursatz] Kombination von Solo- und allen Optionen in einem neuen Menü
&#x200B;* [Textursatz]&#x200B;[Ebenenstapel] Neues Symbol für Aktivierung und Deaktivierung
&#x200B;* [Ebenenstapel]&#x200B;[UX] Einfügen von Effekten über den bereits ausgewählten
&#x200B;* [Ebenenstapel]&#x200B;[UI] Ebenenstapel-Ansichtenauswahlstil überarbeiten
&#x200B;* [Ebenenstapel] Der Mischmodus für instanzierte Ebenen ist jetzt standardmäßig im Durchlaufmodus
&#x200B;* [Exportieren] Option zum Aktivieren und Deaktivieren von Dithering
&#x200B;* [Plugin] Präzisionsmodifikator für Schieberegler unterstützen (SHIFT)
&#x200B;* [Plug-in]&#x200B;[UI] Neues Symbol für automatisches Speichern
&#x200B;* [Scripting] Auflisten des Inhalts eines Ordners
&#x200B;* [Scripting] Löschen von Dateien zulassen
&#x200B;* [Skripterstellung] Lesen aller Stapel-Informationen, einschließlich der verwendeten Ressourcen
&#x200B;* [Inhalt]&#x200B;[Dynamischer Strich] Neue Werkzeuge und Pinselvorgaben
&#x200B;* [Inhalt]&#x200B;[Dynamischer Strich] Zwei neue prozedurale Verläufe: Farbton und Verlaufsgenerator
&#x200B;* [Inhalt] 11 neue Filter: MatFx Peeling Malen, MatFx Wassertropfen und mehr
&#x200B;* [Inhalt] 7 neue Generatoren: &quot;Auto-Stitcher&quot;, &quot;UV-Zufallsfarbe&quot;, &quot;UV-Texeldichte&quot; und weitere Eigenschaften
&#x200B;* [Inhalt] 93 neue Alphas: neue Texte, Pfeile und verschiedene andere Formen
&#x200B;* [Inhalt] 2 neue Verfahren: Verlaufsfarbton, Verlaufsgenerator und mehr
&#x200B;* [Inhalt] 21 neue Tools und Pinselvorgaben für Dynamische Pinselstriche : Kiesel, Fußabdrücke, Spray und mehr
&#x200B;* [Inhalt] 2 Neue HDRs: Canopus Boden- und Herbstwald
&#x200B;* [Inhalt] Aktualisieren von Inhalt mit Kuration nach dem Zufallsprinzip in Regal
&#x200B;* [Inhalt] Neues Symbol mit gelegt Zufallsparameter in Regal

**Fest:**

&#x200B;* [Ebenen-Stapel] Ebenenstapel wird unendlich lange gezogen
&#x200B;* [Mac] &quot;Im Finder anzeigen&quot; kann zum Einfrieren führen
&#x200B;* [Scripting] Einstellungen, die über die benutzerdefinierte Benutzeroberfläche gespeichert wurden, gehen verloren, wenn die Shader-Datei verschoben wird
&#x200B;* [Scripting] API-Versionsnummer ist falsch und nicht aktuell
&#x200B;* [Effekt] Histogramminhalt wird nicht korrekt angezeigt
&#x200B;* [Effekt] Der Histogrammeffekt wird in einigen Fällen nicht aktualisiert
&#x200B;* [Regal] Die Stiche sind auf Material &quot;Plastic Fabric Pyramide&quot; nicht richtig ausgerichtet.

**Bekannte Probleme:**

&#x200B;* Durch Doppelklicken auf den Namen des Textursatzes wird dieser vor dem Umbenennungsmodus ausgewählt.
&#x200B;* [Ebenenstapel]&#x200B;[UI] Wenn Sie mit UMSCHALTTASTE eine Maske umschalten, können Sie mehrere Ebenen gleichzeitig auswählen

## Version 4

### 4.3.3 (2018.3.3)

*(Freigegeben: 7. März 2019)*
Zusammenfassung: **Bugfix**

**Hinzugefügt:**

&#x200B;* [Inhalt] Neue Projektvorlage integrieren: &quot;PBR - Metallische Rauheit Alpha-blend&quot;
&#x200B;* Die Suchreihenfolge der dynamischen Linux-Bibliothek wurde geändert, um Bibliotheken im Installationsverzeichnis Priorität einzuräumen, bevor sie auf dem System installiert werden.

**Fest:**

&#x200B;* Mesh verschwindet manchmal vom 3D-Viewport (drücken Sie F, um die Kamera zurückzusetzen)
&#x200B;* Aktualisieren des Substance Painter Sketchfab-Uploaders mit den neuen Sketchfab-Lizenztypen
&#x200B;* [Import]&#x200B;[glTF] Falsche Handhabung der Modulation der Eingabe-Textur, wie in glTF-Dateien definiert
&#x200B;* [Import]&#x200B;[glTF] Boden-Ebene wird beim glTF-Import in einigen Fällen falsch angezeigt
&#x200B;* [Exportieren]&#x200B;[USD] Deckkraft funktioniert nicht in Arkit
&#x200B;* [Exportieren]&#x200B;[USD] USDz-Export-Absturz in einigen Fällen
&#x200B;* [Exportieren]&#x200B;[USD] Exportieren nach USD ohne Speichern führt zu Absturz
&#x200B;* [Exportieren]&#x200B;[USD] Falsche Kachelung für Texturen, Unterteilungsmodus für Mesh und Ausgabetypen für Shader
&#x200B;* [Exportieren]&#x200B;[USD] Wenig Exporte von nur einigen Textursätzen mit allen Geometrien
&#x200B;* [Instanz] Absturz beim Löschen einer beschädigten Instanzebene
&#x200B;* [Regression]&#x200B;[Exportieren] Einige Maps werden nicht in die ausgewählte Bittiefe exportiert
&#x200B;* [Linux] Problem mit der Bibliothek libtbb.so.2

**Bekannte Probleme:**

&#x200B;* Einfrieren der Berechnung in einigen Fällen auf AMD VEGA-GPUs
&#x200B;* Problem mit Huion-Tablets mit Tastaturbefehlen unter Windows

### 4.3.2 (2018.3.2)

*(Freigegeben: 24. Januar 2019)*
Zusammenfassung: **Hotfix mit neuen Funktionen (USDZ-Export- und Textur-Filterungen im Viewport)**

**Hinzugefügt:**

&#x200B;* [Export] Export nach USDZ zulassen
&#x200B;* [Viewport] Zulassen, dass die Qualität der Textur in den Anzeigeeinstellungen gesteuert wird.
&#x200B;* [Viewport] Die MIP-Voreinstellung wurde in den Anzeigeeinstellungen hinzugefügt.
&#x200B;* [Viewport] Anisotrope Filterung in den Anzeigeeinstellungen hinzugefügt
&#x200B;* [Plug-ins] Offizielle Plug-ins aktualisieren, um den Stil von Substance Painter 2018 zu verwenden
&#x200B;* [Lizenz] Installation der Lizenz standardmäßig in einem Benutzerordner

**Fest:**

&#x200B;* Mit Dekomprimierung verknüpfter Absturz
&#x200B;* Hinzufügen von TAA auf Solo-Material
&#x200B;* Rauschen mit Shadow, TAA und Alpha-Test-Shader mit Dithering
&#x200B;* Specular-Dithering für alle klassischen PBR-Shader entfernen
&#x200B;* Absturz in den Shader-Einstellungen in einigen Fällen
&#x200B;* Die Streuungsaktivierung wird nicht zwischen OpenGL- und Iray-Renderings synchronisiert
&#x200B;* Die Verwisch- und Kopierwerkzeuge funktionieren nicht mehr bei bestimmten Netzen
&#x200B;* Einige Texturensätze können nicht im Iran-Rendering angezeigt werden
&#x200B;* Umbenannte Textursätze werden nach dem Schließen des Projekts nicht gespeichert
&#x200B;* Drahtgitter-Artefakte beim Ziehen und Ablegen von Materialien auf ID-Maps
&#x200B;* [Scripting] Dateipfaderstellung beim Speichern eines Projekts nicht erzwungen
&#x200B;* [Scripting] Rückruf von &quot;onProjectAboutToSave()&quot; funktioniert nicht mehr
&#x200B;* Fehlerhafte Links im Fenster &quot;Fehler melden&quot;

**Bekannte Probleme:**

&#x200B;* Berechnungen frieren in einigen Fällen auf AMD VEGA-GPUs ein
&#x200B;* Problem mit Huion-Tablets mit Tastaturbefehlen unter Windows

### 4.3.1 (2018.3.1)

*(Freigegeben: 6. Dezember 2018)*
Zusammenfassung: **Hotfix**

**Hinzugefügt:**

&#x200B;* [Symmetrie]&#x200B;[Viewport] Symmetrie-Malerei in der 2D-Ansicht ist wieder da und zeigt jetzt eine fixierte Vorschau des Klonpinsels

**Fest:**

&#x200B;* [Exportieren] Beim Export in die 2D-Ansicht wird in einigen Fällen eine schwarze Textur ausgegeben
&#x200B;* [Iray] Normale Informationen werden in Iray falsch, nachdem eine Materialschicht instanziiert wurde
&#x200B;* Nicht quadratische Texturensätze können in einigen Fällen zum Absturz führen
&#x200B;* [Rückgängig] Mehrere Strg+Z können in einigen Fällen zufällig zum Absturz führen
&#x200B;* [QML] AlgScrollView kann in einigen Fällen eine Warnung im Protokoll erstellen (Bindungsschleifen)

**Bekannte Probleme:**

&#x200B;* Berechnungen frieren in einigen Fällen auf AMD VEGA-GPUs ein
&#x200B;* Problem mit Huion-Tablets mit Tastaturbefehlen unter Windows
&#x200B;* Glätten und Schatten können bei gemeinsamer Verwendung zu unerwarteten Ergebnissen führen

### 4.3.0 (2018.3.0)

*(Freigegeben: November 2018)*
Zusammenfassung: <b>Viewport-Upgrades, ordnungsgemäßer Datenexport, neue UI-Helfer, ein erweitertes Symmetrie-Tool, neue 2D-Ansichten und eine enorme Leistungssteigerung</b>

<b>Hinzugefügt:</b>

&#x200B;* [Glätten]&#x200B;[Viewport] Neue temporale Anti-Aliasing-Filterungen für 3D-Viewport (über Anzeigeeinstellungen)
&#x200B;* [Exportieren] Exportieren Sie den Inhalt des 2D-Viewports als eine einzige Textur
&#x200B;* [Exportieren]&#x200B;[Dithering] Dithering beim Exportieren Gelegt
&#x200B;* [Ebenenstapel] Farben auf Ebenen und Ordnern
&#x200B;* [Ebenenstapel] Schnelle Aktivierung und Deaktivierung mehrerer Ebenen und Effekte
&#x200B;* [Ebenenstapel] Einfachere Navigation für Füllmethoden mit Nach-oben-Tasten und Mausbildlauf
&#x200B;* [Proj]&#x200B;[UI] Zusätzlicher Dreh-Manipulator auf allen drei Achsen für triplanar
&#x200B;* [Proj]&#x200B;[Tastaturbefehle] - und +, um die Größe des Manipulators der UV-Projektion zu ändern
&#x200B;* [Shader] Kontrolle beschichteter Schichtparameter mit Kanälen im PBR-beschichteten Shader
&#x200B;* [Substance] Leg neuer Mesh-basierter Textur-Eingänge für Filter und Generatoren
&#x200B;* [Symmetrie]&#x200B;[Viewport]&#x200B;[UI] Steuern des Offsets der Symmetrie auf Manipulator
&#x200B;* [Symmetrie]&#x200B;[Kontextabhängige Symbolleiste]&#x200B;[Benutzeroberfläche] Neues Bedienfeld &quot;Symmetrie&quot; mit Optionen
&#x200B;* [Symmetrie] Neue Symmetrie Linienüberschneidungsmodus
&#x200B;* [Symmetrie] Neuer Symmetrie-Clone-Cursor
&#x200B;* [Symmetrie]&#x200B;[Tastaturbefehle] Q zum Ausblenden und -, + zum Ändern der Größe und Umschalttaste zum einrasten
&#x200B;* [Log] Verbessern von Fehlermeldungen, wenn Texturen nicht exportiert werden können
&#x200B;* [Scripting] Ressourcen in den Anzeigeeinstellungen ändern oder aktualisieren
&#x200B;* [Scripting] Erlaubt das Erstellen oder Entfernen von Kanälen in Textursätzen
&#x200B;* [Content]&#x200B;[Shaders] Unterstützung für Anisotropie mit einem dedizierten Shader hinzufügen (pbr-metal-rau-Anisotropie-angle)
&#x200B;* [Inhalt] Aktualisierung der Vorschaukugel mit Anisotropie und verändertem Winkel
&#x200B;* [Content] Aktualisierte matFx-Shutline
&#x200B;* [Content] Neuer Scanner zur Texturierung.XYZ-Fläche
&#x200B;* [Inhalt] Neue anisotrope Verfahren
&#x200B;* [Inhalt] Neuer Filter: Umgebung mit vorberechnete Beleuchtung
&#x200B;* [Inhalt] Neue Umgebungszuordnung: Studio Automotive Neutral
&#x200B;* [Inhalt] Neue Projektvorlage: PBR - Anisotropie der metallischen Raueit (mit Kanälen für die Anisotropie)
&#x200B;* [Inhalt] Neue Projektvorlage: PBR - mit metallische Rauheit beschichtet
&#x200B;* [SVT]&#x200B;[Engine] Spare virtuelle Texturen (SVT)
&#x200B;* [SVT]&#x200B;[Voreinstellungen]&#x200B;[UI] Beschleunigungsoption für SVT-Hardware-Unterstützung
&#x200B;* [SVT]&#x200B;[Protokoll] Zusätzliche Informationen für die Funktion &quot;Virtuelle Texturierung mit geringer Dichte&quot; (z. B. Festplatte in Größe)
&#x200B;* [SVT]&#x200B;[UI] Meldungsfenster beim Start, wenn die Größe auf der Festplatte für den Cache zu niedrig ist
&#x200B;* [SVT]&#x200B;[Voreinstellungen]&#x200B;[UI] Substance Painter globaler Cachespeicherort
&#x200B;* [SVT] Neue Umgebungsvariable zur Angabe des Pfads des Substance Painter-Cache
&#x200B;* [SVT] Neue Umgebungsvariable zum Aktivieren der SVT-Hardware-Support-Beschleunigung
&#x200B;* [SVT] Erkennen von geringer Unterstützung durch Hardware
&#x200B;* [SVT]&#x200B;[Hardware Sparse] Erhöhen der Mindesttreiberversion für Nvidia-GPU
&#x200B;* [SVT]&#x200B;[Shader]&#x200B;[Viewport]&#x200B;[UI] Warnen Sie den Benutzer, wenn beim Öffnen des Projekts Artefakte mit virtueller Texturierung mit geringer Dichte vorhanden sind

<b>Fest:</b>

&#x200B;* [Farbwähler] Beim Auswählen einer Farbe wird ein Malcursor angezeigt
&#x200B;* Absturz durch Auswählen oder Aufheben der Auswahl von Ebenen in einer bestimmten Reihenfolge kann zum Absturz führen
&#x200B;* Absturz beim Einfügen einer Ebene mit einer Maske als Instanz
&#x200B;* [Benutzerkanal]&#x200B;[Regression] Absturz beim Umbenennen des Benutzerkanals
&#x200B;* [Benutzerkanal] Graue Pinselvorschau
&#x200B;* [Alembic] Nur ein Textursatz aus mehreren Materialien nach dem Import
&#x200B;* [Engine] Exportierte Textur unterscheidet sich vom Viewport für Pinselstempel
&#x200B;* [Engine] Die Umkehrung mit einem Ebeneneffekt wirkt sich nicht vollständig auf eine Textur aus
&#x200B;* Die Materialauswahl wendet beim Auswählen einen Pinselstrich an
&#x200B;* Das Umschalten der Auflösung auf 128 x 128 px führt zu einem Absturz
&#x200B;* Gitterzuordnungs-Verknüpfungen werden beim Umbrechen oder Instanziieren von Ebenen nicht ordnungsgemäß aktualisiert
&#x200B;* [Substance] UserData ColorSpace funktioniert nicht bei der als Eingabe angeforderten Option &quot;Standard für gepuffertes Gitter&quot;
&#x200B;* MDL-Zuordnungskonflikt bei Verwendung mehrerer Shader-Instanzen
&#x200B;* [Symmetrie]&#x200B;[Füllebene] Symmetrieebene und ihr Manipulator in der Füllebene aktiv
&#x200B;* [Viewport] Drehpunkt für Übersetzung wird nach dem Klicken nicht immer aktualisiert
&#x200B;* [UI] Symbole und Entfernen von Platzhaltern für HDPI-Monitore wurden korrigiert

<b>Bekannte Probleme:</b>

&#x200B;* Berechnungen frieren in einigen Fällen auf AMD VEGA-GPUs ein
&#x200B;* Problem mit Huion-Tablets mit Tastaturbefehlen unter Windows
&#x200B;* Glätten und Schatten können bei gemeinsamer Verwendung zu unerwarteten Ergebnissen führen

### 4.2.3 (2018.2.3)

*(Freigegeben: 25. September 2018)*

**Fest:**

&#x200B;* [2D-Ansicht] Die 2D-Ansicht wird bei der Erstellung eines neuen Projekts mit einigen Gittern unterbrochen.
&#x200B;* [Absturz] Das Umschalten von der UV-Projektion- auf die dreiplanare Projektion führt zu einem Absturz
&#x200B;* [RayCollider] Mehrere Abstürze durch &quot;RayCollider&quot;
&#x200B;* [Werkzeug] Beim Wechseln von Ebenen gehen die geänderten Pinseleigenschaften verloren
&#x200B;* Pinseleinstellungen werden beim Wechsel zum Radierer zurückgesetzt

**Bekannte Probleme:**

&#x200B;* Einfrieren der Berechnung auf AMD VEGA-GPUs
&#x200B;* Problem mit Huion-Tablets mit Tastaturbefehlen unter Windows

### 4.2.2 (2018.2.2)

*(Freigegeben: 11. September 2018)*
Zusammenfassung: **Hotfix mit Inhaltsaktualisierung, neuen Skriptfunktionen und der Möglichkeit, das automatische Update zu deaktivieren**

**Hinzugefügt:**

&#x200B;* [Inhalt]&#x200B;[Regal] Hinzufügen einer Skin-Regalvorgabe
&#x200B;* [Inhalt]&#x200B;[Regal] Konvertierung von 19 Hautnormalen in Materialien zur Untergrundstreuung
&#x200B;* [Scripting] Erstellen einer Projektvorlage aus einem geöffneten Projekt
&#x200B;* [Scripting] Abrufen/Festlegen von Exporteinstellungen eines geöffneten Projekts
&#x200B;* [Updates] Deaktivieren des Popups &quot;Automatische Aktualisierung&quot; in den Einstellungen und der Umgebungsvariablen
&#x200B;* [Updates] Anzeige erst in der nächsten Version des veralteten Wartungs-Popup

**Fest:**

&#x200B;* [Kamera] Falscher Zoom durch Wechsel von orthografischer zur Perspektive
&#x200B;* [Anzeige] Einige Maps werden linear anstelle von sRGB angezeigt
&#x200B;* [Viewports] Der Gitterfokus verhält sich nicht ordnungsgemäß.
&#x200B;* [2D-Ansicht] Projekt mit kaputter Kamera enthält verschwindende UVs-Schalen
&#x200B;* [SSS]&#x200B;[QuickInfo] QuickInfos für die unterirdische Streuung werden im Protokoll angezeigt
&#x200B;* Einige Projekte können nicht in 2018.2 geöffnet werden und die Fehlermeldung kann kein Null-Substance-Paket speichern
&#x200B;* [Maske] Die Farbe des Malwerkzeugs kann in einigen Fällen beim Arbeiten in einer Maske hängen bleiben
&#x200B;* [Material] Karten werden in bestimmten Situationen nicht angezeigt
&#x200B;* [Proj]&#x200B;[Tools] Manipulator aktiv mit einem Generator
&#x200B;* [Substance] Fehlende Substance-Parametergruppen
&#x200B;* [Skripterstellung] Falscher Software-Name in der Dokumentation
&#x200B;* [UDIMs] Keine Informationen im Protokoll über UVs-Schalen auf mehreren UVs-Kacheln

**Bekannte Probleme:**

&#x200B;* Einfrieren der Berechnung auf AMD VEGA-GPUs
&#x200B;* Problem mit Huion-Tablets mit Tastaturbefehlen unter Windows

### 4.2.1 (2018.2.1)

*(Freigegeben: 03. August 2018)*

**Fest:**

&#x200B;* Fehlende Parameter für die Teilflächen-Streuungs-Shader beim Aktualisieren von Projekten

**Bekannte Probleme:**

&#x200B;* Einfrieren der Berechnung auf AMD VEGA-GPUs
&#x200B;* Problem mit Huion-Tablets mit Tastaturbefehlen unter Windows

### 4.2.0 (2018.2.0)

*(Freigegeben: 2. August 2018)*
Zusammenfassung: **Sommerversion, Volumenstreuung-Support, Verbesserungen bei Projektion und Füllung, Kamera-Import und -Auswahl, Alembic- und glTF-Unterstützung, Drag-and-Drop auf ID-Map, verbesserte Unterstützung für Substance-Formate und neue Inhalte**

**Hinzugefügt:**

&#x200B;* [SSS]&#x200B;[Viewport]&#x200B;[Iray] Generische Volumenstreuung
&#x200B;* [SSS] Synchronisierungs-MDL- und Volumenstreuung-Parameter
&#x200B;* [SSS] Es wurde ein neuer Graustufenkanal mit dem Namen &quot;Streuung&quot; hinzugefügt.
&#x200B;* [SSS]&#x200B;[Shader-Einstellungen] Streutypparameter für die Volumenstreuung (Skin oder transluzent)
&#x200B;* [SSS]&#x200B;[Shader-Einstellungen] Streuungsparameter für die Volumenstreuung
&#x200B;* [SSS]&#x200B;[Shader Settings] Farbstreuung-Parameter für Volumenstreuung
&#x200B;* [SSS]&#x200B;[Anzeigeeinstellungen] Streuung Beispielanzahl für Volumenstreuung
&#x200B;* [Shader]&#x200B;[Iray] Integrieren von Volumenstreuung-MDL für Iray
&#x200B;* [Shader] Shader-Update über den Ressourcen-Updater
&#x200B;* [Shader] API und Dokumentation für Änderungsprotokoll aktualisieren
&#x200B;* [Werkzeugeigenschaften]&#x200B;[Proj] Neue Parameter für die triplanare Projektion
&#x200B;* [Viewport]&#x200B;[Proj] Steuern Sie die Eigenschaften der Füllebene in der 3D-Ansicht direkt mit Manipulatoren (triplanare Projektion)
&#x200B;* [Shortcuts]&#x200B;[Proj] Neue Shortcuts Q, W, E, R, T für triplanare Projektion Manipulator
&#x200B;* [Viewport]&#x200B;[Proj] Steuern Sie Eigenschaften der Füllebene in 2D-Ansichten direkt mit Manipulatoren (UV-Projektion)
&#x200B;* [Shortcuts]&#x200B;[Proj] Neuer Tastaturbefehl Q für UV-Projektion Manipulator
&#x200B;* [Kontextsymbolleiste]&#x200B;[Proj] triplanare Projektion-Manipulator steuern
&#x200B;* [Kontextsymbolleiste]&#x200B;[Proj] UV-Projektion-Manipulator steuern
&#x200B;* [Werkzeugeigenschaften] Deaktivieren der Kachelung der Textur mit dem Werkzeug Projektion und Schablone
&#x200B;* [Schablone] Verwenden von Nicht-quadratischen Bildern mit dem Projektion-Werkzeug/der Schablone
&#x200B;* [Schablone] Steuerung des Kachelung-Modus im Eigenschaftenfenster zulassen
&#x200B;* [Schablone] Der Zoom ist nicht auf einer Schablone ohne Kachelung zentriert
&#x200B;* [Kameras] Importieren von Kameras aus Maya, Max, Blender, Modo, DAE
&#x200B;* [Kameras]&#x200B;[Viewport] Wählen und steuern Sie die importierten Kameras im Viewport
&#x200B;* [Kameras]&#x200B;[Iray] Auswählen und Steuern von importierten Kameras in Iray
&#x200B;* [Kameras]&#x200B;[UI]&#x200B;[Neues Projekt]&#x200B;[Projektkonfiguration] &quot;Kameras importieren&quot; ist standardmäßig aktiviert.
&#x200B;* [Kameras]&#x200B;[Tastaturbefehle] Hinzufügen von Tastaturbefehlen, um zwischen Kameras zu wechseln
&#x200B;* [Kameras]&#x200B;[Viewport] Frame im Viewport hinzufügen
&#x200B;* [Kameras]&#x200B;[Viewport-Einstellungen] Steuerung der Frame-Deckkraft
&#x200B;* [Kameras]&#x200B;[Kameraeinstellungen] Maximale Brennweite bei 500 mm
&#x200B;* [Kameras]&#x200B;[Kameraeinstellungen] Belichtungsverhältnis
&#x200B;* [Kameras]&#x200B;[Kameraeinstellungen] Fügen Sie eine Sperroption hinzu
&#x200B;* [Kameras]&#x200B;[Kameraeinstellungen] Hinzufügen einer Wiederherstellungsoption
&#x200B;* [Kameras]&#x200B;[Kameraeinstellungen] Attribut für den Fokusabstand hinzufügen
&#x200B;* [glTF] Import einer glTF-Datei
&#x200B;* [glTF] Umgebungskarte für die Verdeckung importieren
&#x200B;* [Alembic] Importieren Sie Alembic 1-Rahmen mit statischer Geometrie
&#x200B;* [Shelf] Ziehen Sie Materialien per Drag &amp; Drop direkt auf das Gitter, indem Sie ID-Zuordnungen mit einem Modifizierer (STRG/Befehlstaste) verwenden.
&#x200B;* [Ebenenstapel] Automatische Erstellung von ID-Masken durch Ziehen und Ablegen von Materialien auf einem Gitter mit ID-Maps
&#x200B;* [Ebenenstapel] Automatischer Bildlauf von Ebenen per Drag &amp; Drop über den Ebenenstapel
&#x200B;* [UI]&#x200B;[Werkzeugeigenschaften] Zeigt die Vorgabe des Substance an.
&#x200B;* [UI]&#x200B;[Hilfemenü] Verbesserung des Hilfemenüs
&#x200B;* [UI]&#x200B;[Neues Projekt]&#x200B;[Projektkonfiguration] Reorganisation des Fensters
&#x200B;* [UI]&#x200B;[Neues Projekt]&#x200B;[Projektkonfiguration] Ersetzen des Gitterbegriffs durch Datei
&#x200B;* [UI]&#x200B;[Substance] Anzeigen von Substance-Attributen in der Benutzeroberfläche
&#x200B;* [Tastaturbefehle] F4 wechselt zwischen 2D- und 3D-Ansicht
&#x200B;* [Tastaturbefehle] Neue Tastaturbefehle für Umschaltschablone N und Schnellmaske U
&#x200B;* [Substance-Integration] Berücksichtigung von &quot;visible if&quot;-Anweisungen in den Substance-Parametern
&#x200B;* [Viewport] Schatten müssen nach dem Verschieben der Kamera nicht berechnet werden.
&#x200B;* [Inhalt] Aktualisieren von MeetMat mit importierten Kameras
&#x200B;* [Inhalt] Muster mit aktivierter Volumenstreuung hinzufügen - JadeToad
&#x200B;* [Inhalt] Neue PBR-Projektvorlage mit aktivierter Untergrundstreuung hinzufügen
&#x200B;* [Inhalt] Exportvorgaben wurden aktualisiert, um einen neuen Streuungskanal hinzuzufügen
&#x200B;* [Content]&#x200B;[Shelf] Zusätzliche Untergrund-Streuunterstützung für: pbr-metal-rau, pbr-metal-rau-alpha-test, pbr-coated, pbr-spec-gloss
&#x200B;* [Content]&#x200B;[Shelf] Hinzugefügter Streuungskanal zu 5 intelligenten Materialien (Marmor und Skins)
&#x200B;* [Inhalt]&#x200B;[Regal] 1 neues Jadematerial
&#x200B;* [Inhalt]&#x200B;[Regal] 1 neues Wachsmaterial

**Fest:**

&#x200B;* [CMD] Verschiedene Ergebnisse über dieselbe Befehlszeile mit unterschiedlichen Versionen
&#x200B;* [TDR] Wenn TdrLevel eingerichtet ist, sind keine Fehler im Protokoll vorhanden.
&#x200B;* [Baker] Umgebungskarte der Verdeckung wird gespiegelt
&#x200B;* [ID Map] Absturz beim Kommissionieren außerhalb des Bereichs 0-1
&#x200B;* [Iray] Absturz beim Wechseln der Textursätze und Zurückkehren zum Malmodus
&#x200B;* [Viewport] Synchronisieren von Ablagebereichen zwischen Viewports für Drag &amp; Drop
&#x200B;* [Engine] Moire-Artefakt beim Kacheln von Füllebenen oder Malen eines kleinen Pinsels
&#x200B;* [Lizenz] Prüfung auf fehlerhafte Softwareversion des Lizenzdiensts
&#x200B;* [Lizenz] Überarbeiten Sie die Art und Weise, wie wir die Authentifizierung verarbeiten
&#x200B;* [API] Rufen Sie das onNewProjectCreated-Skript-API-Ereignis auf, selbst wenn Sie mit einer Vorlage erstellen.
&#x200B;* [Shader] Kompilierter Shader wird nicht aus dem Cache geladen, wenn die Shader-Datei nicht kompiliert wird
&#x200B;* [Shelf] Beim Exportieren der HDR-Datei aus dem Shelf wird eine Datei mit eingespannten Werten ausgegeben
&#x200B;* [Exportieren] EXR-Exportklammern RGB Farbwerte zwischen 0-1
&#x200B;* [Inhalt] Prozedurales Rauschen 3D Perlin-Rauschen Fraktal ist verpixelt

**Bekannte Probleme:**

&#x200B;* Einfrieren der Berechnung auf AMD VEGA-GPUs
&#x200B;* Problem mit Huion-Tablets mit Tastaturbefehlen unter Windows

### 4.1.3 (2018.1.3)

*(Freigegeben: 28. Juni 2018)*

**Hinzugefügt:**

&#x200B;* [Voreinstellungen] Vorschlag zum Speichern des Projekts beim Neustart von Painter

**Fest:**

&#x200B;* [Plug-In] Substance Source &quot;Suchen&quot; funktioniert nicht
&#x200B;* [Intelligenten Materials] Das Importieren von Intelligenten Materials führt in einigen Fällen zu einem Absturz
&#x200B;* [Intelligenten Materials] Das Löschen von Intelligenten Materials führt in einigen Fällen zu einem Absturz
&#x200B;* [Speichern] Das Speichern führt in einigen seltenen Fällen zu einem Absturz
&#x200B;* [Regal] Umkehren funktioniert nicht auf den Zellen 2 und 3 der Zellen
&#x200B;* [Regal] Typo in einigen Alphas
&#x200B;* [Regal] Einige Substance-Material werden nicht richtig gerendert

**Bekannte Probleme:**

&#x200B;* Einfrieren der Berechnung auf AMD VEGA-GPUs

### 4.1.2 (2018.1.2)

*(Freigegeben: Juni 2018)*
Zusammenfassung: **Verbesserte Wiedergabegeschwindigkeit, verbessertes Speichersystem, aktualisierte Schieberegler, aktualisierte Plug-in-API, chinesische Baking, verbesserter Abstand jetzt optional**

**Hinzugefügt:**

&#x200B;* [Baker] Leistungsverbesserung mit neuer Baker-Version
&#x200B;* Erzwungene Anzeige von Dialogfeldern mit inkompatibler GPU
&#x200B;* [Speichern] Leg neuer Kompaktprojekt-Funktionen (vollständiger/kompakter Speichermodus)
&#x200B;* [Speichern] Benutzer informieren, wenn Fehler beim Speichern auftritt
&#x200B;* [Clean] Nächste Speicherung im Voll-/Kompaktmodus
&#x200B;* [Schieberegler] Verbesserung der Präzision der Farb-/Graustufenbalken und Schieberegler
&#x200B;* [Schieberegler] Hinzufügen der Pfeilsteuerungen nach oben/unten
&#x200B;* [Schieberegler] Dieselbe Erkennungszone für Farb- und Graustufenbalkenschieberegler
&#x200B;* [Plugin] Automatische Speicherung immer im inkrementellen Modus
&#x200B;* [Plug-In] Option zum Wechseln von Plug-Ins zu einem neuen Schnittstellenstil
&#x200B;* [Sprache] Chinesische Übersetzung hinzufügen
&#x200B;* [Auffüllung] Option zum Wechseln zwischen UV- und 3D-Raum-Nachbarauffüllung pro Textursatz in den Textursatzeinstellungen
&#x200B;* [Skript] Speichermodus verfügbar machen: Voll/Kompakt oder inkrementell
&#x200B;* [Script] Update Scripting/QML documentation
&#x200B;* [Log] Anzeige des Speichermodus im Protokoll (vollständig/kompakt oder inkrementell)

**Fest:**

&#x200B;* [Werkzeug] Kanalschlitz wird bei Einkanalfüllungen in einen Materialschlitz umgewandelt
&#x200B;* Absturz beim Laden eines Gitters (FBX), bei dem einige Flächen nicht von einem Material zugewiesen wurden
&#x200B;* Absturz in Irak mit NVIDIA GRID 5.2 auf virtuellem Computer
&#x200B;* Absturz beim Rückgängigmachen des Löschens einer Materialvoreinstellung
&#x200B;* Absturz beim Laden einiger Projekte
&#x200B;* [Befehlszeile] Neue Befehlszeile für UDIMs-Gitter, aufgeteilt nach UDIM
&#x200B;* [Symbolleiste] Verkleinern der Symbolleiste
&#x200B;* [Instanz] Bitmaps können nicht über mehrere Textursätze hinweg instanziiert werden
&#x200B;* [Viewport] Die Aktualisierung ist nicht abgeschlossen, wenn mit gekachelten UVs auf ein Gitter gemalt wird
&#x200B;* [Iray] Normalmap wird zweimal für Dielektrika angewendet
&#x200B;* [Shelf] Tippfehler in einigen Substance-Parametern (Alphas, Prozedurals und Matfx)
&#x200B;* [Shelf] Typo für die Bitmap &quot;Nur autorisiertes Personal&quot;
&#x200B;* [Script] Funktion alg.shaders.materials() funktioniert nicht mehr

**Bekannte Probleme:**

&#x200B;* Einfrieren der Berechnung auf AMD VEGA-GPUs

### 4.1.1 (2018.1.1)

*(Freigegeben: 03. April 2018)*

**Fest:**

&#x200B;* [Tablet] Problem beim Ändern der Standardinteraktionsoptionen
&#x200B;* [Baker] Absturz mit Assimp-Bibliothek
&#x200B;* [Baker] Leistungsrückgang mit A.O.-Map
&#x200B;* [Iray] Die Verzerrung des Objektivs wird nicht auf den Alphakanal angewendet
&#x200B;* [Treiber] Aktualisierung der Mindestanforderungen für Treiber
&#x200B;* [3Dview] Normale werden auf UDIM-Meshs ohne Normale-Informationen nicht korrekt generiert
&#x200B;* [Intel] Absturz mit Substance Painter 2018.1.0
&#x200B;* [Intel]&#x200B;[Viewport] Problem mit der Auffüllung (schwarze Artefakte)

**Bekannte Probleme:**

&#x200B;* Einfrieren der Berechnung auf AMD VEGA-GPUs

### 4.1.0 (2018.1.0)

*(Freigegeben: 15. März 2018)*

**Hinzugefügt:**

&#x200B;* Neuer allgemeiner Stil (Symbole, Farbe, Verhalten)
&#x200B;* Neues Standardlayout
&#x200B;* [Tablet] Benutzererfahrung beim Malen verbessert
&#x200B;* [Hauptmenü] Sortieren Sie native Elemente zuerst in Ansichten und Symbolleisten
&#x200B;* [Hauptmenü] Aktionen &quot;schnelle Maske verschieben&quot; im Abschnitt &quot;Viewport&quot;
&#x200B;* [Hauptmenü] Verschieben von Rechtsklickaktionen in den Abschnitt &quot;Viewport&quot;
&#x200B;* [Hauptmenü] Menü &quot;Ansicht&quot; in &quot;Fenster&quot; umbenennen
&#x200B;* [Schnellmenü] Neue Werkzeugeigenschaften durch Rechtsklick im Viewport
&#x200B;* [Dock-Widget] Neue Dock-Symbolleiste zum schnellen Reduzieren/Zurückrufen
&#x200B;* [Anzeigeeinstellungen] Fenster &quot;Kamera- und Anzeigeeinstellungen&quot; wurde zusammengeführt
&#x200B;* [Ebenenstapel] Kontextmenü (rechte Maustaste)
&#x200B;* [Ebenenstapel] Ziehen und Ablegen, um beliebige Effekte innerhalb derselben Ebene zu verschieben
&#x200B;* [Symbolleiste] Neuorganisation der Symbolleiste und neue kontextbezogene Symbolleiste
&#x200B;* [Werkzeugleiste] Klonwerkzeug in zwei separate Werkzeuge teilen
&#x200B;* [Werkzeugeigenschaften] Hellerer Graustufenwert im Hintergrund in der Vorschau
&#x200B;* [Eigenschaften von Tools] Organisation in Registerkarten (Füllung und Werkzeuge)
&#x200B;* [Tool] Malergebnis entspricht der Schablone
&#x200B;* [Viewport] Neuer Cursor für Füllebene
&#x200B;* [Viewport] Einfachere Navigation und besseres Malen (höhere Framerate)
&#x200B;* [Viewport] Kombinationsfeld für Material-/Kanal-/Kartenauswahl im Viewport
&#x200B;* [Viewport] Flackern beim Drehen reduzieren (Schatten aktiviert)
&#x200B;* [Shelf] Zeigt Materialien standardmäßig beim Öffnen von Painter an
&#x200B;* [Shelf] Ladezeitverbesserung von Substance-Texturen und -Materialien (2- bis 6-mal schneller)
&#x200B;* [Shelf] Neuorganisieren von Materialordnern, um die Struktur der Substance Source anzupassen
&#x200B;* [Shelf] Ziehen Sie Materialien per Drag &amp; Drop direkt auf das Gitter im Viewport
&#x200B;* [Shelf] Neue 3D-Geräusche (Perlin, Perlin Fraktal, Simplex und Worley)
&#x200B;* [Shelf] Neuer 3D Linear gradient-Maskengenerator unter Verwendung der Gitterposition
&#x200B;* [Shelf] Basisgeräusche zur Unterstützung der quadratische Ausbreitung aktualisiert
&#x200B;* [Shelf] Neue Vorlage und Exportvorgabe für Lens Studio (Snap-Anwendung) hinzugefügt
&#x200B;* [Shelf] Smart-Materialien und Smart-Masken wurden aktualisiert, um die neueste Version des Masken-Editors zu verwenden (Mikrodetails)
&#x200B;* [Shelf] Neues Beispielprojekt &quot;TilingMaterial&quot; zur Erstellung nahtloser Kachelmaterialien
&#x200B;* [Shelf] Neue Pinselvorgaben (Kalligrafie, Nass, Schraffur usw.)
&#x200B;* [Schieberegler] Neue Schieberegler und Stil und Verhalten von Graustufen-/Farbbalken
&#x200B;* [Bäcker] Verwenden des vollständigen Begrenzungsrahmens der Szene, um die Positionskarte zu berechnen
&#x200B;* [Shader] Entfernen des Height Force-Parameters aus den Standard-Shader-Parametern
&#x200B;* [Engine] Substance-Engine aktualisiert
&#x200B;* [Engine] Keine oder weniger Diskontinuitäten zwischen UV-Blöcken
&#x200B;* [Plug-ins] Importieren Sie schneller aus Substance Source heruntergeladene Materials
&#x200B;* [Plug-ins] Alle Plug-ins aktualisieren, um dem neuen Gesamtstil zu entsprechen
&#x200B;* [Voreinstellungen] Automatische Vorschau der Hintergrundfarbänderungen
&#x200B;* [Clean] Geringeres Risiko für Projektbeschädigung
&#x200B;* [Öffnen] Verbesserung der Projektzeit wird geöffnet
&#x200B;* [Neues Projekt] Neues Projekt - Verbesserung der Aktualisierungszeit des Meshs
&#x200B;* [Speichern] Speichern der Zeitverbesserung für das Projekt
&#x200B;* [Protokoll] Im Protokoll angegebener Lizenztyp
&#x200B;* [TextureSet] Schaltfläche &quot;Baking Texturen&quot; in &quot;Baking Mesh-Map&quot; umbenennen
&#x200B;* Benennen Sie &quot;Zusätzliche Maps&quot; in &quot;Mesh-Map&quot; um

**Fest:**

&#x200B;* [Viewport] Fehlerhafte Bewegungen mit Meshs, die viele Unterobjekte enthalten
&#x200B;* [Werkzeugeigenschaften] Kanal deaktiviert, wenn ein Material per Drag &amp; Drop in den Bildschlitz gezogen wird
&#x200B;* [Werkzeugeigenschaften] Pinselvorschau wird mit Verwisch- und Kopierwerkzeugen beschädigt
&#x200B;* [Textursatz] Die Reihenfolge der Kanäle ist falsch, wenn Vorlagen verwendet werden
&#x200B;* [Regal] Fehlendes Symbol für Graustufenkonvertierung-Generator
&#x200B;* [Regal] Alpha-Zahl für Signaturkreise ist fehlerhaft (fehlende Schriftart)
&#x200B;* Falsche Erkennung integrierter GPUs beim Start
&#x200B;* [Absturz] Ziehen und Ablegen einer importierten Ressource mit dem Namen &quot;#&quot;
&#x200B;* [Engine] Vram-Erkennungsproblem auf integrierter GPU
&#x200B;* [Engine] Mehrere Absturz im Substance Engine Linker behoben
&#x200B;* [Engine] Quadratische Artefakte bei der Änderung der Auflösung
&#x200B;* [Post-Effekte] Die Größe der Benutzeroberfläche ist langsam, wenn Post-Effekte aktiviert sind
&#x200B;* [Baker] Szene wird für Strahlenentfernungswerte nicht korrekt eingehalten
&#x200B;* [Baker] AO vom Mesh-Verdeckungsabstand wird unabhängig vom Eingabewert auf 1 geklemmt
&#x200B;* [Baker] Bei der Namensübereinstimmung werden einige Mesh mit bestimmten Namen ignoriert.
&#x200B;* [Baker] Die Farbe aus den Einstellungen &quot;Mesh-Polygruppe&quot; und &quot;Teilgitter-ID&quot; gibt immer ein schwarzes Bild zurück.
&#x200B;* [Baker] ID-Baking schlägt mit binären FBX-Meshs von Blender fehl
&#x200B;* [Shader] Rauschen in der 2D-Ansicht mit dota-2 und non-pbr-spec-gloss
&#x200B;* [Linux] Beim Baking wird nur ein CPU-Thread verwendet.
&#x200B;* [MacOS] Absturz mit dem Pinselcursor, der sich über den Viewport bewegt

**Bekannte Probleme:**

&#x200B;* Einfrieren der Berechnung auf AMD VEGA-GPUs
&#x200B;* Verzerrungsnachbearbeitung wird beim Export in Iray nicht berücksichtigt (Alpha)

## Version 3

### 3.4.2 (2017.4.2)

*(Freigegeben: 24. Januar 2018)*

**Hinzugefügt:**

&#x200B;* [Export] Erhalten Sie den Status eines Exports mit Schrittfortschritt
&#x200B;* [Exportieren] Abbrechen eines Exports zulassen
&#x200B;* [Exportieren] Exportieren von Texturen in Sketchfab ohne Qualitätsverlust beim Normalen-Map
&#x200B;* [Export] Export im glTF-Binärformat (glb)
&#x200B;* [Export] Zulassen der Spaltengrößenänderung auf der Registerkarte &quot;Konfiguration&quot; des Exportfensters
&#x200B;* [Shader] Fügen Sie ein Änderungsprotokoll für den Shader-API hinzu.
&#x200B;* [Scripting] Vor- und Nachher-Rückruffunktionen beim Exportieren von Texturen hinzufügen
&#x200B;* [Iray] Upgrade auf SDK 2017.1 (Unterstützung für Volta-GPUs)

**Fest:**

&#x200B;* Absturz beim Beenden der Anwendung, bevor das Hauptfenster angezeigt wird
&#x200B;* [MAC] Absturz beim Laden von Graustufenkarten mit IRAY
&#x200B;* [MAC] VRAM Erkennung ist mit dem neuen Betriebssystem High Sierra nicht korrekt.
&#x200B;* [Plug-In] Das Herunterladen von Assets aus Substance Source funktioniert nicht mehr
&#x200B;* [Scripting] Falsche Erkennung der Mindestversion des Plug-ins
&#x200B;* [Exportieren] Exportvorgabe kann nach dem Exportieren von Texturen nicht gespeichert werden
&#x200B;* [Instanz] Problem mit Generatoren, die in einem TextureSet ohne zusätzliche Maps instanziieren werden
&#x200B;* [Viewport] Dithering funktioniert nicht mit einer Auflösung über 4k
&#x200B;* [Viewport] 2D-Ansicht Material Display ist mit Rauschen überzogen
&#x200B;* [Regal] Verbessern der Ladezeit für Regal-Vorgaben
&#x200B;* [Engine] Falsche Füllmethode beim Malen unter Farbauswahl

### 3.4.1 (2017.4.1)

*(Freigegeben: 15. Dezember 2017)*

**Hinzugefügt:**

&#x200B;* [Scripting] Exportieren von Mesh über die Scripting-API
&#x200B;* [Importieren] Import nicht unterstützter Meshdateien deaktivieren (nur obj, fbx, date, play zulassen)
&#x200B;* [Log] Präzisere Angabe des TDR-Problems in der Protokolldatei

**Fest:**

&#x200B;* Absturz, wenn die Anwendung geschlossen wird, bevor das Crawlen der Ressourcen abgeschlossen ist
&#x200B;* Absturz beim Öffnen von Projekten mit dem Verwischen-/Klon-Werkzeug
&#x200B;* Absturz bei der Verwendung von &quot;redo&quot; nach einem Rückgängigmachen einer Shader-Änderung in den Anzeigeeinstellungen
&#x200B;* [Engine] Die Texturierung unterscheidet sich zwischen Painter 2017.2 und 2017.4
&#x200B;* [Viewport] Beim Auswählen auf einem ID-Map aus einer Instanz wird die falsche Farbe aufgenommen.
&#x200B;* [Exportieren] Absturz beim Exportieren einer ungültigen Normal- oder Verdeckung-Textur
&#x200B;* [Exportieren] Beim Öffnen von PSD-Dateien in Photoshop CS6 sind die Gruppen gesperrt
&#x200B;* [Plugin] Photoshop Plugin ignoriert die Kanalauswahl und exportiert immer alles
&#x200B;* [Ebenen] Ankerpunkte brechen beim Kopieren/Einfügen über Textursatz hinweg ab
&#x200B;* [Ebenen] Einige Ankerreferenzen können nicht wiederhergestellt werden, wenn sie beschädigt sind
&#x200B;* [Shader] Der Parameter für die sekundäre Rauheit mit pbr-Beschichtung ist defekt.
&#x200B;* [Steam] Popup zur Versionsprüfung sollte beim Start nicht sichtbar sein

**Bekannte Probleme:**

&#x200B;* [AMD] Absturz/Einfrieren beim Malen auf einem Mesh. Kann mit einem GPU-Treiber-Update behoben werden.

### 3.4.0 (2017.4.0)

*(Freigegeben: 23. November 2017)*

**Hinzugefügt:**

&#x200B;* [Instanz] Ermöglicht den instanziieren von Parametern über Ebenen hinweg
&#x200B;* [Instanz] Erlaubt das Wechseln zwischen einer Quellebene und einer Instanz.
&#x200B;* [Instanz] Hinzufügen einer Aktion &quot;instanziieren über Textursatz hinweg&quot;
&#x200B;* [Instanz] Geben Sie im Ebenenstapel wieder eintretende Instanzen (Zyklen) an.
&#x200B;* [Instanz] Instanzen löschen, wenn eine Quelle entfernt wird
&#x200B;* [Instanz] Verweise auf Anker von außerhalb eines instanzierten Ordners nicht zulassen
&#x200B;* [UI] Verschieben Sie den Stapel &quot;Rückgängig&quot; in ein eigenes Fenster mit dem Namen &quot;Verlauf&quot;
&#x200B;* [Plug-In] DCC-Live-Link-Plug-In integrieren
&#x200B;* [Engine] Verbessern der Malleistung mit Sparse-Malerei
&#x200B;* [Exportieren] Optionen für Entwürfe und Re-Exporte zum Sketchfab-Exporter hinzufügen
&#x200B;* [Regal] Hinzufügen einer &quot;Spiegeln&quot;-Steuerung für Schriftsubstanzen
&#x200B;* [Regal] 20 neue Prozeduren hinzufügen Materials
&#x200B;* [Regal] 40 neue Grunges Maps hinzufügen (Bitmap-basiert und prozedural)
&#x200B;* [Viewport] Aktivieren von Kollisionen in der Pinselvorschau auf anderen sichtbaren Textursätzen
&#x200B;* Mindestanforderungen für AMD GPU-Treiber aktualisieren

**Fest:**

&#x200B;* Absturz Beim Berechnen von Substance mit zu großen Auflösungen
&#x200B;* Absturz beim Malen mit Partikeln
&#x200B;* [Viewport] Falsche Specular-Reflexion in der 2D-Ansicht mit bestimmten Meshs
&#x200B;* [UI] Einige unerwünschte Aktionen werden im Protokollfenster angezeigt

**Bekannte Probleme:**

&#x200B;* [Ebenen] Einige Ankerreferenzen können nicht wiederhergestellt werden, wenn sie beschädigt sind
&#x200B;* Absturz bei der Verwendung von &quot;redo&quot; nach einem Rückgängigmachen einer Shader-Änderung in den Anzeigeeinstellungen

### 3.3.3 (2017.3.3)

*(Freigegeben: 1. Dezember 2017)*

**Fest:**

&#x200B;* [Steam] Popup zur Versionsprüfung sollte beim Start nicht sichtbar sein
&#x200B;* [Exportieren] Beim Öffnen von PSD-Dateien in Photoshop CS6 sind die Gruppen gesperrt

### 3.3.2 (2017.3.2)

*(Freigegeben: 20. November 2017)*

**Hinzugefügt:**

&#x200B;* [UI] Dialogfeld &quot;Neue Version verbessern&quot; und Änderungsprotokoll hinzufügen
&#x200B;* [UI] Geben Sie an, ob die Wartung im Dialogfeld &quot;Neue Version&quot; abgelaufen ist
&#x200B;* [Lizenz] Aktualisieren Sie das Lizenzsystem, um Wartungsdaten zu verarbeiten.
&#x200B;* [Exportieren] Adobe Standard Material in Adobe Dimension umbenennen

**Fest:**

&#x200B;* [Mac] Das Malen führt zu schwarzen Quadraten und Beschädigungen der Textur
&#x200B;* [Engine] Der Cache kann manchmal im Viewport verschwinden
&#x200B;* [Engine] Blockige Artefakte werden angezeigt, wenn der Speicherkomprimierungsauslöser aktiviert wird
&#x200B;* [Baking] Seltsame Fehlermeldungen beim Baking bestimmter Mesh
&#x200B;* [Exportieren] PSD werden falsch geschrieben und von Photoshop nicht richtig erkannt
&#x200B;* [Ebenen] Ebenen sollten nicht projektübergreifend kopiert/eingefügt werden können.
&#x200B;* [Substance] UserData-Farbraum für normale Eingabe wird in einigen Fällen gespiegelt
&#x200B;* [Regal] Mikronormal in Generatoren gibt invertierte Krümmung aus
&#x200B;* [Regal] HSL wirken sich auch auf den Alphakanal aus
&#x200B;* [Linux] Installation auf Centos schlägt aufgrund fehlender Abhängigkeiten fehl.
&#x200B;* Das Installationsprogramm entfernt in bestimmten Fällen nicht alle Ressourcen aus der vorherigen Installation

### 3.3.1 (2017.3.1)

*(Freigegeben: 26. Oktober 2017)*

**Hinzugefügt:**

&#x200B;* [Exportieren] Exportieren des Gitters aus einem Projekt zulassen
&#x200B;* [Shelf] Entfernen Sie &quot;Sub-Shelf&quot; aus den Registerkartentiteln.
&#x200B;* Einstellungen für die Nachbearbeitung in Vorlagen speichern
&#x200B;* Die TDR-Meldung verständlicher machen
&#x200B;* Fenster &quot;Einstellungen&quot; verbessern, um Fehler zu melden

**Fest:**

&#x200B;* Absturz beim Löschen mehrerer Unterböden
&#x200B;* Absturz beim Umschalten von einem Level auf einen anderen während einer Motorberechnung
&#x200B;* [Mac] Absturz auf der Intel-GPU während der Engine-Berechnungen
&#x200B;* [Mac]&#x200B;[Viewport] Fehlerhafte Bewegungen, wenn Dithering aktiviert ist
&#x200B;* [Mac] MacOS 10.13 wird in der Protokolldatei als &quot;Unbekannte Version&quot; erkannt
&#x200B;* [Bäcker] Backen mit einem Käfig funktioniert nicht mehr
&#x200B;* [Ebenen] Strg + C (Aktion kopieren) funktioniert nicht mehr
&#x200B;* [Ebenen] Beim Einfügen von Ebenen wird die Benutzeroberfläche mit Ankerreferenzen nicht aktualisiert
&#x200B;* [Anker] Duplizieren oder Kopieren/Einfügen der Ebene mit Referenzen unterbricht Verknüpfungen
&#x200B;* [Export] 8K-Export kann in einigen Fällen einen Absturz oder eine Deadlock-Anwendung verursachen
&#x200B;* [Export] Mehrere Probleme im generierten glTF-Dateiformat
&#x200B;* [Importieren] Das erneute Importieren eines Gitters mit demselben Dateinamen funktioniert nicht mehr
&#x200B;* [Plugin] Fenster zum automatischen Speichern wird immer über allem angezeigt
&#x200B;* [UI] Endlose Schleife, wenn Sie im TDR-Dialog &quot;Escape&quot; drücken
&#x200B;* [UI] UI zurücksetzen zeigt eine zweite Titelleiste im Shelf-Fenster an

### 3.3.0 (2017.3.0)

*(Freigegeben: 28. September 2017)*

**Hinzugefügt:**

&#x200B;* [Exportieren] Mesh und Texturen für Adobe Project Felix exportieren
&#x200B;* [Exportieren] Export in das glTF-Dateiformat zulassen
&#x200B;* [Engine] Optimieren der Größe von Texturen in VRAM mithilfe der Blockkomprimierung
&#x200B;* [Viewport] Mesh oder Projekt in den Viewport ziehen und dort ablegen
&#x200B;* [UI] Verbessern der Warnmeldung bei TDR
&#x200B;* [UI] Protokoll sollte nur auf Anfrage angezeigt werden
&#x200B;* [UI] Inhalt des Protokollfensters löschen
&#x200B;* [UI] Anzeigen von Warnungen und Fehlern in der Statuszeile
&#x200B;* [UI] Registerkarten oben anzeigen wie in Webbrowsern
&#x200B;* [UI] Verbessern des Kontexts und der Meldungen &quot;nicht bemalbar&quot;
&#x200B;* [UI] Aktion &quot;Als Kopie speichern&quot; im Dateimenü hinzufügen
&#x200B;* [Ebene] Legen Sie die Standardeinstellung für die Kachelung standardmäßig auf 1 fest.
&#x200B;* [Regal] Verbesserter Verlaufsfilter zur Unterstützung von 10 dynamischen Farben
&#x200B;* [Regal] Fügen Sie ein Leerzeichen in der Standardabfrage des Mini-Regals hinzu
&#x200B;* [Regal] Hinzufügen einer Aktion &quot;Im Explorer öffnen&quot; für lokale Ressourcen im Regal
&#x200B;* [Regal] Vorlage und Shader für Adobe Material Standard hinzufügen (Project Felix)
&#x200B;* [Regal] Erhöhen der maximalen Kachelung in Material-Ebenenschattierungen auf 128
&#x200B;* [Regal] Hinzugefügte Sobel-Krümmung für Mikrodetails von Maskengeneratoren
&#x200B;* [Plug-in] Plug-in zum automatischen Speichern mit anpassbarem Zeitintervall hinzufügen
&#x200B;* [Skripterstellung] Hinzufügen einer Funktion zum Speichern als Kopie

**Fest:**

&#x200B;* [UI] Layout wird beim ersten Start beschädigt
&#x200B;* [Exportieren] Beim Exportieren generierte PSD weisen Formatfehler auf
&#x200B;* [Exportieren] EXR exportiert immer 8-Bit-Höhen-Map
&#x200B;* [Export] Absturz beim Exportieren beschädigter zusätzlicher Maps
&#x200B;* [Importieren] Harte Kanten werden in einigen Fällen bei Maschen mit niedrigem Poly-Wert nicht beibehalten.
&#x200B;* [Import] Verbesserte Fehlermeldungen beim Importieren von Netzen mit Problemen
&#x200B;* [Bäcker] ID-Zuordnungssicherung schlägt fehl, wenn &quot;Mit Namen abgleichen&quot; aktiviert ist
&#x200B;* [Viewport] Der Tangent-Bereich wird nicht mit Bäcker synchronisiert
&#x200B;* [Effekt] Das Zurückverschieben einer Ebene stellt die Referenz eines Ankers nicht wieder her.
&#x200B;* [Effekt] Aktualisierungsproblem beim Erstellen einer Verknüpfung zwischen zwei Masken mit Ankern
&#x200B;* [Effekt] Maskenanker über der Maske sollten nicht aufgeführt werden
&#x200B;* [Effekt] Die Einstellung &quot;Alpha aus Ankern extrahieren&quot; funktioniert nicht
&#x200B;* [Engine] Maske kehrt sich nach dem ersten Pinselstrich um
&#x200B;* [Engine] Absturz beim Wechseln des Textursatzes für ein bestimmtes Projekt
&#x200B;* [Shelf] Absturz beim Löschen einer Vorgabe, die sich in einem Projekt befindet
&#x200B;* [Shelf] Typo im erweiterten Tri-Planar Filter
&#x200B;* [Shelf] MG Mask Builder AO Noise Scale funktioniert nicht richtig
&#x200B;* [Shelf] MG Mask Builder hat umgekehrte Krümmungsparameter
&#x200B;* [Shelf] Importierte Alphas erzeugen eine Materialkugel-Vorschau anstelle einer flachen Vorschau

### 3.2.0 (2017.2.0)

*(Freigegeben: 27. Juli 2017)*

**Hinzugefügt:**

&#x200B;* Ankerpunkte - Ebenen- und Maskenreferenzsystem
&#x200B;* [Ebenen] Möglichkeit, Füll- und Maleffekte umzubenennen
&#x200B;* [Plug-In] Aktualisiertes Substance Source-Plug-In
&#x200B;* [Scripting] Abfragen der Textursatz-Auflösung zulassen
&#x200B;* [Scripting] Ermöglicht das Abrufen des Status der Painting-Engine
&#x200B;* [Leistung] Verbessertes Laden des Projekts und Optimieren des Pinselstempels

**Fest:**

&#x200B;* [Tool] Leistungsprobleme beim Anpassen von Material-Parametern
&#x200B;* [Engine] Verschwindende Pinselstriche bei Änderung der Auflösung (4K>2K)
&#x200B;* [3D-Ansicht] Tangente-Speicherplatz wird nicht mit Bakern synchronisiert
&#x200B;* [Regal] Der Regal-Pfad in den Benutzerdokumenten wird nicht automatisch erstellt
&#x200B;* [Regal] Kompatibilität von Vorgaben mit Vorgängerversionen nach einem Update
&#x200B;* [Shader] Nicht-PBR-Shader funktioniert nicht mehr
&#x200B;* [Baker] ID-Map-Baking schlägt fehl, wenn &quot;Nach Name abgleichen&quot; aktiviert ist
&#x200B;* [Beispiel] Die Namen der Meet Mat-Beispielprojekt-Textursatz sind falsch
&#x200B;* Beim Speichern eines Projekts vor dem Erstellen einer Vorlage werden Schreibberechtigungsfehler zurückgegeben.

### 3.1.0 (2017.1.0)

*(Freigegeben: 20. Juni 2017)*

**Hinzugefügt:**

&#x200B;* [Plug-in] Neues Substance Source-Plug-in (ermöglicht das Herunterladen von Assets im Regal)
&#x200B;* [Regal] 4 Neue Schriftarten (Japanisch + vereinfachtes Chinesisch, Schreibmaschine, Segment)
&#x200B;* [Regal] 230 Neue Alpha (Mischung aus Mustern, Pinseln und Fingerabdruckscans)
&#x200B;* [Regal] 50 Neue Prozedurale (Stoffmuster mittelalterlicher und zeitgenössischer Bekleidung)
&#x200B;* [Regal] 2 neue Umgebungs-Map (Mondarrain und Villa Nova Street)
&#x200B;* [Regal] 9 Neue Filter (MatFx-Edge Wear &quot;Details&quot;, &quot;Beschränkt&quot;, HBAO usw.)
&#x200B;* [Regal] Verbessertes standardmäßiges Panorama-Umgebungs-Map
&#x200B;* [Regal] Neue Arnold 5-Exportvorgaben
&#x200B;* [Scripting] Importieren der Ressource in das Regal zulassen

**Bekannte Probleme:**

&#x200B;* [Exportieren] Die Bearbeitung einer Exportvorgabe ist sehr langsam

## Version 2

### 2.6.2

*(Freigegeben: 20. Oktober 2017)*

<b>Hinzugefügt:</b>

&#x200B;* [Textursatz] Löschen deaktivierter Textursatz zulassen
&#x200B;* [Regal] Mehrere Benutzer können im selben Regal-Ordner schreiben
&#x200B;* [Scripting] Ordner &quot;Plug-ins&quot; neu laden können
&#x200B;* [Scripting] Fügen Sie eine erforderliche minimale API-Version in den Plug-in-Metadaten hinzu, um die Kompatibilität zu gewährleisten
&#x200B;* [Iray] Verbesserungen im Dialogfeld &quot;Bild exportieren&quot;

<b>Fest:</b>

&#x200B;* [Engine] Problem mit verschwundenen Strichen beim Ändern der Auflösung (4K>2K)
&#x200B;* [Baker] ID-Map-Baking schlägt fehl, wenn &quot;Nach Name abgleichen&quot; aktiviert ist
&#x200B;* [Baker] Fehlermeldungen sind nicht explizit genug.
&#x200B;* [3D-Ansicht] Tangente-Speicherplatz wird nicht mit Bakern synchronisiert
&#x200B;* [Werkzeug] Schwarze Artefakte bei Verwendung des Verwischen-Werkzeugs
&#x200B;* [Shader] Nicht-PBR-Shader funktioniert nicht mehr
&#x200B;* [Shader] &quot;pbr-coated&quot; ist gebrochen
&#x200B;* [Shader] Die Rauheit von &quot;pbr-beschichtetem&quot; Shader hat keine Auswirkungen mehr
&#x200B;* [Shader] Spec Gloss Shader stimmt nicht mit Iray und SD überein
&#x200B;* [Regal] Absturz beim Laden zweier Dateien mit demselben Namen, aber unterschiedlichen Dateinamenerweiterungen
&#x200B;* [Regal] Vorgabe kann in den Regale nicht mehr bearbeitet werden
&#x200B;* [Regal] Für im Regal importierte Elemente kann keine benutzerdefinierte Vorschau festgelegt werden
&#x200B;* Aus dem Cache geladene Ressourcen verlieren ihre Nutzung
&#x200B;* Beim Speichern eines Projekts vor dem Erstellen einer Vorlage werden Schreibberechtigungsfehler zurückgegeben.
&#x200B;* Falsches Speichern des Projekts, wenn Dateiname zwei Punkte enthält
&#x200B;* Importieren von Dateien mit mehreren Punkten (.) im Dateinamen führt zu Problemen

### 2.6.1

*(Freigegeben: 12. Mai 2017)*

**Hinzugefügt:**

&#x200B;* [TextureSet] Weisen Sie Mesh-Materialien kein Objekt zu.

**Fest:**

&#x200B;* Absturz beim Wechseln von TextureSet nach dem Ersetzen von durch Baking erzeugte Map
&#x200B;* Absturz beim Rückgängigmachen und Wiederholen nach dem Ändern der Füllmethode der Ebene
&#x200B;* Absturz oder Einfrieren bei Verwendung des Effekts &quot;Farbauswahl&quot; mit großem ID-Map
&#x200B;* [Export] Umbenannte Textursatz werden im Exportfenster nicht alphabetisch sortiert.
&#x200B;* [TextureSet] Beim Zurücksetzen auf den Standardnamen wird keine Eindeutigkeit überprüft.
&#x200B;* [TextureSet] Umbenannter Textursatz wird nach dem erneuten Öffnen des Projekts deaktiviert
&#x200B;* [Regal] Fehlender Standardvorlageninhalt
&#x200B;* [Regal] Nicht quadratische Texturen werden als Quadrat angezeigt
&#x200B;* [Shader] Sobald ein Textursatz deaktiviert wurde, wird der zugehörige Shader zerstört.
&#x200B;* [Scripting] alg.Baking.setTextureSetBakingParameters() funktioniert nicht mehr
&#x200B;* [Scripting] Tippfehler in Websocket-Tutorial
&#x200B;* [Scripting] Verschiedene Probleme in AlgWidgets
&#x200B;* [Log] Falsche Erkennung des verfügbaren virtuellen Arbeitsspeichers in einigen Fällen

### 2.6.0

*(Freigegeben: 27. April 2017)*

**Hinzugefügt:**

&#x200B;* Neues Beispielprojekt &quot;Meet Mat&quot; hinzufügen
&#x200B;* [Plug-In] Neues Plug-In &quot;Resources Updater&quot;
&#x200B;* [TextureSet] Umbenennen und Hinzufügen einer Beschreibung zu Textursätzen zulassen
&#x200B;* [TextureSet] Neuzuweisen von Materialien zulassen
&#x200B;* [TextureSet] Hinzufügen einer Einstellungsschaltfläche im Fenster &quot;Textursatz-Liste&quot;
&#x200B;* [TextureSet] &quot;Deaktivierte&quot; Textursatz am Ende der Liste anzeigen
&#x200B;* [Substance] Verwenden Sie bei der aktuellen Textursatz-Auflösung zusätzliche Maps, um die Leistung zu verbessern
&#x200B;* [Scripting] Aktualisieren einer Ressource, die in einem Projekt verwendet wird (Material, Generator usw.)
&#x200B;* [Scripting] Hinzufügen einer Möglichkeit zum Hinzufügen/Entfernen eines Regals
&#x200B;* [Scripting] Ermöglicht das Abfragen von Informationen aus einer Ressource in Projekten.
&#x200B;* [Skripterstellung] Liste der verfügbaren Shelfs abrufen
&#x200B;* [Scripting] Tutorial zur Verbesserung der AlgWidget-Miniaturansicht
&#x200B;* [Exportieren] Deaktivieren/Aktivieren der Bittiefe je nach Dateiformatunterstützung
&#x200B;* [Log] Plug-In-Namen zum Drucken in der Konsole hinzufügen
&#x200B;* [Protokoll] Fehler bei ausgeblendeten Textursätzen entfernen
&#x200B;* &quot;Begrüßungsbildschirm&quot; mit neuen Symbolen und Text für Beispiele aktualisieren

**Fest:**

&#x200B;* Absturz beim Aktualisieren eines Meshs in bestimmten Projekten
&#x200B;* [Viewport] Symmetrie Ebene Innenfarbe ist nicht mehr sichtbar
&#x200B;* [Viewport] Einige Nachbearbeitungseffekte sind aktiviert, wenn die Solo-Ansicht verwendet wird
&#x200B;* [Shaders] Überblendung mit &quot;\_premult&quot; funktioniert nicht richtig
&#x200B;* [Shaders] Warnung vor Alpha-Test mit dem Standard-Shader
&#x200B;* [Regal] Falsches Analysieren von Tags aus Substance
&#x200B;* [Regal] MatFX Rost Verwitterung funktioniert nicht richtig
&#x200B;* [Regal] HSL ist standardmäßig für falsche Kanäle aktiviert.
&#x200B;* [Regal] Der Scharfzeichner ist standardmäßig für den Height-/Normalkanal aktiviert
&#x200B;* [Exportieren] Verschiedene Exportvorgaben verwenden keine OpenGL-Normalen-Map
&#x200B;* [Tool] Ungenauigkeitsprobleme mit dem Klonen-/Verwischen-Werkzeug erzeugen Artefakte

### 2.5.3

*(Freigegeben: 15. März 2017)*

**Fest:**

&#x200B;* [Baker] Absturz beim Baking führ mit bestimmten Meshs

**Bekannte Probleme:**

&#x200B;* [Mac] Partikeln können in einigen Fällen zu Beschädigungen der Textur führen

### 2.5.2

*(Freigegeben: 14. März 2017)*

**Fest:**

&#x200B;* [Tool] Wacom-Tablets funktionieren unter Linux nicht
&#x200B;* [Werkzeug] Schwarze Artefakte bei Verwendung des Verwischen-Werkzeugs
&#x200B;* [Bäcker] Backen schlägt fehl, wenn &quot;Nach Name abgleichen&quot; mit einem Käfig verwendet wird
&#x200B;* [Bäcker] Umgebungs-Verdeckung funktioniert nur bei Backen mit Normalmap nicht
&#x200B;* [Shelf] Generische Filter behandeln Alpha nicht ordnungsgemäß (Kontrast/Luminanz, Hochpass usw.)
&#x200B;* [Viewport] Leistungsproblem beim Laden eines Projekts mit aktivierten Schatten
&#x200B;* [Viewport] Dithering-Problem in der 3D-Ansicht auf MacOS
&#x200B;* [Viewport] Partikelvorschauen werden bei aktiviertem Farbprofil falsch angezeigt
&#x200B;* [Iray] Absturz beim Zurückwechseln des Projekts zu OpenGL, wenn Iray nicht initialisiert werden konnte
&#x200B;* [IRay] Beim Rendern von SpecGloss shader/mdl wird die Glossiness ignoriert.
&#x200B;* [Shader] Spec/Gloss Shader stimmt nicht mit Iray und SD überein
&#x200B;* [Shader] sRGB-Konvertierung unterscheidet sich von der linearen in die sRGB-LUT-Konvertierung
&#x200B;* [Shader] Falsches Rendering beim Laden eines Projekts mit veralteten Shadern
&#x200B;* [Shader] &quot;pbr-coated&quot; Shader funktioniert nicht mehr
&#x200B;* [Exportieren] Einige Kanäle werden weiterhin exportiert, auch wenn sie nicht im Textursatz vorhanden sind
&#x200B;* [Ebenen] Der Mischmodus &quot;Inverse Details der normalen Karte&quot; funktioniert nicht auf Graustufenkanälen
&#x200B;* [UI] Problem beim &quot;Farbauswahlfenster&quot; mit HDPI-Monitor und Anzeigezoom bei 150 %

**Bekannte Probleme:**

&#x200B;* [Mac] Partikel können in einigen Fällen Texturbeschädigungen verursachen

### 2.5.1

*(Freigegeben: 27. Februar 2017)*

**Fest:**

&#x200B;* [Mac] Wacom-Tablet-Eingang in 3D- und 2D-Ansicht defekt
&#x200B;* [Bäcker] Die Zuordnung nach Namen funktioniert nicht mehr
&#x200B;* [Baker] Die Einstellung &quot;Normale Mittelwerte&quot; funktioniert nicht mehr.
&#x200B;* [Iray] Falsches Rendering mit fehlendem Baking geführt Normalen-Map
&#x200B;* [Iray] Farbprofil verhalten sich anders als beim OpenGL-Renderer
&#x200B;* [Iray] Exportieren von Rendering als Bitmap beinhaltet keine Farbprofil-Korrektur
&#x200B;* [Substance] Materialfilter funktionieren nicht mehr
&#x200B;* [Tool] Die Konturdeckkraft wird nicht in Pinselvorgaben gespeichert
&#x200B;* [Tool] Klon Brush UV Alignment funktioniert nicht mehr
&#x200B;* [Versatz] Beim Exportieren in Ganzzahl sollte der Exportkanal auf 0,5 zentriert sein.
&#x200B;* [Vorlage] Absoluter Pfad wird in Vorlagen gespeichert.
&#x200B;* [TextureSet] Die Textur des Kanals bleibt nach dem Entfernen des Kanals bestehen.

**Bekannte Probleme:**

&#x200B;* [Linux] Wacom-Tablet-Eingaben funktionieren nicht in 3D und 2D-Ansicht
&#x200B;* [Mac] Partikeln können in einigen Fällen zu Beschädigungen der Textur führen
&#x200B;* [Exportieren] In sehr seltenen Fällen können auf AMD-GPUs schwarze Rechtecke erscheinen

### 2.5.0

*(Freigegeben: 21. Februar 2017)*

**Hinzugefügt:**

&#x200B;* Unterstützung für AMD Radeon Pro- und AMD FirePro-GPUs
&#x200B;* [Werkzeug] Unterstützung für Konturdeckkraft hinzufügen
&#x200B;* [Werkzeug] Fügen Sie einen Modifizierer hinzu, mit dem Sie den letzten Pinselstrich fortsetzen können
&#x200B;* [Iray] Update zur Unterstützung von Pascal-GPUs
&#x200B;* [Viewport] Unterstützung für Farbprofil hinzufügen (LUT)
&#x200B;* [Substance] Integration eines neuen Frameworks (SD6-Engine)
&#x200B;* [UI] Liste der &quot;zuletzt verwendeten Dateien&quot; im Menü &quot;Datei&quot; vergrößern
&#x200B;* [Importieren] Verwenden Sie die Kategorie aus Stoffen, um das Präfix im Dialogfeld &quot;Importieren&quot; auszufüllen.
&#x200B;* [Baker] Baking von 8K-Texturen zulassen
&#x200B;* [Bäcker] Nicht quadratische Auflösungen backen
&#x200B;* [Bäcker] Verbessern Sie den Speicherverbrauch beim Backen von schweren High-Poly-Netzen
&#x200B;* [Shelf] Sperren Sie Regale (und Projekte), um die gleichzeitige Bearbeitung zu verhindern und Beschädigungen zu vermeiden
&#x200B;* [Shelf] Lesen Sie Kategorie und Schlüsselwörter von Stoffen, um sie für die Filterung zu verwenden
&#x200B;* [Shelf] Ausschließen von Ressourcen aus dem Ergebnis einer Suchabfrage zulassen
&#x200B;* [Shelf] Verbesserte Berechnung der Miniaturansichten
&#x200B;* [Shelf] Einbetten von Vorgaben in Projekte zulassen
&#x200B;* [Shelf] Schnelles Reduzieren/Erweitern der Strukturansicht mit UMSCHALT
&#x200B;* [Shelf] Speichern von Miniaturansichten, wenn Assets schreibgeschützt sind (lokaler Cache)
&#x200B;* [Shelf] Neuer Inhalt : neue Filter (Transformieren, Spiegeln, triplanar usw.)
&#x200B;* [Shelf] Neuer Inhalt : neue LUTs-Profile (klassisch und künstlerisch, z. B. Film Noir, Vintage usw.)
&#x200B;* [Shelf] Neuer Inhalt : 10 neue Font-Substance zur schnellen Generierung benutzerdefinierter Texte
&#x200B;* [Shelf] Neue Vorlagen : Unity 5 und Unreal Engine 4
&#x200B;* [Shelf] Verbesserter HSL-Filter, um künstlerfreundlicher zu sein
&#x200B;* [Shader] Unterstützung für Specular level-Kanal in PBR-Shadern hinzufügen
&#x200B;* [Shader] Unterstützung für Dithering in Alpha Test Shader hinzufügen
&#x200B;* [Shader] Unterstützung für Parallax Verdeckung Mapping in PBR Shadern hinzufügen
&#x200B;* [Shader] Definieren einer benutzerdefinierten Benutzeroberfläche für Shader-Parameter zulassen
&#x200B;* [MatteLayering] Erstellen eines neuen Maskenkanals für den Workflow der Materialschichtung
&#x200B;* [Skripterstellung] Metadaten in einem SP-Projekt schreiben dürfen
&#x200B;* [Scripting] Export mit einer bestimmten Exportvorgabe zulassen
&#x200B;* [Scripting] Ermöglicht das Abrufen von Shader-Parametern als JSON.
&#x200B;* [Scripting] Unterstützung für WebSocket-Verbindungen hinzufügen
&#x200B;* [Scripting] Fügen Sie die Möglichkeit hinzu, Shader-Instanzen zu laden
&#x200B;* [Scripting] Fügen Sie die Möglichkeit hinzu, ein neues Projekt zu erstellen
&#x200B;* [Scripting] Ermöglicht das Abrufen der URL des in ein Projekt importierten Gitters.
&#x200B;* [Skripterstellung] Nicht quadratisches Backen zulassen
&#x200B;* [Scripting] Berichtsfehler beim Festlegen von Daten über die Scripting-API
&#x200B;* [Substance] Benutzerdaten-Tag hinzufügen, um Normalen-Map-Format anzugeben

**Fest:**

&#x200B;* Absturz beim Aufnehmen von Farbe mit Substanzen
&#x200B;* Absturz beim Laden eines Nicht-RGBA32f-Bildes als Umgebungszuordnung
&#x200B;* Absturz beim Malen auf AMD-GPUs
&#x200B;* [Mesh] Der OBJ-Import erkennt Materialien ohne MTL-Datei nicht.
&#x200B;* [Mesh] Die Generierung des Satznamens für UDIM-Texturen kann in einigen Meshes falsch sein
&#x200B;* [UI] Schaltfläche &quot;Rückgängig/Wiederholen&quot; in Anzeigeeinstellung &quot;Fokus stehlen&quot; und Mausbildlauf anhalten
&#x200B;* [UI] Einige Beschriftungen werden in High-DPI falsch beschnitten
&#x200B;* [Ebene] Der Modus &quot;Ersetzen&quot; für den Maleffekt hat ein falsches Verhalten auf der Maske
&#x200B;* [Ebene] Ungültiges Verhalten des Mischmodus &quot;Subtrahieren&quot; mit Alpha
&#x200B;* [Tool] Die Pinselgröße wird in der 2D-Ansicht beim Malen auf UV-Rahmen enorm
&#x200B;* [Tool] Geraden, die ausgerichtet sind, verhalten sich ungleichmäßig mit High-DPI.
&#x200B;* [Werkzeug] Die Auflösung der Schablone ist manchmal falsch
&#x200B;* [Bäcker] Die Werte für &quot;Max. Okklusionsentfernung&quot; werden geklemmt, wenn &quot;relativ zum Begrenzungsrahmen&quot; &quot;Aus&quot; ist.
&#x200B;* [Shader] Die Kanaldefinitionen für Stapel und automatische Parameter stimmen nicht überein
&#x200B;* [3D-Ansicht] Inkonsistente Anzeige des normalen Kanals abhängig von der Projekteinstellung
&#x200B;* [Viewport] Einige Normalmaps haben festgeklemmte Werte, die als Artefakte angezeigt werden
&#x200B;* [Viewport] Nacheffekte sind standardmäßig immer deaktiviert
&#x200B;* [Export] Die normale Mischeinstellung ist falsch, wenn der normale Kanal fehlt
&#x200B;* [Exportieren] Falsche Texturgenerierung in einigen Fällen auf AMD-GPUs
&#x200B;* [Export] Shader-Parameter werden nicht ordnungsgemäß exportiert, wenn sie sich in einer Gruppe befinden
&#x200B;* [Exportieren] Beim Bearbeiten einer Exportvorgabe in einem benutzerdefinierten Regal wird ein Protokollfehler ausgegeben
&#x200B;* [Regal] Die Filterungen der Strukturansicht stimmen nicht genau mit dem Ordnernamen überein
&#x200B;* [Regal] Das Umbenennen einer Regal-Vorgabe ist schwer zu lesen
&#x200B;* [Regal] In das Regal importierte Shader-Ressource bleibt nach dem Neustart nicht erhalten
&#x200B;* [Regal] Inhalt : Werkzeugvorgabe fehlt
&#x200B;* [Regal] Inhalt : Tile Generator funktioniert nicht richtig
&#x200B;* [Regal] Inhalt : Falsche Maske auf Gummireifen-Schmutziges intelligente Material behoben
&#x200B;* [Regal] Inhalt : Falscher Gruppenname auf dem Material der Ledertasche wurde behoben
&#x200B;* [Iray] Die Hälfte der Meshs fehlt in Iray
&#x200B;* [Linux] Absturz beim Ziehen einer Ressource über die 3D-Ansicht
&#x200B;* [Mac] Voreinstellungen werden bei jedem Start in Sierra zurückgesetzt

**Bekannte Probleme:**

&#x200B;* [Exportieren] In sehr seltenen Fällen können auf AMD-GPUs schwarze Rechtecke erscheinen
&#x200B;* [Iray] Farbprofile können sich manchmal seltsam verhalten

### 2.4.1

*(Freigegeben: 28. Oktober 2016)*

**Fest:**

&#x200B;* Absturz beim Erstellen eines Projekts mit einer Vorlage
&#x200B;* Absturz beim Schließen des Exportdialogfelds während eines Exports
&#x200B;* [Mac] Fehler beim Speichern des Projekts (Speichern der Exportvorgabe nicht möglich)
&#x200B;* [Regal] Beim Erstellen einer neuen Vorgabe wird diese zweimal angezeigt
&#x200B;* [Regal] Vorgaben können ohne Administratorrechte nicht im schreibgeschützten Modus geladen werden

### 2.4.0

*(Freigegeben: 27. Oktober 2016)*

**Hinzugefügt:**

&#x200B;* [Regal] Neue Benutzeroberfläche zum Durchsuchen von Ressourcen (Strukturansicht, Filter usw.)
&#x200B;* [Regal] Speichern einer Suche als Vorgabe zulassen
&#x200B;* [Shelf] Erstellen eines neuen Fensters aus einer Vorgabe zulassen
&#x200B;* [Shelf] Neue Schnittstelle zum Importieren von Ressourcen
&#x200B;* [Shelf] Kopieren Sie die standardmäßige allegorische Ablage im Ordner Dokumente nicht
&#x200B;* [Shelf] Neue Partikel-Vorgaben : Stromkreis, elektrische Leitungen, Rokoko, Kleinvenen
&#x200B;* [Shelf] Verbesserte Vorgaben für ältere Partikel, die einfacher zu verwenden sind (z. B. &quot;Rain&quot;)
&#x200B;* [Shelf] Neue Informationen zum Kontextmenü der Ressource hinzufügen
&#x200B;* [Viewport] Verbessern der Leistung beim Laden von Umgebungskarten
&#x200B;* [Viewport] Unterstützung von Umgebungskarten hinzufügen, die nicht die Potenz von zwei sind

**Fest:**

&#x200B;* Absturz beim Entfernen einer Maske
&#x200B;* Absturz beim Malen nach dem Speichern einer Vorgabe
&#x200B;* Absturz mit Umgebungsunschärfe auf einigen GPUs
&#x200B;* Absturz beim Zuweisen einer falschen Ressource mit dem Mini-Regal
&#x200B;* [Shelf] Bereinigen + Speichern: Entfernen Sie Tags und Metadaten für Ressourcen im Projekt.
&#x200B;* [Shelf] Beim Importieren einer Voreinstellung werden die Ressourcen in der Voreinstellung angezeigt.
&#x200B;* [Exportieren] Die Normalmap, die aus dem Height-Kanal generiert wird, hat eine geringe Intensität.
&#x200B;* [Export] Normal aus Mesh ist in der endgültigen Normalmap nicht immer vorhanden.
&#x200B;* [Export] Dilation mit Transparenz kann manchmal ohne Transparenz erfolgen
&#x200B;* [Scripting] &quot;alg.plugin\_root\_directory&quot; kann einen abgeschnittenen Netzwerkpfad zurückgeben
&#x200B;* [TextureSet] Sperrschaltfläche ist aktiviert, wenn nicht quadratische Projekte erneut geöffnet werden

### 2.3.1

*(Freigegeben: 07. Oktober 2016)*

**Hinzugefügt:**

&#x200B;* [Plugin]&#x200B;[Photoshop] Geben Sie an, welches Material/welcher Stapel/welche Kanäle exportiert werden sollen.
&#x200B;* [Scripting] Funktionsnamen weisen einige Inkonsistenzen auf.

**Fest:**

&#x200B;* [Exportieren] Alpha kann in benutzerdefinierten Exportvorgaben verworfen werden
&#x200B;* [Exportieren] Alpha erhält falsche Gamma-Konvertierung auf sRGB-Kanälen
&#x200B;* [Exportieren] Nicht quadratische Dokumente werden als quadratisch exportiert
&#x200B;* [Exportieren] Zusätzliche Karten können nicht exportiert werden, wenn eine fehlt
&#x200B;* [Iray] Einige Parameter (wie die emittierende Intensität) haben keine Auswirkungen
&#x200B;* [NVIDIA] Absturz beim Start mit NVIDIA Quadro K2200/GTX 750/760
&#x200B;* [AMD] Falscher Farbsatz für Miniaturen und Vorschauen
&#x200B;* [AMD] Einfrieren und Treiberfehler beim Öffnen neuer Dateien und Dateien
&#x200B;* [Log] &quot;software-version&quot; fehlt in der Protokolldatei

### 2.3.0

*(Freigegeben: 15. September 2016)*

**Hinzugefügt:**

&#x200B;* [Zusatzmodul] Neues Zusatzmodul &quot;Nach Photoshop exportieren&quot; (vollständiger Ebenenstapel exportieren)
&#x200B;* [Exportieren] Geben Sie die Breite der Auffüllung an (in Pixel oder unendlich).
&#x200B;* [Exportieren] Festlegen des Hintergrundtyps außerhalb der UVs zulassen
&#x200B;* [Regal] Neuer Material-Ebenen-Shader zum Mischen von 10 Materialien
&#x200B;* [Shelf] Neuer Tonschattierer zur Anzeige von Details mit dem Height-/Normalkanal
&#x200B;* [Shelf] Neuer gebackener Lichtfilter mit Umgebungseingabe
&#x200B;* [Shelf] Einige Maskengeneratoren wurden aktualisiert, um nicht quadratische Transformationen hinzuzufügen.
&#x200B;* [Viewport] Hinzufügen einer zusammengesetzten Normalmap (Normal+Height+Backen) zum Solomodus
&#x200B;* [Skripterstellung] Exportieren zusätzlicher Maps zulassen
&#x200B;* [Skripterstellung] Verfügbare zusätzliche Karten pro Textursatz abfragen
&#x200B;* [Scripting] Kanalformat kann abgerufen werden.
&#x200B;* [Scripting] Fügen Sie Beispiele in der Backing-Dokumentation hinzu
&#x200B;* [Scripting] Ermöglicht das Abfragen der Sichtbarkeit einer Ebene.
&#x200B;* [Skripterstellung] Ermöglicht das Abfragen der Füllmethode und Deckkraft der Ebene
&#x200B;* [Skripterstellung] Exportieren konvertierter Maps (endgültige Normalen-Map, gemischte AO usw.)
&#x200B;* [Substance] Benutzerdefinierte Verwendungen lesen und verbinden
&#x200B;* [Shortcuts] Zusatztaste (SHIFT) hinzufügen, um Solo-Modus rückwärts zu durchlaufen
&#x200B;* [Exportieren] Standardvorgabe für den Export wurde aktualisiert, um Alpha zu deaktivieren
&#x200B;* [UI] Miniaturen werden jetzt nur berechnet, wenn das Engine verfügbar ist
&#x200B;* [UI] Anzeigen einer Erwähnung bei der Berechnung von Miniaturansichten

**Fest:**

&#x200B;* Absturz zu einigen alten Projekten beim Öffnen
&#x200B;* Absturz mit beschädigtem Textur-Kanal-Cache
&#x200B;* Absturz beim Mischen von mehr als 4 Materialien mit dem Material-Ebenen-Arbeitsablauf
&#x200B;* [UI] Tastenkombinationen funktionieren nicht, wenn die Symbolleiste ausgeblendet ist
&#x200B;* [UI] Iray-Symbolleiste ist im Menü &quot;Ansicht&quot; mit &quot;Unbenannt&quot; beschriftet
&#x200B;* [UI] Plug-in-Symbolleisten werden im Menü &quot;Ansicht&quot; als &quot;Nicht geneigt&quot; bezeichnet
&#x200B;* [Baker] Drücken der Eingabetaste beim Bearbeiten einer Baking-Einstellung startet den Baking-Prozess
&#x200B;* [Baker] Falsche Bereiche für einige Parameter
&#x200B;* [Importieren] OBJ Mesh können aufgrund sehr großer Zahlen nicht importiert werden.
&#x200B;* [Importieren] Einige OBJ werden mit zu vielen Unterobjekten importiert
&#x200B;* [Export] Kanalhintergrund wird beim Export mit Schwarz anstelle der Standardfarbe gefüllt
&#x200B;* [Tool] Partikeln funktionieren nicht richtig, wenn der FOV-Wert zu niedrig ist
&#x200B;* [Tool] Die Pinselvorschaufarbe ist bei Masken in untergeordneten Stapeln falsch
&#x200B;* [Viewport] Wenn der Pinsel in leere Bereiche in der 2D-Ansicht geht, wird er gigantisch
&#x200B;* [Viewport] Leere Pinselvorschau beim Malen mit normalen Texturen
&#x200B;* [Skripterstellung] Falsche Dokumentation : &quot;ao&quot; anstelle von &quot;ambientocclusion&quot; aufgeführt
&#x200B;* [Skripterstellung] Der mit subprocess() begonnene Prozess wird beim Schließen von Painter beendet
&#x200B;* [Regal] Baking geführt Beleuchtungsfilter verwenden falsche AO-Eingabe
&#x200B;* [MacOS] Entferntes Fire Hydrant-Projekt (inkompatibel)
&#x200B;* Standardprojekt wird beim Laden einer \*.spt-Datei geöffnet (anstelle von \*.spp).

**Bekannte Probleme:**

&#x200B;* [Plugin] Aufgrund von Photoshop können das Height und der normale Kanal nicht wie besehen Kamera bewogen werden

### 2.2.0

*(Freigegeben: 22. Juli 2016)*

**Hinzugefügt:**

&#x200B;* [Regal] Verbesserung des Suchsystems und der Suchanfragen
&#x200B;* [Regal] Hinzufügen eines Suchfelds für Mini-Regals
&#x200B;* [Shader] Festlegen der Schrittgenauigkeit für Schieberegler
&#x200B;* [Shader] Hinzufügen einer Schaltfläche &quot;Rückgängig/Wiederholen&quot; für Shader-Parameter
&#x200B;* [Shader] Das erneute Laden eines Shader sollte seine Parameter nicht zurücksetzen.
&#x200B;* [MathLayering] Unterstützung für Dynamische Materialüberlagerung und Sub-Stapel hinzufügen
&#x200B;* [MatLayering] Importieren der JSON-Datei zum Einrichten der Shader-Einstellungen zulassen
&#x200B;* [MathLayering] Limit für Textur-Sampler entsperren (Wechsel zu Bindless-Texturen)
&#x200B;* [Scripting] Einstellung der Baker erlauben und Berechnung starten
&#x200B;* [Substance] &quot;Verwendung&quot; für Ein-/Ausgangsverbindungen zusätzlich zu Identifizierungen verwenden
&#x200B;* [Tool] Ermöglicht die Auswahl des Vorschaukanals im Viewport für das Projektion-Tool

**Fest:**

&#x200B;* Absturz beim Start, wenn sich die Substanzen im falschen Ordner befinden
&#x200B;* Der Absturz-Bericht funktioniert aufgrund einer falschen Protokolldatei manchmal nicht
&#x200B;* [Iray] Post-Effekte werden nicht aktualisiert, wenn Iray angehalten wird
&#x200B;* [Iray] Autofokus-Tastaturbefehl funktioniert nicht mehr
&#x200B;* [Iray] Das Verhalten des Blende-Schiebereglers ändert sich je nach Elementgröße.
&#x200B;* [Ebenen] Der Kanal des ersten Materials ist standardmäßig nicht aktiviert, wenn alle deaktiviert sind
&#x200B;* [Shader] Es werden keine Fehler ausgegeben, wenn ein &quot;param auto&quot; nicht korrekt ist.

**Bekannte Probleme:**

&#x200B;* [Mac] Grenzwert für Textur-Samples auf 16 gesperrt (GPU-Treiberproblem)

### 2.1.1

*(Freigegeben: 1. Juli 2016)*

**Hinzugefügt:**

&#x200B;* [Lizenz] Ändern des Speicherorts der Lizenzdatei
&#x200B;* [Viewport] Fügen Sie einen &quot;B&quot;-Tastaturbefehl hinzu, um zwischen weiteren Karten zu wechseln.
&#x200B;* [Importieren] FBX 2016/2017 ordnungsgemäß importieren
&#x200B;* [Tool] Entfernen von Häkchen bei Verwendung der schnelle Maske
&#x200B;* [Iray] Informationen zu den Abmessungen der Szene hinzufügen
&#x200B;* [Iray] Maximale Anzahl von Samples und Renderzeit erhöhen
&#x200B;* [UI] Aktualisieren Sie das Ergebnis sofort, wenn Sie die Schaltfläche &quot;+/-&quot; für Schieberegler verwenden
&#x200B;* [UI] Höhere Präzision für Graustufen-Schieberegler
&#x200B;* [Exportieren] Exportieren Sie keinen Alphakanal für Texturen, die nur RGB sind
&#x200B;* [Exportieren] Dota 2-Exportvorgabe aktualisieren
&#x200B;* [Regal] Neues Muster &quot;Sechseckfliesen&quot;
&#x200B;* [Regal] Neues Werkzeug &quot;Verschweißt&quot;
&#x200B;* [Regal] Aktualisierte Abschlussfilter, um Richtungssteuerungen bereitzustellen

**Fest:**

&#x200B;* [Exportieren] PSD-Dateien können nicht in 8 Bit exportiert werden
&#x200B;* [Export] 8K-Export ist bei einigen Hardware-Konfigurationen nicht verfügbar.
&#x200B;* [Exportieren] Sketchfab-Fenster wird beschnitten
&#x200B;* [Exportieren] Falsche Rauheit-Map in der Spezifikation/Glanz-Exportvoreinstellung
&#x200B;* [UI] Die Eingabe in Graustufenreglern funktioniert nicht mehr
&#x200B;* [UI] Filter können nicht in Substance-Eingaben (wie Generatoren) eingefügt werden
&#x200B;* [UI] Einige Regler haben ein seltsames Verhalten.
&#x200B;* [UI] DeltaTime +/- Schritt für Partikel ist zu groß
&#x200B;* [Iray] Einige Projekte blockieren die Anwendung beim Wechsel zu Iray.
&#x200B;* [Iray] Absturz beim Erkennen von Hardware
&#x200B;* [Werkzeug] Die Pinselvorschaufarbe ist im Maskenmodus falsch
&#x200B;* [Tool] Material Picker kann mit inkompatiblen Tools verwendet werden
&#x200B;* [Tool] Projektion-Vorschau wechselt nicht zu Diffuse mit Spec/Gloss-Workflow
&#x200B;* [Regal] Ändern des Standard-Shader unterbricht Smart Mats/intelligente Masken-Vorschauen
&#x200B;* [Regal] Einige intelligente Material haben falsche Namen
&#x200B;* [Regal] Zusätzliche Alpha-Formen sind beschädigt und werden nicht geladen
&#x200B;* [Viewport] Wechseln in den Modus &quot;Zusätzliche Karte&quot; zeigt zuerst &quot;andere&quot; an
&#x200B;* [Viewport] Viewport wechseln zurück zu &quot;Andere&quot;, wenn keine zusätzliche Map vorhanden ist
&#x200B;* [Absturz]&#x200B;[Linux] Absturz-Bericht funktioniert nicht auf Ubuntu (Steam)
&#x200B;* [Absturz]&#x200B;[Linux] Web-URL-Links funktionieren nicht auf Ubuntu (Steam)
&#x200B;* [Absturz]&#x200B;[Windows] Entfernen Sie &quot;crashwatcher&quot;, wenn Substance Painter nicht mehr ausgeführt wird.
&#x200B;* [Absturz]&#x200B;[Mac] Absturz-Berichtssystem funktioniert nicht richtig
&#x200B;* [Absturz] Das Importieren eines Meshs, während bereits ein Mesh importiert wurde, führt zu einem Absturz
&#x200B;* Textursatz beim Auswählen eines Tastaturbefehl nach einem Neustart auf nichts zurückgesetzt

### 2.1.0

*(Freigegeben: Juni 2016)*

**Hinzugefügt:**

&#x200B;* [UDIM] Importieren von UDIM-Kacheln von einem Mesh als Textursatz
&#x200B;* [Linux] Zusätzliche Unterstützung für CentOS 6.6 und Ubuntu 12.4
&#x200B;* [Exportieren] 8K-Auflösung hinzufügen (experimentell)
&#x200B;* [Exportieren] Auswahl der Bittiefe während des Exports zulassen
&#x200B;* [Baker] Mehrere Textursatz gleichzeitig Baking geführt werden können
&#x200B;* Unterstützung hochauflösender Monitore (hohe DPI-Skalierung)
&#x200B;* [Skripterstellung] Benutzerdefinierte Auflösung und Auffüllung pro Textur beim Export festlegen
&#x200B;* [Viewport] Umschalten zwischen Textursatz durch Klicken auf den Mesh zulassen (über Strg+Alt+Klick)
&#x200B;* [Viewport] Setzen Sie den Mauszeiger an die Stelle, wenn Sie mit dem Mausrad zoomen.
&#x200B;* [UI] Standardhintergrundfarbe und Umgebungs-Map-Anzeige aktualisieren
&#x200B;* [UI] Hinzufügen von QuickInfos mit Originalnamen für Benutzerkanäle
&#x200B;* [UI] Hintergrundfarbe für Kanäle ändern, die nicht umbenannt werden können
&#x200B;* [Tool] Entfernen von Häkchen bei Verwendung der Schnellmaske
&#x200B;* [Shader] Gruppen für Shader-Parameter und Materialien/Masken definieren
&#x200B;* [Motor] Optimierung von Kleinstprägungen
&#x200B;* [Schablone] Fügen Sie &quot;W&quot; als Tastaturbefehl hinzu, um die Maske vorübergehend zu aktivieren/deaktivieren
&#x200B;* [Shelf] Fügen Sie eine Kreuzschaltfläche hinzu, um das Suchfeld zu löschen.
&#x200B;* [Shelf] Alpha mit einem Klick laden
&#x200B;* [Shelf] Neue Exportvorgabe : Vray UDIM, Arnold UDIM, Spec/Gloss von Metal/Rough
&#x200B;* [Shelf] Neue Alphas : geometrische Formen, Adern und Zeichen
&#x200B;* Namen und Version in den Eigenschaften der ausführbaren Substance Painter-Datei hinzufügen

**Fest:**

&#x200B;* [Substance] Es ist nicht möglich, den normalen Kanal und die zusätzliche Karte gleichzeitig zu verwenden.
&#x200B;* [Iray] MDL-Brechung und Einstellung der Absorption funktionieren nicht
&#x200B;* [Iray] Originalskala der Szene wird nicht beibehalten
&#x200B;* [Shelf] Specular/Glossiness-Vorlage verwendet einen falschen Shader
&#x200B;* [Exportieren] Die Standard-Exportvorgabe exportiert einige Maps (wie AO) nicht
&#x200B;* [Viewport] Pivot-Punkt wird nicht aktualisiert, wenn Sie außerhalb der UVs in der 2D-Ansicht klicken
&#x200B;* [UI] Reglerwerte sind gerundet
&#x200B;* [UI] Manchmal ist beim Bearbeiten von Reglerwerten ein sehr kleiner freier Speicherplatz vorhanden
&#x200B;* [Neues Projekt] Die Dropdown-Liste &quot;Vorlage&quot; wird nicht korrekt aktualisiert (von 1.x zu 2.x)
&#x200B;* [Scripting] Behobenes &quot;Hover&quot;-Verhalten bei benutzerdefinierten Schaltflächen
&#x200B;* [Mac] Rückgängig machen bei einem leeren Projekt sperrt die Kamera

**Bekannte Probleme:**

&#x200B;* Absturzbericht ist auf Ubuntu nicht verfügbar
&#x200B;* Einige URL-Schaltflächen funktionieren möglicherweise nicht. In unseren FAQs finden Sie eine Problemumgehung

### 2.0.5

*(Freigegeben: 29. April 2016)*

**Hinzugefügt:**

&#x200B;* [Shelf] Hinzugefügte/aktualisierte Nicht-PBR-Vorlage, Shader und Exportvorgabe
&#x200B;* [Shelf] Die UE4-Exportvoreinstellung wurde aktualisiert und enthält nun die Umgebungsgeräusche (Ambient Verdeckung).

**Fest:**

&#x200B;* Absturz beim Öffnen und Speichern einiger Projekte mit beschädigten Ressourcen
&#x200B;* [Viewport] Drahtgitter wird in der 2D-Ansicht als defekt angezeigt
&#x200B;* [Shelf] Verbesserte Leistung einiger Studioumgebungskarten
&#x200B;* [Shelf] Einige Studioumgebungs-Maps werden dupliziert
&#x200B;* [Regal] Fehlendes &quot;gebackenes Leuchtmaterial&quot;
&#x200B;* [Shelf] Fehlender Generator für &quot;Graustufen-Konvertierung&quot;

### 2.0.4

*(Freigegeben: 26. April 2016)*

**Hinzugefügt:**

&#x200B;* Verbessern von Mesh-Kollisionen und Optimieren des Drahtgitter-Renderings
&#x200B;* Verbessern der Performance und des Arbeitsspeicher-Managements durch umfangreiche Projekte
&#x200B;* Verbessern der Schiebereglerpräzision und des Schrittmachers
&#x200B;* [UI] Aktualisierung der Engine nur bei der Validierung eines Schiebereglers (nicht bei der Eingabe eines Werts)
&#x200B;* [UI] Iris-Schalter auf eine dedizierte Schaltfläche in der Hauptsymbolleiste verschieben (und seinen Tastaturbefehl ändern)
&#x200B;* [Tool] Hinzufügen einer Einstellung für das Verhalten &quot;Speicherort der Klonwerkzeugquelle&quot;
&#x200B;* [Shader] Gitterscheitelpunktfarben in benutzerdefinierten Shadern lesen
&#x200B;* [Scripting] Liste der Textursätze, Kanäle und Ebenen abrufen
&#x200B;* [Skripterstellung] Hinzufügen von Hilfsfunktionen (URL zum Pfad, Exportpfad aus Projekt abrufen)
&#x200B;* [Mac] Erkennen der Mac OS-&quot;El Capitan&quot;-Version in der Protokolldatei

**Fest:**

&#x200B;* Absturz nach zweitem Export auf Substance share
&#x200B;* Absturz beim Kopieren einer Ebene zwischen Textursätzen mit Schnellmaskendaten.
&#x200B;* Einige Projekte haben einen sehr langen Updater, der viel Speicher beansprucht
&#x200B;* [Tool] Absturz beim Auswählen einer Partikelvorgabe mit dem Klon-/Verwischen-Werkzeug
&#x200B;* [Baker] Das Laden von FBX-Dateien dauert bei großen Meshes zu lange
&#x200B;* [Viewport] Auf einigen Computern gedehnte Umgebungszuordnung
&#x200B;* [Viewport] Falsche Gamma-Konvertierung der Alpha-Zahl des Pinsels
&#x200B;* [Exportieren] Alpha wird als Transparenz gespeichert und nicht als separater Kanal mit Tiff-Dateien.
&#x200B;* [Export] Der normale Kanal wird immer als OpenGL exportiert
&#x200B;* [Iray] Fehlende Schiebereglernamen für Iray-Einstellungen
&#x200B;* [Iray] Rendern erfolgt mit einer falschen Auflösung auf Retina/High DPI
&#x200B;* [Iray] Absturz beim Ändern der Größe der Schnittstelle im Iray-Modus
&#x200B;* [Iray] Riesige Leistungsverlangsamung beim Rendern mit einigen niedrigen Auflösungen
&#x200B;* [Iray] Pause funktioniert nicht (Iray berechnet noch im Hintergrund)
&#x200B;* Normale Kanäle weisen manchmal schwarze Quadrate auf.
&#x200B;* Normale Kanäle werden durch Graustufenfilter invertiert.
&#x200B;* Der normale Kanal wird nicht richtig überblendet, wenn der Stapel Alpha aufweist.
&#x200B;* Das Projekt wird beim Öffnen eines Projekts auf der Festplatte bearbeitet, auch wenn es noch nicht gespeichert wurde
&#x200B;* Das erneute Importieren eines Gitters in einigen Projekten führt zu sehr schlechten GPU-Leistungen
&#x200B;* Die Pinselausrichtung ist falsch, wenn ein Gitter nicht berührt wird
&#x200B;* Substance share-Logo fehlt auf dem Begrüßungsbildschirm

### 2.0.2

*(Freigegeben: 25. März 2016)*

**Hinzugefügt:**

&#x200B;* [Iray] Spec/Gloss-Vorlage und Shader aktualisieren, um mit Iray kompatibel zu sein
&#x200B;* [Exportieren] Möglichkeit zum Export von Screenshots nach ArtStation
&#x200B;* [Skripterstellung] Unterstützen Sie die Ausführung aus dem Plug-In-Verzeichnis
&#x200B;* [Skripterstellung] &quot;Speichern unter&quot; zulassen
&#x200B;* [UI] Doppelklicken auf einen Schieberegler zulassen, um seinen Wert zu bearbeiten
&#x200B;* Vela-Beispiel auf Substance share verschieben
&#x200B;* Neues Beispielprojekt : Kugelvorschau
&#x200B;* Benutzer vor einem Konflikt mit Shellerweiterungen warnen

**Fest:**

&#x200B;* Installation von Substance Painter 1.x durch Installationsprogramm außer Kraft gesetzt
&#x200B;* [UI] Das Layout der Kanalliste wurde mit Filtern unterbrochen
&#x200B;* [UI] Shader-Parameter werden nicht angezeigt
&#x200B;* [UI] Die Größenänderung des Ebenenfensters schneidet den Inhalt falsch zu
&#x200B;* [Werkzeug] Der Deckkraftkanal wird nicht immer richtig verwendet
&#x200B;* [Werkzeug] Verwischen/Klonen funktioniert nicht mit Symmetrie
&#x200B;* [Werkzeug] Die Deckkraft der Pinselvorschau ist bei einigen Kanälen falsch
&#x200B;* [Iray] Absturz bei Verwendung von Iray, obwohl es noch nicht erstellt wurde
&#x200B;* [Iray] Es können keine Rastereinstellungsdaten aus dem Projekt geladen werden.
&#x200B;* [Iray] Iray kümmert sich nicht um die Änderung der Einstellungen, nachdem sie angehalten wurde
&#x200B;* [Regal] Das Importieren eines Materials in das Regal funktioniert nicht
&#x200B;* Schablone funktioniert nicht mit normalem Kanal
&#x200B;* Absturz beim Malen auf einigen Projekten
&#x200B;* Absturz beim Malen mit Partikeln in einigen Projekten
&#x200B;* Absturz mit Pixelprozessor während einiger Berechnungen

### 2.0.0

*(Freigegeben: 16. März 2016)*

**Hinzugefügt:**

&#x200B;* Tastaturbefehl zum Substance Store in der Hauptsymbolleiste
&#x200B;* Iray-Renderer mit Ansichtsmodus und Screenshot-Export
&#x200B;* Unterstützung für die Erstellung und Verwendung von &quot;Intelligente Masken&quot;
&#x200B;* Unterstützung für Specular/Glossines PBR-Arbeitsablauf (mit neuem diffusen Kanal)
&#x200B;* Verketten von Substance (Einstecken von Stoffen in Substance-Image-Eingaben)
&#x200B;* Scripting-Unterstützung mit benutzerdefinierten Plug-ins
&#x200B;* Verbessern der Konvertierung von Height in Normal mithilfe eines Sobel-Filters
&#x200B;* Wechseln der Schablone-/Projektion-Vorschauauflösung zu 2K
&#x200B;* Hinzufügen eines normalen Kanals standardmäßig für neue Projekte
&#x200B;* Benutzerdaten-Tag vom Ausgabeknoten lesen, um Kanäle einer Substanz standardmäßig zu aktivieren/deaktivieren
&#x200B;* Normale/AO-Füllmethode in den TextureSet-Einstellungen gelegt
&#x200B;* [Werkzeug] Neues Verwischen-Werkzeug zum Mischen und Verteilen von Farben
&#x200B;* [Tool] Neues Klon-Tool zum Kopieren von Teilen von Texturen
&#x200B;* [Tool] Kanäle für das Verwischen-, Klon- und Radiergummi-Werkzeug auswählen
&#x200B;* [Ebene] Hinzufügen eines Substance-Namens für den Namen des Fülleffekts
&#x200B;* [Ebene] Maske in Zwischenablage exportieren
&#x200B;* [Viewport] Wechseln zwischen Perspektive und orthografischem Modus
&#x200B;* [Viewport] Sichtfeld im Perspektive-Modus steuern
&#x200B;* [Viewport] Erlaubt das Festlegen der Tiefe des Feldabstands mit STRG+Mittelklick.
&#x200B;* [Viewport] Lassen Sie zu ziehen und legen Sie Umgebungs-Map in der 3D-Ansicht.
&#x200B;* [Viewport] Verbessertes Feedback, wenn das Engine starke Berechnungen ausführt
&#x200B;* [Exportieren] Exportieren von Shader-Parametern in eine JSON-Datei zulassen
&#x200B;* [UI] Benutzeroberfläche mit neuen Symbolen, Farben und Layout aktualisieren
&#x200B;* [UI] Hinzufügen von Elementnamen zu den Miniregalen
&#x200B;* [UI] &quot;Kanal-Mapping&quot; standardmäßig reduzieren
&#x200B;* [Shader] Wählen Sie eine benutzerdefinierte Farbe für die Parameter der Shader-Textur aus.
&#x200B;* [Shelf] Fragen Sie beim Ziehen und Ablegen von Ressourcen nach dem Importort von Dateien.
&#x200B;* [Shelf] Neuer Vorschaubereich für Smart-Materialien und Generatoren
&#x200B;* [Shelf] Specular-Glossiness-Shader hinzufügen
&#x200B;* [Shelf] Neue harte Oberflächenformen
&#x200B;* [Shelf] Neue Alphas Texturen und Formen
&#x200B;* [Shelf] Neue Skin-Texturen
&#x200B;* [Shelf] Neue Scan-basierte Materialien und Smart-Materialien
&#x200B;* [Shelf] Neue intelligente Materialien und spec/gloss Unterstützung von alten
&#x200B;* [Shelf] Neue Finish-Filter für metallische Oberflächensimulation
&#x200B;* [Shelf] Neuer leistungsstarker Maskengenerator &quot;Maskeneditor&quot;
&#x200B;* [Regal] Nachbearbeitete und gereinigte alte Materialien
&#x200B;* Neues Beispielprojekt &quot;Vela&quot;

**Fest:**

&#x200B;* [Einstellungen] Kameradrehung und Zoomgeschwindigkeit werden vom Projekt überschrieben
&#x200B;* [Viewport] Präzisionsprobleme bei normaler Standardtextur führen zu falschen Reflexionen
&#x200B;* [Viewport] Vignette ist standardmäßig aktiviert
&#x200B;* [Viewport] Artefakte werden an den Rändern der Umgebungszuordnung angezeigt (Nvidia-GPUs)
&#x200B;* [Viewport] Miniaturansicht im Projektions-/Schablonenmodus ist sehr lang zum Laden
&#x200B;* [Baker] Gebackene Texturen in 16 Bit ganzzahlig statt 32 Bit speichern
&#x200B;* [Layer] Veraltete Substanzen werden falsch im Stapel angezeigt
&#x200B;* Standardfarbe und Bit-Tiefe für einige Kanäle sind falsch (z. B. : Specular, Glanzgrad)
&#x200B;* Radierverhalten zum Deaktivieren der Füllmethode im Passthrough-Modus wurde korrigiert

**Bekannte Probleme:**

&#x200B;* Symmetrie funktioniert nicht mit dem Verwischen- und Kopierwerkzeug
&#x200B;* ArtStation-Export fehlt

## Version 1

### 1.7.3

*(Freigegeben: 1. März 2016)*

**Hinzugefügt:**

&#x200B;* [Exportieren] Fügen Sie eine Option hinzu, um die Auffüllung zu deaktivieren.
&#x200B;* [Regal] Untergeordnete Elementhierarchie innerhalb eines Regal-Regals unterstützen

**Fest:**

&#x200B;* Absturz beim Speichern über einer zuvor schreibgeschützten Datei
&#x200B;* Absturz beim Öffnen eines zweiten Projekts
&#x200B;* Absturz beim Laden einiger Miniaturansichten (Regal, Ebenen oder QuickInfos)
&#x200B;* Die Deaktivierung von &quot;Konturpositionen auf dem Mesh beibehalten&quot; funktioniert nicht
&#x200B;* [Exportieren] Hochskalieren von Bitmaps erfolgt mit nächstliegender Filterung
&#x200B;* [Shelf] Die Suche nach Ressourcen ist sehr langsam.
&#x200B;* [Regal] Weichzeichnungsfilter sind nicht 16-Bit-kompatibel.
&#x200B;* [Tool] Symmetrie funktioniert nicht, wenn Sie eine alte Werkzeugvorgabe laden
&#x200B;* Das Farbdialogfeld für den Specular-Kanal führt keine Farbraumkonvertierung durch

### 1.7.2

*(Freigegeben: 13. Januar 2016)*

**Hinzugefügt:**

&#x200B;* [Ebenen] Standardbearbeitung für Füllebenen zulassen

**Fest:**

&#x200B;* [Export] Sketchfab-Export funktioniert nicht mehr
&#x200B;* [Ebene] Bilineare Filterung wird auch auf die Füllung ohne Transformation angewendet
&#x200B;* [Tool] Schlechte Performance bei Verwendung von Substanz mit Bildeingaben im Projektion-Modus
&#x200B;* [Tool] Material-Auswahl ist defekt

### 1.7.1

*(Freigegeben: 18. Dezember 2015)*

**Fest:**

&#x200B;* Absturz beim Wechseln des Textursatzes
&#x200B;* Langsame Bewegungen beim Malen

### 1.7.0

*(Freigegeben: 17. Dezember 2015)*

**Hinzugefügt:**

&#x200B;* [Performances] Berechnen des Inhalts von Ebenen und ihrer Miniaturansichten gleichzeitig
&#x200B;* [Export] Speichern Sie den Exportpfad als relativ, wenn Sie ihn neben dem Projekt
&#x200B;* [Ebenen] Neue Füllmethode hinzugefügt : Subtrahieren und Hinzufügen/Subtrahieren
&#x200B;* [Layers] Neue Bilineare HQ-Filterungen für Füllebenen
&#x200B;* [Shader] Legen Sie in den Voreinstellungen einen Standard-Shader für die Miniaturgenerierung fest.
&#x200B;* [Shader] Geben Sie einen Shader pro Textursatz an.
&#x200B;* [Shader] Texturen aus dem Regal aufnehmen
&#x200B;* [Werkzeug] Neues Pinselverhalten &quot;Umbrechen&quot; für das Malen
&#x200B;* [Tool] Verbesserte Filterung und reduziertes Aliasing beim Malen
&#x200B;* [Tool] Verbesserte Malqualität unter Pixeln
&#x200B;* [Tool] &quot;Einfache&quot; Anzeige für Pinseleinstellungen entfernt und das Symbol zum Öffnen/Schließen des Rahmens verbessert
&#x200B;* [Menü] Hinzufügen von Effektsymbolen im Kontextmenü
&#x200B;* Vorlagenerstellung aus Projekten
&#x200B;* [Regal] Neue Vorlagen : PBR, Dota 2
&#x200B;* [Regal] Neue Exportvorgabe : Dota 2
&#x200B;* [Regal] Neue Shader : Dota 2, PBR Car Malen, PBR Coated, PBR Velvet
&#x200B;* [Regal] Neues Material : Rost und Verschleiß aus Stahl, Stilisierte Beleuchtung
&#x200B;* [Shelf] Neue Filter : Weichzeichnen von gerichtetem, stilisiertem Licht
&#x200B;* [Fach] Neuer Pinsel : Standard-Soft- und Standard-Hard mit einem neuen Alpha für eine bessere Härtekontrolle
&#x200B;* [Shelf] Neue Generatoren : 3D-Abstand und -Licht
&#x200B;* [Ablage] Aktualisierte Pinsel mit Wrap-Projektion und Rückseitenauswaschung (standardmäßig aktiviert)
&#x200B;* [Shelf] Aktualisiertes weißes Rauschen mit Pixelprozessorversion für schnellere Berechnung

**Fest:**

&#x200B;* [Begrüßungsbildschirm] Tutorials-Link an alte Videos senden
&#x200B;* [Kanäle] Wenn Sie &quot;Nein&quot; sagen, um die Ebenenerstellung mit AO zu füllen, erstellen Sie immer noch die Ebene
&#x200B;* [Kanäle] UserX-Kanalnamen werden in der Schnittstelle nicht weitergegeben
&#x200B;* [Viewport] Maskeneintrag ist in der Liste der Solokanäle leer
&#x200B;* [Freigeben] Exportieren eines Alpha-Elements von SP aus in die Freigabe erstellt eine unlesbare .image-Datei
&#x200B;* [Lizenz] Aktivierung für Benutzernamen mit Nicht-ASCII-Zeichen beheben
&#x200B;* [Shader] Farbparameter-Dialogfeld verschwindet beim Auswählen einer Farbe
&#x200B;* [Shelf] Miniaturen werden nicht aus dem Speicher entladen, wenn sie nicht verwendet werden
&#x200B;* [Shelf] Filter mit festem Verlauf
&#x200B;* [Werkzeug] Symmetrie funktioniert nicht mit Schablone/Projektion
&#x200B;* [Tool] Falscher Name beim Erstellen einer neuen Pinselvorgabe
&#x200B;* Die Einstellung &quot;Kontur beibehalten&quot; bleibt auch beim erneuten Importieren eines Gitters deaktiviert
&#x200B;* TDR (Driver Reset) bei der Berechnung von Partikeln mit großer Größe.

### 1.6.1

*(Freigegeben: 9. November 2015)*

**Fest:**

&#x200B;* Absturz beim Öffnen des Projekts, wenn die 2D-Ansicht sichtbar ist
&#x200B;* Absturz beim Erstellen einer neuen Exportvorgabe, wenn das aktuelle Fach nicht vorhanden ist
&#x200B;* [Werkzeug] Symbol für Materialauswahl kann angezeigt bleiben
&#x200B;* [Werkzeug] Materialauswahl blendet den Mauszeiger aus, wenn gleichzeitig gemalt wird
&#x200B;* [Shelf] Metadaten werden nach jedem Beenden auf die Festplatte geschrieben

### 1.6.0

*(Freigegeben: 29. Oktober 2015)*

**Hinzugefügt:**

&#x200B;* Offizielle Unterstützung für Windows 10
&#x200B;* [Substance] Reduzieren von Stoffparametergruppen standardmäßig
&#x200B;* [Substance] Neues Framework hinzufügen (Verbessern der Pixelprozessorleistung)
&#x200B;* [Viewport] Erlauben Sie, die Anzeige der Symmetrieebene im Symmetriemodus zu deaktivieren.
&#x200B;* [Viewport] Verbessern des Renderings von Schatten und der Leistung
&#x200B;* [Viewport] Anhalten der Schattenberechnung beim Malen
&#x200B;* [Viewport] Verbessern der Renderleistung von Drahtgitter
&#x200B;* [Engine] Verbessern Sie das VRAM-Speichermanagement, um die Stellfläche zu reduzieren
&#x200B;* [Engine] Verbessern der Texturaktualisierung auf AMD-GPUs für bessere Leistung
&#x200B;* [Engine] Deaktivieren Sie die Einstellung für die Threaded-Optimierung auf NVIDIA-GPUs, um bessere Leistung zu erzielen.
&#x200B;* [Effekt] Fügen Sie ein Tag hinzu, um eine &quot;aufgefüllte&quot; Bildeingabe anzufordern.
&#x200B;* [Ebene] Präzision des UV-Versatzes/der Skalierung in der Füllung erhöhen
&#x200B;* [Ebene] Skalieren Sie den Schieberegler exponentiell in der Füllung
&#x200B;* [Ebene] Lassen Sie zu, dass Materialien direkt in den Ebenenstapel gezogen und abgelegt werden.
&#x200B;* [Ebene] Filter können direkt in den Ebenenstapel gezogen und abgelegt werden
&#x200B;* [Ebene] Passen Sie die Maskenpinselfarbe an die neu erstellte Maskenfarbe an
&#x200B;* [Shader] Mehrere Texkode freilegen
&#x200B;* [Shader] Belichten Sie die Gamma-/Tonzuordnungsfunktion, um benutzerdefinierte Funktionen zu ermöglichen
&#x200B;* [Bäcker] Ändern Sie die Standardeinstellungen für Positionierungsbaker für die Verwendung von TriPlanar.
&#x200B;* [Werkzeug] Benennen Sie &quot;Geometry Decal&quot; in &quot;Polygon Fill&quot; um.
&#x200B;* [Shelf] Aktualisieren Sie Generatoren zur Unterstützung von TriPlanar : MG Metallkantenverschleiß, MG Maskenbildner, MG Glasfaser, MG Dirt
&#x200B;* [Shelf] Aktualisieren von Materialien mit neuen Einstellungen und Entfernen nicht verwendeter Materialien
&#x200B;* [Shelf] 22 Neue intelligente Materialien (Kunststoff, Eisen, Stoff, Stahl und mehr)
&#x200B;* [Shelf] Aktualisieren Sie Scharfzeichner-, Weichzeichner- und Verkrümmungsfilter mit gepolstertem Bildeingang, um Nähte zu vermeiden
&#x200B;* [Shelf] Verbessern der Verkrümmungseinstellungen für eine einfachere Verwendung
&#x200B;* [Shelf] 2 Neue Verfahrensgeräusche : 3D Perlin und 3D Worley

**Fest:**

&#x200B;* [Engine] Vram-Betragserkennung für dedizierte GPU ist auf Mac falsch
&#x200B;* [Engine] Texturen werden im Viewport dunkler
&#x200B;* [Engine] Schlechte Leistung beim Malen unter mehreren Ebenen
&#x200B;* [Engine] Beim Öffnen des Projekts berechnete Ebenen unterscheiden sich von der zwischengespeicherten Version
&#x200B;* [Substance] Falsche Ergebnisse in 4K auf Mac
&#x200B;* [Substance] Die Parameter haben die falsche Reihenfolge.
&#x200B;* [Shader] Toon- und Pixelshader sind komplett schwarz.
&#x200B;* [Shader] Parameter verschwinden nach dem Ändern der env-map
&#x200B;* [Shelf] Absturz beim Bereitstellen von PNG-Dateien im Generatorordner
&#x200B;* [Shelf] Miniaturansichten werden mit geringer Raueit generiert
&#x200B;* [Tool] Absturz bei Verwendung einer Bitmap im Pinsel-Alpha unter Windows
&#x200B;* [Exportieren] Zusätzliche Kartenexportvoreinstellung exportiert jetzt eine RGB-Karte für die Position

### 1.5.7

*(Freigegeben: 24. September 2015)*

**Fest:**

&#x200B;* Absturzbericht funktioniert nicht mehr

### 1.5.6

*(Freigegeben: 21. September 2015)*

**Hinzugefügt:**

&#x200B;* [Shelf] Verbessern der Qualität der Miniaturansichten (verwenden Sie 1K-Texturen)

**Fest:**

&#x200B;* [Freigeben] Kann nicht mit einem anderen Konto signiert werden
&#x200B;* [Shelf] Miniaturansichten sind auf der Festplatte zu groß
&#x200B;* [Regal] Intelligente Materialien sind sehr langsam zu laden
&#x200B;* [Windows] Installation des Lizenzdiensts beheben
&#x200B;* [Channels] Transmissive Map wird standardmäßig als G8 erstellt

### 1.5.5

*(Freigegeben: 15. September 2015)*

**Hinzugefügt:**

&#x200B;* [Shelf] Exportieren von Assets auf Substance share
&#x200B;* [Shelf] Neue Kugelvorschau für Materialien hinzufügen
&#x200B;* [Regal] Verwenden Sie die Env-Karte &quot;Glasüberdachter Patio&quot; zum Generieren von Miniaturen
&#x200B;* [Shelf] Erhöhung der Auflösung der Miniaturbildgröße auf 512 x 512 Pixel
&#x200B;* [3D-Ansicht] Umgebungsdrehungswert freigeben
&#x200B;* [Windows] Anwendung signieren

**Fest:**

&#x200B;* [Bäcker] Falsche Ergebnisse beim gleichzeitigen Backen von Karten
&#x200B;* [3D-Ansicht] Die Env-Map wird angezeigt, wenn kein Projekt geöffnet ist
&#x200B;* [Ebenen] Maskengeneratoren funktionieren nicht bei Ebeneninhalten
&#x200B;* [Ebenen] Sie können auf ausgeblendeten Ebenen malen
&#x200B;* [Shelf] Dirt\_5 und Dirt\_6 sind identisch.
&#x200B;* [Shelf] Einige Maskengeneratoren sind verpixelt oder haben eine niedrige Qualität.
&#x200B;* [Werkzeug] Falsche Gizmo-Drehung um bestimmte Winkel.
&#x200B;* [Tool] Zu viele Kanäle führen zum Ausschneiden der Kanalschaltflächen
&#x200B;* [Werkzeug] Maskenverknüpfung für Schnellmaske umkehren funktioniert nicht
&#x200B;* [Exportieren] Sketchfab: Schaltfläche &quot;Abbrechen&quot; wird nicht korrekt berücksichtigt
&#x200B;* [Lizenz] Aktivierung fehlgeschlagen, wenn die Lizenz nicht kopiert werden kann
&#x200B;* Der Framerate-Begrenzer funktioniert nicht mehr auf der Benutzeroberfläche

### 1.5.0

*(Freigegeben: 20. August 2015)*

<b>Hinzugefügt:</b>

&#x200B;* [Shader] Zeilennummer in Shader-Kompilierungsfehlermeldungen hinzufügen
&#x200B;* [Shelf] Verbessern der Qualität von Miniaturansichten
&#x200B;* [Regal] Automatisierte Miniaturgenerierung für Intelligenten Materials
&#x200B;* [Tool] Tastaturbefehl zur Einstellung der Härte im Stoff
&#x200B;* [Werkzeug] Graustufen-Widget für Geometrieaufkleber verwenden, wenn Sie sich über einer Maske befinden
&#x200B;* [Tool] Tastaturbefehl zum Invertieren der Malen-Farbe beim Malen auf einer Graustufenkarte
&#x200B;* [Viewport] Drahtgitter anzeigen und Farbänderung zulassen
&#x200B;* [Viewport] Weichzeichnen des Umgebungshintergrunds
&#x200B;* [Steuerelemente] Hinzufügen der Drehung zu Kurzbefehlen der Pinselmaus
&#x200B;* [Exportieren] Nach Sketchfab exportieren
&#x200B;* [Exportieren] Erstellen von Exportvorgaben für Renderer
&#x200B;* [Exportieren] Konvertierte Map-Reflexion hinzufügen, F0 und 1/IOR
&#x200B;* [UI] Begrüßungsbildschirm hinzufügen
&#x200B;* [UI] Standardlayout aktualisieren
&#x200B;* [UI] Hinzufügen fehlender QuickInfos und Umbenennen einiger Menüeinträge
&#x200B;* [Ebenen] Exportieren der aktuell ausgewählten Maske als Bitmap
&#x200B;* [Ebenen] Hinzufügen der Aktion &quot;Maske umkehren&quot; im Kontextmenü

<b>Fest:</b>

&#x200B;* [Project] Wenn sich die Gitter-Pivots in der FBX unterscheiden, werden die Gitter beim Import explodiert
&#x200B;* [Substance] Substance in Projektion-Tools sind in 256\*256 gesperrt
&#x200B;* Absturz [Ebenen] bei Verwendung von &quot;Maske löschen&quot;
&#x200B;* [Exportieren] Falsche Gamma-Konvertierung auf sehr dunklen Texturen
&#x200B;* [Export] Positionszuordnung kann nur in Exportvorgaben als Graustufenzuordnung verwendet werden
&#x200B;* [Tool] Die Anfangsfarbe des Geometrie-Aufklebers ist schwarz, wenn er auf einer Maske verwendet wird
&#x200B;* [Tool] Der Tastaturbefehl &quot;Drehung&quot; funktioniert nicht, wenn keine Härte im Alpha-Wert vorhanden ist

### 1.4.2

*(Freigegeben: 15. Juli 2015)*

**Fest:**

&#x200B;* [Tool] Absturz bei Verwendung von Geometrieaufkleber mit Schnellmaske
&#x200B;* Beim Aktualisieren des Projekts von 1.4.0 auf 1.4.1 wird der gesamte Computerspeicher belegt.
&#x200B;* Falscher Import des alten Projektformats
&#x200B;* In benutzerdefinierten Bibliotheken wird die gesamte Hierarchie analysiert, und Elemente werden überall dupliziert.

### 1.4.1

*(Freigegeben: 23. Juni 2015)*

**Hinzugefügt:**

&#x200B;* [Viewport] Fenster nebeneinander andocken
&#x200B;* [Effekt] Hinzufügen eines Hintergrunds und eines Lineals für den Ebeneneffekt
&#x200B;* [Effekt] Fügen Sie einen Maleffekt hinzu, mit dem Sie andere Effekte übermalen können.

**Fest:**

&#x200B;* [Shelf] Miniaturgenerierung funktioniert nicht, wenn kein Projekt geöffnet ist
&#x200B;* [Shelf] Materialvoreinstellungsvorschau kann nicht generiert werden
&#x200B;* [Shelf] Materialvorschauen werden auf einem Gitter mit invertierten Normalen generiert.
&#x200B;* [Shelf] Miniaturansichten werden aufgrund einer falschen Hash-Funktion immer neu berechnet
&#x200B;* [Regal] Durch Klicken auf ein Substance-Material werden keine zusätzlichen Karten verbunden.
&#x200B;* [Werkzeug] Falscher Wert, der mit der Materialauswahl aufgenommen wurde
&#x200B;* [Tool] Farbwähler wählen Viewport-Cursorfarbe aus
&#x200B;* [2D-Ansicht] Sehr niedrige Framerate/Performance
&#x200B;* [Export] Absturz beim Öffnen des Exportfensters mit zu aktuellen Exportvorgaben.
&#x200B;* [Exportieren] Height-Kanal in normale Map wird in den falschen Raum konvertiert
&#x200B;* [Mac] BaseColor aus Substance-Effekten wird als Linear angezeigt
&#x200B;* [Mac] Das Widget für gerade Linien ist auf der Retina falsch gezeichnet
&#x200B;* Gerade Linien können auch bei Loslassen des Tastaturbefehls aktiviert bleiben.
&#x200B;* Gerade Linien Guizmo verschwinden nach dem Drehen der Umgebungskarte
&#x200B;* Umgebungsluftausgänge von Verdeckungen werden nicht automatisch an den AO-Kanal angeschlossen
&#x200B;* Problem mit Lizenzkopien unter Windows mit Sonderzeichen im Benutzernamen beheben

### 1.4.0

*(Freigegeben: 10. Juni 2015)*

**Hinzugefügt:**

&#x200B;* [Exportieren] Fügen Sie der Liste der verfügbaren Eingabemaps zusätzliche Maps hinzu
&#x200B;* [Shelf] Verwenden von SBSAR-Materialien als Materialvorgaben
&#x200B;* [Shelf] Benutzerdefinierte Bibliothekspfade verwenden
&#x200B;* [Regal] Die Mindestgröße ändern.
&#x200B;* [Shelf] Neuer Inhalt : 20 neue Smart-Materialien
&#x200B;* [Shelf] Neuer Inhalt : neuer verfahrenstechnischer Stoff (Gewebe, Gewebe)
&#x200B;* [Shelf] Aktualisierter Weichzeichnungsfilter
&#x200B;* Zeichnen von geraden Linien mit einer Zusatztaste
&#x200B;* Hinzufügen eines Kanals für die umgebende Verdeckung und Überarbeiten des AO/Normal-Verhaltens im Ebenenstapel
&#x200B;* Lesen der Standardfarbe aus der Bildeingabe, die in den Substance-Benutzerdaten definiert ist
&#x200B;* Exportieren des Protokolls über das Hilfemenü zulassen

**Fest:**

&#x200B;* [Baker]&#x200B;[Mac] Absturz mit &quot;Normal&quot; vom Gitterbaker
&#x200B;* [Baker] Absturz, wenn keine UVs in der Käfigdatei vorhanden sind
&#x200B;* [Baker] Das Abgleichen nach Namen funktioniert nicht mit OBJs, die aus zBrush exportiert wurden
&#x200B;* [Baker] Backen mit einem Käfig überschreibt Backen, wenn mehrere Textursätze und überlappende UVs verwendet werden
&#x200B;* [Baker] Bestimmte OBJ-Dateien führen zu schwarzen Texturen
&#x200B;* [Shelf] Ressourcen können nicht gelesen werden, wenn sie auf schreibgeschützt festgelegt sind
&#x200B;* [Regal] Asset-Dateien werden in Painter geschrieben, wenn sie im Projekt verwendet wurden.
&#x200B;* [Regal] Das erneute Laden von Stoffen aktualisiert auch die Schicht
&#x200B;* [Exportieren] Tiff exportiert 32-Bit-Bilder, die von Photoshop oder Game-Enginen nicht richtig gelesen werden können
&#x200B;* [Exportieren] Standardkanalvoreinstellung exportiert immer als RGB
&#x200B;* [Material] Diffuse-Kanal überschreibt BaseColor-Zuordnung mit Substanzen
&#x200B;* [3D-Ansicht] Falsche Beleuchtung von Diffusen mit spezifischen Umgebungskarten
&#x200B;* [Tool] Ein Pinsel kann nicht in einen bestimmten Winkel gedreht werden
&#x200B;* Viewport erhält den Fokus, wenn der Mauszeiger während der Eingabe in einem Textfeld auf
&#x200B;* Absturz mit zu aktuellen Vorgaben für die aktuelle Version des Regals
&#x200B;* Absturz nach dem Ersetzen von Mesh
&#x200B;* Absturz beim erneuten Laden eines Stoffes mit einer anderen Anzahl von Einsatzstoffen
&#x200B;* FBX von Meshs aus dem Cinema4D-Import mit falschen Material-Namen

### 1.3.5

*(Freigegeben: 29. Mai 2015)*

**Hinzugefügt:**

&#x200B;* [Lizenz] Aktivierungsproblem, wenn eine bereits vorhandene Lizenzdatei vorhanden ist
&#x200B;* [Mac] Absturz beim Laden bestimmter FBX
&#x200B;* [Mac]&#x200B;[3D-Ansicht] Falsche Reflektion für integrierte GPU
&#x200B;* [3D-Ansicht] Schnelle Maske-Schriftart ist defekt
&#x200B;* [3D-Ansicht] Material-Picker macht den Viewport komplett schwarz
&#x200B;* Absturz nach dem Öffnen von Projekten, die in 1.3.3 erstellt wurden
&#x200B;* Die Vorschau des Materials ist leer, wenn Shader mit Alpha verwendet werden
&#x200B;* Malerei funktioniert nicht mehr an bestimmten Meshs
&#x200B;* Die Leistung nimmt mit bestimmten OBJ Meshs stark ab
&#x200B;* Benutzerkanäle werden bei Verwendung von Effekten nicht zugeordnet
&#x200B;* Temporäre Ordner werden beim Start nicht gesäubert

**Fest:**

&#x200B;* Verbesserungen der Berechnungszeit für das Projekt, das extrem lange geladen werden kann
&#x200B;* Ändern Sie das Fenster &quot;GPU-Fehlerbehebung&quot;, um verständlicher zu sein
&#x200B;* [Ebenen] Speichern Sie den Status der Verhältnissperre für Füllebenen und aktivieren Sie sie standardmäßig
&#x200B;* [Bäcker] Bei der Namensübereinstimmung wird jetzt das Suffix als Trennzeichen verwendet.

### 1.3.4

*(Freigegeben: 27. April 2015)*

**Hinzugefügt:**

&#x200B;* [Mac] Absturz mit Mac OS X Yosemite (10.10)
&#x200B;* [Mac] Vollbildmodus kann nicht beendet werden
&#x200B;* [Bäcker] Die Option &quot;Backmatch nach Namen&quot; funktioniert nicht
&#x200B;* [Bäcker] Mikk-Tangentenraum in SP funktioniert nicht mit UE4
&#x200B;* [Bäcker] ID-Bäcker kann keine Material-ID-Farben backen
&#x200B;* [2D-Ansicht] Drahtgitter wird nicht angezeigt, wenn das Geometry-Aufkleber-Werkzeug verwendet wird
&#x200B;* [Tool] Alphakanal des Pinsels wird als Checker anstelle der Transparenz mit Materialien angezeigt
&#x200B;* [Tool] Absturz mit Geometry Decal
&#x200B;* [Ebenen] Materialschlitz ist auf der Füllebene standardmäßig ausgeblendet
&#x200B;* [Export] Absturz beim Exportieren mit einer höheren Größe als der Auflösung des Textursatzes
&#x200B;* Specular-Kanal wird in Filtern nicht erkannt.
&#x200B;* Clean + save entfernt die Ressourcen nicht ordnungsgemäß aus dem Archiv von spp
&#x200B;* Speichern Sie die Low-Poly-Transformation nicht in einer High-Poly-Assbin-Datei
&#x200B;* FBX-Datei wird mit zu vielen Textursätzen importiert

**Fest:**

&#x200B;* Effekte: Die Tonwertspanner sollten standardmäßig aktiviert sein, um &quot;klassische&quot; Pegel nachzuahmen.
&#x200B;* Ebenen: Ändern der minimalen und maximalen Kachelung in der Füllaktion
&#x200B;* Ebenen: Speichern und Wiederherstellen des Stapelstatus
&#x200B;* Baker: AO-Baker berücksichtigen die Normalen-Map, wenn kein HP angegeben ist
&#x200B;* Baker: Hinzugefügte QuickInfos und zusätzliche Informationen im Fenster &quot;Baking&quot;
&#x200B;* Erstellen einer Sicherungsdatei beim Speichern eines Projekts

### 1.3.3

*(Freigegeben: 1. April 2015)*

**Hinzugefügt:**

&#x200B;* Fügen Sie Softwareversion und Projektnamen in der Titelleiste hinzu
&#x200B;* Bereinigen von Textursatznamen und Intelligente Material-Namen
&#x200B;* Substance Engine auf V5 aktualisieren
&#x200B;* [Regal] Neue Umgebungs-Map hinzufügen : Korsika Strand, Studio 05, Tornoco Studio und mehr
&#x200B;* [Regal] MG Mask Builder mit neuen Parametern aktualisieren
&#x200B;* [Regal] Aktualisieren und Kalibrieren alter Umgebungs-Map

**Fest:**

&#x200B;* Absturz beim Öffnen des Exportfensters
&#x200B;* Drag &amp; Drop im UI-Widget ist nicht möglich, wenn abgedockt
&#x200B;* &quot;Nach Updates suchen&quot; funktioniert nicht
&#x200B;* [Ebenen] Wählen Sie die Maske nicht aus, wenn Sie bei gedrückter Alt-Taste darauf klicken
&#x200B;* [Tool] Tri-planar funktioniert nicht mit dem Normalkanal
&#x200B;* [3D-Ansicht] Diffuse Beleuchtung von env map ist falsch
&#x200B;* [3D-Ansicht] Die Berechnung der Belichtung unterscheidet sich von Designer
&#x200B;* [3D-Ansicht] Schatten sollten auf 100% metallic Fläche nicht sichtbar sein.
&#x200B;* [3D-Ansicht] Mesh mit gespiegelten UVs hat gespiegelte Tangente/Binomale
&#x200B;* [3D-Ansicht] Schatten führen bei bestimmten Meshs zu falschen Ergebnissen
&#x200B;* [Baker] Entfernen Sie den Ordner &quot;.alg\_meta&quot;, der mit Assbin-Dateien erstellt wurde
&#x200B;* [Baker] Absturz beim Baking, wenn Painter ein TextureSet gleichzeitig neu berechnet
&#x200B;* [Mac] Benutzeroberflächenfehler beim Starten der Anwendung

### 1.3.2

*(Freigegeben: 06. März 2015)*

**Fest:**

&#x200B;* [3D-Ansicht] Eine mit dem Projekt gespeicherte Env-Map kann nicht neu geladen werden.

### 1.3.1

*(Freigegeben: 05. März 2015)*

**Hinzugefügt:**

&#x200B;* [Baker] Fügen Sie eine zwischengespeicherte Version von Meshs mit hohem Poly hinzu, um die Berechnung zu beschleunigen
&#x200B;* [Baker] Fügen Sie ein Warnsymbol hinzu, wenn kein hochpolarer Mesh geladen wird.
&#x200B;* [Baker] Wenn kein Mesh mit hoher Poly-Qualität geladen wird, verwenden Sie stattdessen den Projekt-Mesh

**Fest:**

&#x200B;* [Baker] Drücken der &quot;Eingabetaste&quot; beim Bearbeiten des Werts eines Schiebereglers, um das Fenster zu schließen
&#x200B;* [Baker] Das Aktivieren/Deaktivieren eines Bakers löst ebenfalls die Schaltfläche aus.
&#x200B;* [Baker] Es kann nicht Baking geführt werden, wenn Sie die Schaltfläche &quot;all/none&quot; verwenden.
&#x200B;* [Baker] Die Sortierung der Baker-Schaltflächen erfolgt nicht in der richtigen Reihenfolge.
&#x200B;* [Baker] Kontrollkästchen werden ignoriert und alle Baker werden immer verarbeitet.
&#x200B;* [Baker] Der Fortschritt der Fortschrittsleiste wurde behoben.

### 1.3.0

*(Freigegeben: 04. März 2015)*

**Hinzugefügt:**

&#x200B;* [Baker]&#x200B;[3D-Ansicht] Verwenden Sie die Mikkt-Tangente-Space-Berechnung, wenn keine Tangenten/Binormale gefunden wurden.
&#x200B;* [Baker] Neue Baker hinzugefügt: Normal, ID, Verdeckung, Krümmung, Thickness, Position
&#x200B;* [Effekte] Effekt-Stapel ist jetzt invertiert und von oben nach unten dargestellt (wie Ebenen)
&#x200B;* [Effects] Hinzufügen neuer Symbole auf dem Stapel des Effekts
&#x200B;* [Effects] Hinzufügen eines Mischmodus zwischen Füllaktionen im Effekt-Stapel
&#x200B;* [Effekte] Umbenennen von Effekten (Substance-Effekt = Filter usw.)
&#x200B;* Hinzufügen einer &quot;gesperrten&quot; Datei während des Speichervorgangs
&#x200B;* [Effects] Aktion &quot;Füllen&quot; im Stapel &quot;Effekt&quot; hinzufügen
&#x200B;* Neue Ressource hinzugefügt : Intelligente Materialien
&#x200B;* [Ebenen] Neuanordnung von Ebeneneffekten zulassen
&#x200B;* [Tool] Drei-Planare Projektion hinzufügen
&#x200B;* [3D-Ansicht] Unterstützung für Schatten hinzufügen
&#x200B;* [3D-Ansicht] Möglichkeit, erforderliche OpenGL-Status in benutzerdefinierte Shader umzuwandeln
&#x200B;* [3D-Ansicht] Unterstützung für Alpha über neue Shader
&#x200B;* [3D-Ansicht] Shader sind jetzt versioniert und vollständig in einem Projekt gespeichert
&#x200B;* [3D-Ansicht] Warnen Sie den Benutzer, wenn der Shader nicht mehr kompiliert wird

**Fest:**

&#x200B;* [Ebenen] Ablegen unter einem reduzierten Ordner korrigieren
&#x200B;* [Regal] Beheben der Filterung von Inhalten in Mini-Regals
&#x200B;* [Regal] Umbenennen von Kategorien und Neuorganisieren von Registerkarten

### 1.2.1

*(Freigegeben: 12. Februar 2015)*

**Hinzugefügt:**

&#x200B;* \*.spp-Dateien können jetzt durch einen Doppelklick im Explorer geöffnet werden
&#x200B;* [Export] Neues Tag &quot;$project&quot; für Exportvorgaben
&#x200B;* [Exportieren] Fügen Sie unter jedem Textursatz eine Kartenliste (mit Nomenklatur) hinzu
&#x200B;* [Exportieren] Hinzufügen einer Schaltfläche Alle/Keine , um die Textursatz auszuwählen
&#x200B;* [Exportieren] Leere Karten werden während des Exports verworfen

**Fest:**

&#x200B;* [Exportieren] Unity5-Vorgaben haben invertierte Karten
&#x200B;* [Exportieren] Das Hinzufügen eines Schrägstrichs in einem Vorgabename führt zu einem beschädigten Ordner
&#x200B;* [Exportieren] Height-Kanal, der in 32-Bit-Formate exportiert wird, ist falsch eingespannt
&#x200B;* [Exportieren] Textursatz-Liste wird nicht wie im Projekt sortiert
&#x200B;* [Tool] Rückseiten-Ausblendung funktioniert nicht mehr
&#x200B;* Speichern funktioniert nicht mit Sonderzeichen im Pfad

### 1.2.0

*(Freigegeben: 28. Januar 2015)*

**Hinzugefügt:**

&#x200B;* Neuer Normalkanal, der das Malen von Normalen-Map-Daten und das Kombinieren der Ergebnisse ermöglicht
&#x200B;* [Exportieren] Neues Exportfenster mit der Möglichkeit, ein benutzerdefiniertes Packing zu erstellen und benutzerdefinierte Namen festzulegen
&#x200B;* Das Projektdateiformat ist jetzt eine einzelne Datei anstelle von Ordnern
&#x200B;* [Exportieren] Unterstützung verschiedener Normalformate (DirectX, OpenGL)
&#x200B;* [Exportieren] Erstellen einer temporären Sperrdatei während des Exports
&#x200B;* [Ebenen] Mit Umschalt+Nach-links-Taste können Sie eine Maske umschalten
&#x200B;* [Parameter] Legt den Farbraum am unteren Rand einer Bildeingabe bei
&#x200B;* [Regal] Effekt &quot;MG Mask Builder&quot; hat jetzt neue Einstellungen
&#x200B;* [3D-Ansicht] Ambient occlusion-Map verschließt jetzt den diffusen Beitrag, nicht den Specular

**Fest:**

&#x200B;* Projektion Material/Schablone Vorschau wird im Viewport nicht richtig angezeigt
&#x200B;* [3D-Ansicht] Tastaturbefehl-QuickInfo wird nicht angezeigt, wenn &quot;S&quot; (Schablone) Tastaturbefehl verwendet wird
&#x200B;* [Regal] Der Effekt &quot;MatFx Skin Scale&quot; bietet jetzt eine bessere Leistung bei niedriger Auflösung.
&#x200B;* [Exportieren] Texturen vom Export werden einfach hochskaliert, wenn eine größere Dokumentgröße angegeben wird

### 1.1.2

*(Freigegeben: 15. Januar 2015)*

**Hinzugefügt:**

&#x200B;* Hinzugefügt: Neue Einstellungen zum Kamera beweg, Drehen und Skalieren in der Füllebene
&#x200B;* Verbesserte Filterung für Pinsel und Füllebenen
&#x200B;* Die Testversion ist jetzt voll funktionsfähig (kann exportiert werden), aber zeitlich begrenzt.

**Fest:**

&#x200B;* Importieren von OBJ-Meshs mit sehr kleinen Präzisionen nicht möglich
&#x200B;* Problem beim Aktivieren einer Lizenz unter Windows 7 und 8
&#x200B;* Absturz während eines &quot;Speichern unter&quot; eines Projekts
&#x200B;* Absturz beim Löschen des letzten Kanals eines Textursatzes
&#x200B;* Absturz beim Löschen einer Ebene in einem bestimmten Kontext

### 1.1.1

*(Freigegeben: 25. Dezember 2014)*

**Hinzugefügt:**

&#x200B;* [Ebene] Wählen Sie die Ebene oben aus, wenn Sie ein Projekt öffnen/den Textursatz wechseln.
&#x200B;* Verbesserte Geschwindigkeit beim Speichern und Speichern unter mit neuem Komprimierungsalgorithmus
&#x200B;* Anzeige eines Fehlers beim Öffnen eines zu aktuellen Projekts für Painter

**Fest:**

&#x200B;* [Tool] Geometrie Decal produziert Speicherbeschädigungen
&#x200B;* [Pinsel] Gleitkommawerte unter 1 können für die Pinselgröße nicht manuell eingegeben werden
&#x200B;* [Ebene] Durch Erstellen eines Farbauswahleffekts wird dieser nicht zum Ebenenstapel hinzugefügt
&#x200B;* [Ebene] Wenn Sie den Mauszeiger über die Ebenen bewegen, schnipst Painter in die Taskleiste
&#x200B;* [Ebene] Das Hinzufügen einer Bitmap als Maske kann zu einem Absturz führen
&#x200B;* GUI für den Solo-Modus mit dem Height-Kanal ist falsch
&#x200B;* &quot;Projekt speichern&quot; kann fehlschlagen und ein Projekt beschädigen
&#x200B;* Absturz beim Öffnen eines Projekts nach dem Laden eines anderen Projekts mit einem veralteten Shader

### 1.1.0

*(Freigegeben: 16. Dezember 2014)*

**Hinzugefügt:**

&#x200B;* [Effekt] Ersteller einer neuen Material-ID-Maske
&#x200B;* Neue gepunktete weiße/schwarze Linie für das Pinsel-Gizmo
&#x200B;* Neuer Parameter &quot;Winkelfolge&quot;
&#x200B;* Neuer Parameter für die Rückseitensperrung
&#x200B;* Neuer Parameter für die faule Maus
&#x200B;* [Ebenen] Unterstützung für Mehrfachauswahl und -verwaltung
&#x200B;* [Ebenen] Kopieren und Einfügen von einem Textursatz in einen anderen
&#x200B;* [Exportieren] Adobe Photoshop PSD-Format
&#x200B;* [Regal] Neues Tool : Fell, Metallstiche und Reißverschluss
&#x200B;* [Regal] Neuer Pinsel : Schimmel, Bleistift, scharfe Linie und Stich
&#x200B;* [Regal] Neues Alpha : Gaußsches Rauschen, scharfe Linie, Form, Stift, Spritzen, Stich, Reißverschluss
&#x200B;* Verbesserte Malleistung durch Aktualisierung nur eines Teils der benötigten Texturen

**Fest:**

&#x200B;* [Regal] Es ist nicht möglich, einen Stoff mit Graf mit identischen Kennzeichnungen zu laden.
&#x200B;* [Ebenen] Der Mischmodus &quot;Hindurchwirken&quot; funktioniert nicht mit Masken
&#x200B;* [Schablone] Skalierung in 2D-Ansicht unterbrochen
&#x200B;* Probleme und Absturz auf Mac OS Yosemite

### 1.0.2

*(Freigegeben: 9. November 2014)*

**Hinzugefügt:**

&#x200B;* Verbesserte Performance bei der Vorschau von Materialien mit Substanzen
&#x200B;* Verbesserte Leistung mit der Vorschau des Pinselstrichs beim Aktualisieren des Dokuments
&#x200B;* Verbesserte Leistung im Viewport mit niedrigerer Aktualisierungsrate für nicht funktionierenden Bereich
&#x200B;* [Post-Effekte] Verbesserte Benutzeroberfläche zum Verwalten von Einstellungen
&#x200B;* [Post-Effekte] Auf Standardwerte zurücksetzen
&#x200B;* Substance von Effekten und Ebenenoperationen im Kontextmenü
&#x200B;* Unterstützung für die vormultiplizierte Ein-/Ausgabe in Stoffen

**Fest:**

&#x200B;* [3D-Ansicht] Benutzerdefinierte Shader-Parameter werden durch einen großen Leerraum voneinander getrennt.
&#x200B;* [Export] Fehlende sRGB-Konvertierung für Unity4-Voreinstellung
&#x200B;* Möglicher Absturz beim Laden von FBX-Meshs
&#x200B;* Absturz kann beim Laden von einfachen obj-Meshs auftreten
&#x200B;* Die Rechenleiste bleibt beim Laden auf 100 % blockiert.
&#x200B;* Durch das erneute Laden eines Stoffes wird dieser in jede Kategorie verschoben
&#x200B;* DirectX/OpenGL-Switch defekt

### 1.0.1

*(Freigegeben: 27. Oktober 2014)*

**Hinzugefügt:**

&#x200B;* [Tool] Verbesserte Verwendung von Material-Parametern
&#x200B;* Neuer Tastaturbefehl zur UserVoice-Website im Hilfemenü
&#x200B;* Verschiedene Leistungsverbesserungen im Engine

**Fest:**

&#x200B;* Parameterwerte sind für Partikeln auf 2 Dezimalstellen begrenzt
&#x200B;* Aus dem Cache geladene Substance werden in der Benutzeroberfläche nicht als veraltet angezeigt
&#x200B;* Absturz beim Laden eines Meshs von einer Netzwerk-URL
&#x200B;* Painter wird jetzt als signiert unter Mac OS X erkannt.

### 1.0.0

*(Freigegeben: 15. Oktober 2014)*

**Hinzugefügt:**

&#x200B;* Unterstützung benutzerdefinierter Shader
&#x200B;* Unterstützung für 4K-Auflösung
&#x200B;* Beispielzeichenprojekte
&#x200B;* Fortschrittsleiste für lange Berechnungen anzeigen
&#x200B;* [Exportieren] Fügen Sie vor dem Nachbearbeiten der Ausdehnung eine Diffusion hinzu.
&#x200B;* Befehlszeilenargumente in SP für einfache Vorgänge
&#x200B;* Neue Material und Effekte
&#x200B;* Werkzeugvorschau (separate Echtzeitvorschau von Materialien und Bereich für Konturtests)
&#x200B;* Beim Starten von Painter kein Standarddokument erstellen
&#x200B;* [Tool] Fügen Sie die Möglichkeit hinzu, einen Graustufenwert manuell zu bearbeiten
&#x200B;* Verschiedene Verbesserungen für die Schablonen (Einrasten, Reset)
&#x200B;* Partikeln sind jetzt Unterwerkzeuge des Malpinsels, des Radiergummis und der Projektion
&#x200B;* [3D-Ansicht] Baking geführt AO im Viewport-Rendering verwenden
&#x200B;* Teilen der Steuerelemente für Schablonen zwischen der 2D- und 3D-Ansicht
&#x200B;* Kleine Anpassung der Daumengröße in der Bibliothek
&#x200B;* Suchfelder sind für jedes Fenster spezifisch
&#x200B;* Anpassen der Benutzeroberfläche

**Fest:**

&#x200B;* [Substance] Switch funktioniert nicht
&#x200B;* [Farbdialogfeld] Farbtonverlauf wird nicht aktualisiert
&#x200B;* Mesh kann nicht aktualisiert werden, wenn der Dateiname identisch ist
&#x200B;* Werkzeug ist in zu kleinen Ansichten nicht sichtbar
&#x200B;* Das Aufkleber-Werkzeug auf dem Retina-Display funktioniert nicht richtig
&#x200B;* [Substance] Int1 werden als float1 angezeigt
&#x200B;* [Substance] Grundfarbeingabe/Ausgabe wird nicht erkannt
&#x200B;* [Substance] Filter können nicht neu geladen werden.
&#x200B;* [Tool] Graustufen-Widget ist immer ausgeblendet

## Beta

### 0.12.1-beta

*(Freigegeben: 18. September 2014)*

**Hinzugefügt:**

&#x200B;* Unity 5-Exportvorgabe

**Fest:**

&#x200B;* PBR Shader, Rendering-Qualität sollte viel verbessern
&#x200B;* Fokusfunktion ist defekt und Mesh werden standardmäßig beschnitten

### 0.12.0-beta

*(Freigegeben: 17. September 2014)*

**Hinzugefügt:**

&#x200B;* Pipette
&#x200B;* Die Option &quot;Konturposition beibehalten&quot; wurde dem Mesh hinzugefügt, der wieder importiert wird, wenn sich der Begrenzungsrahmen ändert.
&#x200B;* Normalen-Map für Cymourai Standard-Mesh
&#x200B;* Verbessern der Benutzeroberfläche für die Werkzeugansicht (Farben werden abgewischt)
&#x200B;* Verschieben Sie das Menü &quot;Hilfe->Einstellungen&quot; nach &quot;Bearbeiten->Einstellungen&quot;.
&#x200B;* Speichern Sie den Exportpfad im Fenster &quot;Alle Kanäle exportieren&quot;.
&#x200B;* Neue Ebenen-GUI mit Histogrammanzeige
&#x200B;* Besseres Asset-Management (Drag &amp; Drop, Ressourcen neu laden, Nicht verwendete löschen)
&#x200B;* Von &quot;Diffus&quot; zu &quot;Grundfarbe&quot; wechseln
&#x200B;* Schieberegler für die Bearbeitung von Anpassungen - Punkte zusätzlich zu Kommas zulassen
&#x200B;* Füllebene: maximale Kachelung erhöhen
&#x200B;* Standard Umgebungs-Map

**Fest:**

&#x200B;* Schlechte Reflexionsartefakte bei extremen Winkeln
&#x200B;* Specular-/Glanzausfuhr unterbrochen
&#x200B;* Links im Fenster &quot;Info&quot; des Malers funktionieren nicht
&#x200B;* Absturz mit OSX Yosemite
&#x200B;* Mesh werden trianguliert gespeichert
&#x200B;* Der Farb-Tastaturbefehl des Toolfensters wird an die Ausgabeeinrichtung anstelle der Graustufen gesendet.
&#x200B;* Der Farbwähler bleibt geöffnet, wenn Sie von Ebene zu Maske wechseln
&#x200B;* Material aus einer Füllebene kann nicht gespeichert werden
&#x200B;* Größenänderung der drei Bereiche des Regals aktivieren

### 0.11.0-beta

*(Freigegeben: 04. September 2014)*

**Hinzugefügt:**

&#x200B;* Hinzufügen einer Trennlinie zwischen der 3D- und der 2D-Ansicht
&#x200B;* Verwenden eines Verlaufshintergrunds in den 2D-/3D-Ansichten
&#x200B;* Schnittstelle für das Histogramm &quot;Tonwertkorrektur&quot;
&#x200B;* Regal und Bibliothek zusammenführen
&#x200B;* Beim Erstellen oder Aktualisieren einer Vorgabe ist keine Speicheraktion erforderlich
&#x200B;* Importieren von Assets im Regal durch Drag &amp; Drop

**Fest:**

&#x200B;* Der Name der Schaltflächen wird in der Hauptsymbolleiste angezeigt

### 0.10.2-beta

*(Freigegeben: 28. August 2014)*

**Fest:**

&#x200B;* Alle Kanäle exportieren führt zu falschen Ergebnissen

### 0.10.1-beta

*(Freigegeben: 26. August 2014)*

**Fest:**

&#x200B;* Shader ergibt schwarzes Ergebnis bei geringer Rauheit
&#x200B;* GPU-Prüfung: &quot;Quadro&quot;-Karten verarbeiten, alle Geräte erkennen und Benutzernachrichten entsprechend anpassen
&#x200B;* Die meisten Substance-Material sind in Beta 9 auf 256 begrenzt
&#x200B;* Height wird beim Export als Bitmap festgeklemmt
&#x200B;* Die Pinselvorschau unterscheidet sich von der Überlagerung der Projektion in Mac
&#x200B;* Die Verwendung des Geometrie-Werkzeugs zum Erstellen einer Maske wird in Viewporten nicht angezeigt
&#x200B;* Schnelle Maske ist defekt
&#x200B;* Mischproblem auf altem Mac Pro beheben

### 0.10.0-beta

*(Freigegeben: 07. August 2014)*

**Hinzugefügt:**

&#x200B;* Schablonen

**Fest:**

&#x200B;* Unterstützung für Quadro-Karten
&#x200B;* Shader ergibt schwarzes Ergebnis bei geringer Rauheit
&#x200B;* Substance-Materialien sind auf 256 begrenzt
&#x200B;* Normalen-Map-Export löscht den grünen Kanal

### 0.9.0-beta

*(Freigegeben: 17. Juli 2014)*

**Hinzugefügt:**

&#x200B;* Yebis 2 Nachbearbeitung
&#x200B;* Mit dem Assistenten für neue Projekte können Sie Eingabe-Map (AO, Krümmung usw.)
&#x200B;* Eingabe-Map (AO, Krümmung usw.) automatisch anschließen auf Substance Effects
&#x200B;* Skalieren der Steuerung von Materialien, die auf Füllebenen angewendet werden

### 0.8.2-beta

*(Freigegeben: 11. Juli 2014)*

**Fest:**

&#x200B;* Farbton-Schieberegler ist standardmäßig Weiß
&#x200B;* Zurücksetzen des Projekts, wenn der Name des Materials Sonderzeichen enthält
&#x200B;* Die Änderung des Material-Namens für ein einzelnes Material-Objekt sollte das Projekt nicht ungültig machen.
&#x200B;* UVs sind nach dem Speichern des Projekts und dem erneuten Öffnen fehlerhaft

### 0.8.1-beta

*(Freigegeben: 04. Juli 2014)*

**Fest:**

&#x200B;* Mehrere GPU-Abstürze
&#x200B;* Absturz beim Exportieren von Kanälen

### 0.8.0-beta

*(Freigegeben: 28. Juni 2014)*

**Hinzugefügt:**

&#x200B;* Mehrere Materialien: Sie können jetzt auf mehrere Materialien im selben Dokument malen.
&#x200B;* Symmetrie-Malen
&#x200B;* Alle Füllmethoden sind jetzt verfügbar

**Fest:**

&#x200B;* Mehrere GPU-Abstürze
&#x200B;* Zurücksetzen des Projekts, wenn der Materialname Sonderzeichen enthält
&#x200B;* UVs werden nach dem Speichern des Projekts durcheinander gebracht und bei mehreren UVs erneut geöffnet

### 0.7.0-beta

*(Freigegeben: 18. Juni 2014)*

**Hinzugefügt:**

&#x200B;* Ebeneneffekte
&#x200B;* Neue Substance Schablone Material
&#x200B;* Maske bereinigen
&#x200B;* Kopieren/Einfügen von Ebenen/Masken zulassen
&#x200B;* Ebene duplizieren
&#x200B;* Werkzeug beim Bearbeiten der Ebenenmaske ändern
&#x200B;* Substance sind jetzt GPU-fähig

**Fest:**

&#x200B;* Beim Höhen-Map-Malen werden keine negativen Werte Malen.
&#x200B;* Das Material Picker-Display sollte die aufgenommene Normalen-Map nicht berücksichtigen.
&#x200B;* Partikeln Determinismus gebrochen
&#x200B;* Schablone in der 2D-Ansicht
&#x200B;* Ngons in obj-Dateien
&#x200B;* Verschiedene Abstürze

### 0.6.0-beta

*(Freigegeben: 4. Juni 2014)*

**Hinzugefügt:**

&#x200B;* Neue Exportoption zum Exportieren einer Specular-Map aus einer Komposition aus Rauheit und metallic Kanälen

**Fest:**

&#x200B;* Kompatibilität mit Windows Vista
&#x200B;* Höhen-Map Malen keine negativen Werte

### 0.5.0-beta

*(Freigegeben: 7. Mai 2014)*

**Hinzugefügt:**

&#x200B;* 3D-/2D-Ansicht-Schalter
&#x200B;* UV-Blockauswahlwerkzeug
&#x200B;* Beim Malen auf Masken ändert sich das Werkzeug automatisch.
&#x200B;* Die Auflösung der Substance hängt vom

**Fest:**

&#x200B;* Absturz beim Start
&#x200B;* Absturz mit ASCII-Meshs
&#x200B;* Matrix fester Schablonen in 2D-Ansichten
&#x200B;* Absturz mit Radiergummi

### 0.4.0-beta

*(Freigegeben: 17. April 2014)*

**Hinzugefügt:**

&#x200B;* Nahtlose 2D-Ansicht
&#x200B;* Bitmap-Ebenenmasken
&#x200B;* Umgebungsbelichtungssteuerung
&#x200B;* Füllebenen verwenden jetzt die Fenster &quot;Werkzeuge&quot;, um ihre Eigenschaften festzulegen.
&#x200B;* Material können auf Füllebenen angewendet werden
&#x200B;* Weitere Schablonen zur Bibliotheksbibliothek für Schablonen hinzugefügt
&#x200B;* Partikeln-Vorgaben für schnellere Berechnung aktualisiert
&#x200B;* PBR-Shader-Optimierung und Qualitätsverbesserung für niedrigere Qualitätseinstellungen

**Fest:**

&#x200B;* Ebenen-Miniaturansichten sind mit dem aktuell ausgewählten Kanal verknüpft
&#x200B;* Viele Absturz

### 0.3.0-beta

*(Freigegeben: 04. April 2014)*

**Hinzugefügt:**

&#x200B;* Negative Werte im Farbwähler für Höhen-Map-Malen zulassen
&#x200B;* Vorschau des ausgewählten Materials/der ausgewählten Farbe anzeigen
&#x200B;* Hinzufügen von Tastaturbefehlen für die Werkzeuge in der Werkzeugleiste (1,2,3,4)
&#x200B;* Globales Wechseln des Normalformats (OpenGL vs. DirectX) bei einem Projekt
&#x200B;* Assistent für neue Projekte
&#x200B;* Abstand-Schieberegler ist nicht mehr geklemmt
&#x200B;* Aktualisierter Reglerstil
&#x200B;* Farbwähler nicht modal machen
&#x200B;* Durch Auswahl eines Materials in der Bibliothek wird der Werkzeugtyp entsprechend festgelegt.

**Fest:**

&#x200B;* Fest: Der Importgitterpfad bleibt nicht erhalten
&#x200B;* Fest: Generierung von falschen Texturen
&#x200B;* Fest: Absturz beim Start

### 0.2.0-beta

*(Freigegeben: 17. März 2014)*

**Hinzugefügt:**

&#x200B;* Material-Pipette (P-Kurzbefehl)
&#x200B;* Miniaturen unter der 3D-Werkzeugvorschau
&#x200B;* Lizenzierungssystem für eigenständige Versionen
&#x200B;* [ und ] Tastaturbefehle für Pinselgröße
&#x200B;* Innenabstände exportierter Karten
&#x200B;* Aktualisierter Werkzeugfensterstil
&#x200B;* Aktualisierter Reglerstil
&#x200B;* Aktualisierte Standard-HDR-Umgebung

**Fest:**

&#x200B;* Schablone: Ändern des Flusswerts in den Anschlägen der 3D-Ansicht bei 52
&#x200B;* Unendliche Schleife im Motor, wenn 0-Druck-Tasten zum Hub hinzugefügt werden, ist fest
&#x200B;* Tool: Winkeljitter gibt keine Werte über +/- 90 % zurück.
&#x200B;* Die Anzeige der 3D-Ansicht ändert sich, wenn eine Ebenenmaske ausgewählt ist
&#x200B;* Invertierter Zoom

### 0.1.0-beta

*(Freigegeben: 02. März 2014)*

**Hinzugefügt:**

&#x200B;* Neue Bibliotheksverwaltung
&#x200B;* Neue Pinsel und Partikeln
&#x200B;* 3D-Pinselvorschau
&#x200B;* Aktualisierter Werkzeugfensterstil
&#x200B;* Aktualisierter Reglerstil
&#x200B;* Aktualisierte Cache-Leistung

**Fest:**

&#x200B;* Kamera
&#x200B;* Pinseldrehung
