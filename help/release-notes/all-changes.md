---
breadcrumb-title: ''
description: Prüfe alle Änderungen und Updates in den verschiedenen Substance 3D Painter-Versionen, um den Funktionsverlauf und Verbesserungen im Laufe der Zeit nachzuverfolgen.
title: Alle Änderungen
user-guide-description: ''
user-guide-title: ''
hold: false
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '34065'
ht-degree: 0%
---

# Alle Änderungen

Diese Seite enthält Versionshinweise für alle früheren Versionen von Substance 3D Painter, sortiert nach aktuellster bis ältester Version.

>[!NOTE]
>
> Informationen zum Anzeigen bekannter Probleme, die sich auf Painter auswirken können, finden Sie auf der [Seite zur dedizierten Dokumentation](known-issues.md).

## Version 12

### 12.1.5

Freigabedatum: **2026/09/15**

Zusammenfassung: **Nebenversion**

**Fest:**

* Das Exportieren eines Bildes aus einem Regal in ein Netzwerk funktioniert nicht mehr
* [Generator] Die Einstellung &quot;Textur verwenden&quot; auf &quot;false&quot; deaktiviert nicht die Verwendung der Textur-Eingabe.
* Einfrieren des Viewports beim Speichern während der Bearbeitung der 3D-Projektion
* Material-Ebenenauflösung ist zu niedrig

### 12.1.4

Freigabedatum: **2026/09/04**

Zusammenfassung: **Nebenversion**

**Fest:**

* \[Absturz\] Absturz beim Importieren oder Exportieren von Dateien, deren Dateinamen Nicht-ASCII-Zeichen enthalten

### 12.1.3

Freigabedatum: **2026/08/26**

Zusammenfassung: **Nebenversion**

**Hinzugefügt:**

* Substance Engine auf Version 9.4.6 aktualisieren

**Fest:**

* [Graustufenwähler] Die Auswahl bleibt nach dem Ändern des Tools geöffnet
* [Baking verzerren] Verzerrungskorrektur wird beim Malen und Rückgängigmachen unterbrochen
* Die Interaktion mit dem [Projektion-Tool]-Viewport wird vom Projektion-Tool blockiert.
* [Dynamische Kontur] Fehlende dynamische Konturparameter in den Pinseleigenschaften
* Export in ein Netzwerk funktioniert nicht mehr

### 12.1.2

Freigabedatum: **2026/08/03**

Zusammenfassung: **Nebenversion**

**Fest:**

* \[Absturz\] Einige Substance können beim Rendern zu einem Absturz führen
* \[Absturz\] Mesh beim Baking erneut importieren
* \[Absturz\] Fehler bei der Initialisierung der Grafikanzeige kann zu einem Absturz führen.
* \[Absturz\] Beim Exportieren von Texturen kann in einigen Fällen ein Absturz beim Aktualisieren des Protokolls auftreten.
* \[Absturz\] Absturz im Baking-Modus in einigen Fällen beim Laden/Aktualisieren der Umgebungs-Map
* \[Baking\] Das erneute Starten des Baking nach dem Ändern einer Datei mit hohem Poly-Wert kann zu einem Einfrieren führen
* \[An Photoshop senden\] Fehler beim Exportieren der Ebenenmaske
* \[Engine\] Das Ergebnis des Ankerpunkts wird nicht zwischen einer Maske und einem Farbkanal gerendert

### 12.1.1

Freigabedatum: <b>2026/07/09</b>

Zusammenfassung: Nebenversion

Hinzugefügt:

* [Skew-Baking] Gelegt: Normaler Neigungsbasismodus: Mesh oder pro Dreieck
* [Eigenschaften] einheitliche Farben immer auf den Standardwert ihres Kanals zurücksetzen lassen
* [OpenPBR] Kanäle nach Kategorien im Fenster &quot;Texturen exportieren&quot; für die Erstellung von Ausgabevorlagen neu gruppieren
* Substance Engine auf Version 9.4.5 aktualisieren

Fest:

* [Projekt] Das Öffnen und Speichern einiger Projekte kann länger als gewöhnlich dauern
* [Absturz] Erneutes Laden mehrerer Mesh kann zu einem Absturz führen
* [Absturz] Löschen eines Kanals im Maskenansichtsmodus führt zu einem Absturz
* [Absturz] Einige Substance können beim Rendern zu einem Absturz führen
* [Malen Skew] Das ausgewählte Tool in Malen Skew bleibt nach dem Wechsel in den Malmodus ausgewählt.
* [Allgemeine Einstellungen Baking geführt] Käfig-Entfernungseinstellungen aktualisieren die Drahtgitter- und Shader-Visualisierung des Käfigs nicht
* [Engine] UV-Auffüllmodus &quot;3D Space Neighbor&quot; funktioniert nicht gut bei dünnen Dreiecken
* Das Ergebnis des [Engine]-Ankerpunkts wird nicht zwischen einer Maske und einem Farbkanal gerendert

### 12.1.0

Freigabedatum: <b>2026/06/23</b>

Zusammenfassung: <b>Dieses Update ist eine Hauptversion. Es enthält Verbesserungen an Bakern mit dem Standardzustand &quot;Neues Baking&quot;, der Zeichnungs-Skew-Map, dem automatischen Reake, einer neuen Option für den automatischen entpack von UV für Mesh und OpenPBR mit fester Oberfläche. Weitere Informationen finden Sie in den vollständigen Versionshinweisen.</b>

<b>Hinzugefügt</b>:

* [Baking Neigen] Malwerkzeuge Neigen
* [Skew-Baking] Hinzufügen von Skew-Vorschau-Shader und Skew-Richtung Vektorgrafiken beim Malen von Skew-Maps
* [Baking verzerren] Option &quot;Kantenschutz hinzufügen&quot;
* [Baking neigen] Automatische Wiederherstellung
* [Skew-Baking] Benutzeroberfläche der Mesh-Map-Liste überarbeiten
* [Baking verzerren] Mesh-Map teilen / Allgemeine Baking-Einstellungen + Allgemeine Einstellungen aus Mesh-Map-Liste verschieben (nur Grundfarbe oder Maske)
* [Baking verzerren] Symbolleistenschaltflächen für Viewport ändern
* [Baking verzerren] Symmetrie für Pinsel in der oberen Symbolleiste anzeigen
* [Skew-Baking] Umbenennungsoptionen im Menü &quot;Synchronisierung der Mesh-Map-Liste&quot;
* [Skew-Baking] Dialogfelder &quot;Synchronisation aktualisieren&quot; und &quot;Überwachter Status&quot;
* [Skew-Baking] Erstellen einer Graustufen-Farbwählervariante
* [Baking verzerren] Symbol &quot;Baking-Modus aktualisieren&quot;
* [Automatisch Entpackt] Option zum Integrieren von Festplatten
* [OpenPBR] Unterstützung für OpenPBR 1.1 hinzufügen
* [OpenPBR] OpenPBR zum Standardarbeitsablauf und -Shader machen
* [OpenPBR] Importieren von OpenPBR-Materials und -Texturen über USD
* [OpenPBR] Exportieren von OpenPBR-Materials und -Texturen über USD
* [OpenPBR] Fenster &quot;Export-Texturen aktualisieren&quot;, um die Namenskonvention für OpenPBR anzuzeigen
* [OpenPBR] Hinzufügen von Dokumentationen zu Änderungen an der Support-OpenPBR
* [OpenPBR][Iray] Fügen Sie eine neue MDL hinzu, um OpenPBR 1.1 in Iray zu unterstützen.
* Mehrere geringfügige Verbesserungen bei USD Exporten
* [UI] Hinzufügen einer Warnung im Viewport beim Malen auf einem anderen Textursatz
* [Reduzieren] Reduzieren aller instanzierten Ebenen über Textursatz hinweg zulassen
* [Kanaleinstellungen] Mehrere Textursätze gleichzeitig über ein neues Fenster auswählen
* [Verlauf] &quot;Wert&quot; aktualisieren Eintragsformulierung rückgängig machen, um den Parameternamen wiederzugeben
* [Ebenenstapel] Fülleffekte in Masken standardmäßig auf Weiß einstellen (1.0)
* [Substance] Neue Engine-Map-Eingabe &quot;Mesh_hard_edges_triangle&quot; hinzufügen
* [Substance] Neue Engine-Map-Eingabe &quot;Mesh_harte_Kanten&quot; hinzufügen
* [Shader] Verhindern von Shader-Instanzen, dieselben Namen zu verwenden
* [Shader] Verwenden Sie den Shader aus der Projektvorlage beim Importieren einer USD- oder GLTF-Datei.
* Adobe Color Engine auf Version 7.0 aktualisieren
* Aktualisieren der MacOSX-Mindestversion auf 13.0 (Ventura)
* [Inhalt] Neue Projektvorlagen für OpenPBR
* [Inhalt] Aktualisieren von Beispielprojekten, um den neuen OpenPBR Shader zu verwenden
* [Python] Erweitern Sie die Geometrie-Masken-API, um Einschluss- und Ausschlussmodi wie in der Benutzeroberfläche zu ermöglichen.

<b>Fest</b>:

* [Absturz][Mesh-Map-Einstellungen] Einstellungen auf andere Textursatz anwenden
* [Absturz] Beim Baking führ von Krümmungen von einer Karte ohne Welt-Raum-Normale
* [Absturz][Baking] Baking mit aktiviertem benutzerdefiniertem Käfig, aber ohne Dateiauswahl-Absturz
* [Absturz] AO-Baking wird abgebrochen
* [Auto-Käfig] Unendliche Ladezeit, wenn der hohe Poly-Dateipfad ungültig ist
* [Linux][Windows] Der Farbwähler kann manchmal ganz schwarz sein oder nicht angezeigt werden.
* [Polygon-Füllwerkzeug] Das Werkzeug funktioniert nicht mit Nicht-PBR
* [[Malen] Beim Löschen des Farbkanals werden zuvor gemalte Grundfarben nicht gelöscht
* [USD] Nicht alle Shader-Instanzen werden korrekt erkannt.
* [Substance] Es wird nur die erste Verwendung eines Eingabe-/Ausgabeknotens berücksichtigt
* [Shader] Ambient occlusion wird zweimal mit Textursätzen unter Verwendung verschiedener Mischmethoden aufgetragen
* [Engine] Normale Texturen mit leerem Blaukanal (Schwarz) können zu falschen Angleichungsergebnissen führen
* [GLTF Import] Alpha-Überblendung ist auf jedem Textursatz aktiviert
* [GLTF-Export] Alpha-Überblendung ist beim Export immer aktiviert
* [Export] Doppelseitige Geometrie ist beim Importieren einer GLTF-Datei immer deaktiviert
* [Javascript] Das Ändern von Shader-Einstellungen trägt nicht zum Rückgängigmachen des Verlaufs bei
* [Beispiele] Volumenstreuung ist in den Anzeigeeinstellungen für die Meetingmatte nicht aktiviert.

### 12.0.3

Freigabedatum: **2026/05/05**

Zusammenfassung: **Nebenversion**

**Hinzugefügt:**

* Baker auf Version 3.22.2 aktualisieren
* Substance Engine auf Version 9.4.3 aktualisieren
* \[Python\] Speichern Sie ein intelligente Material an einem bestimmten Speicherort

**Fest:**

* \[Ubuntu\] Absturz beim Auswählen des Materials
* \[Mac\] Wiederkehrendes Popupfenster fordert den Zugriff auf Daten anderer Anwendungen an
* \[Baking\] Artefakte können auf dem Krümmungs-Map angezeigt werden
* \[Baking\] Das Baking ist in einigen Fällen langsamer
* \[Verformen zu Geometrie\] Verformen zu Geometrie wird in einigen Fällen deaktiviert
* \[UV-Kachel\] Alpha des extrahierten Ankerpunkts wird von anderen Kacheln ignoriert
* \[Python\]\[Mac\] Ausnahmen in der Python-Konsole mit SSL
* \[Python\] Painter-Absturz beim Beenden mit verbleibenden Qt-Widgets

### 12.0.2

Freigabedatum: **2026/04/07**

Zusammenfassung: **Nebenversion**

**Hinzugefügt:**

* [Farbmanagement] Fügen Sie neue OCIO hinzu, um den Standardfarbraum des Farbwählers anzugeben
* [Python] Automatisch entpackt Einstellungen in der Python-API Gelegt

**Fest:**

* [Absturz] Das Speichern mit nicht genügend Speicherplatz kann zu Abstürzen oder beschädigten Projekten führen
* [Absturz] [Menüband] Verwenden des Menübands kann bei einigen Projekten zu Abstürzen führen
* [Absturz] [Baking] Absturz, wenn die .assbin-Datei nicht in den Ordner geschrieben werden kann
* [Importieren] OBJ Meshs aus Stager können bei der Projekterstellung fehlschlagen
* [Importieren] OBJ fehlt in einigen Fällen die Fläche.
* [Importieren] USD Mesh ohne zugewiesenes Material kann beim Importieren Absturz hinzufügen.
* [Ausgefüllter Pfad] Nicht von der Symmetrie betroffen
* [Schablone] Die Vorschau hat eine geringere Auflösung als das gemalte Ergebnis
* [UI] &quot;UV Island&quot; wird weiterhin in der QuickInfo für ID-Map-Farbquellen erwähnt
* [Anzeige] Schatten erscheinen invertiert
* [Viewport] transformieren Warp-Projektion bleibt nach dem Wechsel in den Baking-Modus erhalten
* [Verformen] Raster verschwindet, wenn die Skalierung auf der Z-Achse auf 0 gesetzt ist und &quot;Verformen auf Geometrie&quot; aktiviert ist
* [Python] Unerwarteter Fehler beim Hinzufügen eines Kanals mit umfangreichen Änderungen

### 12.0.1

Freigabedatum: **2026/03/18**

Zusammenfassung: **Nebenversion**

**Fest:**

* \[Absturz\]\[Fixieren\] Exportieren aus bestimmten Projekten

### 12.0.0

Freigabedatum: <b>2026/03/09</b>
Zusammenfassung: <b>Dies ist eine Hauptversion. Diese Version enthält die Funktionen zum Reduzieren von Ebenen, Verformen der Geometrie, neue Post-Effekte, Verbesserung des neuen Projektfensters und weitere Verbesserungen.</b>

<b>Hinzugefügt</b>:

* [Ebenen reduzieren] Ebenen innerhalb des Ebenenstapels reduzieren
* [Ebenen reduzieren] Exportieren reduzierter Ebenen auf die Festplatte
* [Verformen zu Geometrie] Hinzufügen neuer Funktionen für die automatische Verkrümmung zu den Verkrümmen-Projektionen
* [Post-Effects] Ersetzen Sie Post-Effekte durch neue
* [Post-Effects] Aktualisieren der Tonzuordnung
* [Post-Effects] Neue Verwendung für Post-Effects-Assets hinzufügen
* [Inhalt][Nacheffekte] Integrieren von Standard-Nacheffekt-Assets in die Bibliothek
* [Neues Projekt] Verbessern der Benutzeroberfläche für die Projekterstellung
* [Neues Projekt] Änderungen an der Funktion zum erneuten Importieren von Meshs
* [Neues Projekt] Öffnen von \*.geo.usd-Dateien zulassen
* [Projektkonfiguration] Verbessern der Benutzeroberfläche für die Projektkonfiguration
* USD auf Version 25.05 aktualisieren
* Substance Engine auf Version 9.3.4 aktualisieren
* Erhöhen der Mindesttreiber auf 25.3.1/25.Q2 für AMD-GPUs
* Update Qt auf 6.8.6
* [Scripting] JavaScript-API auf Version 1.1.20 aktualisieren
* Aktualisieren von Python auf 3.13

<b>Fest:</b>

* [Absturz] Ändern der Ausgabe eines Material-Kanals in einer Maske kann Absturz verursachen
* [Importieren] EXR Texturen werden beim Importieren von USD in sRGB anstelle von linear erzwungen
* [UV-Kacheln] Bildsequenz mit einem einzigen Bild füllt auch andere UV-Kacheln
* [Baking] AO unterscheidet sich zwischen CPU- und GPU-Baking
* [Farbmanagement][MacOS] Viewport BaseColor stimmt nicht mit dem Farbwähler überein
* [USD] Einheitliche Werte werden in einigen Fällen nicht importiert.

## Version 11

### 11.1.3

Freigabedatum: <b>2026/02/12</b>
Zusammenfassung: <b>Nebenversion</b>

<b>Fest</b>:

* [Malen] Schablone und Symmetrie funktionieren in einigen Fällen nicht
* [Pfad] Keine Aktualisierung beim Ändern des Deckkraftreglers für Verwischungsstrich
* [Projekt] Malen auf einer bestimmten Geometrie nicht möglich
* [Menüband] Instanziieren Pfad verschwindet, wenn die Auflösung des Textursatzes geändert wird
* [UI] Farbwähler kann in einigen Fällen schrumpfen und verschwinden

### 11.1.2

Freigabedatum: <b>2026/01/13</b>
Zusammenfassung: <b>Nebenversion</b>

<b>Hinzugefügt</b>:

* [Baking] Verbessern der Baking-Zeit für UV-Kacheln-Projekt mit asynchronem Speichern
* [Shaders] Erwähnung in Shader-API Changelog ändert sich nach Vulkan migration
* Update OpenEXR auf Version 3.4.4

<b>Fest</b>:

* [Absturz] Absturz beim Starten von Nvidia GTX 10xx
* [Absturz] Die Verwendung des Farbwählers auf verschiedenen Textursätzen kann beim Beenden der Anwendung zu einem Absturz führen
* [Leistung] Leistungsproblem beim Malen im Projekt mit vielen Ebenen
* [Leistung] Verzögerung beim Malen mit Grafiktablett-Stift
* [UI] Kamera-Einstellungen bleiben im Rendermodus deaktiviert (Iray)
* [Menüband] Pfad kann sich in einigen Fällen nach einer Ecke unerwartet überlappen
* [Menüband] Leistungsproblem mit UV-Kacheln
* [Substance][UI] Bildeingaben verschwinden, wenn sie ausgeblendet werden
* [Substance][UI] Verschachtelte Gruppen können auch dann erhalten bleiben, wenn &quot;Sichtbar&quot; sie ausblendet.
* [Baking][UI] Der Krümmungen-Sampling-Radius kann nicht über 0,01 hinaus festgelegt werden.
* [Baking][UI] Max. Verdeckungsabstand kann nicht auf mehr als 1 festgelegt werden
* [Baking] AO-Einstellung &quot;Selbstverdeckung&quot; wird bei mehreren Textursätzen ignoriert und Niedrig als Hoch-Baking
* [Baking] ID-Map Baking führe keine Textfarben aus FBX im Modus &quot;Niedrig bis Hoch&quot;
* [Inhalt] Hochpassfilter führt zu ausgewaschenen Farben in farbverwalteten Kanälen

### 11.1.1

Freigabedatum: <b>2025/12/09</b>
Zusammenfassung: <b>Nebenversion</b>

<b>Hinzugefügt</b>:

* [Performance] Verbessern der UV-Kachel-Performance bei der Berechnung partieller Texturen
* [Baker] Update auf Version 3.15.4

<b>Fest</b>:

* [Absturz][MacOS] Speichern eines Projekts aus einer früheren Version immer Absturz
* [Absturz] Das Schließen eines Projekts kann zu einem Absturz führen.
* [Project] Fehler &quot;Die Mitgliederanzahl stimmt nicht überein&quot; beim Öffnen des in der vorherigen Version erstellten Projekts.
* [Baking] UV-Kacheln werden nicht mit vorherigen Baking-Ergebnissen kombiniert, sofern vorhanden.
* [Baking] Gerät verloren, auch wenn Raytracing auf Nvidia GTX 10XX deaktiviert ist
* [Baking] AO mit Normal weist an Kanten Artefakte auf, da keine Auffüllung erfolgt.
* [Baking] AO-Einstellung &quot;Selbstverdeckung&quot; wird mit mehreren Textursätzen ignoriert und &quot;Namensübereinstimmung&quot; auf
* [Baking] ID-Map ist vollständig schwarz, wenn hochpolare Mesh keine Scheitelpunkt-Farben aufweisen
* [Menüband] QuickInfo für den Modus &quot;Alpha-Überblendung&quot; erwähnt den Modus &quot;Bildschirmüberblendung&quot; anstelle von &quot;Linear abwedeln&quot;
* [Pfad] Tangenten erzeugen eine unerwartete Schleife, wenn der Punkt nahe an das Pfadende verschoben wird
* [Tool] Die Maskenvorschau funktioniert nicht, wenn die Projektion in einer Material verwendet wird
* [Engine] Das Malen kleiner Striche kann zu blockartigen Artefakten führen
* [Shader] Beim Rückgängigmachen der Erstellung von Shader-Instanzen wird diese nicht ordnungsgemäß entfernt.
* [Exportieren] Der Alpha-Modus für den GLTF-Export ist immer auf MASK festgelegt.
* [Python] Unerwarteter Fehler beim Bearbeiten von Ebenenstapel außerhalb des umfangreichen Änderungsblocks

<b>Bekannte Probleme</b>:

* [Menüband] Leistungsproblem mit UV-Kacheln
* [Menüband] Pfad kann sich in einigen Fällen nach einer Ecke unerwartet überlappen
* [Absturz][Menüband] Erstellen sehr langer Texte in Menüband kann Absturz verursachen
* [Farbmanagement] HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen festgeklemmte Farben
* [Regression][UI] Kontextmenü auf HD-Bildschirmen ist zu klein
* [Absturz][Python] USD durch TextureStateEvent ausgelöst
* [Engine] Malen mit dem Klon-Werkzeug in normalen Kanalverschiebungsfarben falsch
* [Python] Phantom-Widget wird angezeigt, weil das Skript noch funktioniert

### 11.1.0

Freigabedatum: <b>2025/11/18</b>
Zusammenfassung: <b>Dieses Update ist eine Hauptversion. Es enthält das neue Tool für die Multifunktionsleiste mit eigenem neuen Inhalt, Unterstützung der Symmetrie für Füllebenen, Leistungsparameter für Versatz, verbesserte Physische Größe durch die aktualisierten Baker, vollständige Vulkan-Unterstützung für Windows und Linux und weitere Verbesserungen.</b>

<b>Hinzugefügt</b>:

* Neues Bandwerkzeug
* [Tool] Neues Werkzeug für die Multifunktionsleiste hinzufügen, um nahtlose Pfade zu erstellen
* [Menüband] Tastenkombinationen für die Menübandvorgabe im Eigenschaftenfenster hinzufügen
* [Menüband] Ermöglicht das Ändern der Deckkraft des Menübands pro Scheitelpunkt auf dem Pfad.
* [Menüband] Ermöglicht das Ändern der Größe des Menübands pro Scheitelpunkt auf dem Pfad.
* [Menüband] Entfernen von Anfang/Ende, definiert auf einer Substance, wenn Pfade geschlossen sind
* [Menüband] Entfernen der Pfad-/Material-Vorschau im Eigenschaftenfenster für Malen-/Radiergummi-/Verwischen-Pfadwerkzeuge
* [Menüband] Hinzufügen von Füllmethoden für Alpha und einige Kanäle bei selbstüberlappender Anordnung
* Symmetrie füllen
* [Füllen] Unterstützung für Symmetrie zu Füllebenen und Effekten hinzufügen
* [Fill][UI] Einstellungen für die Symmetrie im Eigenschaftenfenster für Füllebene und Effekte Gelegt
* [Fill] Benutzeroberfläche für Einstellungen für &quot;Symmetrie nachbearbeiten&quot; im Menü &quot;Viewport&quot; und im Eigenschaftenfenster
* [Füllen] Ordentlich Neuausrichtung normaler Texturen bei Projektion im Verkrümmungsmodus
* Physische Größe Versatz
* [Versatz] Physische Größe als Versatz verwenden
* Leistungssteigerung
* [Leistung] Verbessern der Darstellung kleiner Pinselstriche auf großen Dreiecken
* [Performance] Verbessern der Shader-Kompilierungszeit
* [Performance] Volle Vulkan-Unterstützung für Windows und Linux
* [Leistung] Aktualisierte Baker mit schnellerem GPU-Rendering und Unterstützung von AMD-Raytracing
* [UI] Ordnen Sie Werkzeugeigenschaften neu in Gruppen an und reduzieren Sie einige standardmäßig
* [Engine] Update Substance Engine auf Version 9.2.5
* [Substance] Außerkraftsetzung der Auflösung für Substance-Ressourcen in Tools und Füllungen Gelegt
* [Exportieren] Mesh-Map-Exportvoreinstellung aktualisieren, um Graustufen-Texturen zu exportieren
* Python
* [Baking][Python] Anzeige in Änderungsprotokoll, das Änderungen nach Aktualisierung der Baker umbricht
* [Python] Leg der Einstellungen für die Symmetrie der Füllung in Python
* Content und neue Inhalte.
* [Inhalt] Hinzufügen von 75 neuen Werkzeugvorgaben für das Menüband-Werkzeug
* [Inhalt] Aktualisieren der Verlaufsgenerator-Ressource, um mit dem Menüband kompatibel zu sein

<b>Fest</b>:

* [Absturz] Laden eines anderen Projekts bei aktiviertem einrasten des Pfads kann Absturz werden
* [Absturz] Rechtsklick im Bedienfeld &quot;Pfad&quot; mit Informationen aus einer anderen Sitzung in der Zwischenablage kann Absturz
* [UI] Die Benutzeroberfläche scrollt in den Werkzeugeigenschaften nach oben, wenn ein Pfad erstellt wird
* [UI] Maus-Cursor verschwindet, wenn die Pfadtext-Visualisierung ausgeblendet ist
* [Pfad] Das Kopieren/Einfügen verschiedener Werkzeugeigenschaften im Bedienfeld &quot;Pfad&quot; führt zu instabilen Eigenschaften
* [Tool] Radiergummi- und Verwischen-Werkzeugvorgaben aktualisieren nicht immer die Kanalauswahl
* [Tool] Der gemalte Wert ist grau, aber die Benutzeroberfläche zeigt Weiß an, nachdem farbige Werkzeugvorgabe in die Maske geladen wurde
* [Tool] Die aus der Maske erstellte Voreinstellung behält Kanalwerte bei, die aus einer anderen Voreinstellung geladen wurden
* [Substance] Die in Graf definierte normale Farbraumübersteuerung wird nicht berücksichtigt
* [Inhalt] Die Standard-Pinselformressource verwendet eine veraltete Substance.

<b>Bekannte Probleme</b>:

* Shader-Instanz-Verlauf wird nicht richtig verfolgt
* [Menüband] Leistungsproblem mit UV-Kacheln
* [Menüband] Pfad kann sich in einigen Fällen nach einer Ecke unerwartet überlappen
* [Menüband] Tangenten erzeugen eine unerwünschte Schleife, wenn der Punkt nahe an die Pfadenden verschoben wird
* [Absturz][Menüband] Erstellen sehr langer Texte in Menüband kann Absturz verursachen
* [Tool] Die Maskenvorschau funktioniert nicht, wenn die Projektion in einer Material verwendet wird
* [Baking] AO-Einstellung &quot;Selbstverdeckung&quot; wird bei mehreren Textursätzen ignoriert und &quot;Namensübereinstimmung&quot; aktiviert
* [Baking] AO mit Normal weist an Kanten Artefakte auf, da die Auffüllung fehlt
* [Farbmanagement] HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen festgeklemmte Farben
* [Regression][UI] Kontextmenü auf HD-Bildschirmen ist zu klein
* [Absturz][Python] USD durch TextureStateEvent ausgelöst
* [Engine] Malen mit dem Klon-Werkzeug in normalen Kanalverschiebungsfarben falsch
* [Python] Phantom-Widget wird angezeigt, weil das Skript noch funktioniert

### 11.0.3

Freigabedatum: <b>2025/08/05</b>
Zusammenfassung: <b>Nebenversion</b>

<b>Hinzugefügt</b>:

* [Substance 3D Assets] Hinzufügen eines Benachrichtigungspunkts zum Bedienfeld &quot;3D-Elemente&quot;
* [VFX Platform 2025] Hinzufügen der ACE 2.0-Konfiguration in den Farbmanagementeinstellungen
* [VFX Platform 2025] Update OCIO Version 2.4.2
* Iray auf Version 2024.10 aktualisieren
* [Engine] Update auf Substance Engine v.9.2.3
* [Nvidia] Erhöhung der Nvidia-Mindesttreiberversion auf 572.60 (Win) und 570.169 (Linux)

<b>Fest</b>:

* [Python] Bereichsänderung wird nicht im Verlaufsfenster angezeigt

<b>Bekannte Probleme</b>:

* [Farbmanagement] HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen festgeklemmte Farben
* [Regression][UI] Kontextmenü auf HD-Bildschirmen ist zu klein
* [Absturz][Python] USD durch TextureStateEvent ausgelöst
* [Engine] Malen mit dem Klon-Werkzeug in normalen Kanalverschiebungsfarben falsch
* [Python] Phantom-Widget wird angezeigt, weil das Skript noch funktioniert

### 11.0.2

Freigabedatum: <b>2025/06/10</b>
Zusammenfassung: <b>Nebenversion</b>

<b>Hinzugefügt</b>:

* [Mac] Fügen Sie Warnungen zu bestimmten Betriebssystemversionen hinzu, die zu Artefakten führen
* [Automatische Aktualisierung] Kleine UX-Verbesserungen im Fehlerprotokoll &quot;Assets&quot;
* [Automatisches Entpacken] Update auf Version 1.3.2 mit Seaming-Verbesserungen
* [USD][FBX] Unterstützung für mehrere UV-Satz mit wenigen Daten hinzufügen
* [Exportieren] Meshs, die als FBX exportiert wurden, fehlen ihre zusätzlichen UV-Satz, wenn beim Import vorhanden waren

<b>Fest</b>:

* [MacOS][Linux] Absturz beim Speichern auf dem Netzwerklaufwerk
* [Win][Tablet] Flackern beim Schwenken
* [SpaceMouse] Problem bei der Arbeit mit dem Pfadwerkzeug
* [Auto-Käfig] Kann nach einem erneuten Laden des Meshs nicht Baking geführt werden
* [Automatische Aktualisierung] Bildsequenz wird nicht neu geladen, wenn die erste Kachel fehlt
* [Path] Benutzerdefinierte Tangente kann sich auf andere Tangenten auswirken.
* [Pfad] Pfad wird nicht auf dem Textursatz angezeigt, wenn sich der erste Punkt auf einem anderen Textursatz befindet
* [UI] Einige Menüs sind nach dem Öffnen eines Projekts immer deaktiviert (z. B.: Symmetrie)
* [Eigenschaften] Werkzeugvorgaben mit ausgefülltem Pfadwerkzeug können nicht verwendet/geladen werden
* [USD] Mehrere UV-Satz werden bei Verwendung von USD nicht im benutzerdefinierten Shader erkannt.
* [USD] Kameras mit den gleichen Namen werden überschrieben.
* [Exportieren] &quot;An Photoshop senden&quot; führt zu einem falschen Farbraum für Farb- und Graustufenergebnisse
* [Exportieren] Graustufen-Kanäle mit Alpha werden als Farbe anstatt als Graustufen mit PNG-Format exportiert
* [Exportieren] Exportieren des Graustufenkanals als PSD führt zu einer ungültigen/verkürzten Datei
* [Inhalt] Verkrümmungsfilter im Mehrrichtungsmodus funktioniert nicht
* [Python] Beim Crawlen von Ebenenstapel-Knoten kann kein Listenfehler zugewiesen werden

<b>Bekannte Probleme</b>:

* [Farbmanagement] HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen festgeklemmte Farben
* [Regression][UI] Kontextmenü auf HD-Bildschirmen ist zu klein
* [Absturz][Python] USD durch TextureStateEvent ausgelöst
* [Engine] Malen mit dem Klon-Werkzeug in normalen Kanalverschiebungsfarben falsch
* [Python] Phantom-Widget wird angezeigt, weil das Skript noch funktioniert

### 11.0.1

Freigabedatum: <b>2025/04/10</b>
Zusammenfassung: <b>Nebenversion</b>

Hinweis: <b>Die Linux CCD-Version wird auf den 29. April verschoben.</b>

<b>Hinzugefügt:</b>

* Update auf Qt 6.5.8
* [Substance] Fügen Sie eine Protokollmeldung für Filter hinzu, wenn mehrere Bildeingaben dieselbe Verwendung haben.
* [Nvidia] Warnung über die neuesten Nvidia-Treiber hinzufügen (572.47)

<b>Fest:</b>

* [Absturz] Wenn Sie einen Balken mit einer Verwendung in einem Ein Kanal-Steckplatz ziehen und ablegen
* [Absturz][Pfad] Die Option &quot;Pfadtyp ändern&quot; ist nicht ausgegraut, wenn Sie nicht auf einen bestimmten Pfad klicken.
* [Füllpfad] Sollte nicht in der Lage sein, Substance-Material auszuwählen
* [Engine] Artefakte an Pinselstrichen
* [Engine] Pfade können mit bestimmten Einstellungen unterbrochen werden.
* Problem mit der Dropdown-Liste für den Pipetten-Farbraum
* [Automatische Aktualisierung] [Python] Falsche Fehlermeldung bei Verwendung von ResourceID ohne Version
* [Shader] Absturz beim Öffnen einiger Projekte

<b>Bekannte Probleme:</b>

* [SpaceMouse] Problem bei der Arbeit mit dem Pfadwerkzeug
* [Farbmanagement] HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen festgeklemmte Farben
* [Regression][UI] Kontextmenü auf HD-Bildschirmen ist zu klein
* [Absturz][Python] USD durch TextureStateEvent ausgelöst
* [Engine] Malen mit dem Klon-Werkzeug in normalen Kanalverschiebungsfarben falsch
* [Python] Phantom-Widget wird angezeigt, weil das Skript noch funktioniert

### 11.0.0

Freigabedatum: <b>2025/03/11</b>
Zusammenfassung: <b>Hauptversion, neue Funktion zur automatischen Aktualisierung, Tool für gefüllte Pfade und andere Pfadverbesserungen sowie neue Filter und eine experimentelle Generierung automatischer Käfige für das Baking</b>

<b>Hinzugefügt</b>:

* Automatische Aktualisierung
* [Automatische Aktualisierung] Automatische Aktualisierung geänderter Elemente im Bedienfeld &quot;Elemente&quot;
* [Automatische Aktualisierung] Automatische Aktualisierung geänderter Elemente im gesamten Projekt
* [Automatische Aktualisierung] Automatische Aktualisierung standardmäßig deaktiviert lassen
* [Automatische Aktualisierung] Optionale Aktualisierung, wenn die Ressourcenparameter nicht übereinstimmen (.sbsar, .glsl, .ai, .svg)
* [Automatische Aktualisierung] Umgebungsvariable hinzufügen, um die automatische Aktualisierung zu deaktivieren
* [Automatische Aktualisierung][SBSAR] Optionale Aktualisierung, wenn die Ressourcenparameter nicht übereinstimmen
* Ausgefüllter Pfad
* [Pfad][Füllen] Fügen Sie ein neues Werkzeug hinzu, um gefüllte Pfade zu erstellen.
* Verbesserungen an Pfaden
* [Pfad] Erstellen eines Pfads, der zu Polygonen einrasten
* [Pfad] Wechsel der Pfadtypen zulassen
* [Pfad] Kopieren und Einfügen von Pfadmaskendaten zwischen Scheitelpunkt und Maske zulassen
* [Pfad] Winkel beim Erstellen eines neuen Punkts einschränken
* [Path] Erlaubt das Beschränken der Punkterstellung auf eine Linie.
* [Pfad] Form mit einem Klick schließen
* [Pfad] Anzeigen von Pfadinformationen
* [Pfad] Skalieren und Drehen von Pfad-Scheitelpunkten zulassen
* [Pfad][UX] Einfacherer Zugriff auf Transformations-Gizmos
* [Pfad] Pfadvorschau hinzufügen
* [Pfad] Deaktivieren der Pfadvorschau mit Umschalt + P
* [Path] Verbessern der Tangente Edition von der Seitenansicht
* [Pfad] Fokus auf einen 3D-Pfad festlegen.
* [Pfad] Scheitelpunkt sollten den Auswahlstatus beibehalten, wenn Sie die Benutzeroberfläche aus- und wieder einschalten.
* [Path] Löschen von Pfaden mit Rücktaste zulassen
* [Pfad] Die Pfadliste offen halten, wenn der Benutzer sie erweitert
* [Pfad][Ebenenstapel] Duplikate beim Kopieren/Einfügen richtig umbenennen
* Verbesserungen an der Benutzeroberfläche und der QuickInfo [Path]
* Leistung
* [Performance] Verbessern der Viewport-Performance bei Verwendung einer hohen Tessellation
* [Performance] Nur den ersten Kanal für neue Füllebenen/Effekte aktivieren
* [Leistung] Berechnung des Pinselstrichs parallelisieren
* Baking
* [Baking] Neue vollautomatische Käfig-Generierungsoption für das Baking mit hochpolaren Meshs hinzufügen (experimentell)
* Inhalte
* [Inhalt] Fügen Sie 6 neue Filter hinzu: stilisierung, quantisieren, anisotropic kuwahara, weiche Abschrägung, Richtungsabstand, Graustufen konvertierung
* [Inhalt] Aktualisieren Sie Rauschen und Grunges auf die neueste Version von Designer (mit der neuen 2D-Voronoi)
* [Inhalt] Fügen Sie 3 neue Texturen-Generatoren hinzu (Kachelzufall, Triangle Grid, Scratches-Generator)
* [Inhalt] Unreale Engine-Vorlage umbenennen und Vorgaben exportieren
* Python
* [Regal][Python] Speichern von intelligente Material oder intelligente Maske auf der Festplatte von Python
* [Python] Hinzufügen von automatisch Baking führend Käfigen zur Python-API
* [Python] Bearbeiten von Namen und Beschreibungen von Textursätzen/UV-Kacheln zulassen
* [Python] Freigeben von Auflösungseinstellungen für Vektor- und Schriftartenquellen
* [Automatische Aktualisierung][Python] Leg der Funktionen zur automatischen Aktualisierung von Projekten in Python
* Verschiedenes
* [Exportieren] Erleichtern Sie den Zugriff auf die Optionen für Senden an mit einem neuen Fenster
* [Nvidia] Warnung über die neuesten Nvidia-Treiber hinzufügen (572.16)
* Die einrasten Winkel sollten durch die Auswahl von Objekt/Welt-Raum beeinflusst werden.
* [Liste der Textursatz] Benutzerdefinierten Namen zu UV-Kacheln hinzufügen und diese beim Exportieren verwenden
* Mac
* [Mac] Verwenden von Metal anstelle von OpenGL für das Grafik-Rendering
* [Mac] Mac Intel-Support entfernen

<b>Fest</b>:

* [Absturz] Bildeingabe löschen
* Smart-Matte kann nicht über Ebenenstapel-Taste hinzugefügt werden
* [Python] Effekte auf GroupLayerNode können nicht gefunden werden

<b>Bekannte Probleme</b>:

* [Farbmanagement] HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen festgeklemmte Farben
* [Regression][UI] Kontextmenü auf HD-Bildschirmen ist zu klein
* [Absturz][Python] USD durch TextureStateEvent ausgelöst
* [MacOS Intel] Absturz beim Importieren einiger Vorgaben
* [Engine] Malen mit dem Klon-Werkzeug in normalen Kanalverschiebungsfarben falsch
* [Python] Phantom-Widget wird angezeigt, weil das Skript noch funktioniert
* [RedHat] Probleme mit dem Farbwähler

## Version 10

### 10.1.2

Freigabedatum: <b>2024/12/3</b>
Zusammenfassung: <b>Nebenversion, Fehlerbehebungen</b>

<b>Fest</b>:

* [Absturz] Bildeingabe löschen
* Smart-Matte kann nicht über Ebenenstapel-Taste hinzugefügt werden
* [Python] Effekte auf GroupLayerNode können nicht gefunden werden

<b>Bekannte Probleme</b>:

* [Farbmanagement] HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen festgeklemmte Farben
* [Regression][UI] Kontextmenü auf HD-Bildschirmen ist zu klein
* [Absturz][Python] USD durch TextureStateEvent ausgelöst
* [MacOS Intel] Absturz beim Importieren einiger Vorgaben
* [Engine] Malen mit dem Klon-Werkzeug in normalen Kanalverschiebungsfarben falsch
* [Python] Phantom-Widget wird angezeigt, weil das Skript noch funktioniert
* [RedHat] Probleme mit dem Farbwähler

### 10.1.1

Freigabedatum: <b>2024/11/5</b>
Zusammenfassung: <b>Nebenversion, Fehlerbehebungen</b>

<b>Hinzugefügt</b>:

* [Projekt] Aktuelles Projekt bleibt geöffnet, bis die neue Projektauswahl validiert wurde
* [Automatisches Entpacken] Texeldichte ermöglicht eine bessere Aufteilung von UV-Inseln in UDIM
* [Baking] Mehrdeutige Kopie im Kontextmenü von Mesh-Map reparieren
* [Verformen] Skalierung im Viewport für Z-Achse (Tiefe) entfernen
* [Importieren/Exportieren] Unterstützung nicht verwendeter Bilddateiformate entfernen
* Update Substance Engine auf 9.1.4

<b>Fest</b>:

* [Absturz] Nachdem eine Ressource in &quot;Elemente&quot; verlagert und das Projekt gespeichert wurde
* [Absturz] Probleme mit der Serverbibliothek
* [Absturz] Illustrator Server-Absturz in einigen seltenen Fällen
* [Absturz] Beim Beenden der Anwendung in seltenen Fällen
* Absturz-Berichte können auf einigen Computern nicht gesendet werden
* [Baking] Die Farbe des Scheitelpunkts wird nicht richtig gelesen
* [UI] Position von Fenstern und Neue Funktionen beim Start wurde verschoben
* [Assimp] Maya StandardSurface wird im ID-Baking nicht erkannt
* [Python] Fehlende SSL-Bibliothek gibt einen Fehler aus
* [Python][Win] Fehler beim Aufrufen von QColorConstants.Transparent
* [Python] Ebenen-Miniaturansichten, die über Python erstellt wurden, werden erst aktualisiert, wenn Sie in den Ebenenstapel klicken
* [Shader] Fehlerhafte Verknüpfung im Shader-API-Changelog
* [3D-Elemente] OS-Proxy-Einstellungen für den Zugriff auf 3D-Elemente verwenden

<b>Bekannte Probleme</b>:

* [Farbmanagement] HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen festgeklemmte Farben
* [Regression][UI] Kontextmenü auf HD-Bildschirmen ist zu klein
* [Absturz][Python] USD durch TextureStateEvent ausgelöst
* [MacOS Intel] Absturz beim Importieren einiger Vorgaben
* [Engine] Malen mit dem Klon-Werkzeug in normalen Kanalverschiebungsfarben falsch
* [Python] Widget, das über ein noch funktionierendes Skript gelöscht scheint
* [RedHat] Probleme mit dem Farbwähler

### 10.1.0

Freigabedatum: <b>2024/09/17</b>
Zusammenfassung: <b>Hauptversion, neuer Inhalt: Füllbereichsmaske/Farbfilter, Stickereiaufklebefilter und sechs generische Substance-Filter, USD mit Material- und Shader-Eigenschaften importieren, Leistungsverbesserung, VFX-Plattform 2024-kompatibel und Migration auf Linux RedHat</b>

<b>Hinzugefügt</b>:

* [Inhalt] Neue Füllbereichsmaske/Farbfilter hinzufügen
* [Inhalt] Neuen Stickerei Decal Filter hinzufügen
* [Inhalt] Fügen Sie 6 neue generische Substance-Filter hinzu (FXAA, Vergröberungsfilter, Hochpass, Posterisierung, Glättungsschritt, Schwellenwert).
* [USD] Exportieren USD Ebene mit einem definierten ASM-Material
* [USD] Importieren von USD mit Material- und Shader-Eigenschaften
* [Leistung] Aktivieren Sie standardmäßig optimierte Ebenenstapel-Miniaturansichten
* [Leistung] Reduzieren der Öffnungszeit von Projektdateien und des Speicherverbrauchs (Datendecodierung)
* VFX-Plattform 2024-kompatibel
* [VFX Platform 2024] Update auf Python 3.11
* [VFX Platform 2024] Update auf OpenEXR 3.2
* [VFX Platform 2024] [USD] Update OpenSubdiv 3.6.0
* [VFX Platform 2024][Farbmanagement] Update auf OCIO 2.3.2
* [Linux] Migration zu Linux RedHat
* [Linux] Aktualisieren Sie den Nvidia-Treiber auf Version 535.171.04
* [Importieren] Hinzufügen einer Option zum Spiegeln von Normalen-Map beim Importieren eines GLTF-Meshs
* [UI] Standardwert des Betriebssystems für die Entfernung der Erkennung von Ziehereignissen verwenden
* [Substance Engine] Fügen Sie eine Aufrufstreifenfunktion hinzu, um die Symbole aus der ausführbaren Datei zu entfernen.
* [Begrüßungsbildschirm] Update auf neues Begrüßungsbildschirmformat
* Substance Engine auf Version 9.1.3 aktualisieren
* [Python] Link zu Beispielen im Ebenenstapel-Dokumentationsmenü anzeigen
* [JavaScript] Verschieben von JavaScript-Plugins in den Unterordner &quot;javascript/plugins&quot;

<b>Fest</b>:

* [Illustrator] Absturz beim Exportieren einer UV-Kachel mit .ai-Grafik in bestimmten Fällen
* [Dynamische Pinselstriche][Pfad] Zufällig pro Strich funktioniert nicht auf einem Pfad
* [UI][Eigenschaften] Sperre ist aktiviert, wenn die Kachelung nicht einheitlich ist
* Debug TXT-Datei wird erstellt, wenn Sie auf ein Painter-Projekt doppelklicken
* [USD][Exportieren] Möglicherweise fehlen einige Texturen.
* [ASM] Farbstreuung-Kanal ignoriert metallic
* [Inhalt] Weichzeichnungsfilter funktioniert nicht im &quot;funktionierenden&quot; Farbraum
* [Inhalt] Height Der Filter &quot;Anpassen&quot; ändert auch das Alpha der Ebene.

<b>Bekannte Probleme</b>:

* [Farbmanagement] HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen festgeklemmte Farben
* [Win][Absturz] [ACE] Der sRGB-ICE-Farbraum für die Anzeige wird nicht transformieren.
* [Regression][UI] Kontextmenü auf HD-Bildschirmen ist zu klein
* [Absturz][Python] USD durch TextureStateEvent ausgelöst
* [MacOS Intel] Absturz beim Importieren einiger Vorgaben
* [Absturz] Ressource Verlagert und Projekt gespeichert
* [Engine] Malen mit dem Klon-Werkzeug in normalen Kanalverschiebungsfarben falsch
* [Python] Phantom-Widget wird angezeigt, weil das Skript noch funktioniert
* [RedHat] Probleme mit dem Farbwähler

### 10.0.1

Freigabedatum: <b>2024/06/11</b>
Zusammenfassung: <b>Nebenversion, Fehlerbehebungen</b>

<b>Hinzugefügt:</b>

* [Library] Konvertieren von Substance-Schriftarten in normale Schriftdateien
* [Illustrator][SVG] Miniaturansichten in der Bereichsauswahl einen hellgrauen Hintergrund geben
* [Python] Hinzufügen einer Funktion in der Bitmapquelle, um verfügbare Farbräume aufzulisten

<b>Fest</b>:

* [Ebenenstapel] Ordner immer geschlossen, wenn er in andere Ordner verschoben oder aus anderen Ordnern verschoben wird
* [Speichern] Projektdatei geht verloren, wenn &quot;Speichern als Kopie&quot; oder automatisches Speichern in bestimmten Fällen fehlschlägt
* [Importieren] Assets mit demselben Namen, aber unterschiedlichen Erweiterungen werden überschrieben
* [Eigenschaften] Einstellungen fehlen, wenn Ankerpunkt in Bildeingaben verwendet wird
* [Illustrator] Illustrator-Dateien können nach dem Server-Absturz nicht importiert werden, ohne Painter neu zu starten
* [Python] Übergeordnete Instanz kann nicht mit Typ &quot;Eigenschaften&quot; festgelegt werden
* [Python] Das Festlegen des hohen Poly als Baking führend Parameter lädt das hohe Poly nicht
* [Python] Fehlermeldung für set\_color\_space() ist zu allgemein
* [Python] Referenzquellen ermöglichen das Erstellen von Zyklen

<b>Bekannte Probleme</b>:

* [Farbmanagement] HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen festgeklemmte Farben
* [Regression][UI] Kontextmenü auf HD-Bildschirmen ist zu klein
* [Absturz][Python] USD durch TextureStateEvent ausgelöst
* [MacOS Intel] Absturz beim Importieren einiger Vorgaben
* [Illustrator] Absturz beim Exportieren einer UV-Kachel mit .ai-Grafik in bestimmten Fällen
* [Dynamische Pinselstriche][Pfad] Zufällig pro Strich funktioniert nicht auf einem Pfad

### 10.0.0

Freigabedatum: <b>2024/05/16</b>
Zusammenfassung: <b>Hauptversion, Edition des Ebenenstapels mit Python-API, Lesen nativer Illustrator-Dateien, Integration von 3D-Assets und neuer Textressource</b>

<b>Hinzugefügt</b>:

* [Illustrator] Verwenden von Illustrator-Dateien mit Zeichenflächen in Painter
* [Illustrator][SVG] Hinzufügen von Vorschauen in der Bereichsauswahl
* [Substance 3D Assets] Durchsuchen, Auswählen und Herunterladen von 3D-Assets direkt in Painter
* [Substance 3D Assets][UI] Neues Bedienfeld
* [Substance 3D Assets] Unterstützung für Umgebungs-Map und Materials
* [Substance 3D Assets] Ermöglicht das erneute Laden und Navigieren im Speicherortordner und das Öffnen im neuen Bedienfeld &quot;Substance 3D Assets&quot;.
* [Substance 3D Assets] Hinzufügen eines Download-Managers
* [Textressource] Einbettbare Schriftarten verwenden
* [Textressource] Erlaubt das Rendern einer Schriftart/eines Texts auf einem Mesh.
* [Textressource] Anzeigen von Schriftarten von Benutzer- und anderen freigegebenen Pfaden im Bedienfeld &quot;Elemente&quot; mit einer neuen Kategorie
* [Textressource][Eigenschaften] Unterstützung für erweiterte Schriftarteigenschaften hinzufügen
* [Textressource] Ermöglicht das Suchen/Anzeigen von Schriftarten in Mini-Regalen
* [Textressource] Fehlermeldung/Dialogfeld hinzufügen, wenn eine inkompatible Schriftart importiert wird
* Sonstiges
* [Projektion füllen] Verbessern Sie das Verhalten des Manipulators Skalierung bei Verwendung kleiner Werte
* [Manipulator] Hinzufügen eines neuen präzisen Modus beim Drücken von STRG-Tastaturbefehl
* [Manipulator] Verbessern der Stabilität des Manipulators auf der Oberfläche beim Kamera beweg
* [Exportieren] Hinzufügen eines Farbraumnamens in SBSAR-Ausgaben
* [Performance] Verbessern der Erkennungszeit von Elementen auf der Festplatte in Bibliotheken
* [Substance] Update auf Substance Engine Version 9.1.2
* [Drag &amp; Drop] Ausrichten der Aufkleberdrehung an der Kamera beim Ablegen im Viewport
* [Python] Edition des Ebenenstapels
* [Python] Auswahl von Ebene, Effekt, Maske und Geomaske in der Benutzeroberfläche zulassen
* [Python] Abrufen/Festlegen von Mischmodi für Ebenen
* [Python] Einstellungen für die Füllebene-Projektion abrufen/festlegen
* [Python] Abfrage der Substance-Material-Farbe aus einer Füllebene zulassen
* [Python] Abfragen und Festlegen von einheitliche Farben und Ressourcen in Ebenen und Effekten zulassen
* [Python] Erstellen und Bearbeiten von Textressourcen im Ebenenstapel zulassen
* [Python] Bearbeiten aktiver Kanäle für Ebenen und Effekte zulassen
* [Python] Batch-Aktionen können nur einmal rückgängig gemacht/wiederholt werden.
* [Python] Laden/Bearbeiten von vektoriellen Quellparametern zulassen
* [Python] Bearbeiten von Ebenen- und Effektfarbeneigenschaften mit Farbmanagement zulassen
* [Python] Abfragen und Erstellen instanzierter Ebenen zulassen
* [Python] Hinzufügen des Effekts &quot;Farbauswahl&quot; zulassen
* [Python] Steuern des Farbmanagements für Bitmapbilder
* [Python] Engine anhalten/fortsetzen
* [Python] Navigation zu gleichrangigen und übergeordneten Knoten zulassen
* [Python] Erstellen eines Filter-/Generatoreffekts zulassen
* [Python] Hinzufügen des Ebeneneffekts zulassen
* [Python] Hinzufügen von intelligente Maske zu einer Ebene zulassen
* [Python] Erstellen/Bearbeiten von Ankerpunkten zulassen
* [Python] Maske für Ebenen abrufen/festlegen
* [Python] Erstellen des Effekts &quot;Maske vergleichen&quot; zulassen
* [Python] Zulassen, dass Vorgaben aus Substance-Ressourcen abgefragt und verwendet werden
* [Python] Erlaubt das Auflisten von Vorgaben und ihren Werten über die interne \_properties-Funktion für Substance-Ressourcen.
* [Python] Liste vordefinierter Exportvorgaben zulassen
* [Python] Auflisten der in der Bibliothek verfügbaren Exportvorgaben
* [Python] Abrufen des Inhalts von Exportvorgaben zulassen

<b>Fest</b>:

* [Absturz] Rückgängigmachen von &quot;Shader-Instanz entfernen&quot; mit Strg+Z
* [Absturz] Erstellen einer Ebene auf leerem Stapel, wenn die letzte Auswahl ein Effekt war
* [SVG] Problem mit benutzerdefiniertem Wert für den zugeschnittenen Bereich
* [Automatisches Entpacken] Die Neuberechnung nur des Packings ohne Änderung der Ausrichtung der UV führt zu einem Absturz
* [Drag &amp; Drop] Verzögerung aufgrund externer Ressourcen wird mehrmals vorgeladen
* [UI] Miniaturansicht der Ressource per Drag &amp; Drop kann Warnmeldung im Ebenenstapel ausblenden
* [Performance] Maskierte UV-Kacheln werden noch berechnet
* [USD] Falsche Markierung für die Bereichsauswahl
* [Ressource] Bitmapbild wird beschädigt, nachdem im normalen Kanal gemalt und das Projekt gespeichert wurde
* [USD] Unterstützung für die Bestellung von Meshs für den linkshändigen Scheitelpunkt
* [Substance] Auf die Standardeinstellung zurücksetzen, um immer auf null für Winkel-Widget zurückzusetzen
* [Engine] Das Malen mit einem SVG in einer Schablone funktioniert nicht
* [Engine] Normalen-Map-Pinselstriche brechen nach einem Rückgängigmachen
* [Inhalt] Grafik zu Materialfilter hat falsche Alpha-Überblendung und falschen Farbraum
* [Inhalt] Füllmethoden auf dem Tile Generator funktionieren nicht
* [Inhalt] Histogramm-Scanfilter erzeugt in einigen Fällen Streifenbildung
* [Inhalt] Baking geführt stilisierte Beleuchtung berücksichtigt kein gemaltes Height
* [Python] Unerwarteter Fehler beim Abrufen instanzierter Ebeneninformationen nach Shader-Änderung
* [Speichern] Projektdatei geht verloren, wenn &quot;Speichern unter&quot; in bestimmten Fällen fehlschlägt

<b>Bekannte Probleme</b>:

* [Farbmanagement] HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen festgeklemmte Farben
* [Absturz][Linux][AMD] Ziehen und Ablegen von Ressourcen im Ebenenstapel unter Wayland OS
* [Regression][UI] Kontextmenü auf HD-Bildschirmen ist zu klein
* [Absturz][Python] USD durch TextureStateEvent ausgelöst
* [Speichern] Spp-Projektdatei geht verloren, wenn &quot;Als Kopie speichern&quot; in bestimmten Fällen fehlschlägt
* [MacOS Intel] Absturz beim Importieren einiger Vorgaben
* [Illustrator] Ai-Dateien können nach dem Server-Absturz nicht importiert werden, ohne Painter neu zu starten
* [Importieren] Assets mit demselben Namen, aber unterschiedlichen Erweiterungen werden überschrieben

## Version 9

### 9.1.2

Freigabedatum: <b>2024/01/30</b>
Zusammenfassung: <b>Nebenversion, Fehlerbehebungen</b>

<b>Hinzugefügt</b>:

* [Performance] Verbessern der Erstellungszeit der ersten Füllebene in neuen Projekten
* [Performance] Verkürzung der Ladezeit schwerer Umgebungs-Map
* [Substance] Speichern/Schließen von Projekten zulassen, selbst wenn Miniaturansichten generiert werden

<b>Fest</b>:

* Speichern schlägt in Projekten früherer Versionen fehl, wenn der Viewport geändert wird
* [Absturz] Mesh wird bei Verwendung von benutzerdefiniertem AO und Farbmanagement erneut importiert
* [Projektion füllen] Beim Klicken auf den Manipulator &quot;Skalieren&quot; wird die Meldung &quot;nicht bemalbar&quot; angezeigt.
* [Pinsel] Malen mit UV-Ausrichtung verursacht Artefakte
* [Ebenenstapel] Das Umbenennen der Ebene ist langsam, wenn der Stapel sehr lang ist
* [Ebenenstapel] Falsche Fehlermeldung bei Verwendung eines inkompatiblen Filters in der Maske
* [Ebenenstapel] Die Auswahl wechselt nach dem Löschen zurück zur obersten Ebene
* [Exportieren] Generierte normale Textur befindet sich immer im 3D-Raum-Nachbar-Auffüllmodus
* [Exportieren] Alpha der Textur wird nicht mit der Exportvorgabe der 2D-Ansicht generiert
* [Export] Beim SBSAR-Export werden falsche Verwendungsmöglichkeiten mit konvertierten Karten verwendet.
* [Shader] Shader-API Changelog ist nicht auf dem neuesten Stand bei ASM

<b>Bekannte Probleme</b>:

* [Farbmanagement] HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen festgeklemmte Farben
* [Absturz][Linux][AMD] Ziehen und Ablegen von Ressourcen im Ebenenstapel unter Wayland OS
* [Regression][UI] Kontextmenü auf HD-Bildschirmen ist zu klein
* [Absturz][Python] USD durch TextureStateEvent ausgelöst

### 9.1.1

Freigabedatum: <b>2023/12/05</b>
Zusammenfassung: <b>Nebenversion, Fehlerbehebungen und Senden an After Effects-Funktionen</b>

<b>Hinzugefügt:</b>

* [Interop] Senden eines strukturierten Meshs an After Effects zulassen (Ae 24.1)

<b>Fest:</b>

* [Fill] UV-Satz-zu-UV-Satz-Projektion liest nicht mehr als 2 UV-Satz
* [Absturz] Verwenden von 16.000 Umgebungs-Map
* [Absturz] Exr als Bildeingabe verwendet
* [Absturz] Kopieren und Einfügen von Pfaden über Projekte hinweg
* [QoL] Ziehen und Ablegen von Alpha-Ressourcen im Aufklebermodus erzeugt UV-Projektion in der Maske
* [Pfad] Beim Kopieren von Pfad-Scheitelpunkten wird auch der Zielpfad beim erneuten Öffnen des Projekts umbenannt.
* [Linux] Die Farbauswahl kann mit mehreren Bildschirmen unterbrochen werden
* [Automatisch Entpackt] UI-Problem für Texeldichtesteuerung
* [Farbmanagement] UI-Feedback ist sinnvoll, aber Engine ist nicht
* [Farbmanagement] Falsche Farbraumauswahl in der Maske mit Überschreibung von Benutzerdaten

<b>Bekannte Probleme:</b>

* [Farbmanagement] HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen festgeklemmte Farben
* [Absturz][Linux] mit Linux Wayland auf AMD beim Ziehen und Ablegen von Ressourcen im Ebenenstapel
* [Absturz][Mac] Ändern des Werts für anisotrope Filterungen unter Monterey OS
* [Regression][UI] Kontextmenü auf HD-Bildschirm ist zu klein
* [Python] Absturz exportieren USD ausgelöst durch TextureStateEvent

### 9.1.0

Freigabedatum: <b>2023.11.07</b>
Zusammenfassung: <b>Hauptversion mit SVG- und Transparenzunterstützung sowie Verbesserungen an Drag-and-Drop- und Pfad-Tools</b>

<b>Hinzugefügt:</b>

* [SVG] Importieren von Vektordateien zulassen (SVG)
* [SVG][UI] Unterstützung für SVG-spezifische Eigenschaften hinzufügen
* [SVG] Fügen Sie eine Option hinzu, um die ursprünglichen Bildproportionen einfach beizubehalten
* [SVG] Automatisches Verwenden von Alpha von SVG mit Transparenz zulassen
* [Interop] Senden eines strukturierten Meshs an After Effects zulassen (Ae 24.1 Beta)
* [Interop] Hinzufügen von Einstellungen für &quot;An After Effects senden&quot;
* [QoL][Assets][UI] Automatisches Importieren von Assets beim Ziehen und Ablegen in einen Steckplatz der Benutzeroberfläche
* [QoL] Zulassen, dass externe Elemente per Drag &amp; Drop in den Ebenenstapel gezogen werden
* [QoL][Ebenenstapel] Ziehen Sie Texturen aus dem Bedienfeld &quot;Elemente&quot; in den Ebenenstapel
* [QoL][Viewport] Generatorfilter auf dem Mesh ziehen und ablegen lassen
* [QoL][Viewport] Zulassen, dass externe Elemente auf den Mesh abgelegt werden.
* [QoL][Projektion] Hinzufügen eines neuen UV-Satzes zum UV-Satz-Projektion-Modus
* [QoL] Ziehen und Ablegen von Intelligente Masken als neue Ebenen in Viewport und Ebenenstapel
* [QoL] Hinzufügen eines Selektors für Generatoren mit mehreren Ausgaben, wenn er in der Maske verwendet wird
* [QoL] Ziehen und Ablegen von Ein Kanal-Bildern über einen Fülleffekt zulassen
* [QoL][Ebenenstapel] Verwenden Sie STRG/ALT-Modifizierer mit Drag &amp; Drop, um anzugeben, wo/wie Effekte/Ebenen erstellt werden sollen
* [Pfad] Umschalten der Pfadsichtbarkeit einzeln im Pfadbedienfeld
* [Path] Verwenden von Transformations-Manipulatoren für Pfadpunkte zulassen
* [Path] Tangenten pro Scheitelpunkt manuell steuern
* [Pfad] Kopieren/Einfügen von Pfadeigenschaften
* [Pfad] Schaltfläche &quot;Leerer Tastaturbefehl für Pausen-Tangente einführen&quot;
* [Shader] Unterstützung für Deckkraft und Translucency in ASM-Shader hinzufügen
* [Shader] Unterstützung für Absorptionsfarbe Channel mit ASM Shader hinzufügen
* [Shader] ASM-Shader-Parameter verbessern - QuickInfos
* [Shader] Ändern der Standardfarbe des Translucency-Kanals in Schwarz
* [Anzeigeeinstellungen] Temporale Anti-Aliasing standardmäßig aktivieren
* [Anzeigeeinstellungen] Aktivieren Sie standardmäßig die Einstellung für die Teilflächenstreuung.
* [Substance] Hinzufügen von Unterstützung für die ColorSpace-Eigenschaft von der Eingabe/Ausgabe des Grafen
* [Substance] Substance-Engine auf Version 9.0.3 aktualisieren
* [UI] Zugriff auf die Schaltfläche der kontextbezogenen Symbolleiste, auch wenn das App-Fenster klein ist
* [Automatisch Entpackt] Steuernummer für UV-Kacheln mit Texeldichte
* [Baking] Deaktivieren von GPU-Raytracing auf AMD-GPUs standardmäßig
* [Leistung] Anwendung der verlustfreien Komprimierung auf 16-Bit-Bilder, um den Projektbedarf zu reduzieren
* [Python] Bearbeiten der standardmäßigen Kamera in der 3D-Ansicht zulassen
* [Python] Möglichkeit zum Exportieren von Mesh über Skripterstellung Gelegt
* [Inhalt][Beispiele] Neues Beispielprojekt hinzufügen &quot;Französische Restauranttabelle&quot;
* [Inhalt] Aktualisieren des Alpha-Substance-Logos auf die neue Version
* [Inhalt] Fügen Sie drei Material-Filter mit SVG hinzu (Benutzerdefinierter Aufkleber, Benutzerdefiniertes Sprühen und Grafik zu Material).

<b>Fest:</b>

* [Absturz] Ändern der Größe von Manipulator, wenn das Werkzeug &quot;Symmetrie&quot; nicht verwendet wird
* [Absturz] [Ebenenstapel] Erstellen einer Ebene, wenn nichts ausgewählt ist
* [Project] Mesh-Map können nach dem Entfernen nicht verwendeter Ressourcen beschädigt werden.
* [Projekt] Ressourcenbeschädigung nach dem erneuten Importieren oder Baking des Images
* [Assets] Durch erneutes Laden eines Assets wird es aus den Favoriten entfernt
* [Importieren] Ressourcen können nicht importiert werden, wenn im Bedienfeld &quot;Asset&quot; &quot;Kein Ergebnis gefunden&quot; angezeigt wird
* [UI] Der kontextbezogene Symbolleistenpfeil wird in einigen Fällen nicht angezeigt
* [Substance] Schaltfläche &quot;Nebeneinander&quot; für boolesche Werte wird nicht unterstützt
* [Level] Falsche Kanalbeschriftung bei Verwendung in Maske
* [Exportieren][glTF] glTF/GLB-Dateien, die aus Painter exportiert werden, haben keine Physische Größe
* [Inhalt] Intensität des Weichzeichnungsfilters ist auf 16 eingestellt
* [Inhalt] Farbabstimmungsfilter &quot;Zielfarbe&quot; Bildeingabe ist nicht sichtbar

<b>Bekannte Probleme:</b>

* [Farbmanagement] HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen festgeklemmte Farben
* [Absturz][Linux] mit Linux Wayland auf AMD beim Ziehen und Ablegen von Ressourcen im Ebenenstapel
* [Absturz][Mac] Ändern des Werts für anisotrope Filterungen unter Monterey OS
* [Absturz] Exr als Bildeingabe verwendet
* [Absturz] Verwenden von 16.000 Umgebungs-Map
* [Automatisch Entpackt] UI-Problem für Texeldichtesteuerung
* [Regression][UI] Kontextmenü auf HD-Bildschirm ist zu klein
* [Python] Absturz exportieren USD ausgelöst durch TextureStateEvent
* [QoL] Ziehen und Ablegen von Alpha-Ressourcen im Aufklebermodus erzeugt UV-Projektion in der Maske

### 9.0.1

Freigabedatum: <b>2023/09/19</b>
Zusammenfassung: <b>Geringfügige Fehlerbehebungsversion mit mehreren Verbesserungen</b>

<b>Hinzugefügt:</b>

* [Import] Festlegen des Standard-Importspeicherorts im Importfenster
* [Baking-Modus] Parameter auf ihre Standardwerte zurücksetzen
* [Baking] Legen Sie beim Erstellen eines Projekts die Baking-Auflösung auf Malen fest.
* [Symmetrie] Binden Sie Symmetrie-spezifischen Manipulator von Tastaturbefehl Q ab.
* [Menü] Option &quot;Protokoll anzeigen&quot; im Hilfemenü hinzufügen
* [Viewport] Verbessern der Schatten-Rendering-Geschwindigkeit
* [Substance] Engine auf Version 9.0.1 aktualisieren
* [Farbmanagement] OCIO Konfigurationsdatei kann einen beliebigen Erweiterungstyp haben
* [Assets] Sbsar-Ressource mit der Verwendung von Aufklebern sollte automatisch auf Verkrümmungs-Projektion gesetzt werden.
* [Pfad] Meldung anzeigen, wenn versucht wird, mit dem Pfad-Werkzeug zu interagieren, während UI und Gizmos ausgeblendet sind

<b>Fest:</b>

* [Absturz] Alt + Ziehen im Pfadbedienfeld
* [Ressourcen importieren] Zufälliger Absturz beim Entfernen der zu importierenden Ressourcen
* Absturz beim Importieren einer komprimierten GLB-Datei
* Problem beim Malen auf Meshs, die UVs gemeinsam nutzen
* Mesh blinkt schwarz, wenn der Cache neu berechnet oder geladen wird
* [Eigenschaften] Kontextmenü zum Zurücksetzen von Parametern wird in Dropdown-Listen nicht angezeigt
* [Level] Eingangsregler durch vorherige Ebene gesperrt
* [AMD][Weniger] SVT-Option, wenn aktiviert, erzeugt Artefakte
* [Projektion][Verformen] Absturz beim Doppelklicken auf Scheitelpunkt
* Benutzeroberfläche und Pfad von [Pfad] im Baking-Modus
* [AMD] Textur verloren, wenn mit Sichtbarkeit gespielt wird
* [Gering] Die Auflösung ist zu niedrig, wenn Sie den Mesh umdrehen.

<b>Bekannte Probleme:</b>

* [Farbmanagement] HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen festgeklemmte Farben

### 9.0.0

Freigabedatum: <b>2023/06/20</b>
Zusammenfassung: <b>Hauptversion mit Malen entlang des Pfades, die 3D-Kurven, neue Basismaterialien und das Bereinigen älterer Materialien und neue Vorgaben für 3D-Kurven ermöglicht</b>

<b>Hinzugefügt:</b>

* [Pfad] Neues Malen entlang Pfad-Werkzeug hinzufügen
* [Pfad] Fügen Sie einen leeren Tastaturbefehl für das Pfadwerkzeug hinzu.
* [Pfad] Hinzufügen neuer Punkte zu einem vorhandenen Pfad zulassen
* [Pfad] Tastaturbefehl hinzufügen, um die aktuelle Pfaderstellung zu beenden
* [Pfad] Bearbeiten der Pinseleigenschaften für Pfade zulassen
* [Pfad] Automatische Anpassung der Tangenten beim Platzieren eines Punkts
* [Pfad] Tangenten beim Verschieben eines Punkts neu berechnen
* [Pfad] Einrasten neu erstellter Punkte an der Oberfläche eines Meshs
* [Pfad] Bearbeiten des Drucks pro Scheitelpunkt zulassen
* [Pfad] Anpassen des Drucks des neu erstellten Punkts von benachbarten Punkten
* [Pfad] Umwandeln von Punkten in Übergangspunkte/Eckpunkte zulassen (Tangente umbrechen)
* [Pfad] Sofort einen neu hinzugefügten Punkt verschieben
* [Pfad] Punkte aus vorhandenem Pfad entfernen
* [Pfad] Umkehren der Richtung eines Pfads zulassen
* [Pfad] Wählen Sie einen Pfad im Viewport aus.
* [Pfad] Auswählen von Pfadpunkten mit dem Auswahlrechteck zulassen
* [Pfad] Einführung von STRG+A-Tastaturbefehlen zum Auswählen aller Punkte eines Pfads
* [Pfad] Schließen des Pfads zulassen
* [Pfad] Geben Sie die Achse &quot;Pfad nach oben&quot; in den Eigenschaften an.
* [Path] Hinzufügen eines Scheitelpunkt-Steuerungsmenüs zur kontextabhängigen Symbolleiste
* [Pfad] Einführung in die Malen-/Lösch-/Verwischen-Modi im Pfadwerkzeug
* [Pfad] Erstellen von visuellem Feedback für Pfade im Viewport
* [Pfad] Hinzufügen eines visuellen Indikators für die Pfadrichtung
* [Path] Hinzufügen der Thickness zu den Anzeigeeinstellungen des Pfads
* [Path] Pfade ausblenden - Benutzeroberfläche
* [Pfad] Bedienfeld &quot;Pfad hinzufügen&quot; zur Liste der Pfade der aktuell ausgewählten Ebene
* [Pfad] Fügen Sie visuelles Feedback hinzu, wenn Sie den Mauszeiger über einen Pfad im Pfadbedienfeld bewegen
* [Pfad] Pfadbedienfeld anzeigen, wenn das Pfadwerkzeug ausgewählt ist
* [Pfad] Umbenennen, Löschen, Kopieren, Ausschneiden und Duplizieren von Pfaden im Bedienfeld &quot;Pfad&quot; zulassen
* [Pfad] Meldung anzeigen, wenn versucht wird, im 2D-Viewport mit dem Pfad-Werkzeug zu interagieren
* [Library] Integrieren neuer Inhalte (Pfad-Tools und -Basismaterial)
* [Dynamische Pinselstriche] Eigenschaft &quot;Abstand&quot; für Dynamische Pinselstriche hinzufügen
* [Dynamische Pinselstriche] Hinzufügen von Größen- und Abstand-Eigenschaften zu Dynamischen Pinselstrichen
* [Dynamische Pinselstriche] Hinzufügen der Eigenschaft &quot;Anfang&quot;, &quot;Mitte&quot; und &quot;Ende&quot; für Dynamische Pinselstriche
* [Python][USD] Gelegt Projektkonfigurationsparameter für das USD
* [Python][USD] Gelegt Projekterstellungsparameter für das USD
* [Exportieren][USD] Fügen Sie Projektpfadinformationen innerhalb der exportierten USD hinzu
* [GLTF] Aktualisieren von Texturen in der Bibliothek beim erneuten Laden einer GLTF-Datei
* [Shader] Reduzieren von Artefakten in der Naht für UV-Inseln mit unterschiedlicher Ausrichtung
* [Engine] Update auf Substance Engine Version 9.0

<b>Fest:</b>

* [Importieren] Einige GLB mit Texturen erhalten keine Texturen in Painter
* [AMD] Artefakte an Rändern für alle 3D-Projektion-Flächen
* [Engine] Texturen brechen beim Umschalten der Ebenensichtbarkeit ab
* [Engine] Texturen sind an einigen Stellen leer, wenn der Mischmodus geändert wird
* [Engine] Textur/Projektion ist in einigen Fällen leerer Verkrümmungsmodus
* [Iray] Iteration wird beim Speichern des Renderings auf 0 zurückgesetzt
* [Log] USD Fehlermeldung beim Ausführen von Datei > Neu

<b>Bekannte Probleme:</b>

* [Farbmanagement] HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen festgeklemmte Farben
* [Ebenenstapel] Eingabequelle nicht pro Ebene gespeichert

## Version 8

### 8.3.1

Freigabedatum: <b>2023/04/27</b>

<b>Hinzugefügt:</b>

* [Baking-Modus] Hinzufügen (leeren) Tastaturbefehl, um den Viewport anzuzeigen/auszublenden
* [Baking führend Modus] Bei Verwendung der Schaltfläche &quot;Baking führend Mesh ausblenden&quot; immer niedrige Poly-Werte anzeigen
* [Baking Mode] Suffix für &quot;Matching By Name&quot; basierend auf aktuellem Textursatz anzeigen
* [Import] Unterstützung für GLTF-Binärdateien (glb) hinzufügen
* [Liste der Textursatz] Menü &quot;Hinzufügen&quot;, um Shader-Instanzen auszuwählen oder zu erstellen
* [Liste der Textursatz] Schnelles Ändern der Auflösung von Textursatz und UV-Kachel
* [Physische Größe] Verbessern des Manipulator-Verhaltens bei Verwendung von Physische Größe in UV-Projektion
* [UI] &quot;Speichern unter&quot; wieder im Hauptmenü &quot;Datei&quot; anzeigen
* [UI] Speichern der Ansichtsauswahl (nur 2D, nur 3D, beide) im UI-Layout
* [USD] Weniger vage Fehlermeldung bei der Projekterstellung mit nicht unterstützten USD
* [Python] Hinzufügen von Baking führend Ereignissen, um dem Fortschritt des Bakings zu folgen
* [Python] Abbrechen eines Baking zulassen
* [Python] Leg &quot;Basierend auf Ausgabevorlage&quot; für Dateityp und Bittiefe beim Export
* [Python] Gelegt Aktualisierungszeit für TextureStateEvent.Update

<b>Fest:</b>

* [Absturz] Seltener Absturz beim Schließen eines Projekts
* [Absturz] [Baking] Aktivieren der Mesh-Map-Synchronisierung mit dem Height oder der Krümmung für ein bestimmtes Projekt
* [Absturz][Skripterstellung] Absturz beim Hinzufügen eines Materials nach der Erstellung einer Shader-Instanz
* [Baking Mode] AO-Intensität im neutralen Material hat keine Auswirkung
* [Baking-Modus] Absturz beim Wechseln in den Baking-Modus vor dem Laden des Modells
* [Baking führend Modus] Fehlende Fehlermeldung auf der Registerkarte &quot;Baking führend Prozess&quot;
* [Baking-Modus] Einstellungen für neutrale Material haben nach dem erneuten Importieren eines Meshs keine Auswirkungen
* [Modustrennzeichen] Viewport-Trennzeichen werden global und nicht pro Baking gespeichert.
* [Baking führend Modus] Visualisierungsproblem: Durchschnittliche Normale verändert die Oberfläche des Käfigs nicht
* [Farbmanagement] Die Einstellung &quot;Farbraum automatisch erkennen&quot; ist deaktiviert, wenn OCIO env var vorhanden ist
* [Inhalt] Der Maskenkonturfilter weist ein Artefakt mit Height-Eingabe auf.
* [Inhalt] Regler für die Intensität des Steigung-Weichzeichnungsfilters ist bei 1,0 eingeklemmt
* [Interop] Projekt mit GLTF kann nicht aus Sampler erstellt werden
* [Ebenenstapel] Der Wert für die Kachelung der Projektion wird nicht korrekt mit dem Manipulator aktualisiert.
* [Linux] Versatz zwischen Grafiktablett-Stift und Cursor mit einem HDPI von mehr als 100 %
* [Python] Absturz beim erneuten Importieren eines Meshs nach dem Erstellen eines Projekts
* [Substance] 3D-Rauschen werden nach dem erneuten Importieren eines Meshs beschädigt
* [UV-Kacheln] Offset für UV-Projektion auf 1 geklemmt
* [Viewport] Visuelles Feedback für gerade Linien ist nicht mehr sichtbar
* [WhatsNew] Falscher Zeilenumbruch bei Funktionstiteln

<b>Bekannte Probleme:</b>

* [Importieren] Einige GLB mit Texturen erhalten keine Texturen in Painter

### 8.3.0

*(Freigegeben: 10. Januar 2023)*
Zusammenfassung: <b>Hauptversion mit neuem Importmodus, neuem Baking und Export von USD und Physische Größe-Unterstützung für UV-Projektion</b>

<b>Hinzugefügt:</b>

* [Baking führend Modus] Neuer Baking führend Modus, der dem Baking führend Prozess gewidmet ist
* [Baking-Modus] Stellen Sie den Tastaturbefehl so ein, dass er in den Baking-Modus auf F8 wechselt.
* [Baking-Modus] Hinzufügen der Schaltfläche &quot;Start&quot; und &quot;Baking abbrechen&quot; im Viewport
* [Baking führend Modus] Hinzufügen einer Baking führend Auswahl zur Liste der Textursatz
* [Baking-Modus] Fenster &quot;Neue Mesh-Map-Baker hinzufügen&quot;, um Baker auszuwählen
* [Baking Mode] Neues Mesh-Map-Einstellungsfenster hinzufügen, um Baking-Einstellungen zu bearbeiten
* [Baking führend Modus] Neues Baking führend Protokollfenster hinzufügen, um dem Baking führend Prozess zu folgen
* [Baking Mode] Hinzufügen von Baking-Parametern und Rückgängigmachen von Aktionen zum Verlaufsfenster
* [Baking führend Modus] Hinzufügen von Breadcrumbs in den Mesh-Map-Einstellungen
* [Baking-Modus] Hinzufügen von Mesh-Map-Miniaturansichten im Fenster &quot;Mesh-Map Baker&quot;
* [Baking Mode] Menü &quot;Visualisierungseinstellungen hinzufügen&quot; im 3D-Viewport
* [Baking Mode] Fügen Sie eine Visualisierungseinstellung hinzu, um den Mesh mit der hohen Poly-Dichte ein- bzw. auszublenden.
* [Baking Mode] Fügen Sie eine Visualisierungseinstellung hinzu, um den Käfig Mesh und Drahtgitter ein- bzw. auszublenden
* [Baking Mode] Fügen Sie eine Visualisierungseinstellung hinzu, um den Mesh mit geringer Poly-Zahl ein- bzw. auszublenden.
* [Baking Mode] Fügen Sie eine Visualisierungseinstellung hinzu, um harte Kanten ohne UV-Nähte als Fehler anzuzeigen.
* [Baking Mode] Informieren Sie im Viewport über Mesh- und Baking-Fehler, wenn das Baking Log nicht angezeigt wird.
* [Baking-Modus] Aktion hinzufügen, um die Baker-Einstellungen auf allen Textursätzen zu synchronisieren

  Im Fenster &quot;Mesh-Map-Baker&quot; kann jeder Baker (sowie die allgemeinen Einstellungen) über Textursatz hinweg synchronisiert werden, indem Sie auf das Verknüpfungssymbol neben dem Namen klicken. Dadurch wird ein Fenster geöffnet, in dem Sie auswählen können, welche Textursatz dieselben Parameter verwenden sollen.

* [Baking führend Modus] Hinzufügen von Aktionen zum Kopieren und Einfügen von Baker-Einstellungen

  Im Fenster &quot;Mesh-Map-Baker&quot; stehen Aktionen zum Kopieren und Übergehen der einzelnen Baker-Einstellungen über Textursätze hinweg zur Verfügung, entweder über das spezielle Menü am oberen Fensterrand oder über das Kontextmenü mit der rechten Maustaste.

* [Fehlermodus] Schaltfläche &quot;Hinzufügen&quot; im Fehlerprotokoll, um von den Baking zu den richtigen Baking zu springen

  Wenn ein Baker fehlschlägt oder ein Mesh nicht ordnungsgemäß geladen wird, wird im Protokoll eine Fehlermeldung Baking geführt. Mit einer Schaltfläche neben der Meldung können Sie das Fenster Mesh-Map-Baker und Mesh-Map-Einstellungen ändern, um die entsprechenden Einstellungen anzuzeigen. Dies hilft dabei, die Ursache eines Problems einfacher zu isolieren, um es beheben zu können.

* [Baking-Modus] Hinzufügen von Menüs zum Verwalten von Textursätzen und Auswahl von Bakern

  Sowohl im Fenster &quot;Textursatz-Liste&quot; als auch im Fenster &quot;Mesh-Map-Baker&quot; wurde ein kleines Aktionsmenü hinzugefügt, um das Kopieren und Umkehren von Auswahlen zu unterstützen.

* [Baking-Modus] Auswahlliste für geteilte Baker pro Textursatz
* [Baking-Modus] Gemeinsame Einstellungen pro Textursatz teilen
* [Baking-Modus] Lädt Meshs mit hohem Poly- und Käfig, ohne die Benutzeroberfläche einzufrieren
* [Baking-Modus] Verwenden Sie die Fortschrittsleiste des Viewports, um das Laden des Meshs anzuzeigen
* [Baking Mode] Fügen Sie den Ladestatus des Meshs im Baking-Protokoll hinzu
* [Baking-Modus] Ermöglicht das Umkehren von Mesh im Viewport während des Bakings
* [Baking Mode] Legt die Reihenfolge des Bakings auf der Grundlage der Sichtbarkeit des aktuellen Meshs für den Viewport fest.
* [Baking-Modus] Anzeige des impliziten Baking führend Käfigs im Viewport

  Wenn keine benutzerdefinierte Käfig-Meshdatei verwendet wird, wird ein automatischer Käfig-Mesh generiert und im Viewport angezeigt. Die Größe basiert auf dem Parameter &quot;Max. Frontalentfernung&quot; aus den allgemeinen Einstellungen des Bakings. Mit dem Mesh &quot;Käfig&quot; wird angegeben, wie weit die Anpassung zwischen dem niedrigen und dem hohen Poly-Wert gehen wird.

* [Baking-Modus] Anzeigen einer übereinstimmenden Liste von Mesh-Namen für &quot;Matching By Name&quot; im Baking-Protokoll
* [Modellmodus] Verwenden Sie neutrales Material, um das 3D-Baking im Viewport anzuzeigen.
* [Baking-Modus] Deaktivieren der Engine-Berechnung im Baking-Modus
* [Baking führend Modus] Beim Beenden der App während eines laufenden Baking wird eine Warnung angezeigt
* [Baker] Aktualisieren der Beschriftungen für Anti-Aliasing-Einstellungen

  Die Einstellungswerte für das Anti-Aliasing wurden in &quot;Supersampling&quot; umbenannt und mit einer expliziten Multiplikatornummer versehen, um das Verhalten zu verdeutlichen.

* [Baker] Aktualisieren Sie die Baker auf Version 2.5.7.
* [USD] Importieren und Exportieren von Universal Scene Description (USD)-Dateien
* [USD] Hinzufügen USD Optionen zum Fenster &quot;Neues Projekt&quot; bei Auswahl einer USD
* [USD] Neues Auswahlfenster für Umfang und Varianten hinzufügen

  Wenn Sie eine USD-Datei importieren, können Sie durch Klicken auf die Schaltfläche &quot;Ändern&quot; im Fenster &quot;Neues Projekt&quot; oder &quot;Projektkonfiguration&quot; auswählen, welche Teile und Varianten einer USD-Datei importiert werden sollen.

* [USD] Option &quot;Unterteilungsebenen hinzufügen&quot;

  Beim Erstellen eines neuen Projekts mit einer USD Meshdatei, die Unterteilungen enthält, ist es möglich, die Ebene der Unterteilungen mithilfe eines Schiebereglers auszuwählen. Das Projekt wird mit dem unterteilten Mesh erstellt. Die Ebene kann über die Projektkonfiguration geändert werden.

* [USD] Importieren USD Meshs mit Skin in einem bestimmten Rahmen

  Wenn Sie ein neues Projekt mit einer USD Meshdatei erstellen, die eine Animation enthält, können Sie den Rahmen mithilfe eines Schiebereglers auswählen, der die eingebettete Timeline-Sequenz widerspiegelt. Der Rahmen kann über die Projektkonfiguration modifiziert werden.

* [USD][Exportieren] Fügen Sie eine Option zum Exportieren USD Dateien hinzu.

  Das neue Kontrollkästchen &quot;USD exportieren&quot; wurde dem Fenster &quot;Texturen exportieren&quot; hinzugefügt. Wenn diese Option aktiviert ist, können USD sowie Textur Maps mit einer beliebigen Vorlage exportiert werden.

* [USD][Exportieren] Fügen Sie USD Dateiformat zum Mesh-Export hinzu.
* [USD] Benennen Sie die vorhandene Exportvorgabe &quot;USD PBR Metal Rauheit&quot; um, um ein expliziteres Format zu erhalten.

  Die USD Exportvorlage, die zuvor als &quot;USD PBR Metal Rauheit&quot; bezeichnet wurde, ist weiterhin über &quot;Texturen exportieren&quot; > &quot;Ausgabevorlage&quot; > &quot;USDz&quot; (Apple AR) verfügbar.

* [Automatisch Entpackt] Ausrichtung der Sperre für Packing hinzufügen

  Neue Option für Einstellungen für den automatischen entpack, mit der die Ausrichtung bestehender UV-Inseln beibehalten werden kann, wenn die Funktion &quot;Packing&quot; verwendet wird. Der Zugriff darauf erfolgt über &quot;Neues Projekt&quot; > &quot;Optionen für Automatisches Entpacken&quot; > &quot;Ausrichtung der UV-Insel&quot;.

* [Physische Größe] Fügen Sie eine Einstellung hinzu, um die Physische Größe automatisch in Fülleffekt/Ebene zu verwenden.

  Eine neue Option zum automatischen Umschalten auf die Skalierung der Physische Größe wurde hinzugefügt, wenn ein Material mit eingebetteter Physische Größe verwendet wird. Sie kann pro Projekt über Neues Projekt oder über Bearbeiten > Projektkonfiguration > Physische Größe > Füllebene-Skalierung auf Physische Größe umschalten, wenn Materialien zugewiesen werden, aktiviert werden.

* [Physische Größe] Physische Größe für UV-Projektion Gelegt

  Die Skalierung der Physische Größe ist jetzt für UV-Projektionen verfügbar - sie aktiviert die automatische Größenänderung für ein Material basierend auf der Physische Größe eines Meshs. Sie kann über &quot;Skalieren > Physische Größe&quot; im Fenster &quot;Füllebene&quot; oder &quot;Effekteigenschaften&quot; ausgewählt werden.

* [Scripting][Python] Abfrage der Anwendungsversion zulassen
* [Scripting][JavaScript] Update-API für neue Baking-Parameter
* [Scripting][Python] Baking-Modul: Bearbeiten der Parameter für das Baking
* [Scripting][Python] Baking-Modul: Baking starten/abbrechen
* [Scripting][Python] Baking-Modul: Methode der selektierten Krümmung
* [Scripting][Python] Baking-Modul: Auswahl von Bakern/UV-Kacheln
* [Scripting][Python] Baking-Modul: Baker-Einstellungen auf allen Textursätzen synchronisieren
* [SVT] Aktivieren der Unterstützung für wenig Hardware auf AMD-GPUs

  Die Hardwarebeschleunigung für das Dünn besetzte virtuelle Textur-System kann jetzt mit AMD-GPUs aktiviert werden. Diese Einstellung wird in den allgemeinen Voreinstellungen automatisch aktiviert.

* [Projektion] Parameter für zylindrische Projektion umbenennen

  Der Parameter &quot;Cylinder Cap Culling&quot; wurde in &quot;Rückseiten-Ausblendung&quot; umbenannt, um seine Wirkung besser darzustellen. Die zugehörige QuickInfo wurde entsprechend angepasst.

* [Project] Speichern Sie die Anwendungsversion im Projekt und rufen Sie sie über Skripterstellung ab.

  Seit Version 8.2 wird die Version der Anwendung beim Speichern in der spp-Datei gespeichert.
  Diese Versionsnummer kann mit der Funktion last\_saved\_substance\_painter\_version() im Projektmodul der Python-API abgerufen werden.
  Für Projekte, die vor 8.2 erstellt wurden, ist der zurückgegebene Wert null.

* [Import] Verbessern der allgemeinen Importzeit von 3D-Modellen

  Wir haben die allgemeine Importzeit von Meshs verbessert. Zum Beispiel die Verkürzung der Wartezeit beim Laden von High-Poly-Meshs zum Baking. Diese Optimierung gilt insbesondere für das Laden von OBJ.

<b>Fest:</b>

* [Absturz] Ändern von Kanälen bei Filtern mit bestimmtem Stapel
* [Mac][M1] Absturz beim Erstellen einer Füllebene und beim Verlassen des Ebenenstapels

  Dieses Problem kann durch Aktualisieren auf Mac OS 13 (Ventura) behoben werden.

* [Scripting][Python] Absturz bei Verwendung von ui.add\_dock\_widget() mit falschem Typ
* [Baking] Unvollständige Fehlermeldung im Protokoll, wenn ein Baking fehlschlägt
* [Baking] Speicher wird nach Abschluss des Bakings nicht freigegeben
* [Engine] Texturen-Cache wird nicht aktualisiert, wenn die Effektsichtbarkeit geändert wird
* [Exportieren] 2D-Ansicht exportiert zufällig einheitliche Map
* [Projekt] Speicherzuordnungsfehler beim Speichern eines Projekts mit großem Mesh
* [Viewport] TAA verursacht Artefakte beim Malen in einigen Fällen

<b>Bekannte Probleme:</b>

* [Farbmanagement] HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen festgeklemmte Farben
* [Ebenenstapel] Eingabequelle nicht pro Ebene gespeichert

### 8.2.0

*(Freigegeben: 6. Oktober 2022)*
Zusammenfassung: **Hauptversion mit neuen Onboarding-Bedienfeldern (neues Begrüßungs-Bedienfeld und neues Bedienfeld), Export in SBSAR, Effekten für Ordner, mehreren Verbesserungen für die Lebensqualität und Fehlerbehebungen.**

**Hinzugefügt:**

* [Onboarding] Onboarding-Bereich zur Begrüßung neuer Benutzer

  Es wurde ein neuer Begrüßungsbildschirm hinzugefügt, wenn neue CC-Benutzer Painter zum ersten Mal öffnen.

* [Onboarding] Neuerungen im Bedienfeld zur Verbesserung der Auffindbarkeit neuer Funktionen

  Es wurde ein neuer Bildschirm &quot;Neue Funktionen&quot; hinzugefügt, auf dem die wichtigsten neuen Funktionen angezeigt werden. Es wird automatisch angezeigt, wenn Painter nach einem wichtigen Update zum ersten Mal geöffnet wird, und Sie können erneut auf es über Hilfe > Neue Funktionen zugreifen.

* [Onboarding] Alten Begrüßungsbildschirm in &quot;Startseite&quot; umbenennen

  Alter Begrüßungsbildschirm wurde in Startbildschirm umbenannt, um Verwechslungen mit dem neuen Begrüßungsbildschirm zu vermeiden.

* [UI] Beheben von Skalierungsproblemen für Bildschirme mit hoher DPI

  Verbesserte Anpassung der Painter-Benutzeroberfläche auf HD-Bildschirmen mit benutzerdefinierter Anzeigeskalierung.

* [UI] Vermeiden Sie persistente Fehlermeldungen in der Benutzeroberfläche

  Fehlermeldungen aus vorherigen Projekten werden jetzt aus der unteren Statusleiste entfernt.

* [UI] Menü zum Speichern von Überarbeitung

  Zusätzliche Speicheroptionen sind jetzt in einem Untermenü gruppiert und einige werden aus Konsistenzgründen umbenannt.

* [UI] Speichern und Exportieren/Freigeben von UI-Layouts

  Im Menü &quot;Fenster&quot; (Window) gibt es neue Aktionen, mit denen Sie das UI-Layout in Dateien speichern und neu laden können. Die Layouts &quot;Malen&quot; und &quot;Rendern&quot; werden separat gespeichert.
  &quot;substance\_painter.ui&quot; wurde um verschiedene Funktionen erweitert, mit denen auch UI-Layouts gespeichert, zurückgesetzt und geladen werden können.

* Hinzufügen von Kopier-/Einfügeaktionen für Mischmodi/Deckkraft einer Ebene

  Es wurde ein neuer Eintrag &quot;Fülloptionen&quot; im Kontextmenü von Ebenen hinzugefügt. Damit können Sie den Mischmodus und die Deckkraft aller Kanäle von einer Ebene in eine andere kopieren und einfügen.

* Mischmodus/Deckkraft auf alle Kanäle einer Ebene anwenden

  Dem Mischmodus und der Deckkraft von Ebenen wurde eine Rechtsklick-Funktion hinzugefügt, mit der die derzeit angeklickte Einrichtung auf alle Kanäle angewendet werden kann.

* Mesh mit einem Tastatur-Tastaturbefehl neu laden (STRG+UMSCHALT+R)

  Es wurde ein bearbeitbarer Tastaturbefehl hinzugefügt, um die Meshdatei mit den zuletzt verfügbaren Einstellungen neu zu laden. Sie können auch über Bearbeiten > Mesh erneut importieren darauf zugreifen.

* Substance-Parameter auf die Standardeinstellungen zurücksetzen

  Es wurde eine neue Schaltfläche in den Eigenschaften am unteren Rand von .sbsar-Ressourcen hinzugefügt, mit der die Ressource auf die Standardeinstellungen zurückgesetzt werden kann.

* Malen-Pinsel auf die Standardeinstellungen zurücksetzen

  Es wurde ein neues Menü zum Abschnitt &quot;Pinsel&quot; in den Eigenschaften hinzugefügt, über das Sie den Standard-Standardpinsel zurücksetzen können.

* Rechtsklick zum Zurücksetzen der einzelnen Substance-Parameter auf die Standardeinstellungen

  Es wurde die Möglichkeit hinzugefügt, einzelne Parameter innerhalb einer .sbsar-Ressource per Rechtsklick zurückzusetzen.

* [Bedienfeld &quot;Elemente&quot;] Favoritenelemente &quot;Nadel&quot; werden oben im Bedienfeld &quot;Elemente&quot; angezeigt

  Es wurde eine neue Option zum Klicken mit der rechten Maustaste hinzugefügt, um Elemente zu bibliothekieren, mit der sie oben im Bedienfeld als Favoriten Nadel werden können. Sie können auch alle Ihre bevorzugten Assets über &quot;Gespeicherte Suchen&quot; anzeigen.

* [Bedienfeld &quot;Elemente&quot;] Elemente löschen, neu laden und umbenennen

  Kontextmenüoptionen zum Löschen, erneuten Laden und Umbenennen von Elementen in der Benutzerbibliothek wurden hinzugefügt. Sie werden direkt aus ihrem Bibliotheksspeicherort auf der Festplatte gelöscht und vom ursprünglichen Speicherort neu geladen. Elemente, die Teil eines Pakets wie .abr oder .sbsar sind, können nicht einzeln bearbeitet werden.

* [Farbauswahl] Füllen des Effekts &quot;Farbauswahl&quot; mit Füllmethoden
* [Ebenenstapel] Hinzufügen von Füllmethode und Deckkraft für Filter
* [Ebenenstapel] Kachelung-Werte größer als 128 für Füllebene/Effekte zulassen
* [Ebenenstapel] Zylinderdeckel für zylindrische Projektion in Füllebene/Wirkung

  Bei der zylindrischen Projektion in den Eigenschaften der Füllebene haben Sie jetzt die Möglichkeit, Zylinderkappen zu entfernen.

* [Protokoll] Fehlermeldung anzeigen, wenn sich ein Mesh-Teil beim Erstellen eines UV-Kachel-Projekts in einem negativen Bereich befindet

  Es wurde eine deutlichere Fehlermeldung hinzugefügt, wenn ein UV-Kachel-Projekt nicht erstellt werden kann, da UV-Teile in Leerzeichen gefunden werden.

* [Project] Geben Sie beim Öffnen eines Projekts die Version in der Fehlermeldung &quot;Daten zu aktuell&quot; an.

  Wenn Sie ein Projekt öffnen, das für die Anwendung zu neu ist, wird in der Fehlermeldung jetzt die Version des Projekts angezeigt, damit Sie die richtige Anwendungsversion leichter erkennen können.

* [Viewport] Lassen Sie den Mesh von unten beleuchten

  Ein neuer Parameter für die Umgebungsausrichtung wurde unter Anzeigeeinstellungen > Kamera > Umgebungseinstellungen hinzugefügt, um die Umgebungs-Map-Beleuchtung an der Kamera auszurichten, wenn sie auf &quot;Lokal&quot; eingestellt ist.

* [Viewport] Anzeigen von R, G, B und Alpha im Viewport (Einzelanzeigemodus)

  Unter Anzeigeeinstellungen > Kanaleinstellungen > Kanalanzeige gibt es eine neue Farbkanaleinstellung, mit der nur die R-, G-, B- oder Kanalkomponente eines Viewports im Einzelanzeigemodus angezeigt werden kann.

* [Shader] Benutzerkanäle als RGBA in Material-Layer-Shadern festlegen

  Bei der Einstellung der Kanalkonfiguration innerhalb eines Shader für die Kanalschichtung ist es nun möglich, das Textursatz des Materials so festzulegen, dass es vom Standardwert abweicht. Auf diese Weise können Benutzer-Farbkanäle anstelle von Graustufen angefordert werden.

* [Exportieren] Exportieren von Texturen als SBSAR zulassen

  Beim Exportieren von Texturen über das Fenster Datei > Texturen exportieren kann das Dateiformat SBSAR (Substance Archive) ausgewählt werden, um sie neu zu gruppieren. Der Inhalt des SBSAR richtet sich nach der verwendeten Ausgabevorlage.
  Das Datenformat kann auch in den Exportvorgaben festgelegt werden. Bei Verwendung einer Hybridkonfiguration (SBSAR + Anderes Format) werden Texturen, die ein SBSAR betreffen, gruppiert, während der Rest parallel exportiert wird.

* [Exportieren] 16-Bit-Option für EXR Dateiformat Gelegt

  Beim Exportieren EXR Textur-Dateien können Sie jetzt im Fenster &quot;Exporteinstellungen&quot; die Texturen 16f Bit (halbe Fließkommazahl) oder 32f Bit (Fließkommazahl) auswählen (sowohl für Exporteinstellungen als auch Exportvorgaben). Alte Projekte und alte Exportvorgaben werden standardmäßig auf 16f Bit gesetzt, um das alte Verhalten widerzuspiegeln.

* [Python] Ereignis hinzufügen, um zu wissen, wann Textursatz geändert werden

  Der neue &quot;substance\_painter.event.TextureStateEvent&quot; gibt Aufschluss darüber, ob ein Textursatz entweder aufgrund eines Malen-Strichs, eines hinzugefügten oder eines entfernten Kanals geändert wurde.

* [Python] Abrufen und Festlegen von Mesh-Map-Ressourcen in den Textursatz-Einstellungen zulassen

  Neue Funktionen wurden im Modul &quot;substance\_painter.project&quot; hinzugefügt, um Mesh-Map-Ressourcen abzurufen und einzurichten. Diese Funktionen können verwendet werden, um die Mesh-Map zu aktualisieren, auf die in den Textursatz-Einstellungen verwiesen wird.

* [Plug-ins] Option entfernen, um andere JS-Plug-ins zu erhalten

  Die Option, JavaScript-Plug-ins abzurufen, wurde entfernt, da sie auf der veralteten Freigabe-Website gehostet wurden.

* [Inhalt] Neue Roblox-Vorlage hinzufügen und Vorgabe exportieren

  Eine neue Roblox-Projektvorlage &quot;Material Variant&quot; und &quot;Surface Appearance&quot; sowie eine Exportvorgabe wurden hinzugefügt, um den Export von PBR-Texturen nach Roblox zu erleichtern. Auf die Vorlage kann über das Fenster Datei > Neues Projekt zugegriffen werden.

* Substance Engine auf die neueste Version (8.6.3) aktualisieren
* [Steam] Optimierter Build für Apple Silicon Chipsatz (Apple M1 / M2)

**Fest:**

* Absturz bei Verwendung von 16k exr
* [Absturz] Strg Z Nach dem Löschen einer Shader-Instanz
* [Iray] IoR ist bei einigen Shadern auf 1 blockiert
* [Win][Baking] Einige High-Poly-Fehler beim Laden
* [Farbmanagement] Falscher Farbraumname in der Benutzeroberfläche mit Filtern
* [Python] Von der Importfunktion zurückgegebene Ressourcenobjekte haben keinen Typ

  Beim Importieren eines Substance-Pakets in Python gab die Funktion das Paket anstelle der Graf zurück. Das Ressourcenmodul stellt nun Funktionen und Parameter bereit, um die Graf eines Substance-Pakets abzurufen.

**Bekannte Probleme:**

* [Farbmanagement] HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen festgeklemmte Farben
* [Ebenenstapel] Eingabequelle nicht pro Ebene gespeichert
* [Malen] Zeitweiliges Anti-Aliasing verursacht beim Malen in einigen Fällen Artefakte
* [Exportieren] 2D-Ansicht exportiert zufällig einheitliche Map

### 8.1.3

*(Freigegeben: 25. August 2022)*
Zusammenfassung: **Geringfügige Fehlerbehebungsversion**

**Hinzugefügt:**

* Update auf Iray SDK 1.6

**Fest:**

* [Shader] Absturz mit altem fehlerhaftem Shader
* [Material-Ebenen] Materialien können beim erneuten Öffnen eines Projekts verschwinden

**Bekannte Probleme:**

* [Farbmanagement] HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen festgeklemmte Farben
* [Ebenenstapel] Eingabequelle nicht pro Ebene gespeichert
* [Absturz] Strg Z Nach dem Löschen einer Shader-Instanz
* [Iray] IoR ist bei einigen Shadern auf 1 blockiert

### 8.1.2

*(Freigegeben: 19. Juli 2022)*
Zusammenfassung: **Geringfügige Fehlerbehebungsversion**

**Hinzugefügt:**

* [Automatisch Entpackt] Neue Option &quot;Für organische Mesh optimieren&quot; zur Auswahl des Segmentierungsalgorithmus
* [Physische Größe] Gelegt Einheitsoptionen in &quot;Neues Projekt&quot; und &quot;Projektkonfiguration&quot;
* [Farbmanagement] Verwenden Sie die Monitoranzeige standardmäßig, wenn Sie ACE
* [Farbmanagement][Python] Berücksichtigen Sie ACE env-var-Vorgabedatei beim Erstellen von Projekten
* [Farbmanagement] Setzen Sie die Farbmanagement-Einstellungen im Fenster &quot;Neues Projekt&quot; zurück, wenn sich die Konfiguration ändert
* [Farbmanagement] Deaktivieren Sie den Zugriff auf die OCIO, wenn env-var vorhanden ist
* [Farbmanagement] Sicheres Aktualisieren ACE Einstellungen, wenn ein Parameter nicht mehr vorhanden ist
* Substance Engine auf Version 8.6.0 aktualisieren
* [Exportieren] Fügen Sie eine neue GLTF-Exportvorgabe mit Versatz-Unterstützung hinzu
* [Scripting][Python] Abrufen von Ressourceninformationen (einschließlich benutzerdefinierter Metadaten)
* [Scripting][Python] Funktion zur Abfrageliste der Mesh pro Textursatz hinzufügen
* [Inhalt] Neue Mischervorlage hinzufügen und Vorgabe exportieren

**Fest:**

* [MacOS] Absturz beim Starten von Iray in einigen Fällen
* [Miniaturansichten] Regal-Miniaturansichten werden nicht richtig geladen
* Mehrere UV-Kanäle werden ignoriert.
* [Automatisch Entpackt] Unnötige Berechnung beim Aufteilen langer Inseln
* [Automatisch Entpackt] Option zur Vermeidung länglicher Inseln, die nicht berücksichtigt werden
* [Automatisch Entpackt] Verlust zusätzlicher Daten (Scheitelpunkt-Farben) beim Umpacken von UVs
* [UI] Horizontale Bildlaufleiste im Eigenschaftsfenster, wenn Farbmanagement aktiviert ist
* [Farbmanagement] OCIO fehlen substance\_3d\_painter\_standard\_srgb
* [Generator] Falsche Verwendung von Benutzerdaten &quot;deaktiviert&quot;
* [Farbmanagement] Dropdown-Liste &quot;Nicht kompatibel&quot; für Farbraum sollte nicht klickbar sein
* [Farbmanagement][Shader] sRGB override define funktioniert nicht mehr
* [Generator] Falsche Verwendung von Benutzerdaten &quot;deaktivieren&quot;
* [Ebenenstapel] Fehlerhafte Vorschauen bei Projekten mit UV-Kacheln
* [Shader] Die API-Dokumentation ist mit den Bent normals nicht vollständig auf dem neuesten Stand.
* [Export][Interoperabilität] Kann nicht mit Sonderzeichen an Stager gesendet werden.
* [Inhalt] Einige Miniaturansichten von Pinselvorgaben sind leer oder zu dunkel

**Bekannte Probleme:**

* [Farbmanagement] HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen festgeklemmte Farben
* [Ebenenstapel] Eingabequellen werden nicht pro Ebene gespeichert
* [Absturz] Strg Z Nach dem Löschen einer Shader-Instanz
* [Iray] IoR ist bei einigen Shadern auf 1 blockiert
* [Shader] Absturz mit altem fehlerhaftem Shader

### 8.1.1

*(Freigegeben: 28. Juni 2022)*
Zusammenfassung: **Minor Release-Hotfix**

**Hinzugefügt:**

* [Ebenenstapel] Mit Alt-Klick auf Maske wird die Auswahl von Effekten nicht mehr aufgehoben

**Fest:**

* [Absturz] Öffnen des alten Projekts im Einzelansichtsmodus gespeichert
* [Absturz] Löschen eines Generators in Eigenschaften
* [Textursatz-Einstellungen] Normale/Ambient occlusion-Abmischung und Height-zu-Normal-Methoden sind fehlerhaft
* [Exportieren] Exportieren von Texturen mit Diffusion-Innenabständen rendert schwarze Maps

**Bekannte Probleme:**

* [MacOS] Absturz beim Starten von Iray auf Monterey
* [Vorschau-Miniaturansicht] Vereinfachte Miniaturansichten werden nicht aktualisiert, wenn ein Anker verwendet wird
* [Farbmanagement] HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen festgeklemmte Farben

### 8.1.0

*(Freigegeben: 7. Juni 2022)*
Zusammenfassung: **Hauptversion mit ICC-Unterstützung, Material-Skalierung auf der Grundlage von Physische Größe-Daten, neue Baker, Verbesserungen an der FarbPipette und eine Reihe zusätzlicher Inhalte**

**Hinzugefügt:**

* [Farbmanagement] Unterstützung für ICC-Profile mit Adobe Color Engine hinzufügen (ACE)
* [Farbmanagement] Unterstützung für &quot;Adobe 98 RGB&quot; als Arbeitsfarbraum für ICC hinzufügen
* [Farbmanagement] Konfigurieren von ACE/ICC-Einstellungen über eine Konfigurationsdatei zulassen
* [Farbmanagement] Zulassen, dass lineare Farbwerte im Farbwähler mit dem Legacy-Modus eingegeben werden
* [Farbmanagement] Geben Sie das Farbprofil an, das für die Farbauswahl außerhalb der Benutzeroberfläche verwendet wird.
* [Farbmanagement] Merken Sie sich den letzten im Viewport ausgewählten Anzeigewert.
* [Farbmanagement][Substance] Sorgen Sie dafür, dass Generatoren/Filter mit dem Farbmanagement ordnungsgemäß funktionieren.
* [Farbmanagement][Substance] Fügen Sie neue Schlüsselwörter für die Farbraumüberschreibung $working und $standardsrgb hinzu
* [Physische Größe][Engine] Extrahieren von Physische Größe-Informationen aus Mesh
* [Physische Größe][Engine] Physische Größe Berechnung
* [Physische Größe] Leg von Optionen zur Verwendung von Physische Größe in der Benutzeroberfläche
* [Physische Größe] Visuelle Helfer im Viewport hinzufügen
* [Baking] Height-Baker hinzufügen
* [Baking] Bent normals-Baker hinzufügen
* [Baking] Baker für Deckkraft hinzufügen
* [Pipette] Neue Farb-Pipettenvorschau neben der Maus und Farbmanagement
* [Pipette] Das Farbwählerbedienfeld wird wieder an der letzten Position angezeigt, wenn es erneut geöffnet wird
* [Pipette] Ein neues Symbol für die Material-Auswahl
* [Pipette] Farbe verwaltet die Kanalvorschau des Farbwählers
* [Pipette] Fügen Sie der Pipette eine Funktion zum Klicken hinzu, um diese auszuwählen
* [Eye Dropper] Kanalauswahl aktiviert nicht aktive Materialien nicht mehr
* [Pipette] Pipette mit Tastaturbefehl verwenden
* [Pipette] Die Pipette nimmt den relevanten Kanal auf, falls zutreffend.
* [Pipette] Beim Aufrufen des Farbwählermodus werden alle Tastaturbefehle deaktiviert
* [Pipette] Automatische Auswahl des Hexadezimalfelds entfernen
* [Pipette] Schließen Sie das Bedienfeld nicht, wenn Sie die Material-Auswahl verwenden
* [Pipette] Neuer deaktivierter Zustand, wenn der Kanal nicht zur Auswahl verfügbar ist
* [Exportieren] Fügen Sie das Attribut &quot;Tangente&quot; dem glTF-Export hinzu
* Substance Engine auf Version 8.4 aktualisieren
* Update Auto Entpack auf 0.9.0
* Update auf Qt 5.15.8
* Update auf Python 3.9
* [Shader] Unterstützung für Bent normals-Schattierung hinzufügen
* [MacOS] Unterstützung von 3DConnection SpaceMouse
* [Python] Dokumentieren der in der API verwendeten Python-Version
* [Inhalt] Sechs neue 3D-Rauschen mit 105 Vorgaben hinzufügen
* [Inhalt] 20 neue Schmutz Maps und 2 Stofffalten
* [Inhalt] Aktualisieren der Exportvoreinstellung &quot;Mesh-Map&quot;, um neue Baker zu verwenden
* [Inhalt] Weichzeichnungs- und Verkrümmungsfilter hängen von der Steigung des Textursatzes ab
* [Inhalt] Aktualisieren von Beispielprojekten, um die 3 neuen Baker zu verwenden

**Fest:**

* [glTF] glTF kann nicht mit Sonderzeichen geöffnet werden
* [Engine] Artefakte mit deaktivierter Anisotropie und SVT
* [MacOS][M1] Intelligenten Materials werden nicht korrekt angezeigt
* [Mesh Processing] Mesh können nicht aus Modeler importiert werden.
* [UI] Horizontale Bildlaufleiste in neuem Projektfenster mit aktiviertem Farbmanagement
* [Farbmanagement] Arbeitsfarbraumwert fehlt in der Farbauswahl bei einigen OCIO
* [Farbmanagement] Pinselvorschau im Viewport ist nicht farbverwaltet
* [SpaceMouse] Pivot wird nicht sofort mit Fokusänderung aktualisiert und kann außerhalb des Modells liegen
* [Exportieren][USD] Exportierte USD haben eine falsche Struktur.
* [USD] Ambient occlusion-Problem beim Exportieren
* [Inhalt] Mesh der Miniaturansicht entsprechend dem Vorschaukugel-Beispielprojekt aktualisieren

**Bekannte Probleme:**

* Texturen mit Innenabständen exportieren macht schwarze Diffusionen.
* Normale/Ambient occlusion-Mischung ist defekt
* [MacOS] Absturz beim Starten von Iray in seltenen Fällen
* [Vorschau-Miniaturansicht] Vereinfachte Miniaturansichten werden nicht aktualisiert, wenn ein Anker verwendet wird
* [Farbmanagement] HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen festgeklemmte Farben

## Version 7

### 7.4.3

*(Freigegeben: 11. April 2022)*
Zusammenfassung: **Bugfix mit Unterstützung von 3D-Verbindung SpaceMouse im 2D-Viewport**

**Hinzugefügt:**

* [SpaceMouse] Unterstützung von 3DConnection SpaceMouse im 2D-Viewport

**Fest:**

* [Farbwähler] Kann nicht in das Hexadezimalfeld geschrieben werden
* [Farbmanagement] Ressourcen, die im Projektion-Modus verwendet werden, werden in der Überlagerung nicht farbverwaltet
* [Farbmanagement] Fehler werden nicht im Protokoll gemeldet.
* [SpaceMouse] Generische Fehlermeldung entfernen, wenn der Benutzer keine SpaceMouse hat
* [SpaceMouse] Beim Laden eines Projekts ist der Drehpunkt immer ausgeblendet.
* [Baker] Die Einstellung &quot;Durchschnittliche Normale&quot; hat keine Auswirkungen auf UV-Kachel-Projekte
* [UV-Kachel] Inaktive UV-Kachelüberlagerungen verschwinden beim erneuten Laden von Mesh mit verschiedenen Kacheln
* [Scripting][Python] Remote-Scripting ist beschädigt
* [Scripting][Python] Mehrere Kanäle können nicht von der API abgefragt werden und es wird ein Fehler ausgelöst.
* [Scripting][Python] Absturz bei Verwendung des ProjectEditionEntered-Ereignisses
* [Scripting][Python] Absturz beim Aufruf von get\_active\_Stapel()

**Bekannte Probleme:**

* 3D-Verbindung SpaceMouse wird auf MacOS nicht unterstützt
* [UI] Horizontale Bildlaufleiste mit Farbmanagement, die in einigen Fällen in neuen Projektfenstern angezeigt wird
* [Mac M1] Intelligenten Materials werden nicht korrekt angezeigt

### 7.4.2

*(Freigegeben: 8. März 2022)*
Zusammenfassung: **Bugfix mit Unterstützung von 3D-Verbindung, SpaceMouse und Verbesserungen des Farbmanagements (OCIO)**

**Hinzugefügt:**

* [SpaceMouse][Windows] Unterstützung der 3D-Verbindung von SpaceMouse im 3D-Viewport für die Navigation
* [SpaceMouse][Windows] Grundlegende Tastaturbefehle/Tasten für Pro- und Enterprise-SpaceMouse-Modelle im 3D-Viewport
* [SpaceMouse][Windows] Dediziertes Drehmittelsymbol im 3D-Viewport
* [Farbmanagement] Verwenden Sie Rollen aus OCIO Konfiguration, um Standardeinstellungen zu ändern
* [Farbmanagement] Farbmanagement des Eigenschaftenfensters für Farb-Widgets
* [Farbmanagement] Farbmanagement des Eigenschaftenfensters für die Vorschau des Materials
* [Farbmanagement] Farbfelder im Farbwähler verwalten
* [Farbmanagement] Fügen Sie eine Einstellung hinzu, um den standardmäßigen sRGB-Farbraum zu definieren
* [Farbmanagement] Hinzufügen des sRGB-Standardfarbraums aus OCIO Konfiguration in der Farbwähler-Auswahlliste &quot;Anzeige&quot;
* [Farbmanagement] Verbesserungen für das Menü zum Überschreiben des Farbraums
* [Farbmanagement] Überschreiben des Umgebungs-Map-Farbraums in den Anzeigeeinstellungen zulassen
* [Farbmanagement] Zeichnen von Farbwählerverläufen basierend auf der aktuellen Anzeige
* [Farbmanagement] HDR standardmäßig im Farbeditor Beschränkt
* [Farbmanagement] Passthrough (kein Farbraum) für Filter im Legacy-Modus verwenden
* [Farbmanagement] Anzeige von Farbverläufen im Farbeditor auf Übereinstimmung mit dem Bereich [0-1] beschränken
* [Farbmanagement] Ausblenden der Anzeigeselektor im Farbwähler im Modus &quot;Legacy&quot;
* [Farbmanagement] Hex-Code für Farbwähler immer im sRGB-Farbraum
* [Farbmanagement] Deaktivieren der Farbwähler-Dropdown-Liste &quot;Anzeige&quot; für Datenkanäle
* [Optimierung] Der Verkrümmungs-Raster berechnet nur überdeckte UV-Kacheln neu.
* [Exportieren] Exportieren von UV-Kachel-Projekten für Sketchfab, USD und glTF zulassen
* [Scripting][Python] Ändern der Tonzuordnungsfunktion zulassen

**Fest:**

* [Sketchfab] Durch die Aktualisierung des vorhandenen Modells wird am Ende ein neues Modell erstellt.
* [Sketchfab] Absturz bei der Suche nach einem zuvor aktualisierten Modell
* Absturz beim Exportieren nach USD
* Absturz beim Erstellen einer neuen Shader-Instanz in der Geometriemaske oder beim Ausblenden der Geometrie
* Absturz [Elementfenster importieren] beim Ändern des Typs von importierten Ressourcen
* Normale Mesh-Map werden bei Verwendung in Ebenenstapel invertiert
* [Substance] Der Benutzerdaten-Mischmodus wird nicht berücksichtigt.
* [Farbmanagement] Bitmaps mit Farbraum im Dateinamen werden als UV-Kachel Sequenzen importiert
* [Farbmanagement] Farbverwaltete Ausgaben von Substance Graf befinden sich im falschen Farbraum
* [Farbmanagement] Polygon-Füllwerkzeug zeigt die falsche Farbe an
* [Farbmanagement] ACE Tonwertumsetzer wird auf Kanäle im Solomodus angewendet
* [Farbmanagement] Die Kugelbeleuchtung der Werkzeugvorschau ist nicht farbverwaltet
* [Farbmanagement][Exportieren] Konvertierte Karten werden falsch konvertiert.
* [Scripting][Python][Farbmanagement] Projekte, die mit Vorlage und OCIO Umgebungsvariablen erstellt wurden, befinden sich im Modus &quot;Veraltet&quot;.
* [Scripting][Python] Die JavaScript-Evaluierungsfunktion kann beim Start nicht verwendet werden.
* [3D-Adobe-Angebot] Painter kann nicht gestartet werden, wenn regionale Einstellungen mit Sprachen verwendet werden, die nicht standardmäßig unterstützt werden

**Bekannte Probleme:**

* 3D-Verbindung SpaceMouse wird auf MacOS nicht unterstützt
* [UI] Horizontale Bildlaufleiste mit Farbmanagement, die in einigen Fällen in neuen Projektfenstern angezeigt wird
* [Baker] Die Einstellung &quot;Durchschnittliche Normale&quot; hat keine Auswirkungen auf UV-Kachel-Projekte
* [Mac M1] Intelligenten Materials werden nicht korrekt angezeigt
* [Farbmanagement] Ressourcen, die im Projektion-Modus verwendet werden, werden in der Überlagerung nicht farbverwaltet
* [Farbwähler] Kann nicht in das Hexadezimalfeld geschrieben werden

### 7.4.1

*(Freigegeben: 14. Dezember 2021)*
Zusammenfassung: **Bugfix mit Farbmanagement-Verbesserungen**

**Hinzugefügt:**

* [Farbmanagement] Verwenden der Datenrolle in exportierten Dateinamen
* [Farbmanagement] Erweitern Sie den Abschnitt Farbmanagement standardmäßig, wenn OCIO in den Fenstern für neue Projekt- und Projekteinstellungen ausgewählt ist.
* [Farbmanagement] Hinzufügen ACE Tonwertumsetzers im Legacy-Modus
* [Farbmanagement] Standardkonfigurationseinstellungen anpassen
* [Farbmanagement][Exportieren] Fill $colorSpace in Dateinamen für Datenkanäle
* [Exportieren] Exportieren von UV-Kachel-Projekten in Stager
* [Interoperabilität] Nicht verfügbar für Steam- und Substance-Editionen
* [Interoperabilität] Senden eines UV-Kachel-Projekts an Stager zulassen

**Fest:**

* [MacOS][Absturz] Painter beginnt nicht mit Catalina
* [Farbmanagement][Absturz] Zufälliger Absturz bei der Wiedergabe von Datentyp/Farbmanagement auf Benutzerkanal
* [Farbmanagement] Ressourcen, die als Graustufen in Masken verwendet werden, zeigen den Farbraum an Neues Menü
* [Farbmanagement] Benutzerkanal ist im Viewport im Legacy-Modus + Solo-Ansicht dunkler
* [Farbmanagement] Die Env-Map ist immer linear, wenn sie in iRay verwendet wird
* [Farbmanagement] Die Farbauswahl wählt im Legacy-Modus nicht den richtigen Wert für den Datenkanal aus
* [Farbmanagement] Farbwähler in einer Substance im Legacy-Modus funktioniert nicht
* [Farbmanagement] Der Wechsel zwischen Solokanal-Ansichten im Viewport wird bei Verwendung des Dropdown-Menüs nicht mit dem richtigen Farbraum angezeigt
* [Farbmanagement] Beim Export wird die falsche Konvertierung auf farbverwaltete Benutzerkanäle im Legacy-Modus angewendet.
* In der Einzelansichtsmaske erstellte Konturen werden beim Zurückwechseln zur Material-Ansicht nicht angezeigt
* [Exportieren] Konvertierte Karten werden nicht als farbverwaltete Kanäle exportiert
* [Textursatz] QuickInfo mit Originalnamen fehlt auf umbenannten Benutzerkanälen
* [Steam] Dateien fehlen beim Überprüfen der Dateiintegrität mit Steam

**Bekannte Probleme:**

* [Mac M1] Intelligenten Materials werden nicht korrekt angezeigt

### 7.4.0

*(Freigegeben: 24. November 2021)*
Zusammenfassung: **Hauptversion. Einführung der ersten Farbmanagement-Version, Abdocken der 2D- oder 3D-Ansicht, neue Option für den automatischen entpack von UV zum Vermeiden von länglichen Inseln, Aufruf von JavaScript-Funktionen von der Python-API und neuer Inhalt**

**Hinzugefügt:**

* [Farbmanagement] Unterstützung von Farbmanagement OpenColorIO Version 2
* [Farbmanagement] Hinzufügen von Farbmanagementeinstellungen zu Projekteinstellungen
* [Farbmanagement] Warnfenster zu Farbmanagement-Konfigurationsänderungen beim Öffnen eines Projekts
* [Farbmanagement] Zeigt eine Fehlermeldung an, wenn eine ungültige OCIO-Konfigurationsdatei ausgewählt ist
* [Farbmanagement] Überschreiben der Konfiguration mit OCIO Umgebungsvariablen zulassen
* [Farbmanagement] Mehrere OCIO sind standardmäßig in die Anwendung integriert.
* [Farbmanagement] Extrahieren des Farbraumnamens aus dem importierten Bitmap-Dateinamen
* [Farbmanagement] Überschreiben des Farbraums mit einem Farbraum aus der Konfiguration im Eigenschaftenfenster zulassen
* [Farbmanagement] Hinzufügen von Farbmanagementoptionen in den Textursatz-Einstellungen
* [Farbmanagement][Viewport] Ermöglicht das separate Farbmanagement von 2D- und 3D-Ansichten.
* [Farbmanagement] Laden und Konvertieren von Umgebungs-Map in den Arbeitsfarbraum
* [Farbmanagement] Anpassen des Farbwählers und Editors mit dem aktuellen Farbraum
* [Farbmanagement] Zulassen, dass die Anzeige transformieren Farbraum im Viewport mit einem neuen Dropdown-Menü auswählen
* [Farbmanagement] Anwenden von transformieren Anzeige mit Iray-Rendering-Ergebnissen
* [Farbmanagement] Exportieren von Texturen mit unterschiedlichen Farbräumen
* [Farbmanagement][Python] Anwenden von Farbmanagementeinstellungen aus der Umgebungsvariablen (OCIO) auf neue Projekte
* [Viewport] Abdocken des 2D- oder 3D-Viewports zulassen
* [Automatisch Entpackt] Neue Option zur Vermeidung von länglichen Inseln
* [Scripting Python] Aufrufen von JavaScript-Funktionen über die Python-API
* [Neues Projektfenster] Reduzieren des Abschnitts &quot;Importierte Karten&quot;
* [Projektion][Verformen] Normale Elemente können als Option in den Verkrümmungseinstellungen ausgeblendet werden
* [Content] 11 neue Schmutz-Maps
* [Inhalt] 8 neue Werkzeugvorgaben (Reißverschluss, Spannschnur, Glitter)
* [Inhalt] 8 neue Materialien (Narbe, Hosentasche, ...)
* [Inhalt] 1 neuer Generator (inflate schrumpfwarp)

**Bekannte Probleme:**

* [Mac M1] Intelligenten Materials werden nicht korrekt angezeigt
* [Farbmanagement][Absturz] Zufälliger Absturz bei der Wiedergabe von Datentyp/Farbmanagement auf Benutzerkanal
* [Farbmanagement] Die Farbauswahl wählt im Legacy-Modus nicht den richtigen Wert für den Datenkanal aus
* [Farbmanagement][Iray] Das Speichern des Renderings auf EXR oder TIFF, während das Farbmanagement im Viewport aktiviert ist, wird immer linear gespeichert
* [Farbmanagement] Ressourcen, die als Graustufen in Masken verwendet werden, zeigen das falsche Farbraummenü an
* [Farbmanagement][Iray] Die Env-Map ist immer linear, wenn sie in Iray verwendet wird
* [Farbmanagement][Exportieren] Konvertierte Karten werden nicht als farbverwaltete Kanäle exportiert
* [Farbmanagement][Exportieren] Der Export ignoriert, wenn der Benutzerkanal farbverwaltet ist oder nicht im Legacy-Modus ausgeführt wird

### 7.3.1

*(Freigegeben: 24. November 2021)*
Zusammenfassung: **Bugfix**

**Hinzugefügt:**

* [Projektion] Skalierung sollte nur im Objektbereich funktionieren

**Fest:**

* [Mac M1] Material-Ebene funktioniert nicht
* [Mac M1][Projektion] Verkrümmung funktioniert nicht
* Micro-Details werden nicht richtig angezeigt
* [Projektion][Absturz] Wechseln in den Verkrümmungsmodus mit einer Ebene, die mit einer Vorgängerversion erstellt wurde
* [Projektion][Verkrümmen] Spiegeln funktioniert nicht, wenn die Transformation auf Welt-Raum festgelegt ist
* [Projektion][Verformen] Die Option &quot;Teilen&quot; bleibt nach dem Teilen ausgewählt.
* [Projektion][UV] Der Drehpunkt wird beim Spiegeln der Projektion zurückgesetzt.
* [Filter] Baking Die Beleuchtungsumgebung ändert sich beim erneuten Laden oder Ändern eines Parameters
* [Interoperabilität] Nicht verfügbar für Steam- und Substance-Editionen
* [Interoperabilität] Die Schaltfläche &quot;3D-Assets auf dem Marktplatz durchsuchen&quot; sollte immer CCD auf der Registerkarte &quot;Stock &amp; Marketplace 3D&quot; öffnen.

**Bekannte Probleme:**

* [Mac M1] Intelligenten Materials werden nicht korrekt angezeigt

### 7.3.0

*(Freigegeben: 13. Oktober 2021)*
Zusammenfassung: **Hauptversion. Es enthält eine neue 3D-Verkrümmungsfunktion, eine neue zylindrische Projektion, Projektionen am Farbwähler, neue Funktionen in der Python-API und Fehlerbehebungen**

**Hinzugefügt:**

* [Projektion][Verkrümmen] Gelegt 3D-Verkrümmung als neue Projektion
* [Projektion][Verformen] Erlauben Sie den Aufklebermodus für Alphas, Texturen und Prozedurale mit Drag &amp; Drop im Viewport
* [Projektion][Verkrümmen] Verwenden Sie die Verkrümmungs-Projektion mit dem Decal-Tastaturbefehl (ALT).
* [Projektion][Verkrümmen][Symbolleiste] Transformieren Verkrümmung als Ganzes oder pro Scheitelpunkt
* [Projektion][Verkrümmen][Symbolleiste] Fügen Sie Raster-Punkte mit den Optionen &quot;Geteilte Verkrümmung&quot; quer, horizontal oder vertikal hinzu
* [Projektion][Verkrümmen][Symbolleiste] Dediziertes Menü für Zurücksetzen-Aktionen
* [Projektion][Verkrümmen][Symbolleiste] Option zum automatischen Anpassen der Tangenten beim Verschieben von Punkten
* [Projektion][Verkrümmen][Symbolleiste] Spezielles Menü für die Raster-Edition (Größe, Zurücksetzen, Farbe und Griffgröße)
* [Projektion][Verformen] Neuer Tastatur-Tastaturbefehl zum Schalten des Warp-Editionsmodus für ganze Scheitelpunkt (UMSCHALT+V)
* [Projektion][Verformen] Klicken+Strg ermöglicht den Wechsel zwischen Flächenwerkzeug und anderen Werkzeugen
* [Projektion][Zylindrisch] Gelegt Projektion
* [Projektion][Symbolleiste] Gruppeneinstellungen für Manipulator (Größe, Raster, Winkelschritte)
* [Farbwähler] Neue Benutzeroberfläche für Farbwähler
* [Farbwähler] Verwenden von sRGB-Werten in Farbwähler-Widgets
* [Farbwähler] Farbfelder speichern und löschen
* [Farbwähler] Pipette, die über Farbkanäle und normale Slots zugänglich ist
* [Farbwähler] Dynamische Farbe zwischen 0 und 255 Werten bearbeiten
* [Farbwähler] Gemeinsamer HSV-/RGB-Status in der App
* [Farbwähler] Das Fenster &quot;Farbwähler&quot; ist halbpersistent.
* [Farbwähler] Durch Drücken von Esc wird das Farbwählerfenster geschlossen.
* Leistungsverbesserung für UI-Interaktion und beim Malen
* [Engine] Update auf die neue Substance-Engine-Version (8.3.0)
* [Scripting][Python] Ermöglicht das erneute Laden des Meshs des aktuellen Projekts.
* [Scripting][Python] Aktualisieren von Ressourcen in Projekten zulassen
* [Scripting][Python] Festlegen und Abfragen der Auflösung von UV-Kacheln zulassen
* [Interoperabilität] Nicht verfügbar für Steam- und Substance-Editionen
* [Interoperabilität] Empfangen mehrerer Ressourcen von Bridge

**Fest:**

* Der Farbwähler zeigt nicht die richtige Farbe an
* [Baking] Liste der Textursatz ist nicht korrekt angeordnet
* [FBX Import] 3ds Max-Gruppen-Pivot-Transformationen werden nicht berücksichtigt
* [Substance Engine] Absturz beim Importieren von beschädigtem SBSAR
* [MacOS] Projektkonfigurationsoption in verschiedenen Sprachen ist nicht vorhanden.
* Automatische Speicherung kann Painter während langer Prozesse einfrieren

**Bekannte Probleme:**

* [Projektion][Verformen] Die Option &quot;Teilen&quot; bleibt nach dem Teilen ausgewählt.
* [Projektion][Verkrümmen] Spiegeln funktioniert nicht, wenn die Transformation auf Welt-Raum festgelegt ist
* [Projektion][Verformen] Artefaktlinien zwischen Patches in seltenen Fällen
* [Projektion][UV] Der Drehpunkt wird beim Spiegeln der Projektion zurückgesetzt.
* [Mac M1] Intelligenten Materials werden nicht korrekt angezeigt
* [M1][Regression] Material-Layer funktioniert nicht

### 7.2.3

*(Freigegeben: 24. August 2021)*
Zusammenfassung: **Nebenversion, Bugfix**

**Hinzugefügt:**

* [Bibliotheken] Hinzufügen einer Möglichkeit, unerwünschte Dateien vom Durchsuchen auszuschließen

**Fest:**

* [Win] Mehrere Bildschirme und Schlafprobleme
* [MacOS][Absturz] Wechseln des Shader bei Verwendung von Effekten
* [Viewport] Im vollständigen Vorschaumodus wird der Pinselcursor nicht mehr ohne Alpha angezeigt.
* [UI] Winkel-Widget schlägt falsch
* [Ebenenstapel] Viele Unterordner erstellen eine sehr lange Einfrierung
* [Iray] Verschiedene Ansichten in Iray und OpenGL: Sichtbar, wenn nicht funktionierend
* [Iray] Brechungsindex wird nicht berücksichtigt und erscheint nicht in den mdl-Eigenschaften
* [JavaScript] ShowExportDialog() gibt nie true zurück.
* Kann keine MTL aus Adobe Stock lesen

### 7.2.2

*(Freigegeben: 27. Juli 2021)*
Zusammenfassung: **Nebenversion, Bugfix**

**Hinzugefügt:**

* Aktualisieren Sie die Version der AMD-Treiberanforderungen

**Fest:**

* [Mac M1] Falsche Speichererkennung
* [Exportieren] Sehr lange Pfade werden nicht richtig angezeigt

**Bekannte Probleme:**

* [Inhalt] Veraltete Shader der Samples

### 7.2.1

*(Freigegeben: 2. Juli 2021)*
Zusammenfassung: **Nebenversion, Hotfix**

**Hinzugefügt:**

* [Interop] Fügen Sie eine QuickInfo hinzu, die darüber informiert, dass das Senden von UV-Kachel-Projekten an Stager noch nicht unterstützt wird.
* [Plug-in][UI] Aktualisierung des LiveLink-Symbols

**Fest:**

* [NVIDIA] Treiberversion ab 30 gilt als veraltet
* [Bibliotheken] Der Status des Bedienfelds &quot;Elemente&quot; wird nur gespeichert, wenn ein Projekt geöffnet ist
* [Bibliotheken] Neue gespeicherte Suche behält Stichwörter aus alter gespeicherter Suche bei
* [Baker][UVTiles] ID-Map pro MeshID berücksichtigen auch UV-Kacheln
* [Exportieren] gLTF-Dateien importieren keine Scheitelpunkt-Farbe
* [Iray] Einige QuickInfos fehlen
* [Interop] Senden an Stager ist nicht immer deaktiviert, wenn Stager nicht erkannt wird
* [Resource Updater] Photoshop-Pinselmaker kann nicht aktualisiert werden.
* [Inhalt] Glasfaser-Kantenverschleißgenerator ist defekt

### 7.2.0

*(Freigegeben: 23. Juni 2021)*
Zusammenfassung: **Die Hauptversion bietet eine Aktualisierung des Bedienfelds &quot;Elemente&quot;, einen neuen Shader mit Zugriff auf neue Kanäle und Parameter, eine allgemeine Aktualisierung der Benutzeroberfläche, einige dringend angeforderte Leistungsverbesserungen, erweiterte Sprachunterstützung und vieles mehr!**

**Hinzugefügt:**

* [Bibliotheken] Neues Bedienfeld &quot;Elemente&quot;, um das Regal zu ersetzen
* [Bibliotheken][UI] Neues Bedienfeld &quot;Elemente&quot;
* [Bibliotheken][UI] Ändern der standardmäßigen Ausrichtung des Bedienfelds &quot;Elemente&quot; und der Benutzeroberfläche
* [Bibliotheken][Benutzeroberfläche] Einführung einer Listenansichtsoption in die Bibliothek
* [Bibliotheken][UI] Neue Breadcrumbs-Navigation im Bedienfeld &quot;Elemente&quot;
* [Bibliotheken][UI] Wählen Sie &quot;Alle Bibliotheken&quot; aus, wenn Sie eine gespeicherte Suche auswählen.
* [Bibliotheken][UI] Wählen Sie &quot;Alle Bibliotheken&quot;, wenn alle Ordner deaktiviert sind.
* [Partikeln][UI] Neues Tag für Bibliothekspinsel
* [Libraries][UI] &quot;Regal&quot; wurde durch &quot;Alle Bibliotheken&quot; in der gesamten App ersetzt
* [Bibliotheken][UI] Leere Ordner ausblenden
* [Bibliotheken][UI] Die Standardbenutzerbibliothek sollte auch dann sichtbar sein, wenn sie leer ist
* [Libraries][UI] Neue Datenmethode über die Symbole des Elementtyps
* [Bibliotheken] Tastaturbefehl &quot;STRG&quot;, um mehrere Elementtypen auszuwählen
* [Bibliotheken] Neue Umgebungsvariable zur Steuerung des Speicherbudgets für die Elementvorschau
* [Bibliotheken][Inhalt] Neue Umgebungs-Map
* [Libraries][Content][UI] Versatz auf Standard-Materialien rendern
* [Libraries][Content] Legen Sie den ASM-Shader (Adobe Standard Material) als Standard für die Vorschaugenerierung fest.
* [Libraries][Content][ASM] Neue Projektvorlagen für neuen ASM-Shader
* [Bibliotheken][Miniaturansicht] Neue Studio 6-Umgebungs-Map verwenden
* [Bibliotheken][Miniaturansicht] Miniaturansicht in Ressource lesen, anstatt sie zu generieren
* [Bibliotheken][Miniaturansicht] Versatz zur Miniaturgenerierung hinzufügen
* [Textursatz-Einstellungen]
* [Textursatz Settings][UI] Neues Height zur normalen Konvertierungsmethode Gelegt
* [Kanaleinstellungen][UI] Überarbeitung der Benutzeroberflächenorganisation der Textursätze
* [Kanaleinstellungen] Benutzerkanallimit auf 16 Textursätze erhöht
* [Kanaleinstellungen][UI] Geben Sie an, welche Textursätze mit dem aktuell ausgewählten Shader kompatibel sind.
* [Shader][ASM] Neuer Adobe Standard Material-Shader
* [Shader][ASM] Unterstützung für Anisotropie, Clear Coat, Volumenstreuung, Specular edge color und Glanz hinzugefügt
* [Shader][ASM] Ändern der Farbwerte der Standardkanäle
* [Shader][ASM][Exportieren] Aktualisierte Exportvorlage Adobe Dimension zu Adobe Substance 3D Stager
* [Shader][ASM] Beschriftungen und QuickInfos für Shader- und MDL-Parameter hinzugefügt
* [Shader][ASM] Sichtbarmachen der Streuung-Farbe in der 2D-Ansicht, auch wenn SSS nicht unterstützt wird
* [Shader][ASM][Iray] Unterstützung von ASM-Shader in Iray mit neuer MDL
* [Shader][ASM][Iray] Aktualisierte Volumenstreuung in veraltetem PBR-Spezifikationsglanz und beschichtet
* [Shader][ASM][Content] Der Standard-SSS-Typ für Samples wurde geändert.
* [Shader][ASM] Zusätzliche Dokumentation für ASM API
* [Shader][ASM] Optimieren Sie Shader, um nicht genutzte Kanäle zu ignorieren.
* [Shader] Leg neuer Textursatz-Kanäle
* [Shader] Verbesserte Volumenstreuung
* [Shader] Neue Shader-Parameter für einige Shader wurden ausgeblendet
* [Shader] Sichtbar, wenn für Shader-Parameter
* [Leistung]
* [Bibliotheken] Verbesserungen der Ladezeit der Ressourcenvorschau und der Berechnungsleistung
* [Engine] Verbesserte Malleistung
* [Automatisch Entpackt]
* [Automatisch Entpackt] Leistungsverbesserungen bei Packing
* [Automatisch Entpackt] Automatisch entpackt, kompatibel mit dem Workflow der UV-Kachel
* [Automatisches Entpacken] Neue Option zur Positionierung von UVs entsprechend der Ausrichtung des Meshs
* [Sonstige]
* [Einstellungen] Standardzoomrichtung geändert
* [UI] Gesamte Aktualisierung der Benutzeroberfläche
* [UI] Überarbeitung des Hilfemenüs
* [UI] Symbol &quot;Umkehren ersetzen&quot;
* [UI][Plug-In] Symbol &quot;Ersetzen&quot; für den DCC-Link des Plug-Ins
* [UI][AMD] Mindest erforderliche Version aktualisieren und Popup-Nachricht
* [Ebenenstapel] Neue Ebene innerhalb des ausgewählten leeren Ordners erstellen
* Python-Dokumentation aktualisieren
* [Branding]
* [Branding][UI] Der Anwendungsname wurde in Adobe Substance 3D Painter aktualisiert.
* [Branding][UI] Eigenständige Version auf &quot;Substance Edition&quot; aktualisiert
* [Branding][UI] Aktualisierter Name der ausführbaren Datei der Anwendung, Installationspfad, Paket und Symbole
* [Branding][UI] Standardbibliothek und -pfad wurden umbenannt
* [Branding][UI] Aktualisiert über das Fenster
* [Branding][UI] Aktualisierter Begrüßungsbildschirm
* [Branding][UI] Die jährliche Versionsnummer wurde entfernt.
* [Lokalisierung] Neue Übersetzungen in Deutsch, Französisch und vereinfachtem Chinesisch
* [Interoperabilität] Nicht verfügbar für Steam- und Substance-Editionen
* [Interoperabilität] Interoperabilität mit dem Adobe-Ökosystem: Designer, Sampler, Stager und Bridge
* [Interoperabilität][Benutzeroberfläche] Empfangen und Aktualisieren von Elementen aus Designer
* [Interoperabilität][Benutzeroberfläche] Empfangen von Elementen aus Sampler
* [Interoperabilität][UI] Element an Stager senden
* [Interoperabilität][Benutzeroberfläche] In Adobe Bridge anzeigen
* [Interoperabilität][UI] Schneller Zugriff auf Adobe 3D-Elemente
* [Interoperabilität] Neue Verwendungs-Tags von sbsar
* [Interoperabilität] Umgang mit empfangenen Elementtypen
* [Interoperabilität] Von Adobe Substance 3D Designer oder Adobe Substance 3D Sampler empfangene Elemente werden in der vom Benutzer standardmäßig ausgewählten Bibliothek gespeichert.
* [Interoperabilität][Benutzeroberfläche] Neues Symbol in der linken Symbolleiste zum Senden an Stager oder Photoshop

**Fest:**

* [Tablet] Geringe Leistung beim Malen mit Druck
* [Tablet] Problem auf Tablets mit Schiebereglern
* [Absturz] Namenskonflikt zwischen der Liste der Textursatz und dem Exporter
* [Absturz][Bibliotheken] Doppelklicken Sie auf eine Unterbibliothek.
* [Bibliotheken] Problem beim Durchsuchen von Bibliotheksverzeichnissen
* [Bibliotheken] Befehlszeile zum Erzwingen der Vorschaugenerierung funktioniert nicht wie erwartet
* [Libraries][Content] Der Baking geführt Lichtumgebungsfilter ist standardmäßig schwarz.
* [Linux][MacOS][Mesh exportieren] Kann unter Linux/MacOS erstellte glTF nicht importieren
* [Linux] Das Ziehen und Ablegen einer Datei in das Bedienfeld &quot;Asset&quot; kann zu einem Absturz führen
* [Automatisches Entpacken] Automatisches Entpacken ist auch dann verfügbar, wenn kein Mesh zum erneuten Laden ausgewählt wurde
* [Partikeln] Falsche Partikel mit Schwerkraft
* [Ebenenstapel] Ebenen-Histogramm kann nur Luminanz mit einigen Kanälen verwenden
* [Geometriemaske] Rechtsklick-Menü auf einen Ordner beim Bearbeiten der Geometriemaske funktioniert nicht
* [Projektion] Naht mit sphärische Projektion und bilinearen Filterungen
* [UV-Kacheln] Exportmaske in Datei exportiert nur Kachel 0, 0
* [Mesh exportieren] FBX Mesh-Export ist leer.
* [Iray] Normalen-Map wird beim Rendern in neuen Projekten nicht berücksichtigt
* [Speichern] Speichern von Problemen auf freigegebenen Laufwerken
* [Baking] Beim erneuten Erstellen eines Meshs mit geänderten Parametern wird eine Warnung angezeigt.
* [Baking][Regression] Falsches Ergebnis, wenn der globale Begrenzungsrahmen des hohen Poly-Meshs den Ursprung der Szene nicht enthält
* [Python] Benutzerdefinierte Benutzerbibliotheken werden nicht berücksichtigt

**Bekannte Probleme:**

* [Bibliotheken] Gespeicherte Suchen werden nicht gespeichert, wenn kein Projekt geöffnet wird
* [NVIDIA] Meldung für veralteten Treiber, selbst wenn der Treiber auf dem neuesten Stand ist

### 7.1.1 (2021.1.1)

*(Freigegeben: 23. März 2021)*
Zusammenfassung: **Nebenversion, Bugfix mit der Möglichkeit, Hexadezimalwerte in den Farbwähler einzugeben**

**Hinzugefügt:**

* [Protokoll] Benutzer über inkompatible AMD-GPU-Treiber warnen
* [Farbwähler] Hexadezimalwerte können eingegeben werden

**Fest:**

* [Baker] Leistungseinbruch
* [Geometriemaske] Alt-Klick auf Mesh-Namen kann zu einem Absturz führen
* [Engine] Beim Malen wird bei Bedarf nicht die gesamte Ansicht aktualisiert
* [Ebenenstapel] Auswahl bleibt nach dem Ändern des Shader hängen
* [MacOS][Farbwähler] Die Farbe ist etwas anders als die ausgewählte
* [Exportieren] Bei Verwendung des PSD-Dateiformats wird nicht eine Datei pro UV-Kachel generiert.
* [Scripting][Javascript] alg.mapexport.getPathsExportDocumentMaps() gibt nicht alle Werte zurück.
* [Scripting][Python] Deaktivierte Plug-ins werden beim erneuten Öffnen von Painter wieder aktiviert

### 7.1.0 (2021.1.0)

*(Freigegeben: 28. Januar 2021)*
Zusammenfassung: **Hauptversion, neue Geometriemaske, mit der Teile der UV-Kachel ausgewählt und Malen werden können, Kopier-/Einfügeeffekte im Ebenenstapel, verbesserte Geometriemaske, Aktualisierung von Iray, Bakern, Substance Engine und neuen Inhalten**

**Hinzugefügt:**

* Neue Geometriemaske und Malen ausgewählter Teile der Geometrie
* [Geometriemaske] Erlaubt das Malen ausgewählter Geometrieteile nach Mesh-Namen.
* [Geometriemaske] Rechteckige Auswahl in beiden Viewporten
* [Geometriemaske] Ausgeschlossene Geometrie auf einer Ebene ausblenden/ignorieren
* [Geometriemaske][Eigenschaften] Schnellauswahl für Kontrollkästchen mit Klicken und Ziehen
* [Geometriemaske][Eigenschaften][UI] Alle Elemente mit einer Dropdown-Liste im Eigenschaftenfenster einschließen/ausschließen
* [Geometriemaske][Eigenschaften] Ermöglicht die schnelle Auswahl eines Elements in einer Liste mit ALT+LINKSKLICK.
* [Geometriemaske][Eigenschaften] Überlagerung in Viewporten beim Zeigen auf Mesh-Namen/UV-Kacheln im Eigenschaftenfenster
* [Geometriemaske][Ebenenstapel] Hinzufügen von Kopier-/Einfügeoptionen zur Geometriemaske
* [Geometriemaske] Neues Symbol für Schaltfläche &quot;Ausgeschlossene Geometrie ausblenden/ignorieren&quot;
* [Geometriemaske] Neue QuickInfo für Ausgeschlossene Geometrie ausblenden/ignorieren
* [Geometriemaske] Drücken Sie ALT+H, um die Schaltfläche &quot;Ausgeschlossene Geometrie ignorieren&quot; ein- oder auszublenden. Tastaturbefehl:
* [UV-Kacheln][Ebenenstapel] Neue Miniaturansicht der Kugelvorschau der Füllebene für UV-Kacheln und vereinfachten Modus
* [UV-Kacheln][Ebenenstapel] Ermöglicht das einfache Beenden der UV-Kachel
* [UV-Kacheln][Liste der Textursatz] Ermöglicht die Angabe einer Beschreibung pro UV-Kachel.
* [UV-Kacheln][Textursatz-Einstellungen][UI] Zwei neue Abschnittstitel im Dropdown-Menü zum Ändern der Auflösung der UV-Kachel
* [UV-Kacheln][Viewport] UV-Kachel-Maske beenden, wenn ein Material in den Viewport gezogen wird
* [Ebenenstapel] Optionen zum Kopieren/Einfügen für Effekte hinzufügen
* [Ebenenstapel] Kopieren/Einfügen von Effekten von einem Textursatz in einen anderen zulassen
* [Ebenenstapel] Mehrfachauswahl von Effekten zulassen
* [Ebenenstapel] Hinzufügen von Kopier-/Einfügeoptionen als Verknüpfungen für Ebeneneffekte
* [Ebenenstapel] Automatisch zwischen Maske und Inhalt wechseln, wenn Effekte auf eine andere Ebene gezogen werden
* [Ebenenstapel] Beim Einfügen einer Maske aus einer anderen Ebene automatisch eine Maske erstellen
* [Ebenenstapel] Hinzufügen von Verschiebungseffekt-Aktionen im Kontextmenü der Effekte
* [Ebenenstapel] Ziehen und Ablegen von Effekten von einer Ebene in eine andere zulassen
* [Ebenenstapel] Wenn Elemente in einen Ordner gezogen werden, werden sie oben im Ordner abgelegt.
* Iray auf Version 2020.1.0 aktualisieren
* [Baker] Baker auf Version 2.5.4 aktualisieren
* [Baker] Einzelne UV-Kacheln im Fenster &quot;Baking-Fortschritt&quot; anzeigen
* [Baker][UI] Ermöglicht das schnelle Baking des aktuellen Textursatzes mit einer neuen Schaltfläche.
* [Baker] Benutzer können mit ALT+LINKSKLICK schnell einen der Baker auswählen
* Substance Engine auf Version 8.0.8 aktualisieren
* [Substance Engine] Unterstützung der Standardfarbe in neuen .sbsar-Dateien
* [Automatisch Entpackt] Leistungsverbesserung
* [Exportieren] Fügen Sie visuelles Feedback hinzu, um anzugeben, welche Auflösung der UV-Kachel von der Standardauflösung des Projekts abweicht
* [Exportieren] Szene-Größenfaktor zur exportierten Shader-JSON-Datei hinzufügen
* [Sprache] Japanische Übersetzung hinzufügen
* [UI] Aktualisierung des Fensters mit Versionierung interner Abhängigkeiten
* [Scripting][Python] Verwaltung von Regal-Ressourcen zulassen
* [Scripting][Python] Ermitteln Sie, wann ein Projekt zum Baking und Exportieren bereit ist.
* [Scripting][Python] Ermitteln Sie, wann ein Regal das Crawlen von Ressourcen auf der Festplatte abgeschlossen hat.
* [Scripting][Python] Abfragen der Liste der UV-Kacheln pro Textursatz zulassen
* [Scripting][Python] Weisen Sie Regal-Ressourcen eine benutzerdefinierte Vorschau zu
* [Scripting][Python] Verwalten benutzerdefinierter Regal zulassen
* [Scripting][Python] Hinzufügen eines Methodenindexes in jedem Untermodul in der Dokumentation
* [Scripting][Python] Neuer Stil für die Dokumentation
* [Scripting][Python] Verbesserung der Ressourcen- und Regal-Dokumentation
* [Content] Drei neue Werkzeugvorgaben zum Nähen
* [Regal] Entfernen Sie vorübergehend &quot;Exportieren auf Substance share&quot;, während Sie zur neuen Substance share-Plattform wechseln.

**Fest:**

* Absturz bei Monitoren mit unterschiedlichen Auflösungen
* Absturz im Substance Engine mit einigen seltenen Projekten
* Die Aktualisierung des Viewports schlägt beim Wechseln von Ebenen mit &quot;Ausgeschlossene Geometrie ausblenden/ignorieren&quot; fehl.
* [2D-Ansicht] Bei einigen Projekten kann 2D-Viewport fehlen
* [Baking] &quot;Übereinstimmung nach Mesh&quot; ignoriert Teile des Objekts
* [Ebenenstapel] Durch Klicken auf einen Ebeneneffekt wird der Ordner geöffnet.
* [Geometriemaske] UV-Kachel wird in der Maske immer noch gezählt, auch wenn der Mesh ohne sie erneut importiert wird
* [Geometriemaske] Das Kontextmenü im Viewport bietet nicht die richtigen Werkzeuge
* [Engine] Schwerwiegende Verzögerungen bei bestimmten Projekten
* [Scripting] Hohe Latenz bei Anforderungen an Remote-JSON-POST unter Windows
* [Linux] Vram-Menge wird bei bestimmten integrierten GPUs nicht richtig erkannt
* [Automatisch Entpackt] Absturz oder lange entpack an einigen Projekten

## Version 6

### 6.2.2 (2020.2.2)

*(Freigegeben: 28. September 2020)*
Zusammenfassung: **Nebenversion, Bugfix mit einigen Funktionen in der Python-API**

**Hinzugefügt:**

* [Leistung] Nicht alle UV-Kacheln bei Verwendung der Farb-ID berechnen
* [Baker][UI] Textursatz-Beschreibungen anzeigen
* [Baker] Speichern von Baking-Einstellungen zulassen
* [Baker] Hinzufügen aller reduzierten/erweiterter Optionen zur Registerkarte &quot;Auswahl&quot;
* [Liste der Textursatz] Beschreibung ausblenden, wenn leer
* [UV-Kacheln][Liste der Textursatz] Durch Klicken auf die UV-Kachel sollte die Liste erweitert/reduziert werden.
* [Exportieren][UI] Horizontales Ändern der Größe des Bedienfelds &quot;Textursatz-Liste&quot; zulassen
* [Exportieren][UI] Konsistenter QuickInfo-Text für UV-Kacheln und Textursatz-Arbeitsablauf mit nicht ausgewählten Texturen
* [Scripting][Python] Verwenden von Exportvorgaben zum Exportieren von Texturen zulassen
* [Scripting][Python] Hinzufügen eines Änderungsprotokolls in der Dokumentation
* [Scripting][Python] Ermöglicht die Abfrage aller verfügbaren Kanäle auf einem bestimmten Stapel.
* [Scripting][Python] Verbesserungen der Konsolen-Benutzeroberfläche

**Fest:**

* [AMD] Falsche Erkennung veralteter Treiberversionen
* Absturz beim erneuten Importieren eines Meshs mit unterschiedlichem UV-Kacheln-Layout in einigen Fällen
* Absturz bei der Verwendung von Partikeln mit UDIM auf sehr schweren Meshs
* [UV-Kacheln] Absturz beim Exportieren eines Meshs mit Versatz-Informationen in einigen Fällen
* [Exportieren][Absturz] Exportieren von 2D-Ansichten im PSD-Format kann einen Absturz verursachen
* Das Importieren von Bildern als Sequenzen beim Erstellen eines Projekts funktioniert nicht
* Engine in einer Endlosschleife
* [Tastaturbefehl] Kamera dreht sich immer im einrasten Modus, wenn die Kurzbefehle für den einrasten Modus geändert werden
* Mesh werden immer automatisch entpackt, wenn sie erneut importiert werden, auch wenn die Option deaktiviert ist
* [Liste der Textursatz] Das Textfeld &quot;Beschreibung&quot; ist in der Edition manchmal nicht vollständig sichtbar.
* [Liste der Textursatz] Dropdown-Menü zum Ein-/Ausblenden von Textursätzen ist nicht vollständig sichtbar
* [Liste der Textursatz] Wenn Sie auf das Augensymbol klicken, sollte nicht der Name &quot;Textursatz bearbeiten&quot; eingegeben werden.
* [Kanaleinstellungen] Beim Entfernen eines Textursatzes wird auch der darunter liegende Kanal entfernt
* [Exportieren] Alle einschließen und Alle zurücksetzen berücksichtigt keine UV-Kacheln
* [Baker] Während des Bakings werden nicht ausgewählte Baker angezeigt.
* Die Behebungsaktualisierung wird bei durch Baking erzeugte Map als Eingabe nicht berücksichtigt
* [UV-Kacheln][Viewport] 3D-Viewport friert ein, wenn Intelligente Material nach UV-Kachel mit ausgewählter Ordnermaske hinzugefügt wird
* [UV-Kacheln][Viewport] Drahtgitter ist weiterhin für ausgeblendete Kacheln sichtbar, wenn der Modus &quot;Malen durch&quot; aktiviert ist.
* [Export][Sketchfab] Probleme mit dem Abonnementtyp &quot;Plus&quot;
* [Sketchfab] Das Kontrollkästchen &quot;Dieses Asset ist privat&quot; wird nach dem Kontowechsel nicht angezeigt
* [Exportieren][Inhalt] &quot;Verwackelt&quot;-Pinselvorgaben können zu Leistungsproblemen führen
* [Plugin Photoshop] Meldung im Protokoll: nicht kompatibel mit dem UV-Kachel-Workflow
* [Scripting][Python] PYTHONPATH env var verhindert den Start der Anwendung
* [Scripting][Python] Typo in der Python-Dokumentation

### 6.2.1 (2020.2.1)

*(Freigegeben: 29. Juli 2020)*
Zusammenfassung: **Nebenversion, Hotfix**

**Hinzugefügt:**

* Umgebungsvariable &quot;SUBSTANCE\_PAINTER\_VRAM\_BUDGET&quot; hinzufügen, um GPU-VRam-Wert zu überschreiben
* [UV-Kacheln][Leistung] Nicht alle UV-Kacheln bei Verwendung des Polygon-Füllwerkzeugs berechnen

**Fest:**

* [Iray] Beim Speichern des Renderings wird ein Fehler zurückgegeben, der zu einem schwarzen Bild führt
* [Linux] Absturz nach dem Begrüßungsbildschirm unter CentOS 7.3
* [Linux] Vram-Menge wird bei bestimmten Konfigurationen nicht richtig erkannt
* [Absturz] Öffnen eines Projekts mit dem Namen des duplizierten Textursatzes
* [Engine] Cache-Invalidierungsproblem beim Ändern einer Maske
* [Liste der Textursatz] Falscher Schrifteffekt, wenn Textursatz deaktiviert ist

**Bekannte Probleme:**

* [Liste der Textursatz] Die Beschreibung kann nicht ausgeblendet werden.
* [Textursatz List] UI-Probleme
* [Iray] PSD-Rendering wird nicht geöffnet
* [Plug-In Photoshop] Nicht kompatibel mit dem Arbeitsablauf für UV-Kacheln

### 6.2.0 (2020.2.0)

*(Freigegeben: 23. Juli 2020)*
Zusammenfassung: **Hauptversion mit neuem UV-Kacheln-Workflow, Malen über UV-Kacheln hinweg und Leistungsverbesserung**

**Hinzugefügt:**

* UV-Kacheln (UDIM)
* [UV-Kacheln] Malen über UV-Kacheln
* [UV-Kacheln] Auswahl zwischen neuem und veraltetem Arbeitsablauf für UV-Kacheln zulassen
* [UV-Kacheln] Importieren von UDIM/UV-Kachel-Bildsequenzen als Ressource
* [UV-Kacheln] Liste der UV-Kacheln pro Textursatz im Fenster &quot;Liste der Textursatz&quot; hinzufügen
* [UV-Kacheln] Erlauben Sie, die Auflösung mehrerer UV-Kacheln gleichzeitig in den Textursatz-Einstellungen zu bearbeiten.
* [UV-Kacheln][2D-Ansicht] UV-Kacheln als Raster anzeigen
* [UV-Kacheln][2D-Ansichten] Neue Viewport-Schaltfläche zum Anzeigen oder Ausblenden von UV-Kacheln-Informationen
* [UV-Kacheln] Wechseln des Malwerkzeugs für UV-Kachel-Projekte standardmäßig zum Ein Kanal
* [UV-Kacheln] Neue Schaltfläche in der kontextabhängigen Symbolleiste, um maskierte UV-Kacheln beim Malen zu ignorieren
* [UV-Kacheln][Ebenenstapel] Neue Ebenenstapel-Symbole zur Leistungssteigerung
* [UV-Kacheln][Ebenenstapel] Verbessern der Symbole &quot;Malen und Füllen&quot; in der Symbolleiste
* [UV-Kachel Maske][2D-Ansicht] Mehrere UV-Kacheln gleichzeitig ein- oder ausschließen (Linksklick, Strg+Linksklick)
* [Ebenenmaske] Neue Ebenenmaske zum Einschließen, Ausschließen von Kacheln pro UV-Kachel mit neuem Symbol
* [UV-Kacheln-Maske][Ebenenstapel] Zeigt die Anzahl der UV-Kacheln im UV-Kacheln-Maskensymbol an, wenn nicht alle eingeschlossen sind.
* [UV-Kachel-Maske][2D/3D-Ansicht] Fügen Sie einen Hover-Effekt hinzu, um UV-Kacheln unter dem Cursor darzustellen.
* [UV-Kacheln][Baker] Auswahl und Baking bestimmter UV-Kacheln zulassen
* [UV-Kacheln][Baker] Hinzufügen von Auswahloptionen für Textursatz/UV-Kacheln
* [UV-Kacheln][Baker] Kontextmenüoption zum Auswählen von UV-Kacheln in einem Textursatz
* [UV-Kacheln][Baker] Ermöglichen Sie eine schnelle Auswahl im Textursatz/in den UV-Kacheln durch Ziehen
* [UV-Kacheln][Baker] Ersetzen Sie die Schaltflächen &quot;Alle&quot; und &quot;Keine&quot; in Mesh-Map durch explizitere Auswahloptionen.
* [UV-Kacheln][Baker] Anzahl der zu Baking führend Texturen anzeigen
* [UV-Kacheln][Exportieren] Auswahl und Export bestimmter UV-Kacheln zulassen
* [UV-Kacheln][Exportieren] Ermöglicht die schnelle Auswahl von UV-Kacheln durch Ziehen
* [UV-Kacheln][Exportieren] Dropdown-Menüoptionen für UV-Kacheln hinzufügen
* [UV-Kacheln][Exportieren] Stellen Sie einige Exportvorgaben nicht zur Verfügung, wenn sie nicht mit UV-Kacheln funktionieren (Adobe Dimension, Sketchfab, glTF, USD)
* [UV-Kacheln][Inhalt] Aktualisieren Sie die Exportvorgaben, um das neue $udim-Tag zu verwenden
* [UV-Kacheln] Verbessern der Fehlerberichterstattung beim Importieren von Meshs mit überlappenden UV-Inseln
* [UV-Kacheln] In Iray kompatible UV-Kacheln
* [UV-Kacheln][Skripterstellung] Hinzufügen einer UV-Kachel-Exportdokumentation zu Python-Dokumenten
* Leistung
* [Leistung] Neue Schaltfläche in der kontextabhängigen Symbolleiste, um die Berechnung des Engine bei der Arbeit anzuhalten (UMSCHALT+ESC)
* [Performance] Schnelleres Öffnen von Projekten durch Verzögerung der Textursatz-Cache-Berechnung
* [Performance] Warten Sie nicht, bis Mesh-Map beim Öffnen des Projekts geladen sind.
* [Performance][2D/3D-Ansicht] Der Maskenkanal im Viewport wird nicht berechnet, wenn er nicht verwendet wird.
* [Performance] Anwendung nicht blockieren, wenn Mesh-Map in den Viewporten geladen werden
* [Leistung] Verbessern der inkrementellen Speichergeschwindigkeit beim Speichern eines Projekts
* [Performance][Baker] Ändern Sie die Standardeinstellungen für die Ausdehnung, um Zeit und Projektgröße besser zu sparen.
* [Performance][Baker] Wechseln Sie auf bestimmten Bakern zu Graustufen, um Zeit und Projektgröße zu sparen.
* [Performance][Exportieren] Verbessern der Engine-Performance, um Texturen schneller zu exportieren
* [Performance][Export] Verbessern Sie die Reaktionsfähigkeit beim Öffnen des Exportdialogs mit vielen Textursätzen
* [Leistung][Export] Verbessern Sie die Leistung beim Wechsel zur Registerkarte &quot;Exportliste&quot;.
* [Performance][Iray] Verkürzen der Startzeit von Iray
* Sonstige
* [Baker] Hinzufügen von Auswahloptionen für Textursatz
* Shader-Instanzen-Management auf Textursatz-Einstellungen verschieben
* [2D/3D-Ansicht] Fügen Sie am unteren Rand des Viewports eine Nachricht hinzu, die angibt, welcher Maskentyp bearbeitet wird.
* [Ebenenstapel] Neue Option in den Einstellungen, um zwischen alten und neuen Miniaturansichten zu wechseln
* [Ebenenstapel] Fügen Sie visuelles Feedback hinzu, um den Ladezustand der Miniaturansichten anzuzeigen
* [Proj] Neue Projektion &quot;Fill (Match Per UV-Tile)&quot; zum Laden von Bildsequenzen
* [Proj] Ändern Sie den Modus &quot;Füllebenen-Projektion&quot; in &quot;Füllen (Per UV-Tile abgleichen)&quot; in bestimmten Fällen.
* [Content] Optimierung der Kohle-Pinselvorgaben zur Verbesserung der Performance
* Iray auf Version 2020.0.0 aktualisieren
* [Exportieren] Deaktivieren Sie die Registerkarte &quot;Exportliste&quot;, wenn nichts ausgewählt ist
* Automatisch Entpackt
* [Automatisch Entpackt] Verbessern der Erfolgsrate des automatischen entpack-Prozesses
* [Automatisch Entpackt] Verbesserte Parametrierung zur Erhöhung der Geschwindigkeit und Stabilität

**Fest:**

* [Alembic] Facesets werden beim Importieren von Dateien ignoriert
* [Alembic] Unendliche Ladezeit mit bestimmten Dateien
* [Importieren] Falsche UDIM-Bildsequenz wird importiert, wenn nur die Dateierweiterung unterschiedlich ist
* [Absturz] Der Versuch, ein Projekt zu öffnen, das durch einen anderen Prozess gesperrt wurde, führt zu einem Absturz
* [Projektion] Artefakte an dupliziertem Mesh bei Verwendung von triplanare Projektion
* [Exportieren] Emissive-Kanal wird nicht mit USD exportiert
* [Inhalt] Intelligente Material &quot;Kohle&quot; enthält Malen-Striche

**Bekannte Probleme:**

* [Liste der Textursatz] Die Beschreibung kann nicht ausgeblendet werden.
* [Textursatz List] UI-Probleme

### 6.1.3 (2020.1.3)

*(Freigegeben: 16. Juni 2020)*
Zusammenfassung: **Bugfix**

**Hinzugefügt:**

* [Exportieren] Hinzufügen von Versatz-Einstellungen in der JSON-Datei für Shader-Parameter

**Fest:**

* [Absturz][Engine] Absturz beim Löschen und Ersetzen vorhandener Kanäle
* [Absturz] Ändern des Shader nach dem Malen einer Maske in der Material-Ebene
* [Absturz][Engine] Absturz mit einigen umfangreichen Projekten
* [Baker] Zuordnung nach Name funktioniert nicht mit aus zBrush exportierten OBJ
* [Versatz][SVT] Texturen werden beim Öffnen des Projekts nicht angezeigt, wenn der Versatz aktiviert ist
* [Exportieren] Einige Texturen werden in einheitlichem Grau exportiert.
* [Exportieren] Deaktivierte Textursatz sollten nicht für Dimension- und Sketchfab-Exportvorgaben exportiert werden
* [Scripting][JavaScript]-Absturz bei der Verwendung der JavaScript-API für den Zugriff auf die Exportkonfiguration im onProjectOpened-Ereignis
* [Skripterstellung][Javascript] onExportFinished() wird nach einem Export nicht aufgerufen

### 6.1.2 (2020.1.2)

*(Freigegeben: 28. Mai 2020)*
Zusammenfassung: **Bugfix mit Substance Engine- und Baker-Update**

**Hinzugefügt:**

* [Baker] Update auf die neueste Version
* [Baker] Neue Sampling-Methode in den Bakern Ambient occlusion, Krümmung, Thickness
* Aktualisieren Sie auf die neueste Version von Substance Engine
* [Scripting][Python] Erstellen der ResourceID für Projektressourcen zulassen
* [Scripting][Python] Abfragen von Kanalinformationen zulassen
* [Scripting][Python] Fügen Sie Dryrun- und Rückruffunktionen hinzu, um den Export von Texturen zu simulieren

**Fest:**

* [Baker] Falsche Normale im Welt-Raum-Normale-Baker unter Verwendung einer Tangente-Normalen-Map in bestimmten Fällen
* [Baker] Fehler beim Baking von Ambient occlusion mit Optix, wenn kein hohes Poly
* [Dynamische Pinselstriche] Verzögerung beim Laden eines bestimmten Textursatzes
* [Exportieren] Die deaktivierten Textursatz für USD sollten nicht exportiert werden. glTF
* [Skripterstellung][JavaScript] Die Einstellungen für den neuen Krümmung-Baker können nicht bearbeitet werden.
* [Scripting][JavaScript] alg.texturesets.addChannel() gibt in einigen Fällen keinen Fehler zurück.
* [Scripting][JavaScript] Tippfehler in der JavaScript-API-Dokumentation für setProjectExportOptions()
* [Skripterstellung][JavaScript] Exportiert immer alle Textursatz
* [Scripting][Python] sys.executable gibt einen Pfad zu python.exe anstelle von Substance Painter zurück
* Textur-Cache nicht kompatibel mit Mac OS und Windows/Linux
* [Livelink UE4] Nur das letzte Material wird für alle Textursatz in einem kombinierten Mesh verwendet.

**Bekannte Probleme:**

* [Exportieren][Dimension][Skecthfab] Die deaktivierten Textursatz sollten nicht exportiert werden.
* [Absturz] Ändern des Shader nach dem Malen einer Maske in der Material-Ebene

### 6.1.1 (2020.1.1)

*(Freigegeben: 5. Mai 2020)*
Zusammenfassung: **Hotfix**

**Hinzugefügt:**

* [Export] Überschriebenes visuelles Feedback zu TextureSet

**Fest:**

* [Exportieren] Exporter-Fenstergröße ist auf einem Spezialauflösungsmonitor zu groß und kann nicht geändert werden
* [Export] Optionen werden nach dem Export nicht gespeichert
* [Exportieren] Absturz oder kann nicht mit der Exportvorgabe &quot;Aus Cache&quot; exportiert werden
* [Export] Wenn Sie den Export abbrechen, wird eine unerwartete zusätzliche leere Map generiert.
* [Exportieren] Virtuelle Exportvoreinstellungen korrigieren
* [Python] PYTHONPATH env var wird nicht berücksichtigt
* [Python][Export] Wenn Sie den Export über Python abbrechen, wird ein Ausnahmefehler zurückgegeben.
* [Python][Exportieren] export\_project\_Texturen falsches Ergebnis mit psd-Dateiformat
* [Baker] Absturz unter Linux mit GPU-Raytracing

**Bekannte Probleme:**

* [JavaScript] Die Baker-Einstellungen für neue Krümmungen können nicht bearbeitet werden.
* [JavaScript][Export] Exportiert immer alle Textursatz
* [Exportieren][USD] Die deaktivierten Textursatz sollten nicht exportiert werden.
* [Absturz] Ändern des Shader nach dem Malen einer Maske in der Material-Ebene

### 6.1.0 (2020.1.0)

*(Freigegeben: 22. April 2020)*
Zusammenfassung: **Hauptversion mit neuer Textur und neuem Mesh-Exporter (mit Versatz und Tessellation), aktualisiertem UV mit mehr Steuerelementen, neuen Bakern, neuer Scripting-Python-API, besserer UX für Decal-entpackte und neuem Inhalt**

**Hinzugefügt:**

* Exporter &quot;Neue Textur und neuer Mesh&quot;
* [Exportieren] Neue Exporter-Oberfläche
* [Exportieren][Registerkarte &quot;Exportieren&quot;] Ermöglicht die Auswahl der Kartenkanäle, die pro Textursatz exportiert werden.
* [Exportieren][Registerkarte &quot;Exportieren&quot;] Modifizierung der Größe des Textursatzes für alle Textursatz in einer Aktion zulassen
* [Exportieren][Registerkarte &quot;Exportieren&quot;] Lassen Sie eine andere Vorlage pro Textursatz zu (außer USD, glTF, Sketchfab und Dimension)
* [Exportieren][Registerkarte &quot;Exportieren&quot;] Schnelle Aktivierung und Deaktivierung von Karten und Textursätze
* [Exportieren][Registerkarte &quot;Exportieren&quot;] Die Exportauflösung 8192x8192 ist nicht mehr experimentell
* [Exportieren][Registerkarte &quot;Exportieren&quot;] Änderung des Dateiformats und der Bittiefe pro Map zulassen
* [Exportieren][Registerkarte &quot;Exportieren&quot;] Zurücksetzen auf die Werte der Standardparameter zulassen
* [Exportieren][Registerkarte &quot;Exportieren&quot;] Speichern von Einstellungen ohne Exportieren zulassen
* [Exportieren][Registerkarte &quot;Ausgabevorlagen&quot;] Benennen Sie die Registerkarte &quot;Konfiguration&quot; in die Registerkarte &quot;Ausgabevorlagen&quot; um
* [Exportieren][Registerkarte &quot;Ausgabevorlagen&quot;] Definition von Dateiformat und Bittiefe pro voreingestellter Map zulassen
* [Export][Registerkarte &quot;Liste der Exporte&quot;] Neue Vorschauregisterkarte zum Zusammenfassen und Anzeigen des Exportvorgangs
* [Mesh importieren/exportieren] Optimierung der Performance der Import-/Exportzeit
* [Mesh exportieren] Mesh in FBX exportieren
* [Mesh exportieren] Exportieren von Mesh mit Versatz und Tessellation
* [Mesh exportieren][UI] Neue Einstellungen für die Neuberechnung des normalen Scheitelpunkts, Anwendung der Triangulation
* [Mesh exportieren] Exportieren der ursprünglichen Mesh-Topologie mit neuen UVs, die durch automatischen entpack generiert werden
* Automatischer entpack mit weiteren Steuerelementen wurde aktualisiert
* [UV Entpackend][UI] Fügen Sie die Einstellung hinzu, um die automatische UV-entpack in einem neuen Projektfenster zu aktivieren
* [Entpackend UV][UI] Neue Optionen zum Steuern der entpackend Schritte (Nähte, entpackend Packing)
* [Entpackend UV][UI] Beibehaltung bestehender entpackend Nähte/entpackend /Packing zulassen
* [UV Entpackend][UI] Neue Optionen zur vollständigen Neuberechnung entpackend Schritte
* [Entpackend UV][UI] Neue Option zur Steuerung der Randgröße (keine, kleine, mittlere und große)
* Neue Baker
* [Baker] Alte Krümmung durch neue Krümmung aus Mesh ersetzen
* [Baker] Fügen Sie die Option &quot;Match by Name&quot; hinzu, um die Rückseite im Baker &quot;Ambient occlusion&quot; zu ignorieren
* [Baker] Option &quot;Boden-Ebene hinzufügen&quot; im Baker &quot;Ambient occlusion&quot;
* Neue Python-API für die Skripterstellung (3.7.6)
* [Python][UI] Neues Skriptmenü für Python
* [Python][UI] Neue Python-Dokumentation im Hilfemenü
* [Python] Gelegt Substance Painter Python-Module: substance\_painter, alg, display, project.setting, project, texturesets, ui
* [Python] Neues Python-Modul &quot;substance\_painter&quot; Gelegt
* [Python] Neues Python-Untermodul Gelegt: alg, display, log, project, resource, texturesets, ui
* [Python] Listener für Projektänderungen
* [Python] Neue Beispiele in der Python-Dokumentation
* [JavaScript][UI] Menü &quot;Plug-ins&quot; durch JavaScript ersetzt
* [Viewport] Ermöglichen der Erstellung einer Decal-Projektion durch &quot;Ziehen/Ablegen + ALT&quot; einer Ressource aus dem Regal
* Neue Inhalte
* [Inhalt] 5 neue Decal-Materialien von Substance Source
* [Inhalt] Hinzufügen neuer Projektvorlagen und Exportieren von Vorgaben für den Maxwell-Renderer
* [Inhalt] Hinzufügen einer Projektvorlage für den Keyshot 9-Export
* [Inhalt] Aktualisieren der Keyshot 9-Exportvoreinstellung, um Versatz und emissive zu unterstützen
* [Inhalt][Exporter] Aktualisierung aller Exportvorgaben, um die neuesten Engine- und Renderversionen zu berücksichtigen
* [Inhalt][Exporter] Aktualisieren Sie die Exportvoreinstellungsdateien, um neue Format- und Dithering-Einstellungen zu verwenden.
* [Inhalt] Neue Vorlagen und Shader zur Unterstützung von VRay Material (VRayMtl)
* [Ebenenstapel] Löschen von Ebeneneffekten mit Papierkorb-Symbol oder Tastaturbefehl-Entf-Taste zulassen
* Plug-in-Substance Source entfernen (Launcher mit &quot;Senden an&quot;-Funktion verwenden)
* [Windows] TDR-Warnung nicht auf High-End-GPUs anzeigen

**Fest:**

* Übersetzungsprobleme im Dialogfeld &quot;Neue Projektdatei&quot;
* [Baker] Die Einstellung &quot;Vorverarbeitete Szene speichern&quot; funktioniert nicht mehr.
* [Planare Projektion] Projektion funktioniert nicht bei Meshs mit sich wiederholenden UVs
* [Decal] Verhaltensunterschied im Normalkanal bei Verwendung verschiedener Modi zur Projektion der Füllebene
* [Verwischen][Klon] Beim Malen in einer Maske kann ein Artefakt angezeigt werden
* [Engine] Absturz mit bestimmtem Ebeneninhalt
* [Engine] Zufälliger Absturz beim Malen in einigen Fällen
* [Ankerpunkt] Der Verweis auf eine leere Maske gibt immer Weiß zurück
* [Exportieren] Ebene wird in bestimmten Stapel-Konfigurationen nicht berücksichtigt
* [Mesh exportieren] Kann nicht mit einem Pfad exportiert werden, der Sonderzeichen enthält
* [Mesh exportieren] GLTF-Dateien können beim Exportieren aus Linux oder MacOS nicht gelesen werden
* [Mesh importieren] Der erneute Import von DAE, PLY oder glTF funktioniert nicht wie beabsichtigt

**Bekannte Probleme:**

* [Skripterstellung][JavaScript] Die Einstellungen für den neuen Krümmung-Baker können nicht bearbeitet werden.
* [Baker] Absturz unter Linux mit GPU-Raytracing
* [Exportieren][USD] Die deaktivierten Textursatz sollten nicht exportiert werden.
* [Absturz] Ändern des Shader nach dem Malen einer Maske in der Material-Ebene

## Version 5

### 5.3.3 (2019.3.3)

*(Freigegeben: 6. Februar 2020)*
Zusammenfassung: **Bugfix mit Upgrade auf Iray 2019.3**

**Hinzugefügt:**

* Upgrade auf Iray 2019.3
* [Log] Veraltetes BIOS für Ryzen-CPU anzeigen, was während des Bakings zu Abstürzen führt
* [ABR] Extrahieren von ABR-Alphas nach Regal

**Fest:**

* [Baker] Baking schlägt fehl, wenn High-Poly-Mesh keine UVs enthält
* [Linux] Benutzerdefinierte Mauskürzel werden nicht gespeichert
* [Pinsel] Die Kontur verschwindet mit einigen Alpha-Formen
* [Tablet] Fehlerhafte Erkennung beim Verschieben von Schiebereglern
* [Tastaturbefehle] Mit Strg+Alt+Mausklick kann kein Tastaturbefehl eingerichtet werden
* [Regal] Die Ressourcen-QuickInfo wird bei Verwendung eines Stift-Tablets nicht angezeigt
* [2D-Ansicht][Exportieren] Die voreingestellte 2D-Ansicht berücksichtigt nicht die normalen Informationen
* Einfrieren beim Malen in UV-Ausrichtung mit bestimmten Pinseln
* Malen unter einem Filter erzeugt Artefakt auf dem laufenden Strich
* [Viewport] Falscher Texturen-Cache im Viewport nach dem erneuten Importieren eines Meshs
* [Absturz] Fehler beim Speichern nach dem Export in Photoshop
* [Absturz] Schreiben von Sonderzeichen im Präfix beim Importieren von Ressourcen
* [Absturz] Klicken Sie in den Ankerpunkt-Eigenschaften auf die Referenz.
* [Ankerpunkte] Kanal wird nicht aktualisiert, wenn ein Filter zwischen Ankerpunkt und Referenz vorhanden ist
* Iray-URL-Link im Hilfemenü funktioniert nicht

**Bekannte Probleme:**

* [Entpackend UV] Die Verarbeitung von Meshs mit hohem Poly-Anteil kann lange dauern
* [Entpackend UV] Scheitelpunkt mit genau denselben Koordinaten werden zusammengeführt
* [UV Entpackend] In seltenen Fällen kann die UV-Generierung auf einigen Mesh-Teilen fehlschlagen.
* [UV Entpackend] Ungleichmäßiges oder stark verzerrtes Textilverhältnis in einer einzigen UV-Insel in einigen Fällen
* [UV Entpackend] Ungleichmäßiges Textilverhältnis zwischen Textursätzen
* [UV Entpackend] UV-Insel kann sehr lang sein und passt in manchen Fällen nicht in den UV-Raum
* [UV Entpackend] Flächen mit degenerierten Flächen oder nicht dreieckigem Mesh mit kleinen oder überlappenden Kanten werden möglicherweise nicht in UV entpackt

### 5.3.2 (2019.3.2)

*(Freigegeben: 21. Januar 2020)*
Zusammenfassung: **Bugfix**

**Fest:**

* Beim Öffnen eines Projekts, das im Einzelkanalmodus gespeichert wurde, wird der Mesh nicht angezeigt
* Viewport wird beim Malen unter einer Ebene mit dem Kopierwerkzeug nicht immer aktualisiert

**Bekannte Probleme:**

* [Baker] Absturz im Zusammenhang mit Multithreading auf Ryzen-CPUs
* [Entpackend UV] Die Verarbeitung von Meshs mit hohem Poly-Anteil kann lange dauern
* [Entpackend UV] Scheitelpunkt mit genau denselben Koordinaten werden zusammengeführt
* [UV Entpackend] In seltenen Fällen kann die UV-Generierung auf einigen Mesh-Teilen fehlschlagen.
* [UV Entpackend] Ungleichmäßiges oder stark verzerrtes Textilverhältnis in einer einzigen UV-Insel in einigen Fällen
* [UV Entpackend] Ungleichmäßiges Textilverhältnis zwischen Textursätzen
* [UV Entpackend] UV-Insel kann sehr lang sein und passt in manchen Fällen nicht in den UV-Raum
* [UV Entpackend] Flächen mit degenerierten Flächen oder nicht dreieckigem Mesh mit kleinen oder überlappenden Kanten werden möglicherweise nicht in UV entpackt

### 5.3.1 (2019.3.1)

*(Freigegeben: 20. Dezember 2019)*
Zusammenfassung: **Hotfix**

**Fest:**

* Absturz bei der Arbeit an Meshs mit bestimmten UV-Projektionen
* [ABR] Absturz beim Wechseln zwischen Photoshop-Vorgaben
* [Linux] Substance Painter kann unter CentOS 7.4 aufgrund eines libGLX-Abhängigkeitsproblems nicht gestartet werden
* [Baker] Absturz beim Baking nach Verwendung von &quot;Datei&quot; > &quot;Bereinigen&quot;
* [Baker] Dialogfeld &quot;Baking führend Fortschritt&quot; friert nach Abbruch ein
* [Baker] Das Baking von Mesh nach dem Exportieren von Texturen funktioniert nicht
* [Baker] Verwenden von &quot;Match By Name&quot;-Ergebnissen mit schwarzen Mesh-Map
* [Baker] Käfig wird nicht berücksichtigt.
* [Regal] Das Importieren von PSD-Dateien führt zu fehlerhaften Bildern
* [Beispiel] Das Beispielprojekt &quot;Matte&quot; enthält fehlerhafte Kameras und eine falsche Exportvorgabe.

**Bekannte Probleme:**

* [Baker] Absturz im Zusammenhang mit Multithreading auf Ryzen-CPUs
* [Entpackend UV] Die Verarbeitung von Meshs mit hohem Poly-Anteil kann lange dauern
* [Entpackend UV] Scheitelpunkt mit genau denselben Koordinaten werden zusammengeführt
* [UV Entpackend] In seltenen Fällen kann die UV-Generierung auf einigen Mesh-Teilen fehlschlagen.
* [UV Entpackend] Ungleichmäßiges oder stark verzerrtes Textilverhältnis in einer einzigen UV-Insel in einigen Fällen
* [UV Entpackend] Ungleichmäßiges Textilverhältnis zwischen Textursätzen
* [UV Entpackend] UV-Insel kann sehr lang sein und passt in manchen Fällen nicht in den UV-Raum
* [UV Entpackend] Flächen mit degenerierten Flächen oder nicht dreieckigem Mesh mit kleinen oder überlappenden Kanten werden möglicherweise nicht in UV entpackt

### 5.3.0 (2019.3.0)

*(Freigegeben: 17. Dezember 2019)*
Zusammenfassung: **Hauptversion mit Verbesserung der Benutzererfahrung beim Handmalen, Arbeiten mit Tablets, automatischem UV entpack in der Beta-Version (0.3.0) und verschiedenen neuen Inhalten zum Handmalen**

**Hinzugefügt:**

* Integration von Automatic UV entpack 0.3.0 in Substance Painter
* [UV entpackend] Automatische UV entpackend im Substance Painter, wenn keine UVs oder partielle UVs vorhanden sind
* [entpackend UV] Eine globale Einstellung zum Aktivieren und Deaktivieren
* [entpackend UV] In Protokolldatei gemeldete Version
* [entpackend UV][UI] Anzeige des Fortschritts beim Entpackend UV
* [UI] Neue Einstellungen in der kontextabhängigen Symbolleiste zur Auswahl der Pinselvorschau: Vollständige Vorschau, Pinselkontur und Fadenkreuz
* [Tool] Neuer erweiterter Mischmodus im Alpha-Abschnitt: Aufhellen (Maximal) zusätzlich zu Normal
* [Ebenenstapel] Gammakorrektur-Option pro Ebene für Alpha oder Maske (Kontextmenü)
* [Ebenenstapel][UI] Fügen Sie das Symbol &quot;i&quot; hinzu, wenn ein Alpha-Layer gamma-korrigiert ist
* [Tablet][Tool] Gelegt Mindestdruck für Größe und Fluss
* [Tablet][UI] Neue Einstellung in der kontextabhängigen Symbolleiste zur Auswahl des Kurvendrucks: linear, easy-in, easy-in-out
* [Tablet][UX] Strg+Alt+Klick zum Scrollen hinzufügen
* Photoshop-Pinselvorgaben importieren (ABR-Format)
* [ABR] Support Shape-Parameter
* [ABR] Unterstützung von Parametern für die Formdynamik
* [ABR] Support Transfer-Parameter
* [ABR] Unterstützung von Streuungsparametern
* [ABR][Dynamische Pinselstriche] Unterstützung von Rundheit und Spiegelung
* [ABR][Regal] Legte die Pinselordnerstruktur im Filtereditor
* [ABR][Regal] Photoshop-Symbol in Miniaturansichten hinzufügen
* [ABR][Regal] Liste nicht unterstützter Parameter in der detaillierten Miniaturansicht von ABR hinzufügen
* [Tool][Dynamische Pinselstriche] Neue dynamische Stricheinstellung zur Steuerung der Anzahl der zu generierenden Zufallszahlen
* [Tool][UI] Fügen Sie neue Verteilungs- und Achse-Einstellungen für Streuungs-Jitter hinzu.
* [Tastaturbefehl] Fügen Sie Strg+Umschalt+B hinzu, um das Baking führend Fenster zu öffnen.
* [UI][Menu] Eintrag im Menü &quot;Bearbeiten&quot; hinzufügen, um das Fenster &quot;Baking&quot; zu öffnen
* [UI][Einstellungen] Verbesserte Ausrichtung der Liste der Tastaturbefehle
* [UI] Ersetzen von Drucksteuerelementen (Größe und Fluss) durch Schaltflächen zum Ein- und Ausschalten
* [Viewport] 2D- und 3D-Viewport können separat fokussiert werden.
* Update auf QT 5.12.5
* [UI] Anzeige des Ladefortschritts des Meshs
* [Substance] Zusätzliche Unterstützung für den nicht geklemmten und weichen Bereich mit Schiebereglern
* [Substance] Erhöhung der Präzision der Substance-Parameter auf bis zu 6 Dezimalstellen
* [Substance] Berücksichtigen Sie den durch einen Parameter definierten Schritt.
* [Substance] Optimieren der dynamischen Konturgenerierung mit Unterstützung von Bedingungen in Benutzerdaten
* [Substance] Graphausgabe als Maske für alle Kanäle über Benutzerdaten festlegen
* [Inhalt] Aktualisieren des Mat-Beispielprojekts mit Versatz-freundlicher Topologie, neuer ID-Map und neuen Kameras
* [Inhalt] Integration von drei neuen Filtern (MatFx): Comic-Buch, Aquarell, Öl-Malen (inspiriert von der Arbeit von Emrecan Cubukcu)
* [Content] Integrieren Sie 102 Photoshop-Pinselvorgaben aus den Packs von Kyle T. Webster
* [Inhalt] Integrieren Sie 18 neue Pinselvorgaben: Malen Roller Arrow, Malen Roller Warning text, Charcoal Fine und mehr
* [Inhalt] Integrieren Sie 9 neue Alphas: Brush Maker Malen Roller, Brush Maker Photoshop, Pinselmuster und mehr
* [Inhalt] Integrieren Sie 2 neue Werkzeugvorgaben: Gouache Dense und Gouache Faded
* [Inhalt] 1 neuen Generator integrieren : UV-Checker (UV-Inseln und Nähte hervorheben)
* [Inhalt] Integrieren Sie 2 neue Exportvoreinstellungen: Keyshot 9+ und Spark AR Studio
* [Inhalt] 1 neue Projektvorlage integrieren : Spark AR Studio (Facebook)

**Fest:**

* [Tablet] Das Rückgängigmachen von Stiftstrichen (Strg+Z) verzögert sich mehr als das Rückgängigmachen von Mausstrichen
* [Tablet] Anfangs- und Enddruck werden beim Zeichnen einer Geraden nicht berücksichtigt
* [Tablet] Der erste Stempel wird bei einer geraden Linie zweimal gezeichnet
* [Tablet] Verbessern der Unterstützung für Huion-Tablet-Tastaturbefehle
* [Tablet] Verbesserte Unterstützung für Huion Stift-Buttons
* [Tablet] Abstand zwischen der Pinselvorschau und dem gezeichneten Stempel
* [Tablet] Verknüpfungen zum Ändern von Pinseln mit Stift führen in seltenen Fällen zu geringer Leistung
* [Tablet] Verzögerung beim Malen auf einer bestimmten Ebene
* Unscharfe Texturen können in seltenen Fällen beim Wechseln des Viewport auftreten
* [UI][Substance] Bildeingaben werden nicht immer angezeigt
* Beim Bereinigen werden keine Vorgaben aus dem Regal entfernt, die in ein Projekt importiert wurden
* [Tool][Dynamischer Strich] Leistungsproblem beim Anpassen der Stempelzyklusanzahl
* Aktualisierungsprobleme beim Malen im 3D/2D-Viewport in seltenen Fällen
* Wenn Sie einen sehr langen Pinselstrich zeichnen, kann dies zum Einfrieren führen
* [Tool] Leistungsproblem beim Malen mit bestimmten Dynamischen Pinselstrichen
* [UI] Kontextbezogene Symbolleiste zeigt weiterhin Pinseleigenschaften an, wenn ein Ordner ausgewählt wird
* Werte für die Achse der Symmetrie werden nicht zurückgesetzt
* Import von EXR Texturen mit Fließkommawerten sind komplett schwarz
* Alt+Klicken auf einen Kanal zum Isolieren funktioniert nicht für Filter und Generator
* [Exportieren] Spezifische Projekt-Absturz beim Exportieren
* [Substance] Falscher Standardwert im Dropdown, wenn der Parameter von Visible If ausgeblendet wird
* [Shader] Kanäle, die über Material-Ebenen definiert wurden, werden in der Benutzeroberfläche nicht gleich sortiert
* [Regal] Vorgabenmetadaten werden nicht auf dem Datenträger gespeichert

**Bekannte Probleme:**

* [Entpackend UV] Die Verarbeitung von Meshs mit hohem Poly-Anteil kann lange dauern
* [Entpackend UV] Scheitelpunkt mit genau denselben Koordinaten werden zusammengeführt
* [UV Entpackend] In seltenen Fällen kann die UV-Generierung auf einigen Mesh-Teilen fehlschlagen.
* [UV Entpackend] Ungleichmäßiges oder stark verzerrtes Textilverhältnis in einer einzigen UV-Insel in einigen Fällen
* [UV Entpackend] Ungleichmäßiges Textilverhältnis zwischen Textursätzen
* [UV Entpackend] UV-Insel kann sehr lang sein und passt in manchen Fällen nicht in den UV-Raum
* [UV Entpackend] Flächen mit degenerierten Flächen oder nicht dreieckigem Mesh mit kleinen oder überlappenden Kanten werden möglicherweise nicht in UV entpackt
* Das Metamat-Beispiel hat einige Probleme mit importierten Kameras

### 5.2.3 (2019.2.3)

*(Freigegeben: 23. Oktober 2019)*
Zusammenfassung: **Bugfix-Version**

**Hinzugefügt:**

* [Liste der Textursatz] Schaltfläche &quot;Hinzufügen&quot; zum schnellen Aktivieren/Deaktivieren des Fokusmodus
* [Log] Windows 10-Versionsnummer in die Protokolldatei einfügen
* Aktualisieren Sie auf die neueste Version von Substance Engine
* [MacOS] Die Software wurde notariell beglaubigt, um die neuen MacOS Catalina-Verteilungsanforderungen zu befolgen

**Fest:**

* [Plugin] Plugin Source funktioniert nicht
* [MacOS][Shader] Mac OS 10.14.5 und AMD: Material-Ebenen funktionieren nicht wie vorgesehen

**Bekannte Probleme:**

* Alembic-Dateien mit Unterteilungen können nicht importiert werden
* Seltene Absturz beim Importieren einiger Alembic-Dateien
* Benutzeroberfläche reagiert beim Baking führ mit DXR auf Pascal-GPUs vorübergehend nicht

### 5.2.2 (2019.2.2)

*(Freigegeben: 20. September 2019)*
Zusammenfassung: **Bugfix-Version**

**Fest:**

* Das Importieren von Ressourcen durch Skripterstellung kann zu einem Absturz führen
* [Plugin] Das Herunterladen des Materials von der Quelle kann zu einem Absturz führen

**Bekannte Probleme:**

* Alembic-Dateien mit Unterteilungen können nicht importiert werden
* Seltene Absturz beim Importieren einiger Alembic-Dateien
* Benutzeroberfläche reagiert beim Baking führ mit DXR auf Pascal-GPUs vorübergehend nicht

### 5.2.1 (2019.2.1)

*(Freigegeben: 17. September 2019)*
Zusammenfassung: **Bugfix-Version**

**Fest:**

* [Mac][USD] Exportierte USDZ-Dateien aus MacOS können nicht geöffnet werden.
* [Textursatz] Es ist nicht möglich, einen Textursatz mit dem ALT-Modifizierer zu isolieren
* [Regal] Vorgaben, Intelligente Materialien und Intelligente Masken werden beim Beenden der Anwendung immer geändert
* [Ebenenstapel] Effekt kann nach dem Löschen eines anderen Effekts nicht ausgewählt werden
* Flackern bei Verwendung eines Schiebereglers im Bedienfeld &quot;Werkzeugeigenschaften&quot;
* Absturz beim Exportieren von Vorgaben in Regal
* Absturz beim Exportieren einer Vorgabe mit zu wenig Speicherplatz
* Absturz beim Erstellen einer Vorgabe mit zu wenig Speicherplatz

**Bekannte Probleme:**

* Alembic-Dateien mit Unterteilungen können nicht importiert werden
* Seltene Absturz beim Importieren einiger Alembic-Dateien
* Benutzeroberfläche reagiert beim Baking führ mit DXR auf Pascal-GPUs vorübergehend nicht

### 5.2.0 (2019.2.0)

*(Freigegeben: 25. Juli 2019)*
Zusammenfassung: **Hauptversion mit Leistungsaktualisierungen der Baker und einem neuen Vorvisualisierungsmodus + neuem Inhalt**

**Hinzugefügt:**

* [Baker] Zusätzliche Unterstützung für GPU-Raytracing mit DXR und OptiX (Ambient occlusion, Thickness)
* [Baker] Optimierungen und Beschleunigungen für CPU-Raytracing
* [Baker][VIS-Modus][UI] Neuer Visualisierungsmodus für Baking im Viewport
* [Baker][Voreinstellungen][Benutzeroberfläche] Neue Baking-Option zum Aktivieren/Deaktivieren von GPU-Raytracing
* [Baker][UI] Überarbeitung des Fortschrittsbalken-Dialogfelds
* [Baker] Verbesserung von Warn- und Fehlermeldungen
* [Baker] Responsiveres Abbrechen des Bakings zulassen
* [Baker] Fenster &quot;Baking&quot; nach Klicken auf &quot;Abbrechen&quot; erneut öffnen
* [Proj][UX] Verbesserte Verwendbarkeit des Rotations-Manipulators
* [Einstellungen] Option zur Leistungssteigerung durch Reduzierung der Viewport-Auflösung für HDPI-Bildschirme
* [Skripterstellung] Ändern der Auflösung von Textursätzen
* [Skripterstellung] Ausgewählten Textursatz abrufen
* [Scripting] Benutzer können einen Textursatz auswählen
* [Skripterstellung] Funktion, um zu erfahren, wann die Auswahl des Textursatzes geändert wurde
* [Regal] Es wurden 40 neue intelligente Materialien hinzugefügt.
* [Regal] 20 neue intelligente Masken hinzugefügt

**Fest:**

* [Ebenenstapel] Einfrieren der Benutzeroberfläche bei Mehrfachauswahl von Ebenen
* [Ebenenstapel] Beim Gruppieren vieler Ebenen wird die Benutzeroberfläche länger als gewöhnlich eingefroren.
* [Ebenenstapel] In einigen Fällen können eine Ebene und ein Effekt gleichzeitig ausgewählt werden
* In Malwerkzeugen verwendete Substance-Graf werden nicht mit der richtigen Auflösung generiert
* [Baker] Schaltfläche &quot;Alle Textursatz Baking geführt&quot; ist nicht deaktiviert, wenn keine Baker ausgewählt sind
* [MacOS] Deaktivieren der Warnmeldung zur Tessellation
* Bei Verwendung mit einer Projektion hat das Maskierungswerkzeug keine Vorschau.
* Absturz und beschädigte Projekte beim Speichern mit zu wenig Speicherplatz
* [Regal] Absturz beim Importieren einer Ressource auf dem Datenträger über ein Regal mit nicht genügend Speicherplatz
* [Regal] Absturz beim Wiederherstellen der Sitzungsvorgabe
* [Regal] Das Importieren einer Vorgabe mit einem Namen, der mit einem Leerzeichen endet, führt zu einem Absturz
* [Regal] Das Importieren einer Ressource mit einem Präfix, das mit einem leeren Leerzeichen endet, führt zu einem Absturz

**Bekannte Probleme:**

* Alembic-Dateien mit Unterteilungen können nicht importiert werden
* Seltene Absturz beim Importieren einiger Alembic-Dateien
* Benutzeroberfläche reagiert beim Baking führ mit DXR auf Pascal-GPUs vorübergehend nicht

### 5.1.3 (2019.1.3)

*(Freigegeben: Juli 2019)*
Zusammenfassung: **Bugfix mit 2 neuen Funktionen**

**Hinzugefügt:**

* Geben Sie das VRam-Budget über eine Befehlszeile (z. B. —vram-budget 4096)
* [QML] Leg von wrapMode- und elide-Eigenschaften von QML-Schaltflächen und -Kontrollkästchen

**Fest:**

* &quot;Pfad folgen&quot; funktioniert nicht immer
* Kanalzuordnung funktioniert nicht mit SBSAR, das in Ein Kanal-Steckplätzen verwendet wird
* [Ebenenstapel] Niedrige Leistung beim Scrollen mit ausgeblendeten Ebenen
* [TextureSet] Absturz beim Klicken zwischen Masken
* [SVT] Versatz wird nicht richtig angezeigt und flackert in einigen Fällen
* [Alembic] Absturz mit Mesh, der Punktnormalen anstelle von Scheitelpunkt-Normalen verwendet
* [Alembic][Log] Melden Sie einen Fehler im Log, wenn die Alembic-Datei während des Imports nicht unterstützt wird

**Bekannte Probleme:**

* Alembic-Dateien mit Unterteilungen können nicht importiert werden
* Seltene Absturz beim Importieren einiger Alembic-Dateien

### 5.1.2 (2019.1.2)

*(Freigegeben: 21. Mai 2019)*
Zusammenfassung: **Hotfix**

**Fest:**

* Absturz beim Auswählen von zwei Ressourcen mit einer Bildeingabe

### 5.1.1 (2019.1.1)

*(Freigegeben: 20. Mai 2019)*
Zusammenfassung: **Hotfix**

**Hinzugefügt:**

* Aktualisieren Sie auf die neueste Version von Substance Engine mit der letzten Version von Substance Designer 2019.1

**Fest:**

* [Substance] Visible If wird bei Eingabebildern nicht berücksichtigt
* [SVT][Engine] Das Ändern der Textursatz-Auflösung führt in einigen Fällen zu einem Absturz
* [Engine] In einigen Fällen werden zufällige schwarze Texturen angezeigt
* [Ebenenstapel][UI] Wenn Sie mit UMSCHALTTASTE eine Maske umschalten, können Sie mehrere Ebenen gleichzeitig auswählen
* [Ebenenstapel] Deckkraft hat keine Auswirkungen auf den Malen-Effekt mit dem Mischmodus &quot;Hindurchwirken&quot;
* [Ebenenstapel] Filtereingabe &quot;Height zu Normal&quot; wird mit dem Pinselstrich des Radiergummis nicht ordnungsgemäß aktualisiert
* Absturz [LayersStack] beim Rückgängigmachen des Ablagevorgangs für eine intelligente Maske
* Flackerndes Drahtgitter mit aktiviertem temporalem Anti-Aliasing
* [Versatz] Verzögerung bei AMD mit einigen schweren Meshs
* [Windows] Absturz beim Öffnen einiger Projekte über den Datei-Explorer
* [Histogramm] Absturz beim Entfernen von Masken mit Ankerpunkt in einigen Fällen
* Absturz bei der Vorschauerstellung in einigen seltenen Fällen
* [Absturz] Ein Projekt kann mit zu vielen Klon- und Verwisch-Tools nicht erneut geöffnet werden
* Nach dem Speichern wird in einigen Fällen kein Mesh im Materialmodi angezeigt
* [Scripting] alg.mapexport.documentStructure() gibt falsche Werte für Ordner zurück

**Bekannte Probleme:**

* Durch Doppelklicken auf den Namen des Textursatzes wird dieser vor dem Umbenennungsmodus ausgewählt.

### 5.1.0 (2019.1.0)

*(Freigegeben: 23. April 2019)*
Zusammenfassung: **Dynamischer Pinselstrich mit eigenem neuen Inhalt, Versatz und Tessellation in Echtzeit und Iray, Effekt &quot;Vergleichsmaske&quot;, Radiale Symmetrie, Planar und Sphärische Projektion**

**Hinzugefügt:**

* [Werkzeug] Dynamischer Strich: Substance-Variation entlang eines Pinselstrichs
* [Dynamische Kontur] Leg eines neuen Stempelindexparameters mit Optionen
* [Dynamischer Strich] Parameter $time berücksichtigen
* [Dynamischer Strich] Generieren eines neuen $randomseed-Parameters pro Strich und pro Stempel
* [Dynamischer Strich] Starten eines dynamischen Strichindex aus einer zufälligen Zahl
* [Dynamischer Strich][Regal] Helfen Sie mit dem neuen Symbol, eine dynamische Strichressource zu finden.
* Versatz und Tessellation im Echtzeit-Viewport
* Versatz und Tessellation in Iray
* [Shader-Einstellungen][UI] Neue Registerkarte für die Steuerung von Versatz und Tessellation
* [Ebenenstapel] Neuer Effekt &quot;CompareMask&quot;: durch Vergleich zweier Kanäle eine Maske generieren
* [Ebenenstapel][UI] Neuer Eintrag im Kontextmenü &quot;Height mit Maskenkombination hinzufügen&quot;, um einen CompareMask-Effekt einzufügen
* [Symmetrie] Neue Symmetrie: Radialmalerei
* [Einstellungen für Symmetrie] Erweitern Sie beide Abschnitte &quot;Einstellungen&quot; und &quot;Anzeige&quot;.
* [Symmetrie-Einstellungen][UI] Vorschau für radiales Malen
* Leg zweier neuer Modi für die Projektion: planar und kugelförmig
* [Proj] Neuer Formzuschneidemodus für alle Projektionen
* [Proj] Planarer Modus mit neuem Manipulator: Oberflächenwerkzeug
* [Proj][Tastaturbefehl] Tastaturbefehl UMSCHALTTASTE+W für Oberflächenwerkzeug
* [Proj] Planare Maskierung von Projektionen mit Tiefe ausblenden und Rückseiten-Ausblendung
* [Manipulator] Verbesserung des Manipulators der Drehung auf allen drei Achsen für triplanare
* [Tool][UX] Alt-Klick auf einen Kanal fokussiert diesen Kanal (aktiviert ihn oder deaktiviert alle anderen)
* [Engine] Update auf die neueste Version von Substance Engine
* [Textursatz] Mehrfachauswahl und Auflösungsänderung
* [Textursatz] Schnelle Aktivierung und Deaktivierung der Textursatz
* [Textursatz] Kombination von Solo- und allen Optionen in einem neuen Menü
* [Textursatz][Ebenenstapel] Neues Symbol für Aktivierung und Deaktivierung
* [Ebenenstapel][UX] Einfügen von Effekten über den bereits ausgewählten
* [Ebenenstapel][UI] Ebenenstapel-Ansichtenauswahlstil überarbeiten
* [Ebenenstapel] Der Mischmodus für instanzierte Ebenen ist jetzt standardmäßig im Durchlaufmodus
* [Exportieren] Option zum Aktivieren und Deaktivieren von Dithering
* [Plugin] Präzisionsmodifikator für Schieberegler unterstützen (SHIFT)
* [Plug-in][UI] Neues Symbol für automatisches Speichern
* [Scripting] Auflisten des Inhalts eines Ordners
* [Scripting] Löschen von Dateien zulassen
* [Skripterstellung] Lesen aller Stapel-Informationen, einschließlich der verwendeten Ressourcen
* [Inhalt][Dynamischer Strich] Neue Werkzeuge und Pinselvorgaben
* [Inhalt][Dynamischer Strich] Zwei neue prozedurale Verläufe: Farbton und Verlaufsgenerator
* [Inhalt] 11 neue Filter: MatFx Peeling Malen, MatFx Wassertropfen und mehr
* [Inhalt] 7 neue Generatoren: &quot;Auto-Stitcher&quot;, &quot;UV-Zufallsfarbe&quot;, &quot;UV-Texeldichte&quot; und weitere Eigenschaften
* [Inhalt] 93 neue Alphas: neue Texte, Pfeile und verschiedene andere Formen
* [Inhalt] 2 neue Verfahren: Verlaufsfarbton, Verlaufsgenerator und mehr
* [Inhalt] 21 neue Tools und Pinselvorgaben für Dynamische Pinselstriche : Kiesel, Fußabdrücke, Spray und mehr
* [Inhalt] 2 Neue HDRs: Canopus Boden- und Herbstwald
* [Inhalt] Aktualisieren von Inhalt mit Kuration nach dem Zufallsprinzip in Regal
* [Inhalt] Neues Symbol mit gelegt Zufallsparameter in Regal

**Fest:**

* [Ebenen-Stapel] Ebenenstapel wird unendlich lange gezogen
* [Mac] &quot;Im Finder anzeigen&quot; kann zum Einfrieren führen
* [Scripting] Einstellungen, die über die benutzerdefinierte Benutzeroberfläche gespeichert wurden, gehen verloren, wenn die Shader-Datei verschoben wird
* [Scripting] API-Versionsnummer ist falsch und nicht aktuell
* [Effekt] Histogramminhalt wird nicht korrekt angezeigt
* [Effekt] Der Histogrammeffekt wird in einigen Fällen nicht aktualisiert
* [Regal] Die Stiche sind auf Material &quot;Plastic Fabric Pyramide&quot; nicht richtig ausgerichtet.

**Bekannte Probleme:**

* Durch Doppelklicken auf den Namen des Textursatzes wird dieser vor dem Umbenennungsmodus ausgewählt.
* [Ebenenstapel][UI] Wenn Sie mit UMSCHALTTASTE eine Maske umschalten, können Sie mehrere Ebenen gleichzeitig auswählen

## Version 4

### 4.3.3 (2018.3.3)

*(Freigegeben: 7. März 2019)*
Zusammenfassung: **Bugfix**

**Hinzugefügt:**

* [Inhalt] Neue Projektvorlage integrieren: &quot;PBR - Metallische Rauheit Alpha-blend&quot;
* Die Suchreihenfolge der dynamischen Linux-Bibliothek wurde geändert, um Bibliotheken im Installationsverzeichnis Priorität einzuräumen, bevor sie auf dem System installiert werden.

**Fest:**

* Mesh verschwindet manchmal vom 3D-Viewport (drücken Sie F, um die Kamera zurückzusetzen)
* Aktualisieren des Substance Painter Sketchfab-Uploaders mit den neuen Sketchfab-Lizenztypen
* [Import][glTF] Falsche Handhabung der Modulation der Eingabe-Textur, wie in glTF-Dateien definiert
* [Import][glTF] Boden-Ebene wird beim glTF-Import in einigen Fällen falsch angezeigt
* [Exportieren][USD] Deckkraft funktioniert nicht in Arkit
* [Exportieren][USD] USDz-Export-Absturz in einigen Fällen
* [Exportieren][USD] Exportieren nach USD ohne Speichern führt zu Absturz
* [Exportieren][USD] Falsche Kachelung für Texturen, Unterteilungsmodus für Mesh und Ausgabetypen für Shader
* [Exportieren][USD] Wenig Exporte von nur einigen Textursätzen mit allen Geometrien
* [Instanz] Absturz beim Löschen einer beschädigten Instanzebene
* [Regression][Exportieren] Einige Maps werden nicht in die ausgewählte Bittiefe exportiert
* [Linux] Problem mit der Bibliothek libtbb.so.2

**Bekannte Probleme:**

* Einfrieren der Berechnung in einigen Fällen auf AMD VEGA-GPUs
* Problem mit Huion-Tablets mit Tastaturbefehlen unter Windows

### 4.3.2 (2018.3.2)

*(Freigegeben: 24. Januar 2019)*
Zusammenfassung: **Hotfix mit neuen Funktionen (USDZ-Export- und Textur-Filterungen im Viewport)**

**Hinzugefügt:**

* [Export] Export nach USDZ zulassen
* [Viewport] Zulassen, dass die Qualität der Textur in den Anzeigeeinstellungen gesteuert wird.
* [Viewport] Die MIP-Voreinstellung wurde in den Anzeigeeinstellungen hinzugefügt.
* [Viewport] Anisotrope Filterung in den Anzeigeeinstellungen hinzugefügt
* [Plug-ins] Offizielle Plug-ins aktualisieren, um den Stil von Substance Painter 2018 zu verwenden
* [Lizenz] Installation der Lizenz standardmäßig in einem Benutzerordner

**Fest:**

* Mit Dekomprimierung verknüpfter Absturz
* Hinzufügen von TAA auf Solo-Material
* Rauschen mit Shadow, TAA und Alpha-Test-Shader mit Dithering
* Specular-Dithering für alle klassischen PBR-Shader entfernen
* Absturz in den Shader-Einstellungen in einigen Fällen
* Die Streuungsaktivierung wird nicht zwischen OpenGL- und Iray-Renderings synchronisiert
* Die Verwisch- und Kopierwerkzeuge funktionieren nicht mehr auf bestimmten Meshs
* Einige Textursatz können nicht im Iray-Rendering angezeigt werden
* Umbenannte Textursatz werden nach dem Schließen des Projekts nicht gespeichert
* Drahtgitter-Artefakte beim Ziehen und Ablegen von Materialien auf ID-Map
* [Scripting] Dateipfaderstellung beim Speichern eines Projekts nicht erzwungen
* [Scripting] Rückruf von &quot;onProjectAboutToSave()&quot; funktioniert nicht mehr
* Fehlerhafte Links im Fenster &quot;Fehler melden&quot;

**Bekannte Probleme:**

* Einfrieren der Berechnung in einigen Fällen auf AMD VEGA-GPUs
* Problem mit Huion-Tablets mit Tastaturbefehlen unter Windows

### 4.3.1 (2018.3.1)

*(Freigegeben: 6. Dezember 2018)*
Zusammenfassung: **Hotfix**

**Hinzugefügt:**

* [Symmetrie][Viewport] Das Malen mit Symmetrien in der 2D-Ansicht ist wieder da und zeigt nun eine Vorschau des Klonpinsels an.

**Fest:**

* [Exportieren] Beim Exportieren von 2D-Ansichten wird in einigen Fällen eine schwarze Textur ausgegeben
* [Iray] Normale Informationen werden in Iray falsch, nachdem eine Material-Ebene instanziiert wurde
* Nicht quadratische Textursatz können in einigen Fällen zu Absturz führen
* [Rückgängig] Mehrere Strg+Z können in einigen Fällen zufällig zu Absturz führen
* [QML] AlgScrollView kann in einigen Fällen eine Warnung im Protokoll erstellen (Bindungsschleifen)

**Bekannte Probleme:**

* Einfrieren der Berechnung in einigen Fällen auf AMD VEGA-GPUs
* Problem mit Huion-Tablets mit Tastaturbefehlen unter Windows
* Glätten und Schatten können bei gemeinsamer Verwendung zu unerwarteten Ergebnissen führen

### 4.3.0 (2018.3.0)

*(Freigegeben: November 2018)*
Zusammenfassung: <b>Viewport-Upgrades, ordnungsgemäßer Datenexport, neue UI-Helfer, ein erweitertes Symmetrie-Tool, neue 2D-Ansichten und eine enorme Leistungssteigerung</b>

<b>Hinzugefügt:</b>

* [Glätten][Viewport] Neue temporale Anti-Aliasing-Filterungen für 3D-Viewport (über Anzeigeeinstellungen)
* [Exportieren] Exportieren Sie den Inhalt des 2D-Viewports als eine einzige Textur
* [Exportieren][Dithering] Dithering beim Exportieren Gelegt
* [Ebenenstapel] Farben auf Ebenen und Ordnern
* [Ebenenstapel] Schnelle Aktivierung und Deaktivierung mehrerer Ebenen und Effekte
* [Ebenenstapel] Einfachere Navigation für Füllmethoden mit Nach-oben-Tasten und Mausbildlauf
* [Proj][UI] Zusätzlicher Dreh-Manipulator auf allen drei Achsen für triplanar
* [Proj][Tastaturbefehle] - und +, um die Größe des Manipulators der UV-Projektion zu ändern
* [Shader] Kontrolle beschichteter Schichtparameter mit Kanälen im PBR-beschichteten Shader
* [Substance] Leg neuer Mesh-basierter Textur-Eingänge für Filter und Generatoren
* [Symmetrie][Viewport][UI] Steuern des Offsets der Symmetrie auf Manipulator
* [Symmetrie][Kontextabhängige Symbolleiste][Benutzeroberfläche] Neues Bedienfeld &quot;Symmetrie&quot; mit Optionen
* [Symmetrie] Neue Symmetrie Linienüberschneidungsmodus
* [Symmetrie] Neuer Symmetrie-Clone-Cursor
* [Symmetrie][Tastaturbefehle] Q zum Ausblenden und -, + zum Ändern der Größe und Umschalttaste zum einrasten
* [Log] Verbessern von Fehlermeldungen, wenn Texturen nicht exportiert werden können
* [Scripting] Ressourcen in den Anzeigeeinstellungen ändern oder aktualisieren
* [Scripting] Erlaubt das Erstellen oder Entfernen von Kanälen in Textursätzen
* [Content][Shaders] Unterstützung für Anisotropie mit einem dedizierten Shader hinzufügen (pbr-metal-rau-Anisotropie-angle)
* [Inhalt] Aktualisierung der Vorschaukugel mit Anisotropie und verändertem Winkel
* [Content] Aktualisierte matFx-Shutline
* [Content] Neuer Scanner zur Texturierung.XYZ-Fläche
* [Inhalt] Neue anisotrope Verfahren
* [Inhalt] Neuer Filter: Umgebung mit vorberechnete Beleuchtung
* [Inhalt] Neue Umgebungs-Map: Studio Automotive Neutral
* [Inhalt] Neue Projektvorlage: PBR - metallische Rauheit Anisotropy angle (mit Anisotropie-Kanälen)
* [Inhalt] Neue Projektvorlage: PBR - mit metallische Rauheit beschichtet
* [SVT][Engine] Dünn besetzte virtuelle Texturen (SVT)
* [SVT][Voreinstellungen][UI] Beschleunigungsoption für SVT-Hardware-Unterstützung
* [SVT][Protokoll] Zusätzliche Informationen für die Funktion &quot;Virtuelle Texturierung mit geringer Dichte&quot; (z. B. Festplatte in Größe)
* [SVT][UI] Meldungsfenster beim Start, wenn die Größe auf der Festplatte für den Cache zu niedrig ist
* [SVT][Voreinstellungen][UI] Substance Painter globaler Cachespeicherort
* [SVT] Neue Umgebungsvariable zur Angabe des Pfads des Substance Painter-Cache
* [SVT] Neue Umgebungsvariable zum Aktivieren der SVT-Hardware-Support-Beschleunigung
* [SVT] Erkennen von geringer Unterstützung durch Hardware
* [SVT][Hardware Sparse] Erhöhen der Mindesttreiberversion für Nvidia-GPU
* [SVT][Shader][Viewport][UI] Warnen Sie den Benutzer, wenn beim Öffnen des Projekts Artefakte mit virtueller Texturierung mit geringer Dichte vorhanden sind

<b>Fest:</b>

* [Farbwähler] Beim Auswählen einer Farbe wird ein Malcursor angezeigt
* Absturz durch das Auswählen oder Aufheben der Auswahl von Ebenen in einer bestimmten Reihenfolge kann zu Absturz führen
* Absturz beim Einfügen einer Ebene mit einer Maske als Instanz
* [Benutzerkanal][Regression] Absturz beim Umbenennen des Benutzerkanals
* [Benutzerkanal] Graue Pinselvorschau
* [Alembic] Nur ein Textursatz aus mehreren Materialien nach dem Import
* [Engine] Exportierte Textur unterscheidet sich von Viewport für Pinselstempel
* [Engine] Die Umkehrung mit einem Ebeneneffekt wirkt sich nicht vollständig auf eine Textur aus
* Die Material-Auswahl wendet beim Auswählen einen Pinselstrich an
* Der Wechsel der Auflösung auf 128 x 128 px führt zu einem Absturz
* Mesh-Map-Verknüpfungen werden beim Umbrechen oder Instanziieren von Ebenen nicht ordnungsgemäß aktualisiert
* [Substance] UserData ColorSpace funktioniert nicht bei Baking geführt Mesh Normal, der als Eingabe angefordert wird
* MDL-Zuordnungskonflikt bei Verwendung mehrerer Shader-Instanzen
* [Symmetrie][Füllebene] Symmetrie-Ebene und ihr in der Füllebene aktiver Manipulator
* [Viewport] Pivot-Punkt für Übersetzung wird nach dem Klicken nicht immer aktualisiert
* [UI] Symbole und Entfernen von Platzhaltern für HDPI-Monitore wurden korrigiert

<b>Bekannte Probleme:</b>

* Einfrieren der Berechnung in einigen Fällen auf AMD VEGA-GPUs
* Problem mit Huion-Tablets mit Tastaturbefehlen unter Windows
* Glätten und Schatten können bei gemeinsamer Verwendung zu unerwarteten Ergebnissen führen

### 4.2.3 (2018.2.3)

*(Freigegeben: 25. September 2018)*

**Fest:**

* [2D-Ansicht] Bei der Erstellung eines neuen Projekts ist die 2D-Ansicht mit einigen Meshs beschädigt.
* [Absturz] Der Wechsel von der UV-Projektion zur dreimal planaren Projektion führt zu einem Absturz
* [RayCollider] Mehrere Absturz durch &quot;RayCollider&quot;
* [Werkzeug] Beim Wechseln von Ebenen gehen die geänderten Pinseleigenschaften verloren
* Pinseleinstellungen werden beim Wechsel zum Radierer zurückgesetzt

**Bekannte Probleme:**

* Einfrieren der Berechnung auf AMD VEGA-GPUs
* Problem mit Huion-Tablets mit Tastaturbefehlen unter Windows

### 4.2.2 (2018.2.2)

*(Freigegeben: 11. September 2018)*
Zusammenfassung: **Hotfix mit Inhaltsaktualisierung, neuen Skriptfunktionen und der Möglichkeit, das automatische Update zu deaktivieren**

**Hinzugefügt:**

* [Inhalt][Regal] Hinzufügen einer Skin-Regal-Vorgabe
* [Inhalt][Regal] Konvertierung von 19 Skinnormalen in Materialien zur Volumenstreuung
* [Scripting] Erstellen einer Projektvorlage aus einem geöffneten Projekt
* [Scripting] Abrufen/Festlegen von Exporteinstellungen eines geöffneten Projekts
* [Updates] Deaktivieren des Popups &quot;Automatische Aktualisierung&quot; in den Einstellungen und der Umgebungsvariablen
* [Updates] Anzeige erst in der nächsten Version des veralteten Wartungs-Popup

**Fest:**

* [Kamera] Falscher Zoom durch Wechsel von orthografisch zu Perspektive
* [Anzeige] Einige Maps werden linear anstelle von sRGB angezeigt
* [Viewport] Mesh-Fokus verhält sich nicht richtig
* [2D-Ansicht] Projekt mit beschädigter Kamera enthält verschwindende UVs-Schalen
* [SSS][QuickInfo] QuickInfos zu Volumenstreuung-Tools werden im Protokoll angezeigt
* Einige Projekte können nicht in 2018.2 geöffnet werden und die Fehlermeldung kann kein Null-Substance-Paket speichern
* [Maske] Die Farbe des Malen-Werkzeugs kann in einigen Fällen beim Arbeiten in einer Maske hängen bleiben
* [Material] Karten werden in bestimmten Situationen nicht angezeigt
* [Proj][Tools] Manipulator aktiv mit einem Generator
* [Substance] Fehlende Substance-Parametergruppen
* [Skripterstellung] Falscher Software-Name in der Dokumentation
* [UDIM] Keine Informationen im Protokoll über UVs-Schalen auf mehreren UVs-Kacheln

**Bekannte Probleme:**

* Einfrieren der Berechnung auf AMD VEGA-GPUs
* Problem mit Huion-Tablets mit Tastaturbefehlen unter Windows

### 4.2.1 (2018.2.1)

*(Freigegeben: 03. August 2018)*

**Fest:**

* Fehlende Shader-Parameter für die Volumenstreuung beim Aktualisieren von Projekten

**Bekannte Probleme:**

* Einfrieren der Berechnung auf AMD VEGA-GPUs
* Problem mit Huion-Tablets mit Tastaturbefehlen unter Windows

### 4.2.0 (2018.2.0)

*(Freigegeben: 2. August 2018)*
Zusammenfassung: **Sommerversion, Volumenstreuung-Support, Verbesserungen bei Projektion und Füllung, Kamera-Import und -Auswahl, Alembic- und glTF-Unterstützung, Drag-and-Drop auf ID-Map, verbesserte Unterstützung für Substance-Formate und neue Inhalte**

**Hinzugefügt:**

* [SSS][Viewport][Iray] Generische Volumenstreuung
* [SSS] Synchronisierungs-MDL- und Volumenstreuung-Parameter
* [SSS] Es wurde ein neuer Graustufenkanal mit dem Namen &quot;Streuung&quot; hinzugefügt.
* [SSS][Shader-Einstellungen] Streutypparameter für die Volumenstreuung (Skin oder transluzent)
* [SSS][Shader-Einstellungen] Streuungsparameter für die Volumenstreuung
* [SSS][Shader Settings] Farbstreuung-Parameter für Volumenstreuung
* [SSS][Anzeigeeinstellungen] Streuung Beispielanzahl für Volumenstreuung
* [Shader][Iray] Integrieren von Volumenstreuung-MDL für Iray
* [Shader] Shader-Update über den Ressourcen-Updater
* [Shader] API und Dokumentation für Änderungsprotokoll aktualisieren
* [Werkzeugeigenschaften][Proj] Neue Parameter für die triplanare Projektion
* [Viewport][Proj] Steuern Sie die Eigenschaften der Füllebene in der 3D-Ansicht direkt mit Manipulatoren (triplanare Projektion)
* [Shortcuts][Proj] Neue Shortcuts Q, W, E, R, T für triplanare Projektion Manipulator
* [Viewport][Proj] Steuern Sie Eigenschaften der Füllebene in 2D-Ansichten direkt mit Manipulatoren (UV-Projektion)
* [Shortcuts][Proj] Neuer Tastaturbefehl Q für UV-Projektion Manipulator
* [Kontextsymbolleiste][Proj] triplanare Projektion-Manipulator steuern
* [Kontextsymbolleiste][Proj] UV-Projektion-Manipulator steuern
* [Werkzeugeigenschaften] Deaktivieren der Kachelung der Textur mit dem Werkzeug Projektion und Schablone
* [Schablone] Verwenden von Nicht-quadratischen Bildern mit dem Projektion-Werkzeug/der Schablone
* [Schablone] Steuerung des Kachelung-Modus im Eigenschaftenfenster zulassen
* [Schablone] Der Zoom ist nicht auf einer Schablone ohne Kachelung zentriert
* [Kameras] Importieren von Kameras aus Maya, Max, Blender, Modo, DAE
* [Kameras][Viewport] Wählen und steuern Sie importierte Kameras in Viewport
* [Kameras][Iray] Importierte Kameras in Iray auswählen und steuern
* [Kameras][UI][Neues Projekt][Projektkonfiguration] Kameras importieren ist standardmäßig aktiviert.
* [Kameras][Tastaturbefehle] Hinzufügen von Tastaturbefehlen, um zwischen Kameras zu wechseln
* [Kameras][Viewport] Rahmen im Viewport hinzufügen
* [Kameras][Viewport-Einstellungen] Steuerung der Deckkraft des Rahmens
* [Kameras][Kamera-Einstellungen] Maximale Brennweite bei 500 mm
* [Kameras][Kameras] Gelegt Verhältnis
* [Kameras][Kamera-Einstellungen] Option &quot;Sperren&quot; hinzufügen
* [Kameras][Kamera-Einstellungen] Hinzufügen einer Wiederherstellungsoption
* [Kameras][Kamera-Einstellungen] Attribut für den Fokusabstand hinzufügen
* [glTF] Import einer glTF-Datei
* [glTF] Importieren einer ambient occlusion-Map
* [Alembic] Importieren von Alembic 1-Rahmen mit statischer Geometrie
* [Regal] Ziehen Sie Materialien mithilfe von ID-Map mit einem Modifizierer (STRG/Befehlstaste) direkt auf den Mesh.
* [Ebenenstapel] Automatische Erstellung von ID-Masken durch Ziehen und Ablegen von Materialien auf Mesh mit ID-Map
* [Ebenenstapel] Automatischer Bildlauf von Ebenen per Drag &amp; Drop über den Ebenenstapel
* [UI][Tooleigenschaften] Leg der Vorgabe des Substance
* [UI][Hilfemenü] Verbesserung des Hilfemenüs
* [UI][Neues Projekt][Projektkonfiguration] Reorganisation des Fensters
* [UI][Neues Projekt][Projektkonfiguration] Ersetzen des Meshs durch Datei
* [UI][Substance] Anzeigen von Substance-Attributen in der Benutzeroberfläche
* [Tastaturbefehle] F4 wechselt zwischen 2D- und 3D-Ansicht
* [Tastaturbefehle] Neue Tastaturbefehle zum Umschalten zwischen Schablone N und schnelle Maske U
* [Substance-Integration] Berücksichtigung von &quot;visible if&quot;-Anweisungen in den Substance-Parametern
* [Viewport] Schatten müssen nach dem Verschieben der Kamera nicht berechnet werden.
* [Inhalt] Aktualisieren von MeetMat mit importierten Kameras
* [Inhalt] Beispiel mit aktivierter Volumenstreuung hinzufügen - JadeToad
* [Inhalt] Neue PBR-Projektvorlage mit aktivierter Volumenstreuung hinzufügen
* [Inhalt] Exportvorgaben wurden aktualisiert, um einen neuen Streuungskanal hinzuzufügen
* [Inhalt][Regal] Zusätzliche Unterstützung für Volumenstreuungen für: pbr-metal-rau, pbr-metal-rau-alpha-test, pbr-coated, pbr-spec-gloss
* [Inhalt][Regal] Ein Streuungskanal wurde zu 5 intelligenten Materialien (Marmor und Skin) hinzugefügt.
* [Inhalt][Regal] 1 neues Jade-Material
* [Inhalt][Regal] 1 neues Wachs-Material

**Fest:**

* [CMD] Verschiedene Ergebnisse über dieselbe Befehlszeile mit unterschiedlichen Versionen
* [TDR] Wenn TdrLevel eingerichtet ist, sind keine Fehler im Protokoll vorhanden.
* [Baker] Ambient occlusion-Map wird gespiegelt
* [ID-Map] Absturz beim Kommissionieren außerhalb des 0-1-Bereichs
* [Iray] Absturz beim Wechseln des Textursatzes und beim Wechseln in den Malen
* [Viewport] Synchronisieren von Ablagebereichen zwischen Viewporten für Drag &amp; Drop
* [Engine] Moiré-Artefakt bei der Kachelung von Füllebenen oder beim Malen eines kleinen Pinsels
* [Lizenz] Prüfung auf fehlerhafte Softwareversion des Lizenzdiensts
* [Lizenz] Überarbeiten Sie die Art und Weise, wie wir die Authentifizierung verarbeiten
* [API] Rufen Sie das onNewProjectCreated-Skript-API-Ereignis auf, selbst wenn Sie mit einer Vorlage erstellen.
* [Shader] Kompilierter Shader wird nicht aus dem Cache geladen, wenn die Shader-Datei nicht kompiliert wird
* [Regal] Exportieren der HDR-Datei aus dem Regal gibt eine Datei mit festgeklemmten Werten aus
* [Exportieren] EXR exportieren Klammern RGB Farbwerte zwischen 0-1
* [Inhalt] Prozedurales Rauschen 3D Perlin Rauschen Fraktal ist verpixelt

**Bekannte Probleme:**

* Einfrieren der Berechnung auf AMD VEGA-GPUs
* Problem mit Huion-Tablets mit Tastaturbefehlen unter Windows

### 4.1.3 (2018.1.3)

*(Freigegeben: 28. Juni 2018)*

**Hinzugefügt:**

* [Voreinstellungen] Vorschlag zum Speichern des Projekts beim Neustart von Painter

**Fest:**

* [Plug-In] Substance Source &quot;Suchen&quot; funktioniert nicht
* [Intelligenten Materials] Das Importieren von Intelligenten Materials führt in einigen Fällen zu einem Absturz
* [Intelligenten Materials] Das Löschen von Intelligenten Materials führt in einigen Fällen zu einem Absturz
* [Speichern] Das Speichern führt in einigen seltenen Fällen zu einem Absturz
* [Regal] Umkehren funktioniert nicht auf den Zellen 2 und 3 der Zellen
* [Regal] Typo in einigen Alphas
* [Regal] Einige Substance-Material werden nicht richtig gerendert

**Bekannte Probleme:**

* Einfrieren der Berechnung auf AMD VEGA-GPUs

### 4.1.2 (2018.1.2)

*(Freigegeben: Juni 2018)*
Zusammenfassung: **Verbesserte Wiedergabegeschwindigkeit, verbessertes Speichersystem, aktualisierte Schieberegler, aktualisierte Plug-in-API, chinesische Baking, verbesserter Abstand jetzt optional**

**Hinzugefügt:**

* [Baker] Leistungsverbesserung mit neuer Baker-Version
* Erzwungene Anzeige von Dialogfeldern mit inkompatibler GPU
* [Speichern] Leg neuer Kompaktprojekt-Funktionen (vollständiger/kompakter Speichermodus)
* [Speichern] Benutzer informieren, wenn Fehler beim Speichern auftritt
* [Clean] Nächste Speicherung im Voll-/Kompaktmodus
* [Schieberegler] Verbesserung der Präzision der Farb-/Graustufenbalken und Schieberegler
* [Schieberegler] Hinzufügen der Pfeilsteuerungen nach oben/unten
* [Schieberegler] Dieselbe Erkennungszone für Farb- und Graustufenbalkenschieberegler
* [Plugin] Automatische Speicherung immer im inkrementellen Modus
* [Plug-In] Option zum Wechseln von Plug-Ins zu einem neuen Schnittstellenstil
* [Sprache] Chinesische Übersetzung hinzufügen
* [Auffüllung] Option zum Wechseln zwischen UV- und 3D-Raum, Nachbar-Auffüllung pro Textursatz in den Textursatz-Einstellungen
* [Skript] Gelegt Speichermodus: Voll/Kompakt oder inkrementell
* [Script] Update Scripting/QML documentation
* [Log] Anzeige des Speichermodus im Protokoll (vollständig/kompakt oder inkrementell)

**Fest:**

* [Tool] Kanalsteckplatz transformieren bei Einkanalfüllungen in einen Material-Steckplatz
* Absturz beim Laden eines Meshs (FBX) mit einigen Flächen, die nicht von einem Material zugewiesen wurden
* Absturz in Iray mit NVIDIA RASTER 5.2 auf einem virtuellen Computer
* Absturz beim Rückgängigmachen eines Löschens einer Materialvorgabe
* Absturz beim Laden einiger Projekte
* [Befehlszeile] Neue Befehlszeile für UDIM-Mesh, aufgeteilt nach Audio
* [Symbolleiste] Verkleinern der Symbolleiste
* [Instanz] Bitmaps können nicht über mehrere Textursatz instanziieren werden
* [Viewport] Aktualisierung ist nicht abgeschlossen, wenn auf Mesh mit gekachelten UVs gemalt wird
* [Iray] Normalen-Map wird zweimal für Dielektrika angewendet
* [Regal] Tippfehler in einigen Substance-Parametern (Alphas, Prozeduren und Matfx)
* [Regal] Typo für die Bitmap &quot;Authorized Personnel Only&quot;
* [Script] Funktion alg.shaders.Materials() funktioniert nicht mehr

**Bekannte Probleme:**

* Einfrieren der Berechnung auf AMD VEGA-GPUs

### 4.1.1 (2018.1.1)

*(Freigegeben: 03. April 2018)*

**Fest:**

* [Tablet] Problem beim Ändern der Standardinteraktionsoptionen
* [Baker] Absturz mit Assimp-Bibliothek
* [Baker] Leistungsrückgang mit A.O.-Map
* [Iray] Die Verzerrung des Objektivs wird nicht auf den Alphakanal angewendet
* [Treiber] Aktualisierung der Mindestanforderungen für Treiber
* [3Dview] Normale werden auf UDIM-Meshs ohne Normale-Informationen nicht korrekt generiert
* [Intel] Absturz mit Substance Painter 2018.1.0
* [Intel][Viewport] Problem mit der Auffüllung (schwarze Artefakte)

**Bekannte Probleme:**

* Einfrieren der Berechnung auf AMD VEGA-GPUs

### 4.1.0 (2018.1.0)

*(Freigegeben: 15. März 2018)*

**Hinzugefügt:**

* Neuer allgemeiner Stil (Symbole, Farbe, Verhalten)
* Neues Standardlayout
* [Tablet] Benutzererfahrung beim Malen verbessert
* [Hauptmenü] Sortieren Sie native Elemente zuerst in Ansichten und Symbolleisten
* [Hauptmenü] Aktionen &quot;schnelle Maske verschieben&quot; im Abschnitt &quot;Viewport&quot;
* [Hauptmenü] Verschieben von Rechtsklickaktionen in den Abschnitt &quot;Viewport&quot;
* [Hauptmenü] Menü &quot;Ansicht&quot; in &quot;Fenster&quot; umbenennen
* [Schnellmenü] Neue Werkzeugeigenschaften durch Rechtsklick im Viewport
* [Dock-Widget] Neue Dock-Symbolleiste zum schnellen Reduzieren/Zurückrufen
* [Anzeigeeinstellungen] Fenster &quot;Kamera- und Anzeigeeinstellungen&quot; wurde zusammengeführt
* [Ebenenstapel] Kontextmenü (rechte Maustaste)
* [Ebenenstapel] Ziehen und Ablegen, um einen Effekt innerhalb derselben Ebene zu verschieben
* [Symbolleiste] Neuorganisation der Symbolleiste und neue kontextbezogene Symbolleiste
* [Werkzeugleiste] Klonwerkzeug in zwei separate Werkzeuge teilen
* [Werkzeugeigenschaften] Hellerer Graustufenwert im Hintergrund in der Vorschau
* [Eigenschaften von Tools] Organisation in Registerkarten (Füllung und Werkzeuge)
* [Tool] Das Malergebnis entspricht der Schablone
* [Viewport] Neuer Cursor für Füllebene
* [Viewport] Einfacheres Navigieren und Malen (höhere Rahmen-Rate)
* [Viewport] Auswahlkombination &quot;Material/Kanal/Karte&quot; im Viewport
* [Viewport] Flackern beim Drehen reduzieren (Schatten aktiviert)
* [Regal] Beim Öffnen von Painter werden Materials standardmäßig angezeigt
* [Regal] Ladezeitverbesserung von Substance-Texturen und -Materialien (2- bis 6-mal schneller)
* [Regal] Neuordnen von Materialien-Ordnern zum Anpassen an die Substance Source
* [Regal] Ziehen Sie Materialien per Drag &amp; Drop direkt auf den Mesh im Viewport
* [Regal] Neue 3D-Rauschen (Perlin, Perlin Fractal, Simplex und Worley)
* [Regal] Neuer 3D Linear gradient-Maskengenerator mit Mesh-Position
* [Regal] Die Basis-Rauschen wurden aktualisiert, um die quadratische Ausbreitung zu unterstützen.
* [Regal] Neue Vorlage und Exportvorgabe für Lens Studio hinzugefügt (Anwendung Einrasten)
* [Regal] Intelligenten Materials und Intelligente Masken wurden aktualisiert, um die neueste Version des Maskeneditors zu verwenden (Mikrodetails)
* [Regal] Neues Beispielprojekt &quot;TilingMaterial&quot; zum Erstellen nahtloser Kachelung-Materialien
* [Regal] Neue Pinselvorgaben (Kalligrafie, Nass, Schraffur usw.)
* [Schieberegler] Neue Schieberegler und Stil und Verhalten von Graustufen-/Farbbalken
* [Baker] Erlauben Sie die Verwendung des Begrenzungsrahmens für die volle Szene, um die Positionskarte zu berechnen.
* [Shader] Entfernen des Height Force-Parameters aus den Standard-Shader-Parametern
* [Engine] Substance Engine aktualisiert
* [Engine] Keine oder weniger Diskontinuitäten zwischen UV-Blöcken
* [Plug-ins] Importieren Sie schneller aus Substance Source heruntergeladene Materials
* [Plug-ins] Alle Plug-ins aktualisieren, um dem neuen Gesamtstil zu entsprechen
* [Voreinstellungen] Automatische Vorschau der Hintergrundfarbänderungen
* [Clean] Geringeres Risiko für Projektbeschädigung
* [Öffnen] Verbesserung der Projektzeit wird geöffnet
* [Neues Projekt] Neues Projekt - Verbesserung der Aktualisierungszeit des Meshs
* [Speichern] Speichern der Zeitverbesserung für das Projekt
* [Protokoll] Im Protokoll angegebener Lizenztyp
* [TextureSet] Schaltfläche &quot;Baking Texturen&quot; in &quot;Baking Mesh-Map&quot; umbenennen
* Benennen Sie &quot;Zusätzliche Maps&quot; in &quot;Mesh-Map&quot; um

**Fest:**

* [Viewport] Fehlerhafte Bewegungen mit Meshs, die viele Unterobjekte enthalten
* [Werkzeugeigenschaften] Kanal deaktiviert, wenn ein Material per Drag &amp; Drop in den Bildschlitz gezogen wird
* [Werkzeugeigenschaften] Pinselvorschau wird mit Verwisch- und Kopierwerkzeugen beschädigt
* [Textursatz] Die Reihenfolge der Kanäle ist falsch, wenn Vorlagen verwendet werden
* [Regal] Fehlendes Symbol für Graustufenkonvertierung-Generator
* [Regal] Alpha-Zahl für Signaturkreise ist fehlerhaft (fehlende Schriftart)
* Falsche Erkennung integrierter GPUs beim Start
* [Absturz] Ziehen und Ablegen einer importierten Ressource mit dem Namen &quot;#&quot;
* [Engine] Vram-Erkennungsproblem auf integrierter GPU
* [Engine] Mehrere Absturz im Substance Engine Linker behoben
* [Engine] Quadratische Artefakte bei der Änderung der Auflösung
* [Post-Effekte] Die Größe der Benutzeroberfläche ist langsam, wenn Post-Effekte aktiviert sind
* [Baker] Szene wird für Strahlenentfernungswerte nicht korrekt eingehalten
* [Baker] AO vom Mesh-Verdeckungsabstand wird unabhängig vom Eingabewert auf 1 geklemmt
* [Baker] Bei der Namensübereinstimmung werden einige Mesh mit bestimmten Namen ignoriert.
* [Baker] Die Farbe aus den Einstellungen &quot;Mesh-Polygruppe&quot; und &quot;Teilgitter-ID&quot; gibt immer ein schwarzes Bild zurück.
* [Baker] ID-Baking schlägt mit binären FBX-Meshs von Blender fehl
* [Shader] Rauschen in der 2D-Ansicht mit dota-2 und non-pbr-spec-gloss
* [Linux] Beim Baking wird nur ein CPU-Thread verwendet.
* [MacOS] Absturz mit dem Pinselcursor, der sich über den Viewport bewegt

**Bekannte Probleme:**

* Einfrieren der Berechnung auf AMD VEGA-GPUs
* Verzerrungsnachbearbeitung wird beim Export in Iray nicht berücksichtigt (Alpha)

## Version 3

### 3.4.2 (2017.4.2)

*(Freigegeben: 24. Januar 2018)*

**Hinzugefügt:**

* [Export] Erhalten Sie den Status eines Exports mit Schrittfortschritt
* [Exportieren] Abbrechen eines Exports zulassen
* [Exportieren] Exportieren von Texturen in Sketchfab ohne Qualitätsverlust beim Normalen-Map
* [Export] Export im glTF-Binärformat (glb)
* [Export] Zulassen der Spaltengrößenänderung auf der Registerkarte &quot;Konfiguration&quot; des Exportfensters
* [Shader] Fügen Sie ein Änderungsprotokoll für den Shader-API hinzu.
* [Scripting] Vor- und Nachher-Rückruffunktionen beim Exportieren von Texturen hinzufügen
* [Iray] Upgrade auf SDK 2017.1 (Unterstützung für Volta-GPUs)

**Fest:**

* Absturz beim Beenden der Anwendung, bevor das Hauptfenster angezeigt wird
* [MAC] Absturz beim Laden von Graustufenkarten mit IRAY
* [MAC] VRAM Erkennung ist mit dem neuen Betriebssystem High Sierra nicht korrekt.
* [Plug-In] Das Herunterladen von Assets aus Substance Source funktioniert nicht mehr
* [Scripting] Falsche Erkennung der Mindestversion des Plug-ins
* [Exportieren] Exportvorgabe kann nach dem Exportieren von Texturen nicht gespeichert werden
* [Instanz] Problem mit Generatoren, die in einem TextureSet ohne zusätzliche Maps instanziieren werden
* [Viewport] Dithering funktioniert nicht mit einer Auflösung über 4k
* [Viewport] 2D-Ansicht Material Display ist mit Rauschen überzogen
* [Regal] Verbessern der Ladezeit für Regal-Vorgaben
* [Engine] Falsche Füllmethode beim Malen unter Farbauswahl

### 3.4.1 (2017.4.1)

*(Freigegeben: 15. Dezember 2017)*

**Hinzugefügt:**

* [Scripting] Exportieren von Mesh über die Scripting-API
* [Importieren] Import nicht unterstützter Meshdateien deaktivieren (nur obj, fbx, date, play zulassen)
* [Log] Präzisere Angabe des TDR-Problems in der Protokolldatei

**Fest:**

* Absturz, wenn die Anwendung geschlossen wird, bevor das Crawlen der Ressourcen abgeschlossen ist
* Absturz beim Öffnen von Projekten mit dem Verwischen-/Klon-Werkzeug
* Absturz bei der Verwendung von &quot;redo&quot; nach einem Rückgängigmachen einer Shader-Änderung in den Anzeigeeinstellungen
* [Engine] Die Texturierung unterscheidet sich zwischen Painter 2017.2 und 2017.4
* [Viewport] Beim Auswählen auf einem ID-Map aus einer Instanz wird die falsche Farbe aufgenommen.
* [Exportieren] Absturz beim Exportieren einer ungültigen Normal- oder Verdeckung-Textur
* [Exportieren] Beim Öffnen von PSD-Dateien in Photoshop CS6 sind die Gruppen gesperrt
* [Plugin] Photoshop Plugin ignoriert die Kanalauswahl und exportiert immer alles
* [Ebenen] Ankerpunkte brechen beim Kopieren/Einfügen über Textursatz hinweg ab
* [Ebenen] Einige Ankerreferenzen können nicht wiederhergestellt werden, wenn sie beschädigt sind
* [Shader] Der Parameter für die sekundäre Rauheit mit pbr-Beschichtung ist defekt.
* [Steam] Popup zur Versionsprüfung sollte beim Start nicht sichtbar sein

**Bekannte Probleme:**

* [AMD] Absturz/Einfrieren beim Malen auf einem Mesh. Kann mit einem GPU-Treiber-Update behoben werden.

### 3.4.0 (2017.4.0)

*(Freigegeben: 23. November 2017)*

**Hinzugefügt:**

* [Instanz] Ermöglicht den instanziieren von Parametern über Ebenen hinweg
* [Instanz] Erlaubt das Wechseln zwischen einer Quellebene und einer Instanz.
* [Instanz] Hinzufügen einer Aktion &quot;instanziieren über Textursatz hinweg&quot;
* [Instanz] Geben Sie im Ebenenstapel wieder eintretende Instanzen (Zyklen) an.
* [Instanz] Instanzen löschen, wenn eine Quelle entfernt wird
* [Instanz] Verweise auf Anker von außerhalb eines instanzierten Ordners nicht zulassen
* [UI] Verschieben Sie den Stapel &quot;Rückgängig&quot; in ein eigenes Fenster mit dem Namen &quot;Verlauf&quot;
* [Plug-In] DCC-Live-Link-Plug-In integrieren
* [Engine] Verbessern der Malleistung mit Sparse-Malerei
* [Exportieren] Optionen für Entwürfe und Re-Exporte zum Sketchfab-Exporter hinzufügen
* [Regal] Hinzufügen einer &quot;Spiegeln&quot;-Steuerung für Schriftsubstanzen
* [Regal] 20 neue Prozeduren hinzufügen Materials
* [Regal] 40 neue Grunges Maps hinzufügen (Bitmap-basiert und prozedural)
* [Viewport] Aktivieren von Kollisionen in der Pinselvorschau auf anderen sichtbaren Textursätzen
* Mindestanforderungen für AMD GPU-Treiber aktualisieren

**Fest:**

* Absturz Beim Berechnen von Substance mit zu großen Auflösungen
* Absturz beim Malen mit Partikeln
* [Viewport] Falsche Specular-Reflexion in der 2D-Ansicht mit bestimmten Meshs
* [UI] Einige unerwünschte Aktionen werden im Protokollfenster angezeigt

**Bekannte Probleme:**

* [Ebenen] Einige Ankerreferenzen können nicht wiederhergestellt werden, wenn sie beschädigt sind
* Absturz bei der Verwendung von &quot;redo&quot; nach einem Rückgängigmachen einer Shader-Änderung in den Anzeigeeinstellungen

### 3.3.3 (2017.3.3)

*(Freigegeben: 1. Dezember 2017)*

**Fest:**

* [Steam] Popup zur Versionsprüfung sollte beim Start nicht sichtbar sein
* [Exportieren] Beim Öffnen von PSD-Dateien in Photoshop CS6 sind die Gruppen gesperrt

### 3.3.2 (2017.3.2)

*(Freigegeben: 20. November 2017)*

**Hinzugefügt:**

* [UI] Dialogfeld &quot;Neue Version verbessern&quot; und Änderungsprotokoll hinzufügen
* [UI] Geben Sie an, ob die Wartung im Dialogfeld &quot;Neue Version&quot; abgelaufen ist
* [Lizenz] Aktualisieren Sie das Lizenzsystem, um Wartungsdaten zu verarbeiten.
* [Exportieren] Adobe Standard Material in Adobe Dimension umbenennen

**Fest:**

* [Mac] Das Malen führt zu schwarzen Quadraten und Beschädigungen der Textur
* [Engine] Der Cache kann manchmal im Viewport verschwinden
* [Engine] Blockige Artefakte werden angezeigt, wenn der Speicherkomprimierungsauslöser aktiviert wird
* [Baking] Seltsame Fehlermeldungen beim Baking bestimmter Mesh
* [Exportieren] PSD werden falsch geschrieben und von Photoshop nicht richtig erkannt
* [Ebenen] Ebenen sollten nicht projektübergreifend kopiert/eingefügt werden können.
* [Substance] UserData-Farbraum für normale Eingabe wird in einigen Fällen gespiegelt
* [Regal] Mikronormal in Generatoren gibt invertierte Krümmung aus
* [Regal] HSL wirken sich auch auf den Alphakanal aus
* [Linux] Installation auf Centos schlägt aufgrund fehlender Abhängigkeiten fehl.
* Das Installationsprogramm entfernt in bestimmten Fällen nicht alle Ressourcen aus der vorherigen Installation

### 3.3.1 (2017.3.1)

*(Freigegeben: 26. Oktober 2017)*

**Hinzugefügt:**

* [Exportieren] Mesh aus einem Projekt exportieren
* [Regal] Entfernen Sie &quot;Sub-Regal&quot; aus den Registerkartentiteln.
* Einstellungen für die Nachbearbeitung in Vorlagen speichern
* Die TDR-Meldung verständlicher machen
* Fenster &quot;Einstellungen&quot; verbessern, um Fehler zu melden

**Fest:**

* Absturz beim Löschen mehrerer untergeordneter Regal
* Absturz beim Wechsel von einer Ebene zu einer anderen während einer Engine-Berechnung
* [Mac] Absturz auf der Intel-GPU während der Engine-Berechnungen
* [Mac][Viewport] Fehlerhafte Leistung, wenn Dithering aktiviert ist
* [Mac] MacOS 10.13 wird in der Protokolldatei als &quot;Unbekannte Version&quot; erkannt
* [Baker] Das Baking führ mit einem Käfig funktioniert nicht mehr
* [Ebenen] Strg + C Tastaturbefehl (Aktion kopieren) funktioniert nicht mehr
* [Ebenen] Beim Einfügen von Ebenen wird die Benutzeroberfläche mit Ankerreferenzen nicht aktualisiert
* [Anker] Duplizieren oder Kopieren/Einfügen der Ebene mit Referenzen unterbricht Verknüpfungen
* [Exportieren] 8K-Export kann Absturz oder Deadlock-Anwendung in einigen Fällen
* [Export] Mehrere Probleme im generierten glTF-Dateiformat
* [Importieren] Der erneute Import eines Meshs mit demselben Dateinamen funktioniert nicht mehr
* [Plugin] Fenster zum automatischen Speichern wird immer über allem angezeigt
* [UI] Endlose Schleife, wenn Sie im TDR-Dialog &quot;Escape&quot; drücken
* [UI] &quot;UI zurücksetzen&quot; zeigt eine zweite Titelleiste im Fenster &quot;Regal&quot; an

### 3.3.0 (2017.3.0)

*(Freigegeben: 28. September 2017)*

**Hinzugefügt:**

* [Exportieren] Mesh und Texturen für Adobe Project Felix exportieren
* [Exportieren] Export in das glTF-Dateiformat zulassen
* [Engine] Optimieren der Größe von Texturen in VRAM mithilfe der Blockkomprimierung
* [Viewport] Mesh oder Projekt in den Viewport ziehen und dort ablegen
* [UI] Verbessern der Warnmeldung bei TDR
* [UI] Protokoll sollte nur auf Anfrage angezeigt werden
* [UI] Inhalt des Protokollfensters löschen
* [UI] Anzeigen von Warnungen und Fehlern in der Statuszeile
* [UI] Registerkarten oben anzeigen wie in Webbrowsern
* [UI] Verbessern des Kontexts und der Meldungen &quot;nicht bemalbar&quot;
* [UI] Aktion &quot;Als Kopie speichern&quot; im Dateimenü hinzufügen
* [Ebene] Legen Sie die Standardeinstellung für die Kachelung standardmäßig auf 1 fest.
* [Regal] Verbesserter Verlaufsfilter zur Unterstützung von 10 dynamischen Farben
* [Regal] Fügen Sie ein Leerzeichen in der Standardabfrage des Mini-Regals hinzu
* [Regal] Hinzufügen einer Aktion &quot;Im Explorer öffnen&quot; für lokale Ressourcen im Regal
* [Regal] Vorlage und Shader für Adobe Material Standard hinzufügen (Project Felix)
* [Regal] Erhöhen der maximalen Kachelung in Material-Ebenenschattierungen auf 128
* [Regal] Hinzugefügte Sobel-Krümmung für Mikrodetails von Maskengeneratoren
* [Plug-in] Plug-in zum automatischen Speichern mit anpassbarem Zeitintervall hinzufügen
* [Skripterstellung] Hinzufügen einer Funktion zum Speichern als Kopie

**Fest:**

* [UI] Layout wird beim ersten Start beschädigt
* [Exportieren] Beim Exportieren generierte PSD weisen Formatfehler auf
* [Exportieren] EXR exportiert immer 8-Bit-Höhen-Map
* [Exportieren] Absturz beim Exportieren beschädigter zusätzlicher Maps
* [Importieren] Harte Kanten werden bei niedrigen Poly-Meshs in einigen Fällen nicht beibehalten
* [Import] Verbesserte Fehlermeldungen beim Importieren von Meshs mit Problemen
* [Baker] ID-Map-Baking schlägt fehl, wenn &quot;Nach Name abgleichen&quot; aktiviert ist
* [Viewport] Tangente-Space wird nicht mit Bakern synchronisiert
* [Effekt] Das Zurückverschieben einer Ebene stellt die Referenz eines Ankers nicht wieder her.
* [Effekt] Aktualisierungsproblem beim Erstellen einer Verknüpfung zwischen zwei Masken mit Ankern
* [Effekt] Maskenanker über der Maske sollten nicht aufgeführt werden
* [Effekt] Die Einstellung &quot;Alpha aus Ankern extrahieren&quot; funktioniert nicht
* [Engine] Maske kehrt sich nach dem ersten Pinselstrich um
* [Engine] Absturz beim Wechseln des Textursatzes in einem bestimmten Projekt
* [Regal] Absturz beim Löschen einer Vorgabe, die sich in einem Projekt befindet
* [Regal] Typo in erweitertem Tri-Planar-Filter
* [Regal] MG Mask Builder AO Rauschen Scale funktioniert nicht richtig
* [Regal] MG Mask Builder hat invertierte Parameter für die Krümmung
* [Regal] Importierte Alphas erzeugen eine Material-Kugelvorschau anstelle einer flachen.

### 3.2.0 (2017.2.0)

*(Freigegeben: 27. Juli 2017)*

**Hinzugefügt:**

* Ankerpunkte - Ebenen- und Maskenreferenzsystem
* [Ebenen] Möglichkeit, Füll- und Malen-Effekte umzubenennen
* [Plug-In] Aktualisiertes Substance Source-Plug-In
* [Scripting] Abfrage der Auflösung des Textursatzes zulassen
* [Scripting] Ermöglicht das Abrufen des Status des Painting-Engine
* [Leistung] Verbessertes Laden des Projekts und Optimieren des Pinselstempels

**Fest:**

* [Tool] Leistungsprobleme beim Anpassen von Material-Parametern
* [Engine] Verschwindende Pinselstriche bei Änderung der Auflösung (4K>2K)
* [3D-Ansicht] Tangente-Speicherplatz wird nicht mit Bakern synchronisiert
* [Regal] Der Regal-Pfad in den Benutzerdokumenten wird nicht automatisch erstellt
* [Regal] Kompatibilität von Vorgaben mit Vorgängerversionen nach einem Update
* [Shader] Nicht-PBR-Shader funktioniert nicht mehr
* [Baker] ID-Map-Baking schlägt fehl, wenn &quot;Nach Name abgleichen&quot; aktiviert ist
* [Beispiel] Die Namen der Meet Mat-Beispielprojekt-Textursatz sind falsch
* Beim Speichern eines Projekts vor dem Erstellen einer Vorlage werden Schreibberechtigungsfehler zurückgegeben.

### 3.1.0 (2017.1.0)

*(Freigegeben: 20. Juni 2017)*

**Hinzugefügt:**

* [Plug-in] Neues Substance Source-Plug-in (ermöglicht das Herunterladen von Assets im Regal)
* [Regal] 4 Neue Schriftarten (Japanisch + vereinfachtes Chinesisch, Schreibmaschine, Segment)
* [Regal] 230 Neue Alpha (Mischung aus Mustern, Pinseln und Fingerabdruckscans)
* [Regal] 50 Neue Prozedurale (Stoffmuster mittelalterlicher und zeitgenössischer Bekleidung)
* [Regal] 2 neue Umgebungs-Map (Mondarrain und Villa Nova Street)
* [Regal] 9 Neue Filter (MatFx-Edge Wear &quot;Details&quot;, &quot;Beschränkt&quot;, HBAO usw.)
* [Regal] Verbessertes standardmäßiges Panorama-Umgebungs-Map
* [Regal] Neue Arnold 5-Exportvorgaben
* [Scripting] Importieren der Ressource in das Regal zulassen

**Bekannte Probleme:**

* [Exportieren] Die Bearbeitung einer Exportvorgabe ist sehr langsam

## Version 2

### 2.6.2

*(Freigegeben: 20. Oktober 2017)*

<b>Hinzugefügt:</b>

* [Textursatz] Löschen deaktivierter Textursatz zulassen
* [Regal] Mehrere Benutzer können im selben Regal-Ordner schreiben
* [Scripting] Ordner &quot;Plug-ins&quot; neu laden können
* [Scripting] Fügen Sie eine erforderliche minimale API-Version in den Plug-in-Metadaten hinzu, um die Kompatibilität zu gewährleisten
* [Iray] Verbesserungen im Dialogfeld &quot;Bild exportieren&quot;

<b>Fest:</b>

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

*(Freigegeben: 12. Mai 2017)*

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

*(Freigegeben: 27. April 2017)*

**Hinzugefügt:**

* Neues Beispielprojekt &quot;Meet Mat&quot; hinzufügen
* [Plug-In] Neues Plug-In &quot;Resources Updater&quot;
* [TextureSet] Umbenennen und Hinzufügen einer Beschreibung zu Textursätzen zulassen
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
* [Protokoll] Fehler bei ausgeblendeten Textursätzen entfernen
* &quot;Begrüßungsbildschirm&quot; mit neuen Symbolen und Text für Beispiele aktualisieren

**Fest:**

* Absturz beim Aktualisieren eines Meshs in bestimmten Projekten
* [Viewport] Symmetrie Ebene Innenfarbe ist nicht mehr sichtbar
* [Viewport] Einige Nachbearbeitungseffekte sind aktiviert, wenn die Solo-Ansicht verwendet wird
* [Shaders] Überblendung mit &quot;\_premult&quot; funktioniert nicht richtig
* [Shaders] Warnung vor Alpha-Test mit dem Standard-Shader
* [Regal] Falsches Analysieren von Tags aus Substance
* [Regal] MatFX Rost Verwitterung funktioniert nicht richtig
* [Regal] HSL ist standardmäßig für falsche Kanäle aktiviert.
* [Regal] Der Scharfzeichner ist standardmäßig für den Height-/Normalkanal aktiviert
* [Exportieren] Verschiedene Exportvorgaben verwenden keine OpenGL-Normalen-Map
* [Tool] Ungenauigkeitsprobleme mit dem Klonen-/Verwischen-Werkzeug erzeugen Artefakte

### 2.5.3

*(Freigegeben: 15. März 2017)*

**Fest:**

* [Baker] Absturz beim Baking führ mit bestimmten Meshs

**Bekannte Probleme:**

* [Mac] Partikeln können in einigen Fällen zu Beschädigungen der Textur führen

### 2.5.2

*(Freigegeben: 14. März 2017)*

**Fest:**

* [Tool] Wacom-Tablets funktionieren unter Linux nicht
* [Werkzeug] Schwarze Artefakte bei Verwendung des Verwischen-Werkzeugs
* [Baker] Baking schlägt fehl, wenn &quot;Nach Name abgleichen&quot; mit einem Käfig verwendet wird
* [Baker] Ambient occlusion beim Baking nur mit Normalen-Map unterbrochen
* [Regal] Generische Filter behandeln Alpha nicht ordnungsgemäß (Kontrast/Luminanz, Hochpass usw.)
* [Viewport] Leistungsproblem beim Laden eines Projekts mit aktivierten Schatten
* [Viewport] Dithering-Problem in 3D-Ansichten über MacOS
* [Viewport] Partikel-Vorschauen werden falsch angezeigt, wenn Farbprofil aktiviert ist
* [Iray] Absturz beim Zurückwechseln des Projekts zu OpenGL, wenn Iray nicht initialisiert werden konnte
* [Iray] Glanz wird beim Rendern von SpecGloss Shader/mdl ignoriert
* [Shader] Spec/Gloss Shader stimmt nicht mit Iray und SD überein
* [Shader] sRGB-Konvertierung unterscheidet sich von der linearen in die sRGB-LUT-Konvertierung
* [Shader] Falsches Rendering beim Laden eines Projekts mit veralteten Shadern
* [Shader] &quot;pbr-coated&quot;-Shader funktioniert nicht mehr
* [Exportieren] Einige Kanäle werden weiterhin exportiert, auch wenn sie nicht im Textursatz vorhanden sind
* [Ebenen] Der Mischmodus &quot;Normalen-Map inverse detail&quot; funktioniert nicht auf Graustufenkanälen
* [UI] Problem beim &quot;Farbauswahl window&quot; mit HDPI-Monitor und Anzeigezoom bei 150 %

**Bekannte Probleme:**

* [Mac] Partikeln können in einigen Fällen zu Beschädigungen der Textur führen

### 2.5.1

*(Freigegeben: 27. Februar 2017)*

**Fest:**

* [Mac] Wacom-Tablet-Eingang in 3D und 2D-Ansicht defekt
* [Baker] Die Zuordnung nach Namen funktioniert nicht mehr
* [Baker] Die Einstellung &quot;Normale Mittelwerte&quot; funktioniert nicht mehr.
* [Iray] Falsches Rendering mit fehlendem Baking geführt Normalen-Map
* [Iray] Farbprofil verhalten sich anders als beim OpenGL-Renderer
* [Iray] Exportieren von Rendering als Bitmap beinhaltet keine Farbprofil-Korrektur
* [Substance] Materialfilter funktionieren nicht mehr
* [Tool] Die Konturdeckkraft wird nicht in Pinselvorgaben gespeichert
* [Tool] Klon Brush UV Alignment funktioniert nicht mehr
* [Versatz] Beim Exportieren in Ganzzahl sollte der Exportkanal auf 0,5 zentriert sein.
* [Vorlage] Absoluter Pfad wird in Vorlagen gespeichert.
* [TextureSet] Die Textur des Kanals bleibt nach dem Entfernen des Kanals bestehen.

**Bekannte Probleme:**

* [Linux] Wacom-Tablet-Eingaben funktionieren nicht in 3D und 2D-Ansicht
* [Mac] Partikeln können in einigen Fällen zu Beschädigungen der Textur führen
* [Exportieren] In sehr seltenen Fällen können auf AMD-GPUs schwarze Rechtecke erscheinen

### 2.5.0

*(Freigegeben: 21. Februar 2017)*

**Hinzugefügt:**

* Unterstützung für AMD Radeon Pro- und AMD FirePro-GPUs
* [Werkzeug] Unterstützung für Konturdeckkraft hinzufügen
* [Werkzeug] Fügen Sie einen Modifizierer hinzu, mit dem Sie den letzten Pinselstrich fortsetzen können
* [Iray] Update zur Unterstützung von Pascal-GPUs
* [Viewport] Unterstützung für Farbprofil hinzufügen (LUT)
* [Substance] Integration eines neuen Frameworks (SD6-Engine)
* [UI] Liste der &quot;zuletzt verwendeten Dateien&quot; im Menü &quot;Datei&quot; vergrößern
* [Importieren] Verwenden Sie die Kategorie aus Stoffen, um das Präfix im Dialogfeld &quot;Importieren&quot; auszufüllen.
* [Baker] Baking von 8K-Texturen zulassen
* [Baker] Baking nicht quadratischer Auflösungen zulassen
* [Baker] Verbessern Sie den Speicherverbrauch beim Baking führ von großen High-Poly-Meshs
* [Regal] Sperren von Regalen (und Projekten), um die gleichzeitige Bearbeitung zu verhindern und Beschädigungen zu vermeiden
* [Regal] Lesen Sie Kategorie und Schlüsselwörter von Stoffen, um sie für die Filterung zu verwenden
* [Regal] Ausschließen von Ressourcen vom Ergebnis einer Suchabfrage zulassen
* [Regal] Verbesserte Berechnung der Miniaturansichten
* [Regal] Einbetten von Vorgaben in Projekte zulassen
* [Regal] Schnelles Reduzieren/Erweitern der Strukturansicht mit UMSCHALT
* [Regal] Speichern von Miniaturansichten zulassen, wenn Assets schreibgeschützt sind (lokaler Cache)
* [Regal] Neuer Inhalt : neue Filter (transformieren, Mirror, Tri-planar usw.)
* [Regal] Neuer Inhalt : neue LUTs-Profile (klassisch und künstlerisch, z. B. Film Noir, Vintage usw.)
* [Regal] Neuer Inhalt : 10 neue Font-Substance zur schnellen Generierung benutzerdefinierter Texte
* [Regal] Neue Vorlagen : Unity 5 und Unreal Engine 4
* [Regal] Verbesserter HSL, um künstlerfreundlicher zu sein
* [Shader] Unterstützung für Specular level-Kanal in PBR-Shadern hinzufügen
* [Shader] Unterstützung für Dithering in Alpha Test Shader hinzufügen
* [Shader] Unterstützung für Parallax Verdeckung Mapping in PBR Shadern hinzufügen
* [Shader] Definieren einer benutzerdefinierten Benutzeroberfläche für Shader-Parameter zulassen
* [MatteLayering] Neuen Maskenkanal für den Workflow der Material-Ebene erstellen
* [Skripterstellung] Metadaten in einem SP-Projekt schreiben dürfen
* [Scripting] Export mit einer bestimmten Exportvorgabe zulassen
* [Scripting] Ermöglicht das Abrufen von Shader-Parametern als JSON.
* [Scripting] Unterstützung für WebSocket-Verbindungen hinzufügen
* [Scripting] Hinzufügen der Möglichkeit zum Laden von Shader-Instanzen
* [Scripting] Fügen Sie die Möglichkeit hinzu, ein neues Projekt zu erstellen
* [Scripting] Ermöglicht das Abrufen der URL des in ein Projekt importierten Meshs.
* [Skripterstellung] Nicht quadratisches Baking zulassen
* [Scripting] Berichtsfehler beim Festlegen von Daten über die Scripting-API
* [Substance] Benutzerdaten-Tag hinzufügen, um Normalen-Map-Format anzugeben

**Fest:**

* Absturz bei der Farbauswahl mit Stoffen
* Absturz beim Laden eines Nicht-RGBA32f-Bildes als Umgebungs-Map
* Absturz beim Malen auf AMD-GPUs
* [Mesh] OBJ Import erkennt keine Materialien ohne MTL-Datei.
* [Mesh] Die Generierung des UDIM-Textursatzes kann auf einigen Meshs falsch sein
* [UI] Schaltfläche &quot;Rückgängig/Wiederholen&quot; in Anzeigeeinstellung &quot;Fokus stehlen&quot; und Mausbildlauf anhalten
* [UI] Einige Beschriftungen werden in High-DPI falsch beschnitten
* [Ebene] Der Ersetzungsmodus für den Malen-Effekt hat ein falsches Verhalten auf der Maske.
* [Ebene] Der Subtrahieren-Mischmodus verhält sich mit Alpha nicht korrekt.
* [Tool] Die Pinselgröße wird in der 2D-Ansicht enorm, wenn auf UV-Rahmen gemalt wird
* [Tool] Einrasten gerade Linie hat ein ungleichmäßiges Verhalten mit High-DPI
* [Tool] Die Auflösung der Schablone ist manchmal falsch
* [Baker] Die Werte für &quot;Max. Verdeckungsabstand&quot; werden festgeklemmt, wenn &quot;relativ zum Begrenzungsrahmen&quot; &quot;Aus&quot; ist.
* [Shader] Stapel- und automatische Parameterkanaldefinitionen stimmen nicht überein
* [3D-Ansicht] Inkonsistente Anzeige des Normalkanals je nach Projekteinstellung
* [Viewport] Einige Normalen-Map haben Werte eingeklemmt, die als Artefakte erscheinen
* [Viewport] Nacheffekte sind standardmäßig immer deaktiviert
* [Export] Die normale Mischeinstellung ist falsch, wenn der normale Kanal fehlt
* [Exportieren] Falsche Generierung von Texturen in einigen Fällen auf AMD-GPUs
* [Exportieren] Shader-Parameter werden nicht ordnungsgemäß exportiert, wenn sie sich in einer Gruppe befinden
* [Exportieren] Beim Bearbeiten einer Exportvorgabe in einem benutzerdefinierten Regal wird ein Protokollfehler ausgegeben
* [Regal] Die Filterungen der Strukturansicht stimmen nicht genau mit dem Ordnernamen überein
* [Regal] Das Umbenennen einer Regal-Vorgabe ist schwer zu lesen
* [Regal] In das Regal importierte Shader-Ressource bleibt nach dem Neustart nicht erhalten
* [Regal] Inhalt : Werkzeugvorgabe fehlt
* [Regal] Inhalt : Tile Generator funktioniert nicht richtig
* [Regal] Inhalt : Falsche Maske auf Gummireifen-Schmutziges intelligente Material behoben
* [Regal] Inhalt : Falscher Gruppenname auf dem Material der Ledertasche wurde behoben
* [Iray] Die Hälfte der Meshs fehlt in Iray
* [Linux] Absturz beim Ziehen einer Ressource über die 3D-Ansicht
* [Mac] Voreinstellungen werden bei jedem Start in Sierra zurückgesetzt

**Bekannte Probleme:**

* [Exportieren] In sehr seltenen Fällen können auf AMD-GPUs schwarze Rechtecke erscheinen
* [Iray] Farbprofile können sich manchmal seltsam verhalten

### 2.4.1

*(Freigegeben: 28. Oktober 2016)*

**Fest:**

* Absturz beim Erstellen eines Projekts mit einer Vorlage
* Absturz beim Schließen des Exportdialogfelds während eines Exports
* [Mac] Fehler beim Speichern des Projekts (Speichern der Exportvorgabe nicht möglich)
* [Regal] Beim Erstellen einer neuen Vorgabe wird diese zweimal angezeigt
* [Regal] Vorgaben können ohne Administratorrechte nicht im schreibgeschützten Modus geladen werden

### 2.4.0

*(Freigegeben: 27. Oktober 2016)*

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

### 2.3.1

*(Freigegeben: 07. Oktober 2016)*

**Hinzugefügt:**

* [Plugin][Photoshop] Geben Sie an, welches Material/welcher Stapel/welche Kanäle exportiert werden sollen.
* [Scripting] Funktionsnamen weisen einige Inkonsistenzen auf.

**Fest:**

* [Exportieren] Alpha kann in benutzerdefinierten Exportvorgaben verworfen werden
* [Exportieren] Alpha erhält falsche Gamma-Konvertierung auf sRGB-Kanälen
* [Exportieren] Nicht quadratische Dokumente werden als quadratisch exportiert
* [Exportieren] Zusätzliche Karten können nicht exportiert werden, wenn eine fehlt
* [Iray] Einige Parameter (wie &quot;emissive-Intensität&quot;) haben keine Auswirkungen
* [NVIDIA] Absturz beim Start mit NVIDIA Quadro K2200/GTX 750/760
* [AMD] Falscher Farbsatz für Miniaturen und Vorschauen
* [AMD] Einfrieren und Treiberfehler beim Öffnen neuer Dateien und Dateien
* [Log] &quot;software-version&quot; fehlt in der Protokolldatei

### 2.3.0

*(Freigegeben: 15. September 2016)*

**Hinzugefügt:**

* [Plug-In] Neues Plug-In &quot;Nach Photoshop exportieren&quot; (vollständiger Ebenenstapel exportieren)
* [Exportieren] Geben Sie die Breite der Auffüllung an (in Pixel oder unendlich).
* [Exportieren] Festlegen des Hintergrundtyps außerhalb der UVs zulassen
* [Regal] Neues Material mit Shader-Ebenen zum Überblenden von 10 Materialien
* [Regal] Neuer Tonkanal zur Anzeige von Shadern mit dem Height-/Normalkanal
* [Regal] Neuer Baking geführt Lichtfilter mit Umgebungseingabe
* [Regal] Einige Maskengenerator wurden aktualisiert, um nicht quadratische Transformationen hinzuzufügen.
* [Viewport] Hinzufügen von Composite-Normalen-Map (Normal+Height+Baking) zum Solomodus
* [Skripterstellung] Exportieren zusätzlicher Maps zulassen
* [Skripterstellung] Abfrage verfügbarer zusätzlicher Maps pro Textursatz zulassen
* [Scripting] Kanalformat kann abgerufen werden.
* [Skripterstellung] Hinzufügen von Beispielen in der Dokumentation zum Baking
* [Scripting] Ermöglicht das Abfragen der Sichtbarkeit einer Ebene.
* [Skripterstellung] Ermöglicht das Abfragen der Füllmethode und Deckkraft der Ebene
* [Skripterstellung] Exportieren konvertierter Maps (endgültige Normalen-Map, gemischte AO usw.)
* [Substance] Benutzerdefinierte Verwendungen lesen und verbinden
* [Shortcuts] Zusatztaste (SHIFT) hinzufügen, um Solo-Modus rückwärts zu durchlaufen
* [Exportieren] Standardvorgabe für den Export wurde aktualisiert, um Alpha zu deaktivieren
* [UI] Miniaturen werden jetzt nur berechnet, wenn das Engine verfügbar ist
* [UI] Anzeigen einer Erwähnung bei der Berechnung von Miniaturansichten

**Fest:**

* Absturz zu einigen alten Projekten beim Öffnen
* Absturz mit beschädigtem Textur-Kanal-Cache
* Absturz beim Mischen von mehr als 4 Materialien mit dem Material-Ebenen-Arbeitsablauf
* [UI] Tastenkombinationen funktionieren nicht, wenn die Symbolleiste ausgeblendet ist
* [UI] Iray-Symbolleiste ist im Menü &quot;Ansicht&quot; mit &quot;Unbenannt&quot; beschriftet
* [UI] Plug-in-Symbolleisten werden im Menü &quot;Ansicht&quot; als &quot;Nicht geneigt&quot; bezeichnet
* [Baker] Drücken der Eingabetaste beim Bearbeiten einer Baking-Einstellung startet den Baking-Prozess
* [Baker] Falsche Bereiche für einige Parameter
* [Importieren] OBJ Mesh können aufgrund sehr großer Zahlen nicht importiert werden.
* [Importieren] Einige OBJ werden mit zu vielen Unterobjekten importiert
* [Export] Kanalhintergrund wird beim Export mit Schwarz anstelle der Standardfarbe gefüllt
* [Tool] Partikeln funktionieren nicht richtig, wenn der FOV-Wert zu niedrig ist
* [Tool] Die Pinselvorschaufarbe ist bei Masken in untergeordneten Stapeln falsch
* [Viewport] Wenn der Pinsel in leere Bereiche in der 2D-Ansicht geht, wird er gigantisch
* [Viewport] Leere Pinselvorschau beim Malen mit normalen Texturen
* [Skripterstellung] Falsche Dokumentation : &quot;ao&quot; anstelle von &quot;ambientocclusion&quot; aufgeführt
* [Skripterstellung] Der mit subprocess() begonnene Prozess wird beim Schließen von Painter beendet
* [Regal] Baking geführt Beleuchtungsfilter verwenden falsche AO-Eingabe
* [MacOS] Entferntes Fire Hydrant-Projekt (inkompatibel)
* Standardprojekt wird beim Laden einer \*.spt-Datei geöffnet (anstelle von \*.spp).

**Bekannte Probleme:**

* [Plugin] Aufgrund von Photoshop können das Height und der normale Kanal nicht wie besehen Kamera bewogen werden

### 2.2.0

*(Freigegeben: 22. Juli 2016)*

**Hinzugefügt:**

* [Regal] Verbesserung des Suchsystems und der Suchanfragen
* [Regal] Hinzufügen eines Suchfelds für Mini-Regals
* [Shader] Festlegen der Schrittgenauigkeit für Schieberegler
* [Shader] Hinzufügen einer Schaltfläche &quot;Rückgängig/Wiederholen&quot; für Shader-Parameter
* [Shader] Das erneute Laden eines Shader sollte seine Parameter nicht zurücksetzen.
* [MathLayering] Unterstützung für Dynamische Materialüberlagerung und Sub-Stapel hinzufügen
* [MatLayering] Importieren der JSON-Datei zum Einrichten der Shader-Einstellungen zulassen
* [MathLayering] Limit für Textur-Sampler entsperren (Wechsel zu Bindless-Texturen)
* [Scripting] Einstellung der Baker erlauben und Berechnung starten
* [Substance] &quot;Verwendung&quot; für Ein-/Ausgangsverbindungen zusätzlich zu Identifizierungen verwenden
* [Tool] Ermöglicht die Auswahl des Vorschaukanals im Viewport für das Projektion-Tool

**Fest:**

* Absturz beim Start, wenn sich die Substanzen im falschen Ordner befinden
* Der Absturz-Bericht funktioniert aufgrund einer falschen Protokolldatei manchmal nicht
* [Iray] Post-Effekte werden nicht aktualisiert, wenn Iray angehalten wird
* [Iray] Autofokus-Tastaturbefehl funktioniert nicht mehr
* [Iray] Das Verhalten des Blende-Schiebereglers ändert sich je nach Elementgröße.
* [Ebenen] Der Kanal des ersten Materials ist standardmäßig nicht aktiviert, wenn alle deaktiviert sind
* [Shader] Es werden keine Fehler ausgegeben, wenn ein &quot;param auto&quot; nicht korrekt ist.

**Bekannte Probleme:**

* [Mac] Grenzwert für Textur-Samples auf 16 gesperrt (GPU-Treiberproblem)

### 2.1.1

*(Freigegeben: 1. Juli 2016)*

**Hinzugefügt:**

* [Lizenz] Ändern des Speicherorts der Lizenzdatei
* [Viewport] Fügen Sie einen &quot;B&quot;-Tastaturbefehl hinzu, um zwischen weiteren Karten zu wechseln.
* [Importieren] FBX 2016/2017 ordnungsgemäß importieren
* [Tool] Entfernen von Häkchen bei Verwendung der schnelle Maske
* [Iray] Informationen zu den Abmessungen der Szene hinzufügen
* [Iray] Maximale Anzahl von Samples und Renderzeit erhöhen
* [UI] Aktualisieren Sie das Ergebnis sofort, wenn Sie die Schaltfläche &quot;+/-&quot; für Schieberegler verwenden
* [UI] Höhere Präzision für Graustufen-Schieberegler
* [Exportieren] Exportieren Sie keinen Alphakanal für Texturen, die nur RGB sind
* [Exportieren] Dota 2-Exportvorgabe aktualisieren
* [Regal] Neues Muster &quot;Sechseckfliesen&quot;
* [Regal] Neues Werkzeug &quot;Verschweißt&quot;
* [Regal] Aktualisierte Abschlussfilter, um Richtungssteuerungen bereitzustellen

**Fest:**

* [Exportieren] PSD-Dateien können nicht in 8 Bit exportiert werden
* [Export] 8K-Export ist bei einigen Hardware-Konfigurationen nicht verfügbar.
* [Exportieren] Sketchfab-Fenster wird beschnitten
* [Exportieren] Falsche Rauheit-Map in der Spezifikation/Glanz-Exportvoreinstellung
* [UI] Die Eingabe in Graustufenreglern funktioniert nicht mehr
* [UI] Filter können nicht in Substance-Eingaben (wie Generatoren) eingefügt werden
* [UI] Einige Regler haben ein seltsames Verhalten.
* [UI] DeltaTime +/- für Partikeln ist zu groß
* [Iray] Einige Projekte blockieren die Anwendung beim Wechsel zu Iray
* [Iray] Absturz beim Erkennen der Hardware
* [Werkzeug] Die Pinselvorschaufarbe ist im Maskenmodus falsch
* [Tool] Material Picker kann mit inkompatiblen Tools verwendet werden
* [Tool] Projektion-Vorschau wechselt nicht zu Diffuse mit Spec/Gloss-Workflow
* [Regal] Ändern des Standard-Shader unterbricht Smart Mats/intelligente Masken-Vorschauen
* [Regal] Einige intelligente Material haben falsche Namen
* [Regal] Zusätzliche Alpha-Formen sind beschädigt und werden nicht geladen
* [Viewport] Wechseln in den Modus &quot;Zusätzliche Karte&quot; zeigt zuerst &quot;andere&quot; an
* [Viewport] Viewport wechseln zurück zu &quot;Andere&quot;, wenn keine zusätzliche Map vorhanden ist
* [Absturz][Linux] Absturz-Bericht funktioniert nicht auf Ubuntu (Steam)
* [Absturz][Linux] Web-URL-Links funktionieren nicht auf Ubuntu (Steam)
* [Absturz][Windows] Entfernen Sie &quot;crashwatcher&quot;, wenn Substance Painter nicht mehr ausgeführt wird.
* [Absturz][Mac] Absturz-Berichtssystem funktioniert nicht richtig
* [Absturz] Das Importieren eines Meshs, während bereits ein Mesh importiert wurde, führt zu einem Absturz
* Textursatz beim Auswählen eines Tastaturbefehl nach einem Neustart auf nichts zurückgesetzt

### 2.1.0

*(Freigegeben: Juni 2016)*

**Hinzugefügt:**

* [UDIM] Importieren von UDIM-Kacheln von einem Mesh als Textursatz
* [Linux] Zusätzliche Unterstützung für CentOS 6.6 und Ubuntu 12.4
* [Exportieren] 8K-Auflösung hinzufügen (experimentell)
* [Exportieren] Auswahl der Bittiefe während des Exports zulassen
* [Baker] Mehrere Textursatz gleichzeitig Baking geführt werden können
* Unterstützung hochauflösender Monitore (hohe DPI-Skalierung)
* [Skripterstellung] Benutzerdefinierte Auflösung und Auffüllung pro Textur beim Export festlegen
* [Viewport] Umschalten zwischen Textursatz durch Klicken auf den Mesh zulassen (über Strg+Alt+Klick)
* [Viewport] Setzen Sie den Mauszeiger an die Stelle, wenn Sie mit dem Mausrad zoomen.
* [UI] Standardhintergrundfarbe und Umgebungs-Map-Anzeige aktualisieren
* [UI] Hinzufügen von QuickInfos mit Originalnamen für Benutzerkanäle
* [UI] Hintergrundfarbe für Kanäle ändern, die nicht umbenannt werden können
* [Tool] Entfernen von Häkchen bei Verwendung der schnelle Maske
* [Shader] Gruppen für Shader-Parameter und Materialien/Masken definieren
* [Engine] Optimierung von Kleinstprägungen
* [Schablone] Fügen Sie &quot;W&quot; als Tastaturbefehl hinzu, um die Maske vorübergehend zu aktivieren oder zu deaktivieren.
* [Regal] Fügen Sie eine Kreuzschaltfläche hinzu, um das Suchfeld zu löschen.
* [Regal] Alpha mit einem Klick laden
* [Regal] Neue Exportvorgabe : Vray UDIM, Arnold UDIM, Spec/Gloss von Metal/Rough
* [Regal] Neue Alphas : geometrische Formen, Adern und Zeichen
* Namen und Version in den Eigenschaften der ausführbaren Substance Painter-Datei hinzufügen

**Fest:**

* [Substance] Es ist nicht möglich, den normalen Kanal und die zusätzliche Karte gleichzeitig zu verwenden.
* [Iray] MDL-Brechung und Einstellung der Absorption funktionieren nicht
* [Iray] Originalskala der Szene wird nicht beibehalten
* [Regal] Specular/Glanz-Vorlage verwendet einen falschen Shader
* [Exportieren] Die Standard-Exportvorgabe exportiert einige Maps (wie AO) nicht
* [Viewport] Der Pivot-Punkt wird nicht aktualisiert, wenn Sie außerhalb der UVs in der 2D-Ansicht klicken
* [UI] Reglerwerte sind gerundet
* [UI] Manchmal ist beim Bearbeiten von Reglerwerten ein sehr kleiner freier Speicherplatz vorhanden
* [Neues Projekt] Die Dropdown-Liste &quot;Vorlage&quot; wird nicht korrekt aktualisiert (von 1.x zu 2.x)
* [Scripting] Behobenes &quot;Hover&quot;-Verhalten bei benutzerdefinierten Schaltflächen
* [Mac] Durch Rückgängigmachen in einem leeren Projekt wird die Kamera gesperrt

**Bekannte Probleme:**

* Absturz-Bericht ist auf Ubuntu nicht verfügbar
* Einige URL-Schaltflächen funktionieren möglicherweise nicht. In unseren FAQs finden Sie eine Problemumgehung

### 2.0.5

*(Freigegeben: 29. April 2016)*

**Hinzugefügt:**

* [Regal] Hinzugefügte/aktualisierte Nicht-PBR-Vorlage, Shader- und Exportvoreinstellung
* [Regal] Die UE4-Exportvorgabe wurde aktualisiert und enthält jetzt Ambient occlusion.

**Fest:**

* Absturz beim Öffnen und Speichern einiger Projekte mit beschädigten Ressourcen
* [Viewport] Drahtgitter scheint in der 2D-Ansicht beschädigt zu sein
* [Regal] Verbesserte Leistung einiger Studio-Umgebungs-Map
* [Regal] Einige Studio-Umgebungs-Map werden dupliziert.
* [Regal] Fehlendes &quot;Baking geführt Beleuchtungs-Material&quot;
* [Regal] Fehlender Graustufen-Konvertierungsgenerator

### 2.0.4

*(Freigegeben: 26. April 2016)*

**Hinzugefügt:**

* Verbessern von Mesh-Kollisionen und Optimieren des Drahtgitter-Renderings
* Verbessern der Performance und des Arbeitsspeicher-Managements durch umfangreiche Projekte
* Verbessern der Schiebereglerpräzision und des Schrittmachers
* [UI] Engine nur beim Überprüfen eines Schiebereglers aktualisieren (nicht bei der Eingabe eines Werts)
* [UI] Verschieben Sie den Iray-Schalter auf eine dedizierte Schaltfläche in der Hauptsymbolleiste (und ändern Sie den Tastaturbefehl).
* [Tool] Hinzufügen einer Einstellung für das Verhalten &quot;Speicherort der Klonwerkzeugquelle&quot;
* [Shader] Lesen der Mesh-Scheitelpunkt-Farben in benutzerdefinierten Shadern zulassen
* [Scripting] Liste der Textursatz, Kanäle und Ebenen abrufen
* [Skripterstellung] Hinzufügen von Helfer-Funktionen (URL zum Pfad, Exportpfad aus Projekt abrufen)
* [Mac] Erkennen der Mac OS-&quot;El Capitan&quot;-Version in der Protokolldatei

**Fest:**

* Absturz nach zweitem Export auf Substance share
* Absturz beim Kopieren einer Ebene zwischen Textursätzen mit Schnelle Maske-Daten.
* Einige Projekte haben einen sehr langen Updater, der viel Speicher beansprucht
* [Tool] Absturz bei der Auswahl einer Partikel-Vorgabe mit dem Klon-/Verwischen-Werkzeug
* [Baker] Das Laden von FBX dauert bei großen Meshs zu lange
* [Viewport] Gedehnt Umgebungs-Map auf einigen Computern
* [Viewport] Falsche Gamma-Konvertierung des Alpha-Werts des Pinsels
* [Exportieren] Alpha wird als Transparenz gespeichert und nicht als separater Kanal mit Tiff-Dateien.
* [Export] Der normale Kanal wird immer als OpenGL exportiert
* [Iray] Fehlende Schiebereglernamen für Iray-Einstellungen
* [Iray] Rendern erfolgt mit einer falschen Auflösung bei Retina/hohem DPI-Wert
* [Iray] Absturz beim Ändern der Größe der Benutzeroberfläche im Iray-Modus
* [Iray] Hohe Leistungsverlangsamung beim Rendern mit einigen niedrigen Auflösungen
* [Iray] Pause funktioniert nicht (Iray wird noch im Hintergrund berechnet)
* Normale Kanäle weisen manchmal schwarze Quadrate auf.
* Normale Kanäle werden durch Graustufenfilter invertiert.
* Der Normalkanal wird nicht richtig überblendet, wenn der Stapel über Alpha verfügt
* Das Projekt wird beim Öffnen eines Projekts auf der Festplatte bearbeitet, auch wenn es noch nicht gespeichert wurde
* Das erneute Importieren eines Meshs in einigen Projekten führt zu sehr schlechten GPU-Leistungen
* Die Pinselausrichtung ist falsch, wenn ein Mesh nicht berührt wird
* Substance share-Logo fehlt auf dem Begrüßungsbildschirm

### 2.0.2

*(Freigegeben: 25. März 2016)*

**Hinzugefügt:**

* [Iray] Spezifikations-/Glanzvorlage und Shader aktualisieren, um mit Iray kompatibel zu sein
* [Exportieren] Möglichkeit zum Export von Screenshots nach ArtStation
* [Skripterstellung] Unterstützen Sie die Ausführung aus dem Plug-In-Verzeichnis
* [Skripterstellung] &quot;Speichern unter&quot; zulassen
* [UI] Doppelklicken auf einen Schieberegler zulassen, um seinen Wert zu bearbeiten
* Vela-Beispiel auf Substance share verschieben
* Neues Beispielprojekt : Kugelvorschau
* Benutzer vor einem Konflikt mit Shellerweiterungen warnen

**Fest:**

* Installation von Substance Painter 1.x durch Installationsprogramm außer Kraft gesetzt
* [UI] Das Layout der Kanalliste wurde mit Filtern unterbrochen
* [UI] Shader-Parameter werden nicht angezeigt.
* [UI] Die Größenänderung des Ebenenfensters schneidet den Inhalt falsch zu
* [Werkzeug] Der Deckkraftkanal wird nicht immer richtig verwendet
* [Tool] Verwischen/Klon funktioniert nicht mit Symmetrie
* [Werkzeug] Die Deckkraft der Pinselvorschau ist bei einigen Kanälen falsch
* [Iray] Absturz bei Verwendung von Iray, obwohl es noch nicht erstellt wurde
* [Iray] Die Grafikeinstellungsdaten können nicht aus dem Projekt geladen werden.
* [Iray] Iray kümmert sich nicht um die Einstellungsänderung, nachdem sie angehalten wurde
* [Regal] Das Importieren eines Materials in das Regal funktioniert nicht
* Schablone funktioniert nicht mit dem normalen Kanal
* Absturz beim Malen in einigen Projekten
* Absturz beim Malen mit Partikeln in einigen Projekten
* Absturz mit Pixelprozessor während einiger Berechnungen

### 2.0.0

*(Freigegeben: 16. März 2016)*

**Hinzugefügt:**

* Tastaturbefehl zum Substance Store in der Hauptsymbolleiste
* Iray-Renderer mit Ansichtsmodus und Screenshot-Export
* Unterstützung für die Erstellung und Verwendung von &quot;Intelligente Masken&quot;
* Unterstützung für Specular/Glossines PBR-Arbeitsablauf (mit neuem diffusen Kanal)
* Verketten von Substance (Einstecken von Stoffen in Substance-Image-Eingaben)
* Scripting-Unterstützung mit benutzerdefinierten Plug-ins
* Verbessern der Konvertierung von Height in Normal mithilfe eines Sobel-Filters
* Wechseln der Schablone-/Projektion-Vorschauauflösung zu 2K
* Hinzufügen eines normalen Kanals standardmäßig für neue Projekte
* Benutzerdaten-Tag vom Ausgabeknoten lesen, um Kanäle einer Substanz standardmäßig zu aktivieren/deaktivieren
* Normale/AO-Füllmethode in den TextureSet-Einstellungen gelegt
* [Werkzeug] Neues Verwischen-Werkzeug zum Mischen und Verteilen von Farben
* [Tool] Neues Klon-Tool zum Kopieren von Teilen von Texturen
* [Tool] Kanäle für das Verwischen-, Klon- und Radiergummi-Werkzeug auswählen
* [Ebene] Hinzufügen eines Substance-Namens für den Namen des Fülleffekts
* [Ebene] Maske in Zwischenablage exportieren
* [Viewport] Wechseln zwischen Perspektive und orthografischem Modus
* [Viewport] Sichtfeld im Perspektive-Modus steuern
* [Viewport] Erlaubt das Festlegen der Tiefe des Feldabstands mit STRG+Mittelklick.
* [Viewport] Lassen Sie zu ziehen und legen Sie Umgebungs-Map in der 3D-Ansicht.
* [Viewport] Verbessertes Feedback, wenn das Engine starke Berechnungen ausführt
* [Exportieren] Exportieren von Shader-Parametern in eine JSON-Datei zulassen
* [UI] Benutzeroberfläche mit neuen Symbolen, Farben und Layout aktualisieren
* [UI] Hinzufügen von Elementnamen zu Mini-Regalen
* [UI] &quot;Kanal-Mapping&quot; standardmäßig reduzieren
* [Shader] Wählen Sie eine benutzerdefinierte Farbe für die Parameter der Shader-Textur aus.
* [Regal] Fragen Sie beim Ziehen und Ablegen von Ressourcen nach dem Speicherort für den Import von Dateien
* [Regal] Neuer Vorschaubereich für Intelligente Material und Generatoren
* [Regal] Specular-Glanz-Shader hinzufügen
* [Regal] Neue Hard Surface-Formen
* [Regal] Neue Alphas Texturen und Formen
* [Regal] Neue Skin-Texturen
* [Regal] Neue scanbasierte Material und Smart-Material
* [Regal] Neue intelligenten Materials und Spec/Gloss-Unterstützung für alte
* [Regal] Neue Finish-Filter für metallic Oberflächensimulation
* [Regal] Neuer leistungsstarker Maskengenerator &quot;Mask Editor&quot;
* [Regal] Überarbeitete und bereinigte alte Material
* Neues Beispielprojekt &quot;Vela&quot;

**Fest:**

* [Einstellungen] Drehung und Zoomgeschwindigkeit der Kamera werden vom Projekt überschrieben.
* [Viewport] Präzisionsproblem bei der standardmäßigen normalen Textur führt zu falschen Reflexionen
* [Viewport] Vignette ist standardmäßig aktiviert
* [Viewport] Artefakte erscheinen an den Umgebungs-Map-Rändern (Nvidia-GPUs)
* [Viewport] Miniaturansicht im Modus &quot;Projektion/Schablone&quot; ist sehr lang zum Laden
* [Baker] Baking geführt Texturen in 16-Bit- statt in 32-Bit-Ganzzahl speichern
* [Layer] Veraltete Stoffe werden im Stapel falsch dargestellt
* Standardfarbe und Bit-Tiefe für einige Kanäle sind falsch (z. B. : Specular, Glanz)
* Radierverhalten zum Deaktivieren der Füllmethode im Passthrough-Modus wurde korrigiert

**Bekannte Probleme:**

* Symmetrie funktioniert nicht mit dem Verwischen- und Klon-Werkzeug
* ArtStation-Export fehlt

## Version 1

### 1.7.3

*(Freigegeben: 1. März 2016)*

**Hinzugefügt:**

* [Exportieren] Fügen Sie eine Option hinzu, um die Auffüllung zu deaktivieren.
* [Regal] Untergeordnete Elementhierarchie innerhalb eines Regal-Regals unterstützen

**Fest:**

* Absturz beim Speichern über einer zuvor schreibgeschützten Datei
* Absturz beim Öffnen eines zweiten Projekts
* Absturz beim Laden einiger Miniaturansichten (Regal, Ebenen oder QuickInfos)
* Die Deaktivierung von &quot;Konturpositionen auf dem Mesh beibehalten&quot; funktioniert nicht
* [Exportieren] Hochskalieren von Bitmaps erfolgt mit nächstgelegenen Filterungen
* [Regal] Die Suche nach Ressourcen ist sehr langsam.
* [Regal] Weichzeichnungsfilter sind nicht 16-Bit-kompatibel.
* [Tool] Symmetrie funktioniert nicht, wenn Sie eine alte Werkzeugvorgabe laden
* Das Farbdialogfeld für den Specular-Kanal führt keine Farbraumkonvertierung durch

### 1.7.2

*(Freigegeben: 13. Januar 2016)*

**Hinzugefügt:**

* [Ebenen] Standardbearbeitung für Füllebenen zulassen

**Fest:**

* [Export] Sketchfab-Export funktioniert nicht mehr
* [Ebene] Bilineare Filterungen werden auch auf die Füllung ohne Transformation angewendet
* [Tool] Schlechte Performance bei Verwendung von Substanz mit Bildeingaben im Projektion-Modus
* [Tool] Material-Auswahl ist defekt

### 1.7.1

*(Freigegeben: 18. Dezember 2015)*

**Fest:**

* Absturz beim Wechseln des Textursatzes
* Langsame Bewegungen beim Malen

### 1.7.0

*(Freigegeben: 17. Dezember 2015)*

**Hinzugefügt:**

* [Performances] Berechnen des Inhalts von Ebenen und ihrer Miniaturansichten gleichzeitig
* [Export] Speichern Sie den Exportpfad als relativ, wenn Sie ihn neben dem Projekt
* [Ebenen] Neue Füllmethode hinzugefügt : Subtrahieren und Hinzufügen/Subtrahieren
* [Layers] Neue Bilineare HQ-Filterungen für Füllebenen
* [Shader] Legen Sie in den Voreinstellungen einen Standard-Shader für die Miniaturgenerierung fest.
* [Shader] Geben Sie einen Shader pro Textursatz an.
* [Shader] Texturen aus dem Regal aufnehmen
* [Werkzeug] Neues Pinselverhalten &quot;Umbrechen&quot; für das Malen
* [Tool] Verbesserte Filterung und reduziertes Aliasing beim Malen
* [Tool] Verbesserte Malqualität unter Pixeln
* [Tool] &quot;Einfache&quot; Anzeige für Pinseleinstellungen entfernt und das Symbol zum Öffnen/Schließen des Rahmens verbessert
* [Menü] Hinzufügen von Effektsymbolen im Kontextmenü
* Vorlagenerstellung aus Projekten
* [Regal] Neue Vorlagen : PBR, Dota 2
* [Regal] Neue Exportvorgabe : Dota 2
* [Regal] Neue Shader : Dota 2, PBR Car Malen, PBR Coated, PBR Velvet
* [Regal] Neues Material : Rost und Verschleiß aus Stahl, Stilisierte Beleuchtung
* [Regal] Neue Filter : Weichzeichnen von gerichtetem, stilisiertem Licht
* [Regal] Neuer Pinsel : Standardmäßige weiche und Standardfestplatte mit einem neuen Alpha für eine bessere Steuerung der Härte
* [Regal] Neue Generatoren : 3D-Abstand und -Licht
* [Regal] Aktualisierte Pinsel mit Projektion und Rückseiten-Ausblendung des Umbruchs (standardmäßig aktiviert)
* [Regal] Weißer Rauschen mit Pixelprozessor-Version wurde für eine schnellere Berechnung aktualisiert

**Fest:**

* [Begrüßungsbildschirm] Tutorials-Link an alte Videos senden
* [Channels] Wenn &quot;Nein&quot; zur Erstellung von Füllebenen mit AO gesagt wird, wird immer noch die Ebene erstellt.
* [Kanäle] UserX-Kanalnamen werden in der Schnittstelle nicht weitergegeben
* [Viewport] Der Maskeneintrag ist in der Liste der Solokanäle leer.
* [Freigeben] Exportieren eines Alpha-Elements von SP aus in die Freigabe erstellt eine unlesbare .image-Datei
* [Lizenz] Aktivierung für Benutzernamen mit Nicht-ASCII-Zeichen beheben
* [Shader] Farbparameterdialog verschwindet beim Auswählen einer Farbe
* [Regal] Miniaturansichten werden nicht aus dem Speicher entladen, wenn sie nicht verwendet werden
* [Regal] Filter mit festem Verlauf
* [Tool] Symmetrie funktioniert nicht mit Schablone/Projektion
* [Tool] Falscher Name beim Erstellen einer neuen Pinselvorgabe
* Die Option &quot;Kontur beibehalten&quot; bleibt auch beim erneuten Importieren eines Meshs deaktiviert
* TDR (Driver Reset) beim Berechnen von Partikeln mit großen Abmessungen.

### 1.6.1

*(Freigegeben: 9. November 2015)*

**Fest:**

* Absturz beim Öffnen des Projekts, wenn die 2D-Ansicht sichtbar ist
* Absturz beim Erstellen einer neuen Exportvorgabe, wenn das aktuelle Regal nicht vorhanden ist
* [Tool] Symbol für die Material-Auswahl kann angezeigt bleiben
* [Material] Mausauswahl blendet den Mauszeiger aus, wenn gleichzeitig gemalt wird
* [Regal] Metadaten werden nach jedem Beenden auf die Festplatte geschrieben

### 1.6.0

*(Freigegeben: 29. Oktober 2015)*

**Hinzugefügt:**

* Offizielle Unterstützung für Windows 10
* [Substance] Reduzieren von Stoffparametergruppen standardmäßig
* [Substance] Neues Framework hinzufügen (Verbessern der Leistung des Pixelprozessors)
* [Viewport] Erlaubt die Deaktivierung der Anzeige der Symmetrie im Symmetrie-Modus.
* [Viewport] Verbessern des Schattenrenderings und der Leistung
* [Viewport] Berechnung von Schatten beim Malen anhalten
* [Viewport] Verbessern der Drahtgitter-Renderleistung
* [Engine] Verbessern Sie die VRAM-Speicherverwaltung, um den Speicherbedarf zu reduzieren.
* [Engine] Verbessern der Leistungsaktualisierung auf AMD-GPUs für eine bessere Textur
* [Engine] Deaktivieren der Einstellung für die Threaded-Optimierung auf NVIDIA-GPUs für bessere Leistung
* [Effekt] Fügen Sie ein Tag hinzu, um eine &quot;aufgefüllte&quot; Bildeingabe anzufordern.
* [Ebene] Präzision des UV-Versatzes/der Skalierung in der Füllung erhöhen
* [Ebene] Skalieren Sie den Schieberegler exponentiell in der Füllung
* [Ebene] Materialien können direkt in den Ebenenstapel gezogen und dort abgelegt werden.
* [Ebene] Filter können direkt in den Ebenenstapel gezogen und dort abgelegt werden
* [Ebene] Passen Sie die Maskenpinselfarbe an die neu erstellte Maskenfarbe an
* [Shader] Mehrere Textcodes Gelegt
* [Shader] Leg einer Gamma-/Tonzuordnungsfunktion, um benutzerdefinierte Funktionen zu ermöglichen
* [Baker] Ändern der Standardeinstellungen für den Baker &quot;Position&quot; für die Verwendung von TriPlanar
* [Werkzeug] Benennen Sie &quot;Geometry Decal&quot; in &quot;Polygon Fill&quot; um.
* [Regal] Update-Generatoren zur Unterstützung von TriPlanar : MG Metallkantenverschleiß, MG Maskenbildner, MG Glasfaser, MG Dirt
* [Regal] Aktualisieren von Materialien mit neuen Einstellungen und Entfernen nicht verwendeter Material
* [Regal] 22 Neue intelligente Materialien (Kunststoff, Eisen, Stoff, Stahl und mehr)
* [Regal] Aktualisieren Sie die Scharfzeichner-, Weichzeichner- und Verkrümmungsfilter mit gepolsterter Bildeingabe, um Nähte zu vermeiden
* [Regal] Verbessern der Verkrümmungseinstellungen für eine einfachere Verwendung
* [Regal] 2 Neue prozedurale Rauschen : 3D Perlin Rauschen und 3D Worley Rauschen

**Fest:**

* [Engine] Die Vram-Betragserkennung für die dedizierte GPU ist auf Mac falsch
* [Engine] Texturen werden im Viewport dunkler
* [Engine] Schlechte Performance beim Malen unter mehreren Ebenen
* [Engine] Beim Öffnen des Projekts berechnete Ebenen unterscheiden sich von der zwischengespeicherten Version
* [Substance] Falsche Ergebnisse in 4K auf Mac
* [Substance] Die Parameter haben die falsche Reihenfolge.
* [Shader] Toon- und Pixelshader sind komplett schwarz.
* [Shader] Parameter verschwinden nach dem Ändern von env-map
* [Regal] Absturz beim Bereitstellen von PNG-Dateien im Generatorordner
* [Regal] Miniaturansichten werden mit niedriger Rauheit generiert
* [Tool] Absturz bei Verwendung einer Bitmap im Pinsel-Alpha unter Windows
* [Exportieren] Zusätzliche Kartenexportvoreinstellung exportiert jetzt eine RGB-Karte für die Position

### 1.5.7

*(Freigegeben: 24. September 2015)*

**Fest:**

* Absturz-Bericht funktioniert nicht mehr

### 1.5.6

*(Freigegeben: 21. September 2015)*

**Hinzugefügt:**

* [Regal] Verbessern der Qualität der Miniaturansichten (verwenden Sie 1K-Texturen)

**Fest:**

* [Freigeben] Kann nicht mit einem anderen Konto signiert werden
* [Regal] Miniaturansichten sind auf der Festplatte zu groß
* [Regal] Intelligente Materialien werden sehr langsam geladen
* [Windows] Installation des Lizenzdiensts beheben
* [Channels] Transmissive-Map wird standardmäßig als G8 erstellt

### 1.5.5

*(Freigegeben: 15. September 2015)*

**Hinzugefügt:**

* [Regal] Exportieren von Assets auf Substance share
* [Regal] Hinzufügen einer neuen Kugelvorschau für Materialien
* [Regal] Verwenden Sie die Env-Map &quot;Glaser Patio&quot; zum Generieren von Miniaturen
* [Regal] Erhöhung der Auflösung der Miniaturbildgröße auf 512 x 512 Pixel
* [3D-Ansicht] Umgebungsrotationswert Gelegt
* [Windows] Anwendung signieren

**Fest:**

* [Baker] Falsche Ergebnisse beim gleichzeitigen Baking führ von Maps
* [3D-Ansicht] Die Env-Map wird angezeigt, wenn kein Projekt geöffnet ist
* [Ebenen] Maskengenerator funktionieren nicht auf Ebeneninhalten
* [Ebenen] Sie können auf ausgeblendeten Ebenen Malen
* [Regal] Dirt\_5 und Dirt\_6 Rauschen sind identisch.
* [Regal] Einige Maskengenerator sind verpixelt oder haben eine niedrige Qualität
* [Werkzeug] Falsche Gizmo-Drehung um bestimmte Winkel.
* [Tool] Zu viele Kanäle führen zum Ausschneiden der Kanalschaltflächen
* [Tool] Umkehren des Tastaturbefehl der Maske für die Schnelle Maske funktioniert nicht
* [Exportieren] Sketchfab: Schaltfläche &quot;Abbrechen&quot; wird nicht korrekt berücksichtigt
* [Lizenz] Aktivierung fehlgeschlagen, wenn die Lizenz nicht kopiert werden kann
* Der Framerate-Begrenzer funktioniert nicht mehr auf der Benutzeroberfläche

### 1.5.0

*(Freigegeben: 20. August 2015)*

<b>Hinzugefügt:</b>

* [Shader] Zeilennummer in Fehlermeldungen beim Kompilieren des Shader hinzufügen
* [Regal] Verbessern der Qualität von Miniaturansichten
* [Regal] Automatisierte Miniaturgenerierung für Intelligenten Materials
* [Tool] Tastaturbefehl zur Einstellung der Härte im Stoff
* [Werkzeug] Graustufen-Widget für Geometrieaufkleber verwenden, wenn Sie sich über einer Maske befinden
* [Tool] Tastaturbefehl zum Invertieren der Malen-Farbe beim Malen auf einer Graustufenkarte
* [Viewport] Drahtgitter anzeigen und Farbänderung zulassen
* [Viewport] Weichzeichnen des Umgebungshintergrunds
* [Steuerelemente] Hinzufügen der Drehung zu Kurzbefehlen der Pinselmaus
* [Exportieren] Nach Sketchfab exportieren
* [Exportieren] Erstellen von Exportvorgaben für Renderer
* [Exportieren] Konvertierte Map-Reflexion hinzufügen, F0 und 1/IOR
* [UI] Begrüßungsbildschirm hinzufügen
* [UI] Standardlayout aktualisieren
* [UI] Hinzufügen fehlender QuickInfos und Umbenennen einiger Menüeinträge
* [Ebenen] Exportieren der aktuell ausgewählten Maske als Bitmap
* [Ebenen] Hinzufügen der Aktion &quot;Maske umkehren&quot; im Kontextmenü

<b>Fest:</b>

* [Project] Wenn sich die Mesh-Pivots im FBX unterscheiden, werden die Mesh beim Importieren aufgelöst
* [Substance] Substance in Projektion-Tools sind in 256\*256 gesperrt
* Absturz [Ebenen] bei Verwendung von &quot;Maske löschen&quot;
* [Exportieren] Falsche Gamma-Konvertierung auf sehr dunklen Texturen
* [Export] Positionszuordnung kann nur in Exportvorgaben als Graustufenzuordnung verwendet werden
* [Tool] Die Anfangsfarbe des Geometrie-Aufklebers ist schwarz, wenn er auf einer Maske verwendet wird
* [Tool] Der Tastaturbefehl &quot;Drehung&quot; funktioniert nicht, wenn keine Härte im Alpha-Wert vorhanden ist

### 1.4.2

*(Freigegeben: 15. Juli 2015)*

**Fest:**

* [Tool] Absturz bei Verwendung von Geometrieaufkleber mit schnelle Maske
* Beim Aktualisieren des Projekts von 1.4.0 auf 1.4.1 wird der gesamte Computerspeicher belegt.
* Falscher Import des alten Projektformats
* Bei benutzerdefinierten Regalen wird die gesamte Hierarchie analysiert, und Assets werden überall dupliziert.

### 1.4.1

*(Freigegeben: 23. Juni 2015)*

**Hinzugefügt:**

* [Viewport] Fenster nebeneinander andocken
* [Effekt] Hinzufügen eines Hintergrunds und eines Lineals für den Ebeneneffekt
* [Effekt] Fügen Sie einen Malen-Effekt hinzu, der es ermöglicht, über andere Effekte zu arbeiten

**Fest:**

* [Regal] Miniaturgenerierung funktioniert nicht, wenn kein Projekt geöffnet ist
* [Regal] Materialvorgabe-Vorschau kann nicht generiert werden
* [Regal] Material-Vorschauen werden auf einem Mesh mit invertierten Normalwerten generiert
* [Regal] Miniaturansichten werden aufgrund einer falschen Hashfunktion immer neu berechnet
* [Regal] Durch Klicken auf ein Substance-Material werden keine zusätzlichen Maps verbunden.
* [Tool] Falscher Wert, der mit der Material-Auswahl aufgenommen wurde
* [Tool] Farbwähler wählt Viewport-Cursorfarbe aus
* [2D-Ansicht] Sehr niedrige Framerate/Performance
* [Exportieren] Absturz beim Öffnen des Exportfensters mit zu aktuellen Exportvorgaben.
* [Exportieren] Height-Kanal auf Normalen-Map wird in den falschen Speicherplatz konvertiert
* [Mac] BaseColor aus Substance-Effekten wird als Linear angezeigt
* [Mac] Das Widget für gerade Linien ist auf der Retina falsch gezeichnet
* Gerade Linien können auch bei einem Loslassen des Tastaturbefehl aktiviert bleiben.
* Gerade Linien Guizmo verschwinden nach dem Drehen des Umgebungs-Map
* Ambient occlusion-Ausgänge von Stoffen werden nicht automatisch an den AO-Kanal angeschlossen
* Problem mit Lizenzkopien unter Windows mit Sonderzeichen im Benutzernamen beheben

### 1.4.0

*(Freigegeben: 10. Juni 2015)*

**Hinzugefügt:**

* [Exportieren] Fügen Sie der Liste der verfügbaren Eingabe-Map weitere Maps hinzu
* [Regal] Verwenden von SBSAR-Materialien als Materialvorgaben
* [Regal] Benutzerdefinierte Bibliothekspfade verwenden
* [Regal] Mindestgröße ändern
* [Regal] Neuer Inhalt : 20 neue intelligente Material
* [Regal] Neuer Inhalt : neuer prozeduraler Stoff (Gewebe, Mesh)
* [Regal] Aktualisierter Weichzeichnungsfilter
* Zeichnen von geraden Linien mit einer Zusatztaste
* Hinzufügen eines Ambient occlusion-Kanals und Überarbeiten des AO/Normal-Verhaltens im Ebenenstapel
* Lesen der Standardfarbe aus der Bildeingabe, die in den Substance-Benutzerdaten definiert ist
* Exportieren des Protokolls über das Hilfemenü zulassen

**Fest:**

* [Baker][Mac] Absturz mit Normal vom Mesh Baker
* [Baker] Absturz, wenn die Käfig-Datei keine UVs enthält
* [Baker] Das Abgleichen nach Namen funktioniert nicht mit aus zBrush exportierten OBJ
* [Baker] Das Baking mit einem Käfig überschreibt das Baking, wenn mehrere Textursatz und überlappende UVs verwendet werden.
* [Baker] Bestimmte OBJ führen zu schwarzen Texturen
* [Regal] Ressourcen können nicht gelesen werden, wenn sie auf schreibgeschützt festgelegt sind
* [Regal] Asset-Dateien werden in Painter geschrieben, wenn sie im Projekt verwendet wurden.
* [Regal] Das erneute Laden von Stoffen aktualisiert auch die Schicht
* [Exportieren] Tiff exportiert 32-Bit-Bilder, die von Photoshop oder Game-Enginen nicht richtig gelesen werden können
* [Exportieren] Standardkanalvoreinstellung exportiert immer als RGB
* [Material] Diffuse-Kanal überschreibt BaseColor-Zuordnung mit Substanzen
* [3D-Ansicht] Falsche Beleuchtung von Diffusen mit spezifischen Umgebungskarten
* [Tool] Ein Pinsel kann nicht in einen bestimmten Winkel gedreht werden
* Viewport erhält den Fokus, wenn der Mauszeiger während der Eingabe in einem Textfeld auf
* Absturz mit zu aktuellen Vorgaben für die aktuelle Version des Regals
* Absturz nach dem Ersetzen von Mesh
* Absturz beim erneuten Laden eines Stoffes mit einer anderen Anzahl von Einsatzstoffen
* FBX von Meshs aus dem Cinema4D-Import mit falschen Material-Namen

### 1.3.5

*(Freigegeben: 29. Mai 2015)*

**Hinzugefügt:**

* [Lizenz] Aktivierungsproblem, wenn eine bereits vorhandene Lizenzdatei vorhanden ist
* [Mac] Absturz beim Laden bestimmter FBX
* [Mac][3D-Ansicht] Falsche Reflektion für integrierte GPU
* [3D-Ansicht] Schnelle Maske-Schriftart ist defekt
* [3D-Ansicht] Material-Picker macht den Viewport komplett schwarz
* Absturz nach dem Öffnen von Projekten, die in 1.3.3 erstellt wurden
* Die Vorschau des Materials ist leer, wenn Shader mit Alpha verwendet werden
* Malerei funktioniert nicht mehr an bestimmten Meshs
* Die Leistung nimmt mit bestimmten OBJ Meshs stark ab
* Benutzerkanäle werden bei Verwendung von Effekten nicht zugeordnet
* Temporäre Ordner werden beim Start nicht gesäubert

**Fest:**

* Verbesserte Berechnung des Projekts, das extrem lange geladen werden muss
* Ändern Sie das Fenster &quot;GPU-Fehlerbehebung&quot;, um verständlicher zu sein
* [Ebenen] Speichern Sie den Status der Verhältnissperre für Füllebenen und machen Sie sie standardmäßig &quot;Ein&quot;
* [Baker] Bei der Namensübereinstimmung wird jetzt das Suffix als Trennzeichen verwendet.

### 1.3.4

*(Freigegeben: 27. April 2015)*

**Hinzugefügt:**

* [Mac] Absturz mit Mac OS X Yosemite (10.10)
* [Mac] Vollbildmodus kann nicht beendet werden
* [Baker] Das Baking der Option &quot;Nach Namen abgleichen&quot; funktioniert nicht
* [Baker] Mikk-Tangente-Speicherplatz in SP funktioniert nicht mit UE4
* [Baker] ID-Baker kann die ID-Farben des Materials nicht Baking geführt werden
* [2D-Ansicht] Drahtgitter wird bei Verwendung des Geometry Decal-Werkzeugs nicht angezeigt
* [Tool] Pinsel-Alphakanal wird bei Materialien als Checker anstelle von Transparenz angezeigt
* [Tool] Absturz mit Geometry Decal
* [Ebenen] Material-Slot ist bei der Füllebene standardmäßig ausgeblendet
* [Exportieren] Absturz beim Exportieren mit einer höheren Auflösung als der Textursatz
* Specular-Kanal wird in Filtern nicht erkannt.
* Clean + save entfernt die Ressourcen nicht ordnungsgemäß aus dem Archiv von spp
* Speichern Sie die Low-Poly-Transformation nicht in einer High-Poly-Assbin-Datei
* FBX Datei wird mit zu vielen Textursätzen importiert

**Fest:**

* Effekte: Beschränkt Stufen sollten standardmäßig aktiviert sein, um &quot;klassische&quot; Stufen nachzuahmen
* Ebenen: Ändern der minimalen und maximalen Kachelung in der Füllaktion
* Ebenen: Speichern und Wiederherstellen des Status des Stapels
* Baker: AO-Baker berücksichtigen die Normalen-Map, wenn kein HP angegeben ist
* Baker: Hinzugefügte QuickInfos und zusätzliche Informationen im Fenster &quot;Baking&quot;
* Erstellen einer Sicherungsdatei beim Speichern eines Projekts

### 1.3.3

*(Freigegeben: 1. April 2015)*

**Hinzugefügt:**

* Fügen Sie Softwareversion und Projektnamen in der Titelleiste hinzu
* Bereinigen von Textursatznamen und Intelligente Material-Namen
* Substance Engine auf V5 aktualisieren
* [Regal] Neue Umgebungs-Map hinzufügen : Korsika Strand, Studio 05, Tornoco Studio und mehr
* [Regal] MG Mask Builder mit neuen Parametern aktualisieren
* [Regal] Aktualisieren und Kalibrieren alter Umgebungs-Map

**Fest:**

* Absturz beim Öffnen des Exportfensters
* Drag &amp; Drop im UI-Widget ist nicht möglich, wenn abgedockt
* &quot;Nach Updates suchen&quot; funktioniert nicht
* [Ebenen] Wählen Sie die Maske nicht aus, wenn Sie bei gedrückter Alt-Taste darauf klicken
* [Tool] Tri-planar funktioniert nicht mit dem Normalkanal
* [3D-Ansicht] Diffuse Beleuchtung von env map ist falsch
* [3D-Ansicht] Die Berechnung der Belichtung unterscheidet sich von Designer
* [3D-Ansicht] Schatten sollten auf 100% metallic Fläche nicht sichtbar sein.
* [3D-Ansicht] Mesh mit gespiegelten UVs hat gespiegelte Tangente/Binomale
* [3D-Ansicht] Schatten führen bei bestimmten Meshs zu falschen Ergebnissen
* [Baker] Entfernen Sie den Ordner &quot;.alg\_meta&quot;, der mit Assbin-Dateien erstellt wurde
* [Baker] Absturz beim Baking, wenn Painter ein TextureSet gleichzeitig neu berechnet
* [Mac] Benutzeroberflächenfehler beim Starten der Anwendung

### 1.3.2

*(Freigegeben: 06. März 2015)*

**Fest:**

* [3D-Ansicht] Eine mit dem Projekt gespeicherte Env-Map kann nicht neu geladen werden.

### 1.3.1

*(Freigegeben: 05. März 2015)*

**Hinzugefügt:**

* [Baker] Fügen Sie eine zwischengespeicherte Version von Meshs mit hohem Poly hinzu, um die Berechnung zu beschleunigen
* [Baker] Fügen Sie ein Warnsymbol hinzu, wenn kein hochpolarer Mesh geladen wird.
* [Baker] Wenn kein Mesh mit hoher Poly-Qualität geladen wird, verwenden Sie stattdessen den Projekt-Mesh

**Fest:**

* [Baker] Drücken der &quot;Eingabetaste&quot; beim Bearbeiten des Werts eines Schiebereglers, um das Fenster zu schließen
* [Baker] Das Aktivieren/Deaktivieren eines Bakers löst ebenfalls die Schaltfläche aus.
* [Baker] Es kann nicht Baking geführt werden, wenn Sie die Schaltfläche &quot;all/none&quot; verwenden.
* [Baker] Die Sortierung der Baker-Schaltflächen erfolgt nicht in der richtigen Reihenfolge.
* [Baker] Kontrollkästchen werden ignoriert und alle Baker werden immer verarbeitet.
* [Baker] Der Fortschritt der Fortschrittsleiste wurde behoben.

### 1.3.0

*(Freigegeben: 04. März 2015)*

**Hinzugefügt:**

* [Baker][3D-Ansicht] Verwenden Sie die Mikkt-Tangente-Space-Berechnung, wenn keine Tangenten/Binormale gefunden wurden.
* [Baker] Neue Baker hinzugefügt: Normal, ID, Verdeckung, Krümmung, Thickness, Position
* [Effekte] Effekt-Stapel ist jetzt invertiert und von oben nach unten dargestellt (wie Ebenen)
* [Effects] Hinzufügen neuer Symbole auf dem Stapel des Effekts
* [Effects] Hinzufügen eines Mischmodus zwischen Füllaktionen im Effekt-Stapel
* [Effekte] Umbenennen von Effekten (Substance-Effekt = Filter usw.)
* Hinzufügen einer &quot;gesperrten&quot; Datei während des Speichervorgangs
* [Effects] Aktion &quot;Füllen&quot; im Stapel &quot;Effekt&quot; hinzufügen
* Neue Ressource hinzugefügt : Intelligente Materialien
* [Ebenen] Neuanordnung von Ebeneneffekten zulassen
* [Tool] Drei-Planare Projektion hinzufügen
* [3D-Ansicht] Unterstützung für Schatten hinzufügen
* [3D-Ansicht] Möglichkeit, erforderliche OpenGL-Status in benutzerdefinierte Shader umzuwandeln
* [3D-Ansicht] Unterstützung für Alpha über neue Shader
* [3D-Ansicht] Shader sind jetzt versioniert und vollständig in einem Projekt gespeichert
* [3D-Ansicht] Warnen Sie den Benutzer, wenn der Shader nicht mehr kompiliert wird

**Fest:**

* [Ebenen] Ablegen unter einem reduzierten Ordner korrigieren
* [Regal] Beheben der Filterung von Inhalten in Mini-Regals
* [Regal] Umbenennen von Kategorien und Neuorganisieren von Registerkarten

### 1.2.1

*(Freigegeben: 12. Februar 2015)*

**Hinzugefügt:**

* \*.spp-Dateien können jetzt durch einen Doppelklick im Explorer geöffnet werden
* [Export] Neues Tag &quot;$project&quot; für Exportvorgaben
* [Exportieren] Fügen Sie unter jedem Textursatz eine Kartenliste (mit Nomenklatur) hinzu
* [Exportieren] Hinzufügen einer Schaltfläche Alle/Keine , um die Textursatz auszuwählen
* [Exportieren] Leere Karten werden während des Exports verworfen

**Fest:**

* [Exportieren] Unity5-Vorgaben haben invertierte Karten
* [Exportieren] Das Hinzufügen eines Schrägstrichs in einem Vorgabename führt zu einem beschädigten Ordner
* [Exportieren] Height-Kanal, der in 32-Bit-Formate exportiert wird, ist falsch eingespannt
* [Exportieren] Textursatz-Liste wird nicht wie im Projekt sortiert
* [Tool] Rückseiten-Ausblendung funktioniert nicht mehr
* Speichern funktioniert nicht mit Sonderzeichen im Pfad

### 1.2.0

*(Freigegeben: 28. Januar 2015)*

**Hinzugefügt:**

* Neuer Normalkanal, der das Malen von Normalen-Map-Daten und das Kombinieren der Ergebnisse ermöglicht
* [Exportieren] Neues Exportfenster mit der Möglichkeit, ein benutzerdefiniertes Packing zu erstellen und benutzerdefinierte Namen festzulegen
* Das Projektdateiformat ist jetzt eine einzelne Datei anstelle von Ordnern
* [Exportieren] Unterstützung verschiedener Normalformate (DirectX, OpenGL)
* [Exportieren] Erstellen einer temporären Sperrdatei während des Exports
* [Ebenen] Mit Umschalt+Nach-links-Taste können Sie eine Maske umschalten
* [Parameter] Legt den Farbraum am unteren Rand einer Bildeingabe bei
* [Regal] Effekt &quot;MG Mask Builder&quot; hat jetzt neue Einstellungen
* [3D-Ansicht] Ambient occlusion-Map verschließt jetzt den diffusen Beitrag, nicht den Specular

**Fest:**

* Projektion Material/Schablone Vorschau wird im Viewport nicht richtig angezeigt
* [3D-Ansicht] Tastaturbefehl-QuickInfo wird nicht angezeigt, wenn &quot;S&quot; (Schablone) Tastaturbefehl verwendet wird
* [Regal] Der Effekt &quot;MatFx Skin Scale&quot; bietet jetzt eine bessere Leistung bei niedriger Auflösung.
* [Exportieren] Texturen vom Export werden einfach hochskaliert, wenn eine größere Dokumentgröße angegeben wird

### 1.1.2

*(Freigegeben: 15. Januar 2015)*

**Hinzugefügt:**

* Hinzugefügt: Neue Einstellungen zum Kamera beweg, Drehen und Skalieren in der Füllebene
* Verbesserte Filterung für Pinsel und Füllebenen
* Die Testversion ist jetzt voll funktionsfähig (kann exportiert werden), aber zeitlich begrenzt.

**Fest:**

* Importieren von OBJ-Meshs mit sehr kleinen Präzisionen nicht möglich
* Problem beim Aktivieren einer Lizenz unter Windows 7 und 8
* Absturz beim Speichern eines Projekts
* Absturz beim Löschen des letzten Kanals eines Textursatzes
* Absturz beim Löschen einer Ebene in einem bestimmten Kontext

### 1.1.1

*(Freigegeben: 25. Dezember 2014)*

**Hinzugefügt:**

* [Ebene] Wählen Sie die Ebene oben aus, wenn Sie ein Projekt öffnen/den Textursatz wechseln.
* Verbesserte Geschwindigkeit beim Speichern und Speichern unter mit neuem Komprimierungsalgorithmus
* Anzeige eines Fehlers beim Öffnen eines zu aktuellen Projekts für Painter

**Fest:**

* [Tool] Geometrie Decal produziert Speicherbeschädigungen
* [Pinsel] Gleitkommawerte unter 1 können für die Pinselgröße nicht manuell eingegeben werden
* [Ebene] Durch Erstellen eines Farbauswahl-Effekts wird dieser nicht in den Ebenenstapel eingefügt
* [Ebene] Wenn Sie den Mauszeiger über die Ebenen bewegen, schnipst Painter in die Taskleiste
* [Ebene] Das Hinzufügen einer Bitmap als Maske kann zu einem Absturz führen
* GUI für den Solo-Modus mit dem Height-Kanal ist falsch
* &quot;Projekt speichern&quot; kann fehlschlagen und ein Projekt beschädigen
* Absturz beim Öffnen eines Projekts nach dem Laden eines anderen Projekts mit einem veralteten Shader

### 1.1.0

*(Freigegeben: 16. Dezember 2014)*

**Hinzugefügt:**

* [Effekt] Ersteller einer neuen Materialien-ID-Maske
* Neue gepunktete weiße/schwarze Linie für das Pinsel-Gizmo
* Neuer Parameter &quot;Winkelfolge&quot;
* Neuer Parameter &quot;Rückseiten-Ausblendung&quot;
* Neuer Parameter für die Verzögerte Mausbewegung
* [Ebenen] Unterstützung für Mehrfachauswahl und -verwaltung
* [Ebenen] Kopieren und Einfügen von einem Textursatz in einen anderen
* [Exportieren] Adobe Photoshop PSD-Format
* [Regal] Neues Tool : Fell, Metallstiche und Reißverschluss
* [Regal] Neuer Pinsel : Schimmel, Bleistift, scharfe Linie und Stich
* [Regal] Neues Alpha : Gaußsches Rauschen, scharfe Linie, Form, Stift, Spritzen, Stich, Reißverschluss
* Verbesserte Malleistung durch Aktualisierung nur eines Teils der benötigten Texturen

**Fest:**

* [Regal] Es ist nicht möglich, einen Stoff mit Graf mit identischen Kennzeichnungen zu laden.
* [Ebenen] Der Mischmodus &quot;Hindurchwirken&quot; funktioniert nicht mit Masken
* [Schablone] Skalierung in 2D-Ansicht unterbrochen
* Probleme und Absturz auf Mac OS Yosemite

### 1.0.2

*(Freigegeben: 9. November 2014)*

**Hinzugefügt:**

* Verbesserte Performance bei der Vorschau von Materialien mit Substanzen
* Verbesserte Leistung mit der Vorschau des Pinselstrichs beim Aktualisieren des Dokuments
* Verbesserte Leistung im Viewport mit niedrigerer Aktualisierungsrate für nicht funktionierenden Bereich
* [Post-Effekte] Verbesserte Benutzeroberfläche zum Verwalten von Einstellungen
* [Post-Effekte] Auf Standardwerte zurücksetzen
* Substance von Effekten und Ebenenoperationen im Kontextmenü
* Unterstützung für die vormultiplizierte Ein-/Ausgabe in Stoffen

**Fest:**

* [3D-Ansicht] Benutzerdefinierte Shader-Parameter werden durch einen großen Leerraum voneinander getrennt.
* [Export] Fehlende sRGB-Konvertierung für Unity4-Voreinstellung
* Möglicher Absturz beim Laden von FBX-Meshs
* Absturz kann beim Laden von einfachen obj-Meshs auftreten
* Die Rechenleiste bleibt beim Laden auf 100 % blockiert.
* Durch das erneute Laden eines Stoffes wird dieser in jede Kategorie verschoben
* DirectX/OpenGL-Switch defekt

### 1.0.1

*(Freigegeben: 27. Oktober 2014)*

**Hinzugefügt:**

* [Tool] Verbesserte Verwendung von Material-Parametern
* Neuer Tastaturbefehl zur UserVoice-Website im Hilfemenü
* Verschiedene Leistungsverbesserungen im Engine

**Fest:**

* Parameterwerte sind für Partikeln auf 2 Dezimalstellen begrenzt
* Aus dem Cache geladene Substance werden in der Benutzeroberfläche nicht als veraltet angezeigt
* Absturz beim Laden eines Meshs von einer Netzwerk-URL
* Painter wird jetzt als signiert unter Mac OS X erkannt.

### 1.0.0

*(Freigegeben: 15. Oktober 2014)*

**Hinzugefügt:**

* Unterstützung benutzerdefinierter Shader
* Unterstützung für 4K-Auflösung
* Beispielzeichenprojekte
* Fortschrittsleiste für lange Berechnungen anzeigen
* [Exportieren] Fügen Sie vor dem Nachbearbeiten der Ausdehnung eine Diffusion hinzu.
* Befehlszeilenargumente in SP für einfache Vorgänge
* Neue Material und Effekte
* Werkzeugvorschau (separate Echtzeitvorschau von Materialien und Bereich für Konturtests)
* Beim Starten von Painter kein Standarddokument erstellen
* [Tool] Fügen Sie die Möglichkeit hinzu, einen Graustufenwert manuell zu bearbeiten
* Verschiedene Verbesserungen für die Schablonen (Einrasten, Reset)
* Partikeln sind jetzt Unterwerkzeuge des Malpinsels, des Radiergummis und der Projektion
* [3D-Ansicht] Baking geführt AO im Viewport-Rendering verwenden
* Teilen der Steuerelemente für Schablonen zwischen der 2D- und 3D-Ansicht
* Kleine Anpassung der Daumengröße in der Bibliothek
* Suchfelder sind für jedes Fenster spezifisch
* Anpassen der Benutzeroberfläche

**Fest:**

* [Substance] Switch funktioniert nicht
* [Farbdialogfeld] Farbtonverlauf wird nicht aktualisiert
* Mesh kann nicht aktualisiert werden, wenn der Dateiname identisch ist
* Werkzeug ist in zu kleinen Ansichten nicht sichtbar
* Das Aufkleber-Werkzeug auf dem Retina-Display funktioniert nicht richtig
* [Substance] Int1 werden als float1 angezeigt
* [Substance] Grundfarbeingabe/Ausgabe wird nicht erkannt
* [Substance] Filter können nicht neu geladen werden.
* [Tool] Graustufen-Widget ist immer ausgeblendet

## Beta

### 0.12.1-beta

*(Freigegeben: 18. September 2014)*

**Hinzugefügt:**

* Unity 5-Exportvorgabe

**Fest:**

* PBR Shader, Rendering-Qualität sollte viel verbessern
* Fokusfunktion ist defekt und Mesh werden standardmäßig beschnitten

### 0.12.0-beta

*(Freigegeben: 17. September 2014)*

**Hinzugefügt:**

* Pipette
* Die Option &quot;Konturposition beibehalten&quot; wurde dem Mesh hinzugefügt, der wieder importiert wird, wenn sich der Begrenzungsrahmen ändert.
* Normalen-Map für Cymourai Standard-Mesh
* Verbessern der Benutzeroberfläche für die Werkzeugansicht (Farben werden abgewischt)
* Verschieben Sie das Menü &quot;Hilfe->Einstellungen&quot; nach &quot;Bearbeiten->Einstellungen&quot;.
* Speichern Sie den Exportpfad im Fenster &quot;Alle Kanäle exportieren&quot;.
* Neue Ebenen-GUI mit Histogrammanzeige
* Besseres Asset-Management (Drag &amp; Drop, Ressourcen neu laden, Nicht verwendete löschen)
* Von &quot;Diffus&quot; zu &quot;Grundfarbe&quot; wechseln
* Schieberegler für die Bearbeitung von Anpassungen - Punkte zusätzlich zu Kommas zulassen
* Füllebene: maximale Kachelung erhöhen
* Standard Umgebungs-Map

**Fest:**

* Schlechte Reflexionsartefakte bei extremen Winkeln
* Specular-/Glanzausfuhr unterbrochen
* Links im Fenster &quot;Info&quot; des Malers funktionieren nicht
* Absturz mit OSX Yosemite
* Mesh werden trianguliert gespeichert
* Der Farb-Tastaturbefehl des Toolfensters wird an die Ausgabeeinrichtung anstelle der Graustufen gesendet.
* Der Farbwähler bleibt geöffnet, wenn Sie von Ebene zu Maske wechseln
* Material aus einer Füllebene kann nicht gespeichert werden
* Größenänderung der drei Bereiche des Regals aktivieren

### 0.11.0-beta

*(Freigegeben: 04. September 2014)*

**Hinzugefügt:**

* Hinzufügen einer Trennlinie zwischen der 3D- und der 2D-Ansicht
* Verwenden eines Verlaufshintergrunds in den 2D-/3D-Ansichten
* Schnittstelle für das Histogramm &quot;Tonwertkorrektur&quot;
* Regal und Bibliothek zusammenführen
* Beim Erstellen oder Aktualisieren einer Vorgabe ist keine Speicheraktion erforderlich
* Importieren von Assets im Regal durch Drag &amp; Drop

**Fest:**

* Der Name der Schaltflächen wird in der Hauptsymbolleiste angezeigt

### 0.10.2-beta

*(Freigegeben: 28. August 2014)*

**Fest:**

* Alle Kanäle exportieren führt zu falschen Ergebnissen

### 0.10.1-beta

*(Freigegeben: 26. August 2014)*

**Fest:**

* Shader ergibt schwarzes Ergebnis bei geringer Rauheit
* GPU-Prüfung: &quot;Quadro&quot;-Karten verarbeiten, alle Geräte erkennen und Benutzernachrichten entsprechend anpassen
* Die meisten Substance-Material sind in Beta 9 auf 256 begrenzt
* Height wird beim Export als Bitmap festgeklemmt
* Die Pinselvorschau unterscheidet sich von der Überlagerung der Projektion in Mac
* Die Verwendung des Geometrie-Werkzeugs zum Erstellen einer Maske wird in Viewporten nicht angezeigt
* Schnelle Maske ist defekt
* Mischproblem auf altem Mac Pro beheben

### 0.10.0-beta

*(Freigegeben: 07. August 2014)*

**Hinzugefügt:**

* Schablonen

**Fest:**

* Unterstützung für Quadro-Karten
* Shader ergibt schwarzes Ergebnis bei geringer Rauheit
* Substance-Materialien sind auf 256 begrenzt
* Normalen-Map-Export löscht den grünen Kanal

### 0.9.0-beta

*(Freigegeben: 17. Juli 2014)*

**Hinzugefügt:**

* Yebis 2 Nachbearbeitung
* Mit dem Assistenten für neue Projekte können Sie Eingabe-Map (AO, Krümmung usw.)
* Eingabe-Map (AO, Krümmung usw.) automatisch anschließen auf Substance Effects
* Skalieren der Steuerung von Materialien, die auf Füllebenen angewendet werden

### 0.8.2-beta

*(Freigegeben: 11. Juli 2014)*

**Fest:**

* Farbton-Schieberegler ist standardmäßig Weiß
* Zurücksetzen des Projekts, wenn der Name des Materials Sonderzeichen enthält
* Die Änderung des Material-Namens für ein einzelnes Material-Objekt sollte das Projekt nicht ungültig machen.
* UVs sind nach dem Speichern des Projekts und dem erneuten Öffnen fehlerhaft

### 0.8.1-beta

*(Freigegeben: 04. Juli 2014)*

**Fest:**

* Mehrere GPU-Absturz
* Absturz beim Exportieren von Kanälen

### 0.8.0-beta

*(Freigegeben: 28. Juni 2014)*

**Hinzugefügt:**

* Mehrere Material - Sie können jetzt auf mehreren Materialien im selben Dokument Malen
* Symmetrie
* Alle Füllmethoden sind jetzt verfügbar

**Fest:**

* Mehrere GPU-Absturz
* Zurücksetzen des Projekts, wenn der Name des Materials Sonderzeichen enthält
* UVs werden nach dem Speichern des Projekts durcheinander gebracht und bei mehreren UVs erneut geöffnet

### 0.7.0-beta

*(Freigegeben: 18. Juni 2014)*

**Hinzugefügt:**

* Ebeneneffekte
* Neue Substance Schablone Material
* Maske bereinigen
* Kopieren/Einfügen von Ebenen/Masken zulassen
* Ebene duplizieren
* Werkzeug beim Bearbeiten der Ebenenmaske ändern
* Substance sind jetzt GPU-fähig

**Fest:**

* Beim Höhen-Map-Malen werden keine negativen Werte Malen.
* Das Material Picker-Display sollte die aufgenommene Normalen-Map nicht berücksichtigen.
* Partikeln Determinismus gebrochen
* Schablone in der 2D-Ansicht
* Ngons in obj-Dateien
* Verschiedene Abstürze

### 0.6.0-beta

*(Freigegeben: 4. Juni 2014)*

**Hinzugefügt:**

* Neue Exportoption zum Exportieren einer Specular-Map aus einer Komposition aus Rauheit und metallic Kanälen

**Fest:**

* Kompatibilität mit Windows Vista
* Höhen-Map Malen keine negativen Werte

### 0.5.0-beta

*(Freigegeben: 7. Mai 2014)*

**Hinzugefügt:**

* 3D-/2D-Ansicht-Schalter
* UV-Blockauswahlwerkzeug
* Beim Malen auf Masken ändert sich das Werkzeug automatisch.
* Die Auflösung der Substance hängt vom

**Fest:**

* Absturz beim Start
* Absturz mit ASCII-Meshs
* Matrix fester Schablonen in 2D-Ansichten
* Absturz mit Radiergummi

### 0.4.0-beta

*(Freigegeben: 17. April 2014)*

**Hinzugefügt:**

* Nahtlose 2D-Ansicht
* Bitmap-Ebenenmasken
* Umgebungsbelichtungssteuerung
* Füllebenen verwenden jetzt die Fenster &quot;Werkzeuge&quot;, um ihre Eigenschaften festzulegen.
* Material können auf Füllebenen angewendet werden
* Weitere Schablonen zur Bibliotheksbibliothek für Schablonen hinzugefügt
* Partikeln-Vorgaben für schnellere Berechnung aktualisiert
* PBR-Shader-Optimierung und Qualitätsverbesserung für niedrigere Qualitätseinstellungen

**Fest:**

* Ebenen-Miniaturansichten sind mit dem aktuell ausgewählten Kanal verknüpft
* Viele Absturz

### 0.3.0-beta

*(Freigegeben: 04. April 2014)*

**Hinzugefügt:**

* Negative Werte im Farbwähler für Höhen-Map-Malen zulassen
* Vorschau des ausgewählten Materials/der ausgewählten Farbe anzeigen
* Hinzufügen von Tastaturbefehlen für die Werkzeuge in der Werkzeugleiste (1,2,3,4)
* Globales Wechseln des Normalformats (OpenGL vs. DirectX) bei einem Projekt
* Assistent für neue Projekte
* Abstand-Schieberegler ist nicht mehr geklemmt
* Aktualisierter Reglerstil
* Farbwähler nicht modal machen
* Wenn Sie ein Material in der Bibliothek auswählen, wird der Werkzeugtyp entsprechend festgelegt

**Fest:**

* Fest: Pfad des importierten Meshs wird nicht beibehalten
* Fest: Generierung von falschen Texturen
* Fest: Absturz beim Starten

### 0.2.0-beta

*(Freigegeben: 17. März 2014)*

**Hinzugefügt:**

* Material-Pipette (P Tastaturbefehl)
* Miniaturen unter der 3D-Werkzeugvorschau
* Lizenzierungssystem für eigenständige Versionen
* [ und ] Tastaturbefehle für Pinselgröße
* Innenabstände exportierter Karten
* Aktualisierter Werkzeugfensterstil
* Aktualisierter Reglerstil
* Aktualisierte HDR.

**Fest:**

* Schablone: Durchflusswert in den 3D-Ansicht-Stopps bei 52 ändern
* Endlose Schleife im Engine, wenn das Hinzufügen von 0-Drucktasten zum Strich festgelegt ist
* Tool: angle Jitter gibt keine Werte über +/- 90 % zurück.
* Anzeigeänderung der 3D-Ansicht, wenn eine Ebenenmaske ausgewählt ist
* Invertierter Zoom

### 0.1.0-beta

*(Freigegeben: 02. März 2014)*

**Hinzugefügt:**

* Neue Bibliotheksverwaltung
* Neue Pinsel und Partikeln
* 3D-Pinselvorschau
* Aktualisierter Werkzeugfensterstil
* Aktualisierter Reglerstil
* Aktualisierte Cache-Leistung

**Fest:**

* Kamera
* Pinseldrehung
