---
breadcrumb-title: ''
description: Prüfe alle Änderungen und Updates in den verschiedenen Substance 3D Painter-Versionen, um den Funktionsverlauf und Verbesserungen im Laufe der Zeit nachzuverfolgen.
title: Alle Änderungen
user-guide-description: ''
user-guide-title: ''
source-git-commit: 479eb327180dd223bbff362e3f200995565cbcfa
workflow-type: tm+mt
source-wordcount: '40713'
ht-degree: 0%
---

# Alle Änderungen

Diese Seite enthält Versionshinweise für alle früheren Versionen von Substance 3D Painter, sortiert nach aktuellster bis ältester Version.

>[!NOTE]
>
> Informationen zum Anzeigen bekannter Probleme, die sich auf Painter auswirken können, finden Sie auf der [Seite zur dedizierten Dokumentation](known-issues.md).

## Version 12

### 12.2.0

Freigabedatum: **2026/10/21**

Zusammenfassung: **Dieses Update ist eine Hauptversion, es fügt eine neue Funktion zum Zeichnen von Käfigen für das Baking hinzu und verbessert die Funktionen zum Füllen von Polygonen. Weitere Informationen finden Sie in den vollständigen Versionshinweisen.**

**Hinzugefügt:**

* Baking, Käfig malen
* &amp;lbrack;Käfig malen&amp;rbrack; Einfache Käfig-Malen-Benutzeroberfläche erstellen
* &amp;lbrack;Käfig malen&amp;rbrack; Neue Optionen zur Visualisierung von Käfig
* &amp;lbrack;Käfig malen&amp;rbrack; Bearbeitbares Auswahl-/Füllwerkzeug
* &amp;lbrack;Käfig malen&amp;rbrack; Überblendung-Modus in Symbolleiste anzeigen
* &amp;lbrack;Käfig malen&amp;rbrack; HDR. Regler Änderungen an der Benutzeroberfläche
* &amp;lbrack;Käfig malen&amp;rbrack; Visualisierungs-Shader
* &amp;lbrack;Käfig malen&amp;rbrack; Optionen zum Zurücksetzen des Stapels
* Verbesserungen am Werkzeug &quot;Polygonfüllung&quot;
* &amp;blbrack;Polygon Fill&amp;rbrack; Polygon-Ausbesserung hinzufügen
* &amp;blbrack;Polygon Fill&amp;rbrack; Polygonschleife hinzufügen
* &amp;blbrack;Polygon Fill&amp;rbrack; Symmetrie-Unterstützung mit Loop/Patch
* &amp;blbrack;Polygon Fill&amp;rbrack; Symmetrie Edge Preview
* &amp;blbrack;Polygon Fill&amp;rbrack; Dreiecke mit Endlosschleifen und Partialschleifen entfernen
* &amp;blbrack;Polygon Fill&amp;rbrack; Drahtgitter nur für aktiven Textursatz sichtbar
* &amp;Klammer;Polygonfüllung&amp;Klammer; Rote Kantenmarkierung bei nicht klickbaren Dreiecken
* &amp;Klammer;Polygonfüllung&amp;Klammer; Deaktivieren Sie nicht die Füllmodusoptionen
* &amp;blbrack;Polygon Fill&amp;rbrack; Festlegen aller Kanaleigenschaften mit der Polygonfüllung zulassen
* &amp;blbrack;Polygon Fill&amp;rbrack; Vorherigen Strich fortsetzen funktioniert mit Polygonfüllung
* &amp;Klammer;Polygonfüllung&amp;Klammer; Unzulässige Cursorposition auf nicht aktiven Textursätzen anzeigen
* &amp;blbrack;Polygon Fill&amp;rbrack; ALT-Sofortvorschau
* &amp;blbrack;Polygon Fill&amp;rbrack; Tastaturbefehl für temporären Wechsel zu Polyloop (UMSCHALT+A)
* &amp;lbrack;Viewport&amp;rbrack; Markierung für Textursatz-/UV-Kacheln-Auswahl anzeigen
* &amp;lbrack;Viewport&amp;rbrack; Unterstützung für &quot;Order Independent Transparency&quot; im Echtzeit-Viewport hinzufügen
* &amp;lbrack;Anzeigeeinstellungen&amp;rbrack; Anzeigeeinstellungen in neuen Gruppen neu organisieren
* &amp;lbrack;Werkzeug&amp;rbrack; Hinzufügen von Unterstützung für das additive Mischen mit Pinselstrichen
* &amp;lbrack;Werkzeug&amp;rbrack; Unterstützung für additive Überblendung mit der Polygonfüllung hinzufügen
* &amp;lbrack;USD&amp;rbrack; Exportierte USD mit Deckkraftmap werden in Arnold transparent dargestellt
* &amp;lbrack;Nvidia&amp;rbrack; Fügen Sie eine Warnung zu den neuesten Nvidia-Treibern hinzu (616.56 bis 617.14)
* Neue Eingabe für &quot;Mesh_UV_Neighbor&quot;-Engine hinzufügen
* Baker auf Version 3.23.0 aktualisieren
* Substance Engine auf Version 9.6.1 aktualisieren

**Fest:**

* &amp;blbrack;Baking&amp;rbrack; Ambient occlusion &quot;Rückseitige ignorierung nach Mesh&quot; funktioniert nicht
* &amp;blbrack;Baking&amp;rbrack; &amp;lbrack;AMD&amp;rbrack; Gerät beim Baking führ mit hochpolaren Meshs verloren
* &amp;lbrack;Performances&amp;rbrack; Painter VRAM Verwendung
* &amp;lbrack;Viewport&amp;rbrack; Fehlende Texturen beim Öffnen von Projekten auf HDPI-Bildschirmen
* &amp;lbrack;Werkzeug&amp;rbrack; Füllmethode ist ausgegraut, wenn in eine Maske gemalt wird
* Temporäre Ordner werden nach dem Export im Netzwerk nicht gelöscht
* &amp;lbrack;USD&amp;rbrack; Die exportierte USD wird entlang der UV-Begrenzungslinien geteilt
* &amp;lbrack;USD&amp;rbrack; Einfrieren beim Laden von falsch geformtem USDz

### 12.1.5

Freigabedatum: **2026/09/15**

Zusammenfassung: **Nebenversion**

**Fest:**

* Das Exportieren eines Bildes aus einem Regal in ein Netzwerk funktioniert nicht mehr
* &amp;lbrack;Generator&amp;rbrack; Die Einstellung &quot;Textur verwenden&quot; auf &quot;false&quot; deaktiviert nicht die Verwendung der Textur-Eingabe.
* Einfrieren des Viewports beim Speichern während der Bearbeitung der 3D-Projektion
* Material-Ebenenauflösung ist zu niedrig

### 12.1.4

Freigabedatum: **2026/09/04**

Zusammenfassung: **Nebenversion**

**Fest:**

* &amp;lbrack;Absturz&amp;rbrack; Absturz beim Importieren oder Exportieren von Dateien, deren Dateinamen Nicht-ASCII-Zeichen enthalten

### 12.1.3

Freigabedatum: **2026/08/26**

Zusammenfassung: **Nebenversion**

**Hinzugefügt:**

* Substance Engine auf Version 9.4.6 aktualisieren

**Fest:**

* &amp;lbrack;Graustufenwähler&amp;rbrack; Picker bleibt nach dem Ändern des Werkzeugs geöffnet
* &amp;Klammer;Baking&amp;Klammer verzerren; Verzerrungskorrektur bricht beim Malen und Rückgängigmachen
* &amp;blbrack;Projektion-Werkzeug&amp;blbrack; Viewport-Interaktion wird vom Projektion-Werkzeug blockiert
* &amp;lbrack;Dynamischer Strich&amp;rbrack; Fehlende dynamische Konturparameter in den Pinseleigenschaften
* Export in ein Netzwerk funktioniert nicht mehr

### 12.1.2

Freigabedatum: **2026/08/03**

Zusammenfassung: **Nebenversion**

**Fest:**

* &amp;lbrack;Absturz&amp;rbrack; Einige Substance können beim Rendern zu einem Absturz führen
* &amp;lbrack;Absturz&amp;rbrack; Mesh beim Baking erneut importieren
* &amp;lbrack;Absturz&amp;rbrack; Wenn die Grafikanzeige nicht initialisiert wird, kann dies zu einem Absturz führen
* &amp;lbrack;Absturz&amp;rbrack; Beim Exportieren von Texturen kann in einigen Fällen ein Absturz beim Aktualisieren des Protokolls auftreten
* &amp;lbrack;Absturz&amp;rbrack; Absturz im Baking-Modus in einigen Fällen beim Laden/Aktualisieren der Umgebungs-Map
* &amp;blbrack;Baking&amp;rbrack; Das erneute Starten von Baking nach dem Ändern einer Datei mit hohem Poly-Wert kann zum Einfrieren führen
* &amp;lbrack;An Photoshop senden&amp;rbrack; Fehler beim Exportieren der Ebenenmaske
* &amp;lbrack;Engine&amp;rbrack; Das Ergebnis des Ankerpunkts wird nicht zwischen einer Maske und einem Farbkanal gerendert

### 12.1.1

Freigabedatum: **2026/07/09**

Zusammenfassung: Nebenversion

Hinzugefügt:

* &amp;Klammer;Baking&amp;Klammer verzerren; Leg des normalen Neigungsbasismodus: Mesh oder pro Dreieck
* &amp;lbrack;Eigenschaften&amp;rbrack; Einheitliche Farben immer auf den Standardwert ihres Kanals zurücksetzen lassen
* &amp;lbrack;OpenPBR&amp;rbrack; Kanäle zur Erstellung von Ausgabevorlagen im Fenster &quot;Texturen exportieren&quot; nach Kategorien neu gruppieren
* Substance Engine auf Version 9.4.5 aktualisieren

Fest:

* &amp;lbrack;Projekt&amp;rbrack; Das Öffnen und Speichern einiger Projekte kann länger als gewöhnlich dauern
* &amp;lbrack;Absturz&amp;rbrack; Das erneute Laden mehrerer Mesh kann zu einem Absturz führen
* &amp;lbrack;Absturz&amp;rbrack; Das Löschen eines Kanals im Maskenansichtsmodus führt zu einem Absturz
* &amp;lbrack;Absturz&amp;rbrack; Einige Substance können beim Rendern zu einem Absturz führen
* &amp;lbrack;Malen Skew&amp;rbrack; Das ausgewählte Werkzeug in Malen Skew bleibt nach dem Wechsel in den Malmodus ausgewählt
* &amp;lbrack;Baking Allgemeine Einstellungen&amp;rbrack; Käfig-Entfernungseinstellungen aktualisieren die Käfig-Drahtgitter- und Shader-Visualisierung nicht
* &amp;lbrack;Engine&amp;rbrack; UV-Auffüllmodus &quot;3D-Raum-Nachbar&quot; funktioniert nicht gut bei dünnen Dreiecken
* &amp;lbrack;Engine&amp;rbrack; Das Ergebnis des Ankerpunkts wird nicht zwischen einer Maske und einem Farbkanal gerendert

### 12.1.0

Freigabedatum: **2026/06/23**

Zusammenfassung: **Dieses Update ist eine Hauptversion. Es enthält Verbesserungen an Bakern mit dem Standardzustand &quot;Neues Baking&quot;, der Zeichnungs-Skew-Map, dem automatischen Reake, einer neuen Option für den automatischen entpack von UV für Mesh und OpenPBR mit fester Oberfläche. Weitere Informationen finden Sie in den vollständigen Versionshinweisen.**

**Hinzugefügt**:

* &amp;Klammer;Baking&amp;Klammer verzerren; Malwerkzeuge verzerren
* &amp;Klammer;Baking&amp;Klammer verzerren; Skew-Vorschau hinzufügen Shader und Skew-Richtung Vektorgrafiken beim Malen einer Skew-Map
* &amp;Klammer;Baking&amp;Klammer verzerren; Option &quot;Kantenschutz hinzufügen&quot;
* &amp;Klammer;Baking&amp;Klammer verzerren; Auto-Reake
* &amp;Klammer;Baking&amp;Klammer verzerren; Benutzeroberfläche der Mesh-Map-Liste überarbeiten
* &amp;Klammer;Baking&amp;Klammer verzerren; Mesh-Map teilen/Allgemeine Baking-Einstellungen + Allgemeine Einstellungen aus Mesh-Map-Liste verschieben (nur Grundfarbe oder Maske)
* &amp;Klammer;Baking&amp;Klammer verzerren; Symbolleistenschaltflächen für Viewport ändern
* &amp;Klammer;Baking&amp;Klammer verzerren; Symmetrie-Schalter für Pinsel in der oberen Symbolleiste anzeigen
* &amp;Klammer;Baking&amp;Klammer verzerren; Umbenennungsoptionen im Menü &quot;Synchronisierung der Mesh-Map-Liste&quot;
* &amp;Klammer;Baking&amp;Klammer verzerren; Dialogfelder &quot;Synchronisation aktualisieren&quot; und &quot;Überwachter Status&quot;
* &amp;Klammer;Baking&amp;Klammer verzerren; Variante des Graustufen-Farbwählers erstellen
* &amp;Klammer;Baking&amp;Klammer verzerren; Symbol &quot;Baking aktualisieren&quot;
* &amp;lbrack;Automatisch Entpackt&amp;rbrack; Option &quot;Festplatte integrieren&quot;
* &amp;lbrack;OpenPBR&amp;rbrack; Unterstützung für OpenPBR 1.1 hinzufügen
* &amp;lbrack;OpenPBR&amp;rbrack; OpenPBR zum Standard-Arbeitsablauf und -Shader machen
* &amp;lbrack;OpenPBR&amp;rbrack; Importieren von OpenPBR Materials und Texturen über USD
* &amp;lbrack;OpenPBR&amp;rbrack; Exportieren von OpenPBR und Texturen über USD
* &amp;lbrack;OpenPBR&amp;rbrack; Fenster &quot;Texturen exportieren&quot; aktualisieren, um die Namenskonvention für OpenPBR anzuzeigen
* &amp;lbrack;OpenPBR&amp;rbrack; Fügen Sie Dokumentationen zu Änderungen an der Support-OpenPBR hinzu
* &amp;lbrack;OpenPBR&amp;rbrack;&amp;lbrack;Iray&amp;rbrack; Neue MDL zur Unterstützung von OpenPBR 1.1 in Iray hinzufügen
* Mehrere geringfügige Verbesserungen bei USD Exporten
* &amp;lbrack;UI&amp;rbrack; Warnmeldung im Viewport beim Malen auf einem anderen Textursatz hinzufügen
* &amp;lbrack;Reduzieren&amp;rbrack; Reduzieren aller instanzierten Ebenen über Textursatz hinweg zulassen
* &amp;Textursatz&amp;rbrack;Einstellungen&amp;rbrack; Auswahl mehrerer Kanäle gleichzeitig über neues Fenster zulassen
* &amp;lbrack;Verlauf&amp;rbrack; &quot;Wert&quot; aktualisieren Eintragstext rückgängig machen, um den Parameternamen anzugeben
* &amp;lbrack;Ebenenstapel&amp;rbrack; Fülleffekte in Masken auf Weiß (1.0) festlegen
* &amp;lbrack;Substance&amp;rbrack; Neue Eingabe für &quot;Mesh_harte_Kanten_Dreieck&quot;-Engine hinzufügen
* &amp;lbrack;Substance&amp;rbrack; Neue Eingabe für Engine &quot;Mesh_hard_edges&quot; hinzufügen
* &amp;lbrack;Shader&amp;rbrack; Shader-Instanzen zum Freigeben derselben Namen verhindern
* &amp;lbrack;Shader&amp;rbrack; Verwenden des Shaders aus der Projektvorlage beim Importieren einer USD- oder GLTF-Datei
* Adobe Color Engine auf Version 7.0 aktualisieren
* Aktualisieren der MacOSX-Mindestversion auf 13.0 (Ventura)
* &amp;lbrack;Inhalt&amp;rbrack; Neue Projektvorlagen für OpenPBR
* &amp;lbrack;Inhalt&amp;rbrack; Aktualisieren von Beispielprojekten, um den neuen OpenPBR-Shader zu verwenden
* &amp;lbrack;Python&amp;rbrack; Erweitern Sie die Geometrie-Masken-API, um Einschluss- und Ausschlussmodi wie in der Benutzeroberfläche zuzulassen.

**Fest**:

* &amp;lbrack;Absturz&amp;rbrack;&amp;lbrack;Mesh-Map-Einstellungen&amp;rbrack; Einstellungen auf andere Textursatz anwenden
* &amp;lbrack;Absturz&amp;rbrack; Beim Baking von Krümmungen von einer Karte ohne Welt-Raum-Normale
* &amp;lbrack;Absturz&amp;rbrack;&amp;lbrack;Baking&amp;rbrack; Baking mit aktiviertem benutzerdefiniertem Käfig, aber ohne Dateiauswahl-Absturz
* &amp;lbrack;Absturz&amp;rbrack; AO-Baking wird abgebrochen
* &amp;lbrack;Käfig&amp;rbrack; Unendliche Ladung, wenn der hohe Polydateipfad ungültig ist
* &amp;lbrack;Linux&amp;rbrack;&amp;lbrack;Windows&amp;rbrack; Der Farbwähler kann ganz schwarz sein oder nicht angezeigt werden.
* &amp;blbrack;Polygon-Füllwerkzeug&amp;rbrack; Das Tool funktioniert nicht mit Nicht-PBR
* &amp;lbrack;&amp;lbrack;Malen&amp;rbrack; Durch Löschen des Farbkanals werden zuvor gemalte Grundfarben nicht gelöscht.
* &amp;lbrack;USD&amp;rbrack; Shader-Instanzen werden nicht alle korrekt erkannt
* &amp;lbrack;Substance&amp;rbrack; Es wird nur die erste Verwendung eines Eingabe-/Ausgabeknotens berücksichtigt
* &amp;lbrack;Shader&amp;rbrack; Ambient occlusion wird zweimal mit Textursätzen unter Verwendung unterschiedlicher Mischmethoden aufgetragen
* &amp;lbrack;Engine&amp;rbrack; Normale Texturen mit leerem Blaukanal (Schwarz) können zu falschen Füllergebnissen führen.
* &amp;lbrack;GLTF Import&amp;rbrack; Alpha-Überblendung ist auf jedem Textursatz aktiviert
* &amp;lbrack;GLTF Export&amp;rbrack; Alpha-Überblendung ist beim Export immer aktiviert
* &amp;lbrack;Export&amp;rbrack; Doppelseitige Geometrie ist beim Importieren einer GLTF-Datei immer deaktiviert
* &amp;lbrack;Javascript&amp;rbrack; Das Ändern der Shader-Einstellungen trägt nicht zum Rückgängig-Verlauf bei
* &amp;lbrack;Samples&amp;rbrack; Volumenstreuung ist in den Anzeigeeinstellungen für Meet Mat nicht aktiviert

### 12.0.3

Freigabedatum: **2026/05/05**

Zusammenfassung: **Nebenversion**

**Hinzugefügt:**

* Baker auf Version 3.22.2 aktualisieren
* Substance Engine auf Version 9.4.3 aktualisieren
* &amp;lbrack;Python&amp;rbrack; Speichern eines intelligenten Materials an einem bestimmten Speicherort

**Fest:**

* &amp;lbrack;Ubuntu&amp;rbrack; Absturz bei der Auswahl von Material
* &amp;lbrack;Mac&amp;rbrack; Es wird ein Popup angezeigt, in dem Sie um Zugriff auf Daten anderer Anwendungen gebeten werden.
* &amp;blbrack;Baking&amp;rbrack; Artefakte können auf dem Krümmungs-Map erscheinen
* &amp;blbrack;Baking&amp;rbrack; Das Baking ist in manchen Fällen langsamer
* &amp;lbrack;Verkrümmen auf Geometrie&amp;rbrack; In einigen Fällen wird &quot;Auf Geometrie verformen&quot; deaktiviert
* &amp;lbrack;UV-Kachel&amp;rbrack; Der extrahierte Alpha-Wert des Ankerpunkts wird von anderen Kacheln ignoriert
* &amp;lbrack;Python&amp;rbrack;&amp;lbrack;Mac&amp;rbrack; Ausnahmen in der Python-Konsole mit SSL
* &amp;lbrack;Python&amp;rbrack; Painter Absturz beim Beenden mit verbleibenden Qt-Widgets

### 12.0.2

Freigabedatum: **2026/04/07**

Zusammenfassung: **Nebenversion**

**Hinzugefügt:**

* &amp;lbrack;Farbmanagement&amp;rbrack; Fügen Sie neue OCIO hinzu, um den Standardfarbraum des Farbwählers anzugeben
* &amp;lbrack;Python&amp;rbrack; Leg der Einstellungen für den automatischen entpack in der Python-API

**Fest:**

* &amp;lbrack;Absturz&amp;rbrack; Das Speichern bei zu wenig Speicherplatz kann zu einem Absturz oder einer Beschädigung der Projekte führen.
* &amp;lbrack;Absturz&amp;rbrack; &amp;lbrack;Menüband&amp;rbrack; Die Verwendung des Menübands kann bei einigen Projekten zu Abstürzen führen
* &amp;lbrack;Absturz&amp;rbrack; &amp;blbrack;Baking&amp;rbrack; Absturz, wenn die .assbin-Datei nicht in den Ordner geschrieben werden kann
* &amp;lbrack;Import&amp;rbrack; OBJ Meshs aus Stager können bei der Projekterstellung fehlschlagen
* &amp;lbrack;Import&amp;rbrack; OBJ fehlt in einigen Fällen die Fläche
* &amp;lbrack;Import&amp;rbrack; USD Mesh ohne zugewiesenes Material kann beim Importieren Absturz hinzufügen.
* &amp;lbrack;Ausgefüllter Pfad&amp;rbrack; Nicht von der Symmetrie betroffen
* &amp;lbrack;Schablone&amp;rbrack; Die Vorschau hat eine geringere Auflösung als das gemalte Ergebnis
* &amp;lbrack;UI&amp;rbrack; &quot;uv island&quot; wird in der QuickInfo für ID-Map-Farbquellen noch erwähnt
* &amp;lbrack;Anzeige&amp;rbrack; Schatten erscheinen invertiert
* &amp;lbrack;Viewport&amp;rbrack; Transformieren Projektion der Verkrümmung bleibt nach dem Wechsel in den Baking-Modus erhalten
* &amp;lbrack;Verkrümmen&amp;rbrack; Raster verschwindet, wenn die Skalierung auf der Z-Achse auf 0 eingestellt ist und &quot;Auf Geometrie verformen&quot; aktiviert ist
* &amp;lbrack;Python&amp;rbrack; Unerwarteter Fehler beim Hinzufügen eines Kanals mit bereichsbezogener Änderung

### 12.0.1

Freigabedatum: **2026/03/18**

Zusammenfassung: **Nebenversion**

**Fest:**

* &amp;lbrack;Absturz&amp;rbrack;&amp;lbrack;Freeze&amp;rbrack; Exportieren aus bestimmten Projekten

### 12.0.0

Freigabedatum: **2026/03/09** Zusammenfassung: **Dies ist eine Hauptversion. Diese Version enthält die Funktionen zum Reduzieren von Ebenen, Verformen der Geometrie, neue Post-Effekte, Verbesserung des neuen Projektfensters und weitere Verbesserungen.**

**Hinzugefügt**:

* &amp;lbrack;Ebenen reduzieren&amp;rbrack; Ebenen innerhalb des Ebenenstapels reduzieren
* &amp;lbrack;Ebenen reduzieren&amp;rbrack; Exportieren reduzierter Ebenen auf die Festplatte
* &amp;lbrack;Verkrümmen auf Geometrie&amp;rbrack; Neue Funktion für die automatische Verkrümmung in Verkrümmen-Projektionen hinzufügen
* &amp;lbrack;Post-effects&amp;rbrack; Post-Effekte durch neue ersetzen
* &amp;lbrack;Post-effects&amp;rbrack; Tonzuordnung aktualisieren
* &amp;lbrack;Post-effects&amp;rbrack; Neue Verwendung für Post-Effects-Elemente hinzufügen
* &amp;lbrack;Content&amp;rbrack;&amp;lbrack;Post-effects&amp;rbrack; Standard-Post-Effects-Elemente in die Bibliothek integrieren
* &amp;lbrack;Neues Projekt&amp;rbrack; Verbessern der Benutzeroberfläche für die Projekterstellung
* &amp;lbrack;Neues Projekt&amp;rbrack; Änderungen an der Funktion zum erneuten Importieren von Mesh
* &amp;lbrack;Neues Projekt&amp;rbrack; Öffnen von \*.geo.usd-Dateien zulassen
* &amp;lbrack;Projektkonfiguration&amp;rbrack; Verbessern der Benutzeroberfläche für die Projektkonfiguration
* USD auf Version 25.05 aktualisieren
* Substance Engine auf Version 9.3.4 aktualisieren
* Erhöhen der Mindesttreiber auf 25.3.1/25.Q2 für AMD-GPUs
* Update Qt auf 6.8.6
* &amp;lbrack;Skripterstellung&amp;rbrack; JavaScript-API auf Version 1.1.20 aktualisieren
* Aktualisieren von Python auf 3.13

**Fest:**

* &amp;lbrack;Absturz&amp;rbrack; Ändern der Ausgabe eines Material-Kanals in einer Maske kann Absturz verursachen
* &amp;lbrack;Import&amp;rbrack; EXR Texturen werden beim Importieren von USD in sRGB anstelle von linear erzwungen
* &amp;blbrack;UV-Kacheln&amp;rbrack; Bildsequenz mit einem einzigen Bild füllt auch andere UV-Kacheln
* &amp;blbrack;Baking&amp;rbrack; AO unterscheidet sich zwischen CPU- und GPU-Baking
* &amp;lbrack;Farbmanagement&amp;rbrack;&amp;lbrack;MacOS&amp;rbrack; Viewport &quot;BaseColor&quot; stimmt nicht mit dem Farbwähler überein
* &amp;lbrack;USD&amp;rbrack; Einheitliche Werte werden in einigen Fällen nicht importiert

## Version 11

### 11.1.3

Freigabedatum: **2026/02/12** Zusammenfassung: **Nebenversion**

**Fest**:

* &amp;lbrack;Malen&amp;rbrack; Schablone und Symmetrie funktionieren in einigen Fällen nicht
* &amp;lbrack;Pfad&amp;rbrack; Keine Aktualisierung beim Ändern des Deckkraftreglers für den Verwischungsstrich
* &amp;lbrack;Projekt&amp;rbrack; Malen auf einer bestimmten Geometrie nicht möglich
* &amp;lbrack;Menüband&amp;rbrack; Der instanziieren Pfad verschwindet, wenn die Auflösung des Textursatzes geändert wird
* &amp;lbrack;UI&amp;rbrack; Der Farbwähler kann sich verkleinern und in einigen Fällen verschwinden

### 11.1.2

Freigabedatum: **2026/01/13** Zusammenfassung: **Nebenversion**

**Hinzugefügt**:

* &amp;blbrack;Baking&amp;rbrack; Verbessern des Bakings von UV-Kacheln-Projekten durch asynchrones Speichern
* &amp;lbrack;Shaders&amp;rbrack; Erwähnung in Shader-API Changelog Veränderungen nach Vulkan Migration
* Update OpenEXR auf Version 3.4.4

**Fest**:

* &amp;lbrack;Absturz&amp;rbrack; Absturz beim Starten von Nvidia GTX 10xx
* &amp;lbrack;Absturz&amp;rbrack; Die Verwendung des Farbwählers auf verschiedenen Textursätzen kann beim Beenden der Anwendung zu einem Absturz führen
* &amp;lbrack;Performance&amp;rbrack; Leistungsproblem beim Malen im Projekt mit vielen Ebenen
* &amp;lbrack;Performance&amp;rbrack; Verzögerung beim Malen mit Grafiktablett-Stift
* &amp;lbrack;UI&amp;rbrack; Kamera-Einstellungen bleiben im Rendermodus deaktiviert (Iray)
* &amp;lbrack;Menüband&amp;rbrack; Pfad kann sich in einigen Fällen nach einer Ecke unerwartet überlappen
* &amp;lbrack;Menüband&amp;rbrack; Leistungsproblem mit UV-Kacheln
* &amp;lbrack;Substance&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Bildeingaben verschwinden, wenn sie ausgeblendet werden
* &amp;lbrack;Substance&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Verschachtelte Gruppen können auch dann beibehalten werden, wenn sie unter Sichtbar, wenn sie ausgeblendet sind.
* &amp;lbrack;Baking&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Der Krümmung-Sampling-Radius kann nicht über 0,01 hinaus festgelegt werden
* &amp;lbrack;Baking&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Max. Verdeckungsabstand kann nicht auf mehr als 1 eingestellt werden
* &amp;blbrack;Baking&amp;rbrack; AO-Einstellung &quot;Selbstverdeckung&quot; wird bei mehreren Textursätzen ignoriert und &quot;Niedrig&quot; steht für &quot;Hoch&quot; Baking geführt
* &amp;blbrack;Baking&amp;rbrack; ID-Map Baking führe keine Textfarben aus FBX im Scheitelpunkt &quot;Niedrig bis Hoch&quot;
* &amp;lbrack;Inhalt&amp;rbrack; Hochpassfilter führt zu ausgewaschenen Farben in farbverwalteten Kanälen

### 11.1.1

Freigabedatum: **2025/12/09** Zusammenfassung: **Nebenversion**

**Hinzugefügt**:

* &amp;lbrack;Performance&amp;rbrack; Verbessern der UV-Kacheln-Performance bei der Berechnung partieller Texturen
* &amp;lbrack;Baker&amp;rbrack; Update auf Version 3.15.4

**Fest**:

* &amp;lbrack;Absturz&amp;rbrack;&amp;lbrack;MacOS&amp;rbrack; Speichern eines Projekts aus einer früheren Version immer mit dem Absturz
* &amp;lbrack;Absturz&amp;rbrack; Das Schließen eines Projekts kann zu einem Absturz führen
* &amp;lbrack;Projekt&amp;rbrack; Fehler &quot;Die Mitgliederanzahl stimmt nicht überein&quot; beim Öffnen des Projekts, das in der vorherigen Version erstellt wurde
* &amp;blbrack;Baking&amp;rbrack; UV-Kacheln werden nicht mit vorherigen Baking-Ergebnissen kombiniert, sofern vorhanden.
* &amp;blbrack;Baking&amp;rbrack; Gerät verloren, selbst wenn Raytracing in der Nvidia GTX 10XX-Serie deaktiviert ist
* &amp;blbrack;Baking&amp;rbrack; AO mit Normal weist an Kanten Artefakte auf, da keine Auffüllung erfolgt.
* &amp;blbrack;Baking&amp;rbrack; AO-Einstellung &quot;Selbstverdeckung&quot; wird bei mehreren Textursätzen ignoriert und &quot;Namensübereinstimmung&quot; aktiviert.
* &amp;blbrack;Baking&amp;rbrack; ID-Map ist vollständig schwarz, wenn Scheitelpunkt-Farben bei Meshs mit hohem Poly fehlen
* &amp;lbrack;Menüband&amp;rbrack; QuickInfo für den Modus &quot;Alpha-Überblendung&quot; nennt den Bildschirmüberblendmodus anstelle von &quot;Linear abwedeln&quot;
* &amp;lbrack;Pfad&amp;rbrack; Tangenten erstellen eine unerwartete Schleife, wenn der Punkt dicht an das Pfadende verschoben wird
* &amp;lbrack;Werkzeug&amp;rbrack; Die Maskenvorschau funktioniert nicht, wenn die Projektion in einer Material verwendet wird
* &amp;lbrack;Engine&amp;rbrack; Das Malen kleiner Striche kann zu blockartigen Artefakten führen
* &amp;lbrack;Shader&amp;rbrack; Durch Rückgängigmachen der Erstellung von Shader-Instanzen wird sie nicht ordnungsgemäß entfernt.
* &amp;lbrack;Export&amp;rbrack; Alpha-Modus für GLTF-Export ist immer auf MASK festgelegt
* &amp;lbrack;Python&amp;rbrack; Unerwarteter Fehler beim Bearbeiten von Ebenenstapel außerhalb des umfangreichen Änderungsblocks

**Bekannte Probleme**:

* &amp;lbrack;Menüband&amp;rbrack; Leistungsproblem mit UV-Kacheln
* &amp;lbrack;Menüband&amp;rbrack; Pfad kann sich in einigen Fällen nach einer Ecke unerwartet überlappen
* &amp;lbrack;Absturz&amp;rbrack;&amp;lbrack;Ribbon&amp;rbrack; Erstellen von sehr langen Texten im Menüband kann Absturz
* &amp;lbrack;Farbmanagement&amp;rbrack; HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen geklemmte Farben
* &amp;lbrack;Regression&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Kontextmenü ist auf HD-Bildschirmen zu klein
* &amp;lbrack;Absturz&amp;rbrack;&amp;lbrack;Python&amp;rbrack; USD Export ausgelöst durch TextureStateEvent
* &amp;lbrack;Engine&amp;rbrack; Malen mit dem Klon-Werkzeug in normalen Kanalverschiebungsfarben falsch
* &amp;lbrack;Python&amp;rbrack; Phantom-Widget wird angezeigt, weil das Skript noch funktioniert

### 11.1.0

Veröffentlichungsdatum: **2025/11/18** Zusammenfassung: **Dieses Update ist eine Hauptversion, es enthält das neue Multifunktionsleisten-Tool mit eigenem neuen Inhalt, Unterstützung von Füllebenen, Leistungsparameter für Versatz, verbesserte Physische Größe durch die aktualisierten Baker, vollständige Vulkan-Unterstützung für Windows und Linux und weitere Symmetrien.**

**Hinzugefügt**:

* Neues Bandwerkzeug
* &amp;lbrack;Werkzeug&amp;rbrack; Neues Werkzeug &quot;Menüband&quot; für nahtlose Pfade hinzufügen
* &amp;lbrack;Menüband&amp;rbrack; Tastenkombinationen für die Bandvorgabe im Eigenschaftenfenster hinzufügen
* &amp;lbrack;Menüband&amp;rbrack; Zulassen, dass die Deckkraft des Menübands pro Scheitelpunkt auf dem Pfad geändert wird
* &amp;lbrack;Menüband&amp;rbrack; Ändern der Größe des Menübands pro Scheitelpunkt auf dem Pfad zulassen
* &amp;lbrack;Menüband&amp;rbrack; In einer Substance definierte Anfang-/Endpunkte entfernen, wenn Pfade geschlossen sind
* &amp;lbrack;Menüband&amp;rbrack; Entfernen der Pfad-/Material-Vorschau im Eigenschaftenfenster für Malen-/Radiergummi-/Verwisch-Pfadwerkzeuge
* &amp;lbrack;Menüband&amp;rbrack; Fülloptionen für Alpha und einige Kanäle bei Selbstüberlappung hinzufügen
* Symmetrie füllen
* &amp;lbrack;Füllen&amp;rbrack; Unterstützung für Symmetrie zu Füllebenen und Effekten hinzufügen
* &amp;lbrack;Fill&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Einstellungen für die Symmetrie von Füllebene und Effekten im Eigenschaftenfenster gelegt
* &amp;lbrack;Füllen&amp;rbrack; Benutzeroberfläche für Symmetrie-Einstellungen im Viewport- und Eigenschaftenfenster überarbeiten
* &amp;lbrack;Füllen&amp;rbrack; Normale Texturen bei Projektion im Verkrümmungsmodus korrekt neu ausrichten
* Physische Größe Versatz
* &amp;lbrack;Versatz&amp;rbrack; Physische Größe als Versatz verwenden
* Leistungssteigerung
* &amp;lbrack;Performance&amp;rbrack; Verbessern der Darstellung kleiner Pinselstriche auf großen Dreiecken
* &amp;lbrack;Performance&amp;rbrack; Verbessern der Shader-Kompilierungszeit
* &amp;lbrack;Performance&amp;rbrack; Vollständige Vulkan-Unterstützung für Windows und Linux
* &amp;lbrack;Performance&amp;rbrack; Aktualisierte Baker mit schnellerem GPU-Rendering und Unterstützung von AMD-Raytracing
* &amp;lbrack;UI&amp;rbrack; Werkzeugeigenschaften neu in Gruppen organisieren und einige standardmäßig reduzieren
* &amp;lbrack;Engine&amp;rbrack; Substance Engine auf Version 9.2.5 aktualisieren
* &amp;lbrack;Substance&amp;rbrack; Irreguläre Auflösung für Substance-Ressourcen in &quot;Extras und Füllungen&quot; gelegt
* &amp;lbrack;Export&amp;rbrack; Exportvoreinstellung für Mesh-Map aktualisieren, um Graustufen-Texturen zu exportieren
* Python
* &amp;lbrack;Baking&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Anzeige der Änderungen im Änderungsprotokoll nach Aktualisierung der Baker
* &amp;lbrack;Python&amp;rbrack; Leg der Einstellungen für die Symmetrie der Füllung in Python
* Content und neue Inhalte.
* &amp;lbrack;Inhalt&amp;rbrack; 75 neue Werkzeugvorgaben für das Menüband-Werkzeug hinzufügen
* &amp;lbrack;Inhalt&amp;rbrack; Verlaufsgenerator-Ressource so aktualisieren, dass sie mit dem Menüband kompatibel ist

**Fest**:

* &amp;lbrack;Absturz&amp;rbrack; Laden eines anderen Projekts bei aktiviertem einrasten des Pfads kann Absturz
* &amp;lbrack;Absturz&amp;rbrack; Rechtsklick im Bedienfeld &quot;Pfad&quot; mit Informationen aus einer anderen Session in der Zwischenablage kann Absturz enthalten
* &amp;lbrack;UI&amp;rbrack; Oberfläche scrollt in den Werkzeugeigenschaften nach oben, wenn ein Pfad erstellt wird
* &amp;lbrack;UI&amp;rbrack; Mauszeiger verschwindet, wenn die Pfadzeigerdarstellung ausgeblendet ist
* &amp;lbrack;Pfad&amp;rbrack; Kopieren/Einfügen verschiedener Werkzeugeigenschaften im Bedienfeld &quot;Pfad&quot; führt zu instabilen Eigenschaften
* &amp;lbrack;Werkzeug&amp;rbrack; Radiergummi- und Verwischen-Werkzeugvorgaben aktualisieren nicht immer die Kanalauswahl
* &amp;lbrack;Werkzeug&amp;rbrack; Gemalter Wert ist grau, aber Benutzeroberfläche zeigt Weiß an, nachdem farbige Werkzeugvorgabe in die Maske geladen wurde
* &amp;lbrack;Werkzeug&amp;rbrack; Die aus der Maske erstellte Vorgabe behält Kanalwerte bei, die aus einer anderen Vorgabe geladen wurden.
* &amp;lbrack;Substance&amp;rbrack; Die in Graf definierte normale Farbraumübersteuerung wird nicht berücksichtigt
* &amp;lbrack;Inhalt&amp;rbrack; Die Standard-Pinselform-Ressource verwendet eine veraltete Substance

**Bekannte Probleme**:

* Shader-Instanz-Verlauf wird nicht richtig verfolgt
* &amp;lbrack;Menüband&amp;rbrack; Leistungsproblem mit UV-Kacheln
* &amp;lbrack;Menüband&amp;rbrack; Pfad kann sich in einigen Fällen nach einer Ecke unerwartet überlappen
* &amp;lbrack;Menüband&amp;rbrack; Tangenten erzeugen eine unerwünschte Schleife, wenn der Punkt nahe an das Pfadende verschoben wird
* &amp;lbrack;Absturz&amp;rbrack;&amp;lbrack;Ribbon&amp;rbrack; Erstellen von sehr langen Texten im Menüband kann Absturz
* &amp;lbrack;Werkzeug&amp;rbrack; Die Maskenvorschau funktioniert nicht, wenn die Projektion in einer Material verwendet wird
* &amp;blbrack;Baking&amp;rbrack; AO-Einstellung &quot;Selbstverdeckung&quot; wird bei mehreren Textursätzen ignoriert und &quot;Namensübereinstimmung&quot; ist aktiviert
* &amp;blbrack;Baking&amp;rbrack; AO mit Normal weist an den Kanten Artefakte auf, da die Auffüllung fehlt.
* &amp;lbrack;Farbmanagement&amp;rbrack; HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen geklemmte Farben
* &amp;lbrack;Regression&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Kontextmenü ist auf HD-Bildschirmen zu klein
* &amp;lbrack;Absturz&amp;rbrack;&amp;lbrack;Python&amp;rbrack; USD Export ausgelöst durch TextureStateEvent
* &amp;lbrack;Engine&amp;rbrack; Malen mit dem Klon-Werkzeug in normalen Kanalverschiebungsfarben falsch
* &amp;lbrack;Python&amp;rbrack; Phantom-Widget wird angezeigt, weil das Skript noch funktioniert

### 11.0.3

Freigabedatum: **2025/08/05** Zusammenfassung: **Nebenversion**

**Hinzugefügt**:

* &amp;lbrack;Substance 3D Assets&amp;rbrack; Hinzufügen eines Benachrichtigungspunkts zum Bedienfeld &quot;3D-Elemente&quot;
* &amp;lbrack;VFX Platform 2025&amp;rbrack; Hinzufügen der ACE 2.0-Konfiguration in den Farbmanagementeinstellungen
* &amp;lbrack;VFX Platform 2025&amp;rbrack; Aktualisieren Sie OCIO auf Version 2.4.2
* Iray auf Version 2024.10 aktualisieren
* &amp;lbrack;Engine&amp;rbrack; Update auf Substance Engine v.9.2.3
* &amp;lbrack;Nvidia&amp;rbrack; Erhöhen der Nvidia-Mindesttreiberversion auf 572.60 (Win) und 570.169 (Linux)

**Fest**:

* &amp;lbrack;Python&amp;rbrack; Die Änderung des Gültigkeitsbereichs wird nicht im Verlaufsfenster angezeigt

**Bekannte Probleme**:

* &amp;lbrack;Farbmanagement&amp;rbrack; HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen geklemmte Farben
* &amp;lbrack;Regression&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Kontextmenü ist auf HD-Bildschirmen zu klein
* &amp;lbrack;Absturz&amp;rbrack;&amp;lbrack;Python&amp;rbrack; USD Export ausgelöst durch TextureStateEvent
* &amp;lbrack;Engine&amp;rbrack; Malen mit dem Klon-Werkzeug in normalen Kanalverschiebungsfarben falsch
* &amp;lbrack;Python&amp;rbrack; Phantom-Widget wird angezeigt, weil das Skript noch funktioniert

### 11.0.2

Freigabedatum: **2025/06/10** Zusammenfassung: **Nebenversion**

**Hinzugefügt**:

* &amp;lbrack;Mac&amp;rbrack; Warnmeldungen zu bestimmten Betriebssystemversionen hinzufügen, die zu Artefakten führen
* &amp;lbrack;Automatische Aktualisierung&amp;rbrack; Kleine UX-Verbesserungen im Fehlerprotokoll &quot;Assets&quot;
* &amp;lbrack;Automatisches Entpacken&amp;rbrack; Update auf Version 1.3.2 mit Seaming-Verbesserungen
* &amp;lbrack;USD&amp;rbrack;&amp;lbrack;FBX&amp;rbrack; Unterstützung für mehrere UV-Satz mit wenigen Daten hinzufügen
* &amp;lbrack;Export&amp;rbrack; Meshs, die als FBX exportiert wurden, fehlen ihre zusätzlichen UV-Satz, wenn beim Import vorhanden waren

**Fest**:

* &amp;lbrack;MacOS&amp;rbrack;&amp;lbrack;Linux&amp;rbrack; Absturz beim Speichern auf dem Netzlaufwerk
* &amp;lbrack;Win&amp;rbrack;&amp;lbrack;Tablet&amp;rbrack; Flackern beim Schwenken
* &amp;lbrack;SpaceMouse&amp;rbrack; Problem beim Arbeiten mit dem Pfadwerkzeug
* &amp;lbrack;Käfig&amp;rbrack; Nach einem erneuten Laden des Meshs kann kein Baking ausgeführt werden
* &amp;lbrack;Automatische Aktualisierung&amp;rbrack; Bildsequenz wird nicht neu geladen, wenn die erste Kachel fehlt
* &amp;lbrack;Pfad&amp;rbrack; Benutzerdefinierte Tangente kann sich auf andere Tangenten auswirken
* &amp;lbrack;Pfad&amp;rbrack; Pfad wird auf dem Textursatz nicht angezeigt, wenn sich der erste Punkt auf einem anderen Textursatz befindet
* &amp;lbrack;UI&amp;rbrack; Einige Menüs sind nach dem Öffnen eines Projekts immer deaktiviert (z. B.: Symmetrie)
* &amp;lbrack;Eigenschaften&amp;rbrack; Werkzeugvorgaben mit ausgefülltem Pfadwerkzeug können nicht verwendet/geladen werden
* &amp;lbrack;USD&amp;rbrack; Mehrere UV-Satz werden bei Verwendung von USD nicht im benutzerdefinierten Shader erkannt.
* &amp;lbrack;USD&amp;rbrack; Kameras mit dem gleichen Namen werden überschrieben
* &amp;lbrack;Export&amp;rbrack; &quot;An Photoshop senden&quot; führt zu einem falschen Farbraum für Farb- und Graustufenergebnisse
* &amp;lbrack;Export&amp;rbrack; Graustufen-Kanäle mit Alpha werden als Farbe anstatt als Graustufen mit PNG-Format exportiert
* &amp;lbrack;Export&amp;rbrack; Exportieren des Graustufenkanals als PSD führt zu einer ungültigen/abgeschnittenen Datei
* &amp;lbrack;Inhalt&amp;rbrack; Der Verkrümmungsfilter im Mehrrichtungsmodus funktioniert nicht
* &amp;lbrack;Python&amp;rbrack; Listenfehler beim Crawlen von Ebenenstapel-Knoten kann nicht zugewiesen werden

**Bekannte Probleme**:

* &amp;lbrack;Farbmanagement&amp;rbrack; HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen geklemmte Farben
* &amp;lbrack;Regression&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Kontextmenü ist auf HD-Bildschirmen zu klein
* &amp;lbrack;Absturz&amp;rbrack;&amp;lbrack;Python&amp;rbrack; USD Export ausgelöst durch TextureStateEvent
* &amp;lbrack;Engine&amp;rbrack; Malen mit dem Klon-Werkzeug in normalen Kanalverschiebungsfarben falsch
* &amp;lbrack;Python&amp;rbrack; Phantom-Widget wird angezeigt, weil das Skript noch funktioniert

### 11.0.1

Freigabedatum: **2025/04/10** Zusammenfassung: **Nebenversion**

Hinweis: **Die Linux CCD-Version wird auf den 29. April verschoben.**

**Hinzugefügt:**

* Update auf Qt 6.5.8
* &amp;lbrack;Substance&amp;rbrack; Fügen Sie eine Protokollmeldung für Filter hinzu, wenn mehrere Bildeingaben dieselbe Verwendung haben
* &amp;lbrack;Nvidia&amp;rbrack; Fügen Sie eine Warnung zu den neuesten Nvidia-Treibern hinzu (572.47)

**Fest:**

* &amp;lbrack;Absturz&amp;rbrack; Wenn Sie einen Balken mit einer Verwendung in einem Ein Kanal-Steckplatz ziehen und ablegen
* &amp;lbrack;Absturz&amp;rbrack;&amp;lbrack;Pfad&amp;rbrack; Die Option &quot;Pfadtyp ändern&quot; ist nicht ausgegraut, wenn nicht auf einen bestimmten Pfad geklickt wird
* &amp;lbrack;Pfad füllen&amp;rbrack; Sollte nicht in der Lage sein, Substance-Material auszuwählen
* &amp;lbrack;Engine&amp;rbrack; Artefakte an Pinselstrichen
* &amp;lbrack;Engine&amp;rbrack; Pfade können mit bestimmten Einstellungen unterbrochen werden.
* Problem mit der Dropdown-Liste für den Pipetten-Farbraum
* &amp;lbrack;Automatische Aktualisierung&amp;rbrack; &amp;lbrack;Python&amp;rbrack; Falsche Fehlermeldung bei Verwendung von ResourceID ohne Version
* &amp;lbrack;Shader&amp;rbrack; Absturz beim Öffnen einiger Projekte

**Bekannte Probleme:**

* &amp;lbrack;SpaceMouse&amp;rbrack; Problem beim Arbeiten mit dem Pfadwerkzeug
* &amp;lbrack;Farbmanagement&amp;rbrack; HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen geklemmte Farben
* &amp;lbrack;Regression&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Kontextmenü ist auf HD-Bildschirmen zu klein
* &amp;lbrack;Absturz&amp;rbrack;&amp;lbrack;Python&amp;rbrack; USD Export ausgelöst durch TextureStateEvent
* &amp;lbrack;Engine&amp;rbrack; Malen mit dem Klon-Werkzeug in normalen Kanalverschiebungsfarben falsch
* &amp;lbrack;Python&amp;rbrack; Phantom-Widget wird angezeigt, weil das Skript noch funktioniert

### 11.0.0

Freigabedatum: **2025/03/11** Zusammenfassung: **Hauptversion, neue Funktion zur automatischen Aktualisierung, ausgefülltes Pfadwerkzeug und andere Pfadverbesserungen sowie neue Filter und eine experimentelle Generierung von automatischen Käfigen für das Baking**

**Hinzugefügt**:

* Automatische Aktualisierung
* &amp;lbrack;Automatische Aktualisierung&amp;rbrack; Geänderte Elemente im Bedienfeld &quot;Elemente&quot; automatisch aktualisieren
* &amp;lbrack;Automatische Aktualisierung&amp;rbrack; Geänderte Elemente im gesamten Projekt automatisch aktualisieren
* &amp;lbrack;Automatische Aktualisierung&amp;rbrack; Automatische Aktualisierung standardmäßig deaktiviert lassen
* &amp;lbrack;Automatische Aktualisierung&amp;rbrack; Optionale Aktualisierung, wenn die Ressourcenparameter nicht übereinstimmen (.sbsar, .glsl, .ai, .svg)
* &amp;lbrack;Automatische Aktualisierung&amp;rbrack; Umgebungsvariable zum Deaktivieren der automatischen Aktualisierung hinzufügen
* &amp;lbrack;Auto-update&amp;rbrack;&amp;lbrack;SBSAR&amp;rbrack; Update optional machen, wenn die Ressourcenparameter nicht übereinstimmen
* Ausgefüllter Pfad
* &amp;lbrack;Pfad&amp;rbrack;&amp;lbrack;Füllen&amp;rbrack; Neues Werkzeug zum Erstellen ausgefüllter Pfade hinzufügen
* Verbesserungen an Pfaden
* &amp;lbrack;Pfad&amp;rbrack; Erstellen eines zu Polygonen einrasten Pfads
* &amp;lbrack;Pfad&amp;rbrack; Wechseln von Pfadtypen zulassen
* &amp;lbrack;Pfad&amp;rbrack; Kopieren und Einfügen von Pfadmaskendaten zwischen Scheitelpunkt und Maske zulassen
* &amp;lbrack;Pfad&amp;rbrack; Winkel beim Erstellen eines neuen Punkts einschränken
* &amp;lbrack;Pfad&amp;rbrack; Zuzulassen, dass die Punkterstellung auf eine Linie beschränkt wird
* &amp;lbrack;Pfad&amp;rbrack; Form mit einem Klick schließen
* &amp;lbrack;Pfad&amp;rbrack; Anzeigen von Pfadinformationen
* &amp;lbrack;Pfad&amp;rbrack; Skalieren und Drehen von Pfad-Scheitelpunkten zulassen
* &amp;lbrack;Path&amp;rbrack;&amp;lbrack;UX&amp;rbrack; Gizmos für Transformation leichter zugänglich machen
* &amp;lbrack;Pfad&amp;rbrack; Pfadvorschau hinzufügen
* &amp;lbrack;Pfad&amp;rbrack; Pfadvorschau mit Umschalt + P deaktivieren
* &amp;lbrack;Pfad&amp;rbrack; Verbessern der Tangente Edition in der Seitenansicht
* &amp;lbrack;Pfad&amp;rbrack; Fokus auf einen 3D-Pfad festlegen.
* &amp;lbrack;Pfad&amp;rbrack; Scheitelpunkt sollten den Auswahlstatus beibehalten, wenn sie die Benutzeroberfläche aus- und wieder einschalten
* &amp;lbrack;Pfad&amp;rbrack; Löschen von Pfaden mit Rücktaste zulassen
* &amp;lbrack;Pfad&amp;rbrack; Pfadliste offen halten, wenn der Benutzer sie erweitert
* &amp;lbrack;Pfad&amp;rbrack;&amp;lbrack;Ebenenstapel&amp;rbrack; Duplikate beim Kopieren/Einfügen richtig umbenennen
* &amp;lbrack;Pfad&amp;rbrack; Verbesserungen an Benutzeroberfläche und QuickInfo
* Leistung
* &amp;lbrack;Performance&amp;rbrack; Verbessern der Viewport-Performance bei Verwendung einer hohen Tessellation
* &amp;lbrack;Performance&amp;rbrack; Nur den ersten Kanal für neue Füllebenen/Effekte aktivieren
* &amp;lbrack;Performance&amp;rbrack; Berechnung des Pinselstrichs parallelisieren
* Baking
* &amp;blbrack;Baking&amp;rbrack; Neue vollautomatische Option zur Generierung von Käfigen für das Baking führ mit Meshs mit hohem Poly (experimentell)
* Inhalte
* &amp;lbrack;Inhalt&amp;rbrack; Fügen Sie sechs neue Filter hinzu: stilisierung, quantisieren, anisotropic kuwahara, weiche Abschrägung, Richtungsabstand, Graustufen konvertierung
* &amp;lbrack;Inhalt&amp;rbrack; Aktualisieren von Rauschen und Grunges auf die neueste Version von Designer (mit der neuen 2D-Voronoi)
* &amp;lbrack;Inhalt&amp;rbrack; 3 neue Textur-Generatoren hinzufügen (Kachel-Zufallsgenerator, Triangle Grid, Scratches-Generator)
* &amp;lbrack;Inhalt&amp;rbrack; Vorlage für &quot;Unreales Engine umbenennen&quot; und Exportvorgaben
* Python
* &amp;lbrack;Regal&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Intelligente Material oder intelligente Maske aus Python auf Festplatte speichern
* &amp;lbrack;Python&amp;rbrack; Hinzufügen von automatischem Baking-Käfig zur Python-API
* &amp;lbrack;Python&amp;rbrack; Bearbeiten von Namen und Beschreibungen von Textursätzen/UV-Kacheln zulassen
* &amp;lbrack;Python&amp;rbrack; Auflösungseinstellungen für Vektor- und Schriftquellen freigeben
* &amp;lbrack;Automatische Aktualisierung&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Automatische Aktualisierung von Projekten in Python gelegt
* Verschiedenes
* &amp;lbrack;Export&amp;rbrack; Erleichtern Sie den Zugriff auf die Optionen für &quot;Senden an&quot; mit einem neuen Bedienfeld
* &amp;lbrack;Nvidia&amp;rbrack; Fügen Sie eine Warnung zu den neuesten Nvidia-Treibern hinzu (572.16)
* Die einrasten Winkel sollten durch die Auswahl von Objekt/Welt-Raum beeinflusst werden.
* &amp;lbrack;Textursatz list&amp;rbrack; UV-Kacheln benutzerdefinierten Namen hinzufügen und beim Exportieren verwenden
* Mac
* &amp;lbrack;Mac&amp;rbrack; Verwenden von Metal anstelle von OpenGL für das Grafik-Rendering
* &amp;lbrack;Mac&amp;rbrack; Drop Mac Intel-Support

**Fest**:

* &amp;lbrack;Absturz&amp;rbrack; Löschen der Bildeingabe
* Smart-Matte kann nicht über Ebenenstapel-Taste hinzugefügt werden
* &amp;lbrack;Python&amp;rbrack; Effekte für GroupLayerNode können nicht gefunden werden

**Bekannte Probleme**:

* &amp;lbrack;Farbmanagement&amp;rbrack; HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen geklemmte Farben
* &amp;lbrack;Regression&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Kontextmenü ist auf HD-Bildschirmen zu klein
* &amp;lbrack;Absturz&amp;rbrack;&amp;lbrack;Python&amp;rbrack; USD Export ausgelöst durch TextureStateEvent
* &amp;lbrack;MacOS Intel&amp;rbrack; Absturz beim Importieren einiger Vorgaben
* &amp;lbrack;Engine&amp;rbrack; Malen mit dem Klon-Werkzeug in normalen Kanalverschiebungsfarben falsch
* &amp;lbrack;Python&amp;rbrack; Phantom-Widget wird angezeigt, weil das Skript noch funktioniert
* &amp;lbrack;RedHat&amp;rbrack; Probleme mit dem Farbwähler

## Version 10

### 10.1.2

Veröffentlichungsdatum: **2024/12/3** Zusammenfassung: **Nebenversion, Fehlerbehebungen**

**Fest**:

* &amp;lbrack;Absturz&amp;rbrack; Löschen der Bildeingabe
* Smart-Matte kann nicht über Ebenenstapel-Taste hinzugefügt werden
* &amp;lbrack;Python&amp;rbrack; Effekte für GroupLayerNode können nicht gefunden werden

**Bekannte Probleme**:

* &amp;lbrack;Farbmanagement&amp;rbrack; HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen geklemmte Farben
* &amp;lbrack;Regression&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Kontextmenü ist auf HD-Bildschirmen zu klein
* &amp;lbrack;Absturz&amp;rbrack;&amp;lbrack;Python&amp;rbrack; USD Export ausgelöst durch TextureStateEvent
* &amp;lbrack;MacOS Intel&amp;rbrack; Absturz beim Importieren einiger Vorgaben
* &amp;lbrack;Engine&amp;rbrack; Malen mit dem Klon-Werkzeug in normalen Kanalverschiebungsfarben falsch
* &amp;lbrack;Python&amp;rbrack; Phantom-Widget wird angezeigt, weil das Skript noch funktioniert
* &amp;lbrack;RedHat&amp;rbrack; Probleme mit dem Farbwähler

### 10.1.1

Veröffentlichungsdatum: **2024/11/5** Zusammenfassung: **Nebenversion, Fehlerbehebungen**

**Hinzugefügt**:

* &amp;lbrack;Projekt&amp;rbrack; Aktuelles Projekt geöffnet lassen, bis die Auswahl eines neuen Projekts überprüft wurde
* &amp;lbrack;Automatisches Entpacken&amp;rbrack; Texeldichte ermöglicht eine bessere Aufteilung von UV-Inseln in UDIM
* &amp;blbrack;Baking&amp;rbrack; Mehrdeutige Kopie im Kontextmenü von Mesh-Map reparieren
* &amp;lbrack;Verkrümmen&amp;rbrack; Entfernen der Skalierung im Viewport für die Z-Achse (Tiefe)
* &amp;lbrack;Import/Export&amp;rbrack; Unterstützung nicht verwendeter Bilddateiformate entfernen
* Update Substance Engine auf 9.1.4

**Fest**:

* &amp;lbrack;Absturz&amp;rbrack; Nachdem Sie Ressourcen in &quot;Elemente&quot; verlagert und das Projekt gespeichert haben
* &amp;lbrack;Absturz&amp;rbrack; Probleme mit der Aiserver-Bibliothek
* &amp;lbrack;Absturz&amp;rbrack; Illustrator Server-Absturz in einigen seltenen Fällen
* &amp;lbrack;Absturz&amp;rbrack; Beim Beenden der Anwendung in seltenen Fällen
* Absturz-Berichte können auf einigen Computern nicht gesendet werden
* &amp;blbrack;Baking&amp;rbrack; Die Farbe des Scheitelpunkts ist nicht richtig gelesen
* &amp;lbrack;UI&amp;rbrack; Position von Fenstern und Neuerungen beim Start wurde verschoben
* &amp;lbrack;Assimp&amp;rbrack; Maya&#39;s StandardSurface wird im ID-Baking nicht erkannt
* &amp;lbrack;Python&amp;rbrack; Fehlende SSL-Bibliothek gibt einen Fehler aus
* &amp;lbrack;Python&amp;rbrack;&amp;lbrack;Win&amp;rbrack; Fehler beim Aufrufen von QColorConstants.Transparent
* &amp;lbrack;Python&amp;rbrack; Über Python erstellte Ebenen-Miniaturansichten werden erst aktualisiert, wenn Sie in den Ebenenstapel klicken
* &amp;lbrack;Shader&amp;rbrack; Fehlerhafte Verknüpfung im Shader-API-Changelog
* &amp;lbrack;3D Assets&amp;rbrack; OS-Proxy-Einstellungen beim Zugriff auf 3D-Elemente verwenden

**Bekannte Probleme**:

* &amp;lbrack;Farbmanagement&amp;rbrack; HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen geklemmte Farben
* &amp;lbrack;Regression&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Kontextmenü ist auf HD-Bildschirmen zu klein
* &amp;lbrack;Absturz&amp;rbrack;&amp;lbrack;Python&amp;rbrack; USD Export ausgelöst durch TextureStateEvent
* &amp;lbrack;MacOS Intel&amp;rbrack; Absturz beim Importieren einiger Vorgaben
* &amp;lbrack;Engine&amp;rbrack; Malen mit dem Klon-Werkzeug in normalen Kanalverschiebungsfarben falsch
* &amp;lbrack;Python&amp;rbrack; Widget, das über ein Skript gelöscht scheint, das noch funktioniert
* &amp;lbrack;RedHat&amp;rbrack; Probleme mit dem Farbwähler

### 10.1.0

Freigabedatum: **2024/09/17** Zusammenfassung: **Hauptversion, neuer Inhalt: Füllbereichsmaske/Farbfilter, Stickereiaufklebefilter und sechs generische Substance-Filter, USD mit Material- und Shader-Eigenschaften importieren, Leistungsverbesserung, VFX-Plattform 2024-kompatibel und Migration auf Linux RedHat**

**Hinzugefügt**:

* &amp;lbrack;Inhalt&amp;rbrack; Neue Füllbereichsmaske/neuer Farbfilter hinzufügen
* &amp;lbrack;Inhalt&amp;rbrack; Neuen Stickerei Aufkleber Filter hinzufügen
* &amp;lbrack;Inhalt&amp;rbrack; Fügen Sie 6 neue generische Substance-Filter hinzu (FXAA, Vergröberungsfilter, Hochpass, Posterisierung, Glättungsschritt, Schwellenwert).
* &amp;lbrack;USD&amp;rbrack; Exportieren USD Ebene mit einem definierten ASM-Material
* &amp;lbrack;USD&amp;rbrack; USD mit Material- und Shader-Eigenschaften importieren
* &amp;lbrack;Performance&amp;rbrack; Optimierte Ebenenstapel-Miniaturansichten standardmäßig aktivieren
* &amp;lbrack;Performance&amp;rbrack; Reduzieren der Öffnungszeit von Projektdateien und des Speicherverbrauchs (Datendecodierung)
* VFX-Plattform 2024-kompatibel
* &amp;lbrack;VFX Platform 2024&amp;rbrack; Update auf Python 3.11
* &amp;lbrack;VFX Platform 2024&amp;rbrack; Update auf OpenEXR 3.2
* &amp;lbrack;VFX Platform 2024&amp;rbrack; &amp;lbrack;USD&amp;rbrack; Update OpenSubdiv 3.6.0
* &amp;lbrack;VFX Platform 2024&amp;rbrack;&amp;lbrack;Farbmanagement&amp;rbrack; Update auf OCIO 2.3.2
* &amp;lbrack;Linux&amp;rbrack; Migration zu Linux RedHat
* &amp;lbrack;Linux&amp;rbrack; Aktualisieren Sie die NVIDIA-Treibermindestversion auf 535.171.04
* &amp;lbrack;Import&amp;rbrack; Hinzufügen einer Option zum Spiegeln von Normalen-Map beim Importieren eines GLTF-Meshs
* &amp;lbrack;UI&amp;rbrack; Standardwert des Betriebssystems für die Entfernung der Erkennung von Ziehereignissen verwenden
* &amp;lbrack;Substance Engine&amp;rbrack; Aufrufstreifenfunktion hinzufügen, um die Symbole aus der ausführbaren Datei zu entfernen
* &amp;lbrack;Startbildschirm&amp;rbrack; Update auf neues Startbildschirmformat
* Substance Engine auf Version 9.1.3 aktualisieren
* &amp;lbrack;Python&amp;rbrack; Link zu Beispielen im Ebenenstapel-Dokumentationsmenü anzeigen
* &amp;lbrack;JavaScript&amp;rbrack; Javascript-Plug-ins in den Unterordner &quot;javascript/plugins&quot; verschieben

**Fest**:

* &amp;lbrack;Illustrator&amp;rbrack; Absturz beim Exportieren einer UV-Kachel mit .ai-Grafik in bestimmten Fällen
* &amp;lbrack;Dynamische Pinselstriche&amp;rbrack;&amp;lbrack;Pfad&amp;rbrack; Zufällig pro Strich funktioniert nicht auf einem Pfad
* &amp;lbrack;UI&amp;rbrack;&amp;lbrack;Eigenschaften&amp;rbrack; Sperre ist aktiviert, wenn die Kachelung nicht einheitlich ist
* Debug TXT-Datei wird erstellt, wenn Sie auf ein Painter-Projekt doppelklicken
* &amp;lbrack;USD&amp;rbrack;&amp;lbrack;Export&amp;rbrack; Möglicherweise fehlen einige Texturen
* &amp;lbrack;ASM&amp;rbrack; Farbstreuung-Kanal ignoriert metallic
* &amp;lbrack;Inhalt&amp;rbrack; Weichzeichnungsfilter funktioniert nicht im &quot;funktionierenden&quot; Farbraum
* &amp;lbrack;Inhalt&amp;rbrack; Mit dem Filter &quot;Height anpassen&quot; wird auch das Alpha der Ebene geändert.

**Bekannte Probleme**:

* &amp;lbrack;Farbmanagement&amp;rbrack; HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen geklemmte Farben
* &amp;lbrack;Win&amp;rbrack;&amp;lbrack;Absturz&amp;rbrack; &amp;lbrack;ACE&amp;rbrack; Kein Verwenden des sRGB ICE-Farbraums für die Anzeige transformieren
* &amp;lbrack;Regression&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Kontextmenü ist auf HD-Bildschirmen zu klein
* &amp;lbrack;Absturz&amp;rbrack;&amp;lbrack;Python&amp;rbrack; USD Export ausgelöst durch TextureStateEvent
* &amp;lbrack;MacOS Intel&amp;rbrack; Absturz beim Importieren einiger Vorgaben
* &amp;lbrack;Absturz&amp;rbrack; Ressource verlagern und Projekt speichern
* &amp;lbrack;Engine&amp;rbrack; Malen mit dem Klon-Werkzeug in normalen Kanalverschiebungsfarben falsch
* &amp;lbrack;Python&amp;rbrack; Phantom-Widget wird angezeigt, weil das Skript noch funktioniert
* &amp;lbrack;RedHat&amp;rbrack; Probleme mit dem Farbwähler

### 10.0.1

Freigabedatum: **2024/06/11** Zusammenfassung: **Nebenversion, Fehlerbehebungen**

**Hinzugefügt:**

* &amp;lbrack;Library&amp;rbrack; Konvertieren von Substance-Schriftarten in normale Schriftdateien
* &amp;lbrack;Illustrator&amp;rbrack;&amp;lbrack;SVG&amp;rbrack; Miniaturen in der Bereichsauswahl einen hellgrauen Hintergrund geben
* &amp;lbrack;Python&amp;rbrack; Hinzufügen einer Funktion zur Bitmapquelle, um verfügbare Farbräume aufzulisten

**Fest**:

* &amp;lbrack;Ebenenstapel&amp;rbrack; Ordner immer geschlossen, wenn er in andere Ordner verschoben oder aus anderen Ordnern verschoben wird
* &amp;lbrack;Speichern&amp;rbrack; Die Projektdatei geht verloren, wenn das &quot;Speichern als Kopie&quot; oder das automatische Speichern in bestimmten Fällen fehlschlägt
* &amp;lbrack;Import&amp;rbrack; Assets mit demselben Namen, aber unterschiedlichen Erweiterungen werden überschrieben
* &amp;lbrack;Eigenschaften&amp;rbrack; Einstellungen fehlen, wenn Ankerpunkt in Bildeingaben verwendet wird
* &amp;lbrack;Illustrator&amp;rbrack; Illustrator-Dateien können nach dem Server-Absturz nicht importiert werden, ohne Painter neu zu starten
* &amp;lbrack;Python&amp;rbrack; Übergeordnete Instanz kann nicht mit Typ &quot;Eigenschaften&quot; festgelegt werden
* &amp;lbrack;Python&amp;rbrack; Das Festlegen des hohen Poly-Werts als Baking führend Parameter lädt das hohe Poly nicht
* &amp;lbrack;Python&amp;rbrack; Fehlermeldung für set_color_space() ist zu allgemein
* &amp;lbrack;Python&amp;rbrack; Mit Referenzquellen können Zyklen erstellt werden.

**Bekannte Probleme**:

* &amp;lbrack;Farbmanagement&amp;rbrack; HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen geklemmte Farben
* &amp;lbrack;Regression&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Kontextmenü ist auf HD-Bildschirmen zu klein
* &amp;lbrack;Absturz&amp;rbrack;&amp;lbrack;Python&amp;rbrack; USD Export ausgelöst durch TextureStateEvent
* &amp;lbrack;MacOS Intel&amp;rbrack; Absturz beim Importieren einiger Vorgaben
* &amp;lbrack;Illustrator&amp;rbrack; Absturz beim Exportieren einer UV-Kachel mit .ai-Grafik in bestimmten Fällen
* &amp;lbrack;Dynamische Pinselstriche&amp;rbrack;&amp;lbrack;Pfad&amp;rbrack; Zufällig pro Strich funktioniert nicht auf einem Pfad

### 10.0.0

Freigabedatum: **2024/05/16** Zusammenfassung: **Hauptversion, Edition des Ebenenstapels mit Python-API, Lesen nativer Illustrator-Dateien, Integration von 3D-Assets und neuer Textressource**

**Hinzugefügt**:

* &amp;lbrack;Illustrator&amp;rbrack; Verwenden von Illustrator-Dateien mit Zeichenflächen in Painter
* &amp;lbrack;Illustrator&amp;rbrack;&amp;lbrack;SVG&amp;rbrack; Vorschauen in der Bereichsauswahl hinzufügen
* &amp;lbrack;Substance 3D Assets&amp;rbrack; Durchsuchen, Auswählen und Herunterladen von 3D-Elementen direkt in Painter
* &amp;lbrack;Substance 3D Assets&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Neues Bedienfeld
* &amp;lbrack;Substance 3D Assets&amp;rbrack; Unterstützung für Umgebungs-Map und Materials
* &amp;lbrack;Substance 3D Assets&amp;rbrack; Ermöglicht das erneute Laden und Navigieren im und Öffnen des Speicherortordners in einem neuen Substance 3D Assets-Bedienfeld
* &amp;lbrack;Substance 3D Assets&amp;rbrack; Hinzufügen eines Download-Managers
* &amp;lbrack;Textressource&amp;rbrack; Einbettbare Schriften verwenden
* &amp;lbrack;Textressource&amp;rbrack; Rendern einer Schrift/eines Textes auf einem Mesh zulassen
* &amp;lbrack;Textressource&amp;rbrack; Schriften von Benutzern und anderen freigegebenen Pfaden im Bedienfeld &quot;Elemente&quot; mit einer neuen Kategorie anzeigen
* &amp;lbrack;Textressource&amp;rbrack;&amp;lbrack;Eigenschaften&amp;rbrack; Unterstützung für erweiterte Schrifteigenschaften hinzufügen
* &amp;lbrack;Textressource&amp;rbrack; Suchen/Anzeigen von Schriftarten in Mini-Regalen zulassen
* &amp;lbrack;Textressource&amp;rbrack; Fehlermeldung/Dialogfeld beim Importieren einer inkompatiblen Schrift hinzufügen
* Sonstiges
* &amp;Klammer;Projektion&amp;Klammer füllen; Verbessern des Verhaltens von Skalierungs-Manipulatoren bei Verwendung kleiner Werte
* &amp;lbrack;Manipulator&amp;rbrack; Hinzufügen eines neuen präzisen Modus beim Drücken von STRG-Tastaturbefehl
* &amp;lbrack;Manipulator&amp;rbrack; Verbessern der Stabilität des Manipulators auf der Oberfläche beim Kamera beweg
* &amp;lbrack;Export&amp;rbrack; Hinzufügen eines Farbraumnamens in SBSAR-Ausgaben
* &amp;lbrack;Performance&amp;rbrack; Verbessern der Erkennungszeit von Elementen auf der Festplatte in der Bibliothek
* &amp;lbrack;Substance&amp;rbrack; Update auf Substance Engine Version 9.1.2
* &amp;lbrack;Drag &amp; Drop&amp;rbrack; Ausrichtung der Aufkleberdrehung an der Kamera beim Ablegen im Viewport
* &amp;lbrack;Python&amp;rbrack; Edition des Ebenenstapels
* &amp;lbrack;Python&amp;rbrack; Auswahl von Ebene, Effekt, Maske und Geomaske in der Benutzeroberfläche zulassen
* &amp;lbrack;Python&amp;rbrack; Ebenen-Mischmodi abrufen/festlegen
* &amp;lbrack;Python&amp;rbrack; Einstellungen für die Projektion der Füllebene abrufen/festlegen
* &amp;lbrack;Python&amp;rbrack; Abfragen der Substance-Material-Farbe aus einer Füllebene zulassen
* &amp;lbrack;Python&amp;rbrack; Abfragen und Festlegen von einheitliche Farben und Ressourcen in Ebenen und Effekten zulassen
* &amp;lbrack;Python&amp;rbrack; Erstellen und Bearbeiten von Textressourcen im Ebenenstapel zulassen
* &amp;lbrack;Python&amp;rbrack; Bearbeiten aktiver Kanäle für Ebenen und Effekte zulassen
* &amp;lbrack;Python&amp;rbrack; Stapelverarbeitung von Aktionen zum Rückgängigmachen/Wiederholen einzelner Vorgänge
* &amp;lbrack;Python&amp;rbrack; Laden/Bearbeiten von vektoriellen Quellparametern zulassen
* &amp;lbrack;Python&amp;rbrack; Bearbeitung von Farbegenschaften für Ebenen und Effekte mit Farbmanagement zulassen
* &amp;lbrack;Python&amp;rbrack; Abfragen und Erstellen von instanzierten Ebenen zulassen
* &amp;lbrack;Python&amp;rbrack; Hinzufügen des Effekts &quot;Farbauswahl&quot; zulassen
* &amp;lbrack;Python&amp;rbrack; Steuerung des Farbmanagements für Bitmapbilder zulassen
* &amp;lbrack;Python&amp;rbrack; Engine anhalten/fortsetzen
* &amp;lbrack;Python&amp;rbrack; Navigation zu gleichrangigen und übergeordneten Knoten zulassen
* &amp;lbrack;Python&amp;rbrack; Erstellen eines Filter-/Generatoreffekts zulassen
* &amp;lbrack;Python&amp;rbrack; Hinzufügen eines Ebeneneffekts zulassen
* &amp;lbrack;Python&amp;rbrack; Hinzufügen von intelligente Maske zu einer Ebene zulassen
* &amp;lbrack;Python&amp;rbrack; Erstellen/Bearbeiten von Ankerpunkten zulassen
* &amp;lbrack;Python&amp;rbrack; Maske auf Ebenen abrufen/festlegen
* &amp;lbrack;Python&amp;rbrack; Erstellen des Effekts &quot;Maske vergleichen&quot; zulassen
* &amp;lbrack;Python&amp;rbrack; Abfragen und Verwenden von Vorgaben aus Substance-Ressourcen zulassen
* &amp;lbrack;Python&amp;rbrack; Zulassen, dass Vorgaben und ihre Werte über die Funktion internal_properties für Substance-Ressourcen aufgelistet werden
* &amp;lbrack;Python&amp;rbrack; Auflisten vordefinierter Exportvorgaben zulassen
* &amp;lbrack;Python&amp;rbrack; Erlaubt das Auflisten der in der Bibliothek verfügbaren Exportvorgaben
* &amp;lbrack;Python&amp;rbrack; Abrufen des Inhalts von Exportvorgaben zulassen

**Fest**:

* &amp;lbrack;Absturz&amp;rbrack; &quot;Shader-Instanz entfernen&quot; mit Strg+Z rückgängig machen
* &amp;lbrack;Absturz&amp;rbrack; Erstellen einer Ebene auf leerem Stapel, wenn die letzte Auswahl ein Effekt war
* &amp;lbrack;SVG&amp;rbrack; Problem mit benutzerdefiniertem Wert für den zugeschnittenen Bereich
* &amp;lbrack;Automatisches Entpacken&amp;rbrack; Die Neuberechnung nur des Packings ohne Änderung der UV-Ausrichtung führt zu Absturz
* &amp;blbrack;Drag &amp; Drop&amp;rbrack; Verzögerung aufgrund externer Ressourcen wird mehrmals vorgeladen
* &amp;lbrack;UI&amp;rbrack; Durch Ziehen und Ablegen der Ressourcen-Miniaturansicht kann eine Warnmeldung im Ebenenstapel ausgeblendet werden
* &amp;lbrack;Performance&amp;rbrack; Maskierte UV-Kacheln werden noch berechnet
* &amp;lbrack;USD&amp;rbrack; Falsche Markierung für die Bereichsauswahl
* &amp;lbrack;Ressource&amp;rbrack; Bitmapbild wird beschädigt, nachdem im normalen Kanal gemalt und das Projekt gespeichert wurde
* &amp;lbrack;USD&amp;rbrack; Unterstützung der Bestellung von Meshs für linkshändige Scheitelpunkt
* &amp;lbrack;Substance&amp;rbrack; Auf die Standardeinstellung zurücksetzen, für Winkel-Widget immer wieder auf null zurücksetzen
* &amp;lbrack;Engine&amp;rbrack; Das Malen mit einem SVG in einer Schablone funktioniert nicht
* &amp;lbrack;Engine&amp;rbrack; Normalen-Map-Pinselstriche brechen nach einem Rückgängigmachen ab
* &amp;lbrack;Inhalt&amp;rbrack; &quot;Grafik zu Materialfilter&quot; hat falsche Alpha-Überblendung und falschen Farbraum
* &amp;lbrack;Inhalt&amp;rbrack; Füllmethoden auf dem Tile Generator funktionieren nicht
* &amp;lbrack;Inhalt&amp;rbrack; Histogramm-Scanfilter erzeugt in einigen Fällen Streifenbildung
* &amp;lbrack;Inhalt&amp;rbrack; Baking geführt Beleuchtungsstil berücksichtigt kein gemaltes Height
* &amp;lbrack;Python&amp;rbrack; Unerwarteter Fehler beim Abrufen der instanzierten Ebeneninformationen nach dem Shader-Wechsel
* &amp;lbrack;Speichern&amp;rbrack; Projektdatei geht verloren, wenn &quot;Speichern unter&quot; in bestimmten Fällen fehlschlägt

**Bekannte Probleme**:

* &amp;lbrack;Farbmanagement&amp;rbrack; HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen geklemmte Farben
* &amp;lbrack;Absturz&amp;rbrack;&amp;lbrack;Linux&amp;rbrack;&amp;lbrack;AMD&amp;rbrack; Ziehen und Ablegen von Ressourcen in Ebenenstapel unter Mac OS
* &amp;lbrack;Regression&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Kontextmenü ist auf HD-Bildschirmen zu klein
* &amp;lbrack;Absturz&amp;rbrack;&amp;lbrack;Python&amp;rbrack; USD Export ausgelöst durch TextureStateEvent
* &amp;lbrack;Speichern&amp;rbrack; Die SPP-Projektdatei geht verloren, wenn &quot;Als Kopie speichern&quot; in bestimmten Fällen fehlschlägt
* &amp;lbrack;MacOS Intel&amp;rbrack; Absturz beim Importieren einiger Vorgaben
* &amp;lbrack;Illustrator&amp;rbrack; Ai-Dateien können nach dem Server-Absturz nicht importiert werden, ohne Painter neu zu starten
* &amp;lbrack;Import&amp;rbrack; Assets mit demselben Namen, aber unterschiedlichen Erweiterungen werden überschrieben

## Version 9

### 9.1.2

Veröffentlichungsdatum: **2024/01/30** Zusammenfassung: **Nebenversion, Fehlerbehebungen**

**Hinzugefügt**:

* &amp;lbrack;Performance&amp;rbrack; Verkürzung der Erstellungszeit für erste Füllebenen in neuen Projekten
* &amp;lbrack;Performance&amp;rbrack; Verkürzung der Ladezeit bei großen Umgebungs-Map
* &amp;lbrack;Substance&amp;rbrack; Speichern/Schließen von Projekten zulassen, selbst wenn Miniaturansichten generiert werden

**Fest**:

* Speichern schlägt in Projekten früherer Versionen fehl, wenn der Viewport geändert wird
* &amp;lbrack;Absturz&amp;rbrack; Mesh bei Verwendung von benutzerdefiniertem AO und Farbmanagement erneut importieren
* &amp;Klammer;Projektion&amp;Klammer füllen; Durch Klicken auf den Manipulator &quot;Skalieren&quot; wird die Meldung &quot;nicht bemalbar&quot; angezeigt.
* &amp;Klammer;Pinsel&amp;Klammer; Malen mit UV-Ausrichtung verursacht Artefakte
* &amp;lbrack;Ebenenstapel&amp;rbrack; Das Umbenennen der Ebene ist langsam, wenn der Stapel sehr lang ist
* &amp;lbrack;Ebenenstapel&amp;rbrack; Falsche Fehlermeldung bei Verwendung eines inkompatiblen Filters in der Maske
* &amp;lbrack;Ebenenstapel&amp;rbrack; Die Auswahl wechselt nach dem Löschen wieder zur obersten Ebene
* &amp;lbrack;Export&amp;rbrack; Generierte normale Textur befindet sich immer im 3D-Raum-Nachbar-Auffüllmodus
* &amp;lbrack;Export&amp;rbrack; Textur Alpha wird nicht mit der Exportvorgabe 2D-Ansicht generiert
* &amp;lbrack;Export&amp;rbrack; SBSAR-Export hat falsche Verwendungen mit konvertierten Karten
* &amp;lbrack;Shader&amp;rbrack; Shader-API Changelog ist nicht auf dem neuesten Stand bei ASM

**Bekannte Probleme**:

* &amp;lbrack;Farbmanagement&amp;rbrack; HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen geklemmte Farben
* &amp;lbrack;Absturz&amp;rbrack;&amp;lbrack;Linux&amp;rbrack;&amp;lbrack;AMD&amp;rbrack; Ziehen und Ablegen von Ressourcen in Ebenenstapel unter Mac OS
* &amp;lbrack;Regression&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Kontextmenü ist auf HD-Bildschirmen zu klein
* &amp;lbrack;Absturz&amp;rbrack;&amp;lbrack;Python&amp;rbrack; USD Export ausgelöst durch TextureStateEvent

### 9.1.1

Veröffentlichungsdatum: **2023/12/05** Zusammenfassung: **Nebenversion, Fehlerbehebungen und Senden an After Effects-Funktionen**

**Hinzugefügt:**

* &amp;lbrack;Interop&amp;rbrack; Senden eines strukturierten Meshs an After Effects zulassen (Ae 24.1)

**Fest:**

* &amp;lbrack;Füllen&amp;rbrack; Projektion UV-Satz zu UV-Satz liest nicht mehr als 2 UV-Satz
* &amp;lbrack;Absturz&amp;rbrack; 16.000 Umgebungs-Map
* &amp;lbrack;Absturz&amp;rbrack; Exr als Bildeingabe verwendet
* &amp;lbrack;Absturz&amp;rbrack; Kopieren und Einfügen von Pfaden in andere Projekte
* &amp;lbrack;QoL&amp;rbrack; Ziehen und Ablegen der Alpha-Ressource im Aufklebermodus erstellt UV-Projektion in der Maske
* &amp;lbrack;Pfad&amp;rbrack; Durch Kopieren von Pfad-Scheitelpunkten wird auch der Zielpfad beim erneuten Öffnen des Projekts umbenannt.
* &amp;lbrack;Linux&amp;rbrack; Die Farbauswahl kann mit mehreren Bildschirmen unterbrochen werden
* &amp;lbrack;Automatisch Entpackt&amp;rbrack; UI-Problem für die Texeldichtesteuerung
* &amp;lbrack;Farbmanagement&amp;rbrack; UI-Feedback ist sinnvoll, aber Engine ist nicht
* &amp;lbrack;Farbmanagement&amp;rbrack; Falsche Farbraumauswahl in der Maske mit Überschreibung der Benutzerdaten

**Bekannte Probleme:**

* &amp;lbrack;Farbmanagement&amp;rbrack; HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen geklemmte Farben
* &amp;lbrack;Absturz&amp;rbrack;&amp;lbrack;Linux&amp;rbrack; mit Linux Wayland auf AMD, wenn Ressourcen per Drag &amp; Drop in den Ebenenstapel gezogen werden
* &amp;lbrack;Absturz&amp;rbrack;&amp;lbrack;Mac&amp;rbrack; Anisotropische Filterung ändern unter Monterey OS
* &amp;lbrack;Regression&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Kontextmenü ist auf dem HD-Bildschirm zu klein
* &amp;lbrack;Python&amp;rbrack; Absturz beim Exportieren von USD, die durch TextureStateEvent ausgelöst werden

### 9.1.0

Freigabedatum: **2023/11/07** Zusammenfassung: **Hauptversion mit SVG- und Transparenzunterstützung sowie Verbesserungen an Drag-and-Drop- und Pfad-Tools**

**Hinzugefügt:**

* &amp;lbrack;SVG&amp;rbrack; Importieren von Vektordateien zulassen (SVG)
* &amp;lbrack;SVG&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Unterstützung für SVG-spezifische Eigenschaften hinzufügen
* &amp;lbrack;SVG&amp;rbrack; Mit dieser Option werden die Proportionen des Originalbilds beibehalten.
* &amp;lbrack;SVG&amp;rbrack; Automatisches Verwenden von Alpha von SVG mit Transparenz zulassen
* &amp;lbrack;Interop&amp;rbrack; Senden eines strukturierten Meshs an After Effects zulassen (Ae 24.1 Beta)
* &amp;lbrack;Interop&amp;rbrack; Hinzufügen von Einstellungen für &quot;An After Effects senden&quot;
* &amp;lbrack;QoL&amp;rbrack;&amp;lbrack;Assets&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Element automatisch importieren, wenn es per Drag &amp; Drop in einen Benutzeroberflächensteckplatz gezogen wird
* &amp;lbrack;QoL&amp;rbrack; Zulassen, dass externe Elemente in den Ebenenstapel gezogen und dort abgelegt werden
* &amp;lbrack;QoL&amp;rbrack;&amp;lbrack;Ebenenstapel&amp;rbrack; Ziehen Sie Texturen per Drag &amp; Drop aus dem Bedienfeld &quot;Elemente&quot; in den Ebenenstapel
* &amp;lbrack;QoL&amp;rbrack;&amp;lbrack;Viewport&amp;rbrack; Generator ziehen und ablegen, Filter auf dem Mesh zulassen
* &amp;lbrack;QoL&amp;rbrack;&amp;lbrack;Viewport&amp;rbrack; Zulassen, dass externe Elemente auf den Mesh gezogen werden
* &amp;lbrack;QoL&amp;rbrack;&amp;lbrack;Projektion&amp;rbrack; Neuen UV-Satz zum UV-Satz-Projektion hinzufügen
* &amp;lbrack;QoL&amp;rbrack; Intelligente Masken in Viewport und Ebenenstapel als neue Ebenen ziehen und ablegen
* &amp;lbrack;QoL&amp;rbrack; Selektor für Generatoren mit mehreren Ausgaben hinzufügen, wenn er in der Maske verwendet wird
* &amp;lbrack;QoL&amp;rbrack; Ziehen und Ablegen von Ein Kanal-Bildern über einen Fülleffekt zulassen
* &amp;lbrack;QoL&amp;rbrack;&amp;lbrack;Ebenenstapel&amp;rbrack; Verwenden Sie STRG/ALT-Modifizierer mit Drag &amp; Drop, um anzugeben, wo/wie Effekte/Ebenen erstellt werden sollen
* &amp;lbrack;Pfad&amp;rbrack; Sichtbarkeit einzelner Pfade im Pfadbedienfeld ein-/ausschalten
* &amp;lbrack;Pfad&amp;rbrack; Verwenden von Transformations-Manipulatoren für Pfadpunkte zulassen
* &amp;lbrack;Pfad&amp;rbrack; Manuelles Steuern der Tangenten pro Scheitelpunkt zulassen
* &amp;lbrack;Pfad&amp;rbrack; Kopieren/Einfügen von Pfadeigenschaften
* &amp;lbrack;Pfad&amp;rbrack; Leerer Tastaturbefehl für die Tangente der Unterbrechung
* &amp;lbrack;Shader&amp;rbrack; Unterstützung für Deckkraft und Translucency in ASM Shader hinzufügen
* &amp;lbrack;Shader&amp;rbrack; Unterstützung für Absorptionsfarbe Channel mit ASM Shader hinzufügen
* &amp;lbrack;Shader&amp;rbrack; QuickInfos zu ASM-Shader-Parametern verbessern
* &amp;lbrack;Shader&amp;rbrack; Standardfarbe des Translucency-Kanals in Schwarz ändern
* &amp;lbrack;Anzeigeeinstellungen&amp;rbrack; Temporale Anti-Aliasing standardmäßig aktivieren
* &amp;lbrack;Anzeigeeinstellungen&amp;rbrack; Standardeinstellung für die Teilflächenstreuung aktivieren
* &amp;lbrack;Substance&amp;rbrack; Hinzufügen von Unterstützung für die ColorSpace-Eigenschaft von der Eingabe/Ausgabe durch den Graf
* &amp;lbrack;Substance&amp;rbrack; Substance Engine auf Version 9.0.3 aktualisieren
* &amp;lbrack;UI&amp;rbrack; Kontextabhängige Symbolleistenschaltfläche barrierefrei machen, selbst wenn das App-Fenster klein ist
* &amp;lbrack;Automatisch Entpackt&amp;rbrack; Steuert die Anzahl der UV-Kacheln mit der Texeldichte
* &amp;blbrack;Baking&amp;rbrack; GPU-Raytracing auf AMD-GPUs standardmäßig deaktivieren
* &amp;lbrack;Performance&amp;rbrack; Verlustfreie Komprimierung auf 16-Bit-Bilder anwenden, um den Projektbedarf zu verringern
* &amp;lbrack;Python&amp;rbrack; Ändern der standardmäßigen Kamera in der 3D-Ansicht zulassen
* &amp;lbrack;Python&amp;rbrack; Gelegt Möglichkeit, Mesh über Skripterstellung zu exportieren
* &amp;lbrack;Content&amp;rbrack;&amp;lbrack;Samples&amp;rbrack; Neues Beispielprojekt &quot;Französischer Restauranttisch&quot; hinzufügen
* &amp;lbrack;Inhalt&amp;rbrack; Alpha-Substance-Logo auf neue Version aktualisieren
* &amp;lbrack;Inhalt&amp;rbrack; Drei Material-Filter auf SVG anwenden (Custom Sticker, Custom Spray und Graphic to Material)

**Fest:**

* &amp;lbrack;Absturz&amp;rbrack; Ändern der Manipulator-Größe, wenn das Symmetrie-Werkzeug nicht verwendet wird
* &amp;lbrack;Absturz&amp;rbrack; &amp;lbrack;Ebenenstapel&amp;rbrack; Erstellen einer Ebene, wenn nichts ausgewählt ist
* &amp;lbrack;Projekt&amp;rbrack; Mesh-Map können beschädigt werden, nachdem nicht verwendete Ressourcen entfernt wurden.
* &amp;lbrack;Projekt&amp;rbrack; Ressourcenbeschädigung nach dem erneuten Importieren oder Baking des Images
* &amp;lbrack;Assets&amp;rbrack; Durch erneutes Laden eines Assets wird es aus den Favoriten entfernt
* &amp;lbrack;Import&amp;rbrack; Ressourcen können nicht importiert werden, wenn im Bedienfeld &quot;Elemente&quot; &quot;Kein Ergebnis gefunden&quot; angezeigt wird
* &amp;lbrack;UI&amp;rbrack; Der Pfeil der kontextbezogenen Symbolleiste wird in einigen Fällen nicht angezeigt
* &amp;lbrack;Substance&amp;rbrack; Schaltfläche &quot;Nebeneinander&quot; für boolesche Werte wird nicht unterstützt
* &amp;lbrack;Ebene&amp;rbrack; Falsche Kanalbeschriftung bei Verwendung in der Maske
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;glTF&amp;rbrack; glTF/GLB-Dateien, die aus Painter exportiert werden, haben keine Physische Größe
* &amp;lbrack;Inhalt&amp;rbrack; Intensität des Weichzeichnungsfilters ist auf 16 eingestellt
* &amp;lbrack;Inhalt&amp;rbrack; Farbabstimmungsfilter &quot;Zielfarbe&quot; Bildeingabe ist nicht sichtbar

**Bekannte Probleme:**

* &amp;lbrack;Farbmanagement&amp;rbrack; HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen geklemmte Farben
* &amp;lbrack;Absturz&amp;rbrack;&amp;lbrack;Linux&amp;rbrack; mit Linux Wayland auf AMD, wenn Ressourcen per Drag &amp; Drop in den Ebenenstapel gezogen werden
* &amp;lbrack;Absturz&amp;rbrack;&amp;lbrack;Mac&amp;rbrack; Anisotropische Filterung ändern unter Monterey OS
* &amp;lbrack;Absturz&amp;rbrack; Exr als Bildeingabe verwendet
* &amp;lbrack;Absturz&amp;rbrack; 16.000 Umgebungs-Map
* &amp;lbrack;Automatisch Entpackt&amp;rbrack; UI-Problem für die Texeldichtesteuerung
* &amp;lbrack;Regression&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Kontextmenü ist auf dem HD-Bildschirm zu klein
* &amp;lbrack;Python&amp;rbrack; Absturz beim Exportieren von USD, die durch TextureStateEvent ausgelöst werden
* &amp;lbrack;QoL&amp;rbrack; Ziehen und Ablegen der Alpha-Ressource im Aufklebermodus erstellt UV-Projektion in der Maske

### 9.0.1

Freigabedatum: **2023/09/19** Zusammenfassung: **Geringfügige Fehlerbehebungsversion mit mehreren Verbesserungen**

**Hinzugefügt:**

* &amp;lbrack;Import&amp;rbrack; Standard-Importspeicherort im Importfenster festlegen
* &amp;blbrack;Baking-Modus&amp;rbrack; Parameter auf ihre Standardwerte zurücksetzen
* &amp;blbrack;Baking&amp;rbrack; Baking beim Erstellen eines Projekts auf Malen-Auflösung festlegen
* &amp;lbrack;Symmetrie&amp;rbrack; Symmetrie-spezifischen Manipulator vom Tastaturbefehl Q lösen
* &amp;lbrack;Menü&amp;rbrack; Option &quot;Protokoll anzeigen&quot; im Hilfemenü hinzufügen
* &amp;lbrack;Viewport&amp;rbrack; Verbessern der Schatten-Rendering-Geschwindigkeit
* &amp;lbrack;Substance&amp;rbrack; Engine auf Version 9.0.1 aktualisieren
* &amp;lbrack;Farbmanagement&amp;rbrack; OCIO Konfigurationsdatei kann einen beliebigen Erweiterungstyp haben
* &amp;lbrack;Assets&amp;rbrack; SBSAR-Ressource mit &#39;Aufkleber&#39; sollte automatisch auf Warp-Projektion gesetzt werden
* &amp;lbrack;Pfad&amp;rbrack; Anzeigen einer Meldung, wenn versucht wird, mit dem Pfadwerkzeug zu interagieren, während UI und Gizmos ausgeblendet sind

**Fest:**

* &amp;lbrack;Absturz&amp;rbrack; Alt + Ziehen im Pfadbedienfeld
* &amp;lbrack;Ressourcen&amp;rbrack; importieren Zufälliger Absturz beim Entfernen der zu importierenden Ressourcen
* Absturz beim Importieren einer komprimierten GLB-Datei
* Problem beim Malen auf Meshs, die UVs gemeinsam nutzen
* Mesh blinkt schwarz, wenn der Cache neu berechnet oder geladen wird
* &amp;lbrack;Eigenschaften&amp;rbrack; Kontextmenü zum Zurücksetzen der Parameter wird in Dropdown-Listen nicht angezeigt
* &amp;lbrack;Ebene&amp;rbrack; Schieberegler für Eingabe nach vorheriger Ebene gesperrt
* &amp;lbrack;AMD&amp;rbrack;&amp;lbrack;Sparse&amp;rbrack; SVT-Option, wenn aktiviert, erzeugt Artefakte
* &amp;lbrack;Projektion&amp;rbrack;&amp;lbrack;Verkrümmen&amp;rbrack; Absturz beim Doppelklicken auf Scheitelpunkte
* &amp;lbrack;Pfad&amp;rbrack; Benutzeroberfläche und Pfad werden im Baking-Modus angezeigt
* &amp;lbrack;AMD&amp;rbrack; Textur verloren, wenn mit Sicht gespielt wird
* &amp;lbrack;Sparse&amp;rbrack; Zu niedrige Auflösung beim Umdrehen des Meshs

**Bekannte Probleme:**

* &amp;lbrack;Farbmanagement&amp;rbrack; HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen geklemmte Farben

### 9.0.0

Freigabedatum: **2023/06/20** Zusammenfassung: **Hauptversion mit Malen entlang des Pfades, die 3D-Kurven, neue Basismaterialien und das Bereinigen älterer Materialien sowie neue Vorgaben für 3D-Kurven ermöglicht**

**Hinzugefügt:**

* &amp;lbrack;Pfad&amp;rbrack; Neue Malen entlang des Pfads hinzufügen
* &amp;lbrack;Pfad&amp;rbrack; Hinzufügen eines leeren Tastaturbefehls für das Pfadwerkzeug
* &amp;lbrack;Pfad&amp;rbrack; Hinzufügen neuer Punkte zu einem vorhandenen Pfad zulassen
* &amp;lbrack;Pfad&amp;rbrack; Tastaturbefehl hinzufügen, um die aktuelle Pfaderstellung zu beenden
* &amp;lbrack;Pfad&amp;rbrack; Bearbeiten der Pinseleigenschaften für Pfade zulassen
* &amp;lbrack;Pfad&amp;rbrack; Tangenten beim Platzieren eines Punkts automatisch anpassen
* &amp;lbrack;Pfad&amp;rbrack; Tangenten beim Verschieben eines Punkts neu berechnen
* &amp;lbrack;Pfad&amp;rbrack; Einrasten neu erzeugter Ankerpunkte an die Fläche eines Meshs
* &amp;lbrack;Pfad&amp;rbrack; Bearbeiten des Drucks pro Scheitelpunkt zulassen
* &amp;lbrack;Pfad&amp;rbrack; Anpassen des Drucks des neu erstellten Punkts von benachbarten Punkten
* &amp;lbrack;Pfad&amp;rbrack; Umwandeln von Punkten in Übergangspunkte/Eckpunkte zulassen (Tangente umbrechen)
* &amp;lbrack;Pfad&amp;rbrack; Verschieben eines neu hinzugefügten Punkts sofort zulassen
* &amp;lbrack;Pfad&amp;rbrack; Entfernen von Punkten aus vorhandenem Pfad zulassen
* &amp;lbrack;Pfad&amp;rbrack; Umkehren der Richtung eines Pfades zulassen
* &amp;lbrack;Pfad&amp;rbrack; Auswahl eines Pfads im Viewport zulassen
* &amp;lbrack;Pfad&amp;rbrack; Auswählen von Pfadpunkten mit dem Auswahlrechteck zulassen
* &amp;lbrack;Pfad&amp;rbrack; Einführung von STRG+A-Tastaturbefehlen zum Auswählen aller Punkte eines Pfades
* &amp;lbrack;Pfad&amp;rbrack; Schließen des Pfads zulassen
* &amp;lbrack;Pfad&amp;rbrack; Geben Sie die Achse &quot;Pfad nach oben&quot; in den Eigenschaften an
* &amp;lbrack;Pfad&amp;rbrack; Hinzufügen eines Scheitelpunkt-Steuerungsmenüs zur kontextabhängigen Symbolleiste
* &amp;lbrack;Pfad&amp;rbrack; Hinzufügen von Malen-/Radier-/Verwischen-Modi zum Pfadwerkzeug
* &amp;lbrack;Pfad&amp;rbrack; Visuelles Feedback für Pfade im Viewport erstellen
* &amp;lbrack;Pfad&amp;rbrack; Visuelle Anzeige der Pfadrichtung hinzufügen
* &amp;lbrack;Pfad&amp;rbrack; Thickness der Pfadanzeige hinzufügen
* &amp;lbrack;Pfad&amp;rbrack; Pfade ausblenden.
* &amp;lbrack;Pfad&amp;rbrack; Bedienfeld &quot;Pfad hinzufügen&quot;, um Pfade der aktuell ausgewählten Ebene aufzulisten
* &amp;lbrack;Pfad&amp;rbrack; Visuelles Feedback beim Bewegen des Mauszeigers über einen Pfad im Pfadbedienfeld hinzufügen
* &amp;lbrack;Pfad&amp;rbrack; Pfadbedienfeld anzeigen, wenn das Pfadwerkzeug ausgewählt ist
* &amp;lbrack;Pfad&amp;rbrack; Umbenennen, Löschen, Kopieren, Ausschneiden und Duplizieren von Pfaden im Bedienfeld &quot;Pfad&quot; zulassen
* &amp;lbrack;Pfad&amp;rbrack; Meldung anzeigen, wenn versucht wird, im 2D-Viewport mit dem Pfadwerkzeug zu interagieren
* &amp;lbrack;Library&amp;rbrack; Neue Inhalte integrieren (Pfadwerkzeuge und Basismaterialien)
* &amp;lbrack;Dynamische Pinselstriche&amp;rbrack; Eigenschaft &quot;Abstand&quot; für Dynamische Pinselstriche hinzufügen
* &amp;lbrack;Dynamische Pinselstriche&amp;rbrack; Hinzufügen von Größen- und Abstand-Eigenschaften zu Dynamischen Pinselstrichen
* &amp;lbrack;Dynamische Pinselstriche&amp;rbrack; Hinzufügen der Eigenschaft &quot;Anfang/Mitte/Ende&quot; für Dynamische Pinselstriche
* &amp;lbrack;Python&amp;rbrack;&amp;lbrack;USD&amp;rbrack; Leg von Projektkonfigurationsparametern für das USD
* &amp;lbrack;Python&amp;rbrack;&amp;lbrack;USD&amp;rbrack; Leg der Projekterstellungsparameter für das USD
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;USD&amp;rbrack; Projektpfadinformationen in exportierten USD hinzufügen
* &amp;lbrack;GLTF&amp;rbrack; Texturen in der Bibliothek beim erneuten Laden einer GLTF-Datei aktualisieren
* &amp;lbrack;Shader&amp;rbrack; Reduzieren von Artefakten in der Naht von UV-Inseln mit unterschiedlicher Ausrichtung
* &amp;lbrack;Engine&amp;rbrack; Update auf Substance Engine Version 9.0

**Fest:**

* &amp;lbrack;Import&amp;rbrack; Einige GLB mit Texturen erhalten keine Texturen in Painter
* &amp;lbrack;AMD&amp;rbrack; Artefakte an Rahmen für alle 3D-Projektion-Flächen
* &amp;lbrack;Engine&amp;rbrack; Texturen brechen beim Umschalten der Ebenensichtbarkeit ab
* &amp;lbrack;Engine&amp;rbrack; Beim Ändern des Mischmodus sind an einigen Stellen Texturen leer
* &amp;lbrack;Engine&amp;rbrack; Textur/Projektion ist in einigen Fällen leerer Verkrümmungsmodus
* &amp;lbrack;Iray&amp;rbrack; Iteration wird beim Speichern des Renderings auf 0 zurückgesetzt
* &amp;lbrack;Log&amp;rbrack; USD Fehlermeldung beim Ausführen von &quot;Datei&quot; > &quot;Neu&quot;

**Bekannte Probleme:**

* &amp;lbrack;Farbmanagement&amp;rbrack; HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen geklemmte Farben
* &amp;lbrack;Ebenenstapel&amp;rbrack; Eingabequelle nicht pro Ebene gespeichert

## Version 8

### 8.3.1

Freigabedatum: **2023/04/27**

**Hinzugefügt:**

* &amp;blbrack;Baking-Modus&amp;rbrack; Tastaturbefehl hinzufügen (leer), um den Viewport anzuzeigen/auszublenden
* &amp;blbrack;Baking-Modus&amp;rbrack; Bei Verwendung der Schaltfläche &quot;Baking führend Mesh ausblenden&quot; immer niedrige Poly-Werte anzeigen
* &amp;blbrack;Baking-Modus&amp;rbrack; Suffix für &quot;Zuordnung nach Name&quot; basierend auf aktuellem Textursatz anzeigen
* &amp;lbrack;Import&amp;rbrack; Unterstützung für GLTF-Binärdateien (glb) hinzufügen
* &amp;lbrack;Textursatz list&amp;rbrack; Menü &quot;Hinzufügen&quot; zum Auswählen oder Erstellen von Shader-Instanzen
* &amp;lbrack;Textursatz list&amp;rbrack; Schnelles Ändern der Auflösung von Textursatz und UV-Kachel
* &amp;lbrack;Physische Größe&amp;rbrack; Verbessern des Manipulator-Verhaltens bei der Verwendung von Physische Größe in UV-Projektionen
* &amp;lbrack;UI&amp;rbrack; &quot;Speichern unter&quot; wieder im Dateimenü anzeigen
* &amp;lbrack;UI&amp;rbrack; Speichern der Ansichtsauswahl (nur 2D, nur 3D, beide) im UI-Layout
* &amp;lbrack;USD&amp;rbrack; Weniger vage Fehlermeldung bei der Projekterstellung mit nicht unterstützten USD
* &amp;lbrack;Python&amp;rbrack; Hinzufügen von Baking führend Ereignissen, um den Fortschritt des Bakings zu verfolgen
* &amp;lbrack;Python&amp;rbrack; Abbrechen eines Baking zulassen
* &amp;lbrack;Python&amp;rbrack; &quot;Basierend auf Ausgabevorlage&quot; für Dateityp und Bittiefe beim Exportieren gelegt
* &amp;lbrack;Python&amp;rbrack; Gelegt Aktualisierungszeit für TextureStateEvent.Update

**Fest:**

* &amp;lbrack;Absturz&amp;rbrack; Seltener Absturz beim Schließen eines Projekts
* &amp;lbrack;Absturz&amp;rbrack; &amp;blbrack;Baking&amp;rbrack; Mesh-Map-Synchronisierung mit Height oder Krümmung für ein bestimmtes Projekt aktivieren
* &amp;lbrack;Absturz&amp;rbrack;&amp;lbrack;Scripting&amp;rbrack; Absturz beim Hinzufügen eines Materials nach dem Erstellen einer Shader-Instanz
* &amp;blbrack;Baking-Modus&amp;rbrack; Die AO-Intensität im neutralen Material hat keine Auswirkungen
* &amp;blbrack;Baking-Modus&amp;rbrack; Absturz beim Wechseln in den Baking-Modus, bevor das Modell geladen wird
* &amp;blbrack;Baking-Modus&amp;rbrack; Fehlermeldung &quot;Fehlende Fehlermeldung&quot; auf der Registerkarte &quot;Baking führend Prozess&quot;
* &amp;blbrack;Baking-Modus&amp;rbrack; Einstellungen für neutrales Material haben nach dem erneuten Importieren eines Meshs keine Auswirkungen
* &amp;blbrack;Baking-Modus&amp;rbrack; Viewport-Trennzeichen werden global und nicht pro Modus gespeichert.
* &amp;blbrack;Baking-Modus&amp;rbrack; Visualisierungsproblem: Durchschnittliche Normale verändert die Oberfläche des Käfigs nicht
* &amp;lbrack;Farbmanagement&amp;rbrack; Die Einstellung &quot;Farbraum automatisch erkennen&quot; ist deaktiviert, wenn OCIO env var vorhanden ist
* &amp;lbrack;Inhalt&amp;rbrack; Der Maskenkonturfilter weist ein Artefakt mit Height-Eingabe auf.
* &amp;lbrack;Inhalt&amp;rbrack; Intensitätsregler des Steigung-Weichzeichnungsfilters ist auf 1,0 geklemmt
* &amp;lbrack;Interop&amp;rbrack; Projekt mit GLTF kann nicht aus Sampler erstellt werden
* &amp;lbrack;Ebenenstapel&amp;rbrack; Der Wert für die Kachelung der Projektion wird nicht korrekt mit dem Manipulator aktualisiert
* &amp;lbrack;Linux&amp;rbrack; Versatz zwischen Grafiktablett-Stift und Cursor mit einem HDPI-Wert von mehr als 100 %
* &amp;lbrack;Python&amp;rbrack; Absturz beim erneuten Importieren eines Meshs nach dem Erstellen eines Projekts
* &amp;lbrack;Substance&amp;rbrack; 3D-Rauschen funktionieren nach dem erneuten Importieren eines Meshs nicht mehr
* &amp;blbrack;UV-Kacheln&amp;rbrack; Offset für UV-Projektion wird auf 1 geklemmt
* &amp;lbrack;Viewport&amp;rbrack; Visuelles Feedback zu geraden Linien ist nicht mehr sichtbar
* &amp;lbrack;WhatsNew&amp;rbrack; Falscher Zeilenumbruch bei Funktionstiteln

**Bekannte Probleme:**

* &amp;lbrack;Import&amp;rbrack; Einige GLB mit Texturen erhalten keine Texturen in Painter

### 8.3.0

*(Freigegeben: 10. Januar 2023 (1})Zusammenfassung:**Hauptversion mit neuem Importmodus, neuem Baking und Export von USD und Physische Größe-Unterstützung für UV-Projektion***

**Hinzugefügt:**

* &amp;blbrack;Baking-Modus&amp;rbrack; Neuer Baking-Modus, der dem Baking gewidmet ist

* &amp;blbrack;Baking-Modus&amp;rbrack; Tastaturbefehl so einstellen, dass er in den Baking-Modus auf F8 wechselt

* &amp;blbrack;Baking-Modus&amp;rbrack; Schaltfläche &quot;Baking hinzufügen&quot; und &quot;Abbrechen&quot; im Viewport

* &amp;blbrack;Baking-Modus&amp;rbrack; Hinzufügen einer Baking führend Auswahl in der Liste &quot;Textursatz&quot;

* &amp;blbrack;Baking-Modus&amp;rbrack; Fenster &quot;Neue Mesh-Map-Baker hinzufügen&quot;, um Baker auszuwählen

* &amp;blbrack;Baking-Modus&amp;rbrack; Neues Fenster &quot;Mesh-Map-Einstellungen hinzufügen&quot; zum Bearbeiten der Baking-Einstellungen

* &amp;blbrack;Baking-Modus&amp;rbrack; Neues Baking-Protokollfenster hinzufügen, um dem Baking zu folgen

* &amp;blbrack;Baking-Modus&amp;rbrack; Hinzufügen von Baking führend Parametern und Rückgängigmachen von Aktionen zum Verlaufsfenster

* &amp;blbrack;Baking-Modus&amp;rbrack; Breadcrumbs in den Mesh-Map-Einstellungen hinzufügen

* &amp;blbrack;Baking-Modus&amp;rbrack; Hinzufügen von Mesh-Map-Miniaturansichten im Fenster &quot;Mesh-Map Baker&quot;

* &amp;blbrack;Baking-Modus&amp;rbrack; Minimierbares Menü &quot;Visualisierungseinstellungen hinzufügen&quot; im 3D-Viewport

* &amp;blbrack;Baking-Modus&amp;rbrack; Hinzufügen einer Visualisierungseinstellung zum Ein-/Ausblenden des Meshs mit hoher Poly-Intensität

* &amp;blbrack;Baking-Modus&amp;rbrack; Visualisierungseinstellung zum Ein-/Ausblenden des Käfig-Meshs und der Drahtgitter hinzufügen

* &amp;blbrack;Baking-Modus&amp;rbrack; Visualisierungseinstellung hinzufügen, um den Mesh mit geringer Poly-Intensität ein- oder auszublenden

* &amp;blbrack;Baking-Modus&amp;rbrack; Visualisierungseinstellung hinzufügen, um harte Kanten ohne UV-Nähte als Fehler darzustellen

* &amp;blbrack;Baking-Modus&amp;rbrack; Im Viewport über Mesh- und Baking-Fehler informieren, wenn das Baking-Protokoll nicht angezeigt wird

* &amp;blbrack;Baking-Modus&amp;rbrack; Aktion zum Synchronisieren der Baker-Einstellungen auf allen Textursätzen hinzufügen

  Im Fenster &quot;Mesh-Map-Baker&quot; kann jeder Baker (sowie die allgemeinen Einstellungen) über Textursatz hinweg synchronisiert werden, indem Sie auf das Verknüpfungssymbol neben dem Namen klicken. Dadurch wird ein Fenster geöffnet, in dem Sie auswählen können, welche Textursatz dieselben Parameter verwenden sollen.

* &amp;blbrack;Baking-Modus&amp;rbrack; Hinzufügen von Aktionen zum Kopieren und Einfügen von Baker

  Im Fenster &quot;Mesh-Map-Baker&quot; stehen Aktionen zum Kopieren und Übergehen der einzelnen Baker-Einstellungen über Textursätze hinweg zur Verfügung, entweder über das spezielle Menü am oberen Fensterrand oder über das Kontextmenü mit der rechten Maustaste.

* &amp;blbrack;Baking-Modus&amp;rbrack; Schaltfläche &quot;Baking hinzufügen&quot; im Fehlerprotokoll, um von den Fehlereinstellungen nach rechts zu springen

  Wenn ein Baker fehlschlägt oder ein Mesh nicht ordnungsgemäß geladen wird, wird im Protokoll eine Fehlermeldung Baking geführt. Mit einer Schaltfläche neben der Meldung können Sie das Fenster Mesh-Map-Baker und Mesh-Map-Einstellungen ändern, um die entsprechenden Einstellungen anzuzeigen. Dies hilft dabei, die Ursache eines Problems einfacher zu isolieren, um es beheben zu können.

* &amp;blbrack;Baking-Modus&amp;rbrack; Menüs hinzufügen, um Textursatz und Baker zu verwalten

  Sowohl im Fenster &quot;Textursatz-Liste&quot; als auch im Fenster &quot;Mesh-Map-Baker&quot; wurde ein kleines Aktionsmenü hinzugefügt, um das Kopieren und Umkehren von Auswahlen zu unterstützen.

* &amp;blbrack;Baking-Modus&amp;rbrack; Baker-Auswahlliste pro Textursatz teilen

* &amp;blbrack;Baking-Modus&amp;rbrack; Gemeinsame Einstellungen pro Textursatz teilen

* &amp;blbrack;Baking-Modus&amp;rbrack; Mesh mit hoher Poly- und Käfig-Auflösung laden, ohne die Oberfläche einzufrieren

* &amp;blbrack;Baking-Modus&amp;rbrack; Verwenden Sie die Fortschrittsleiste des Viewports, um das Laden des Meshs anzuzeigen

* &amp;blbrack;Baking-Modus&amp;rbrack; Ladestatus des Meshs im Baking-Protokoll hinzufügen

* &amp;blbrack;Baking-Modus&amp;rbrack; Mesh im Viewport während des Bakings umkehren

* &amp;blbrack;Baking-Modus&amp;rbrack; Baking-Reihenfolge auf der Grundlage der Sichtbarkeit des aktuellen Viewports des Meshs festlegen

* &amp;blbrack;Baking-Modus&amp;rbrack; Implizit Baking führend Käfig in Viewport anzeigen

  Wenn keine benutzerdefinierte Käfig-Meshdatei verwendet wird, wird ein automatischer Käfig-Mesh generiert und im Viewport angezeigt. Die Größe basiert auf dem Parameter &quot;Max. Frontalentfernung&quot; aus den allgemeinen Einstellungen des Bakings. Mit dem Mesh &quot;Käfig&quot; wird angegeben, wie weit die Anpassung zwischen dem niedrigen und dem hohen Poly-Wert gehen wird.

* &amp;blbrack;Baking-Modus&amp;rbrack; Übereinstimmende Liste von Mesh-Namen für &quot;Übereinstimmender Name&quot; im Baking-Protokoll anzeigen

* &amp;blbrack;Baking-Modus&amp;rbrack; 3D-Material im Viewport mit neutralem Modell anzeigen

* &amp;blbrack;Baking-Modus&amp;rbrack; Berechnung des Engine im Baking deaktivieren

* &amp;blbrack;Baking-Modus&amp;rbrack; Beim Beenden der App während eines Baking wird eine Warnung angezeigt

* &amp;lbrack;Baker&amp;rbrack; Aktualisieren der Beschriftungen für Anti-Aliasing-Einstellungen

  Die Einstellungswerte für das Anti-Aliasing wurden in &quot;Supersampling&quot; umbenannt und mit einer expliziten Multiplikatornummer versehen, um das Verhalten zu verdeutlichen.

* &amp;lbrack;Baker&amp;rbrack; Aktualisieren Sie die Baker auf Version 2.5.7.

* &amp;lbrack;USD&amp;rbrack; Importieren und Exportieren von Universal Scene Description-Dateien (USD)

* &amp;lbrack;USD&amp;rbrack; Hinzufügen USD Optionen zum Fenster &quot;Neues Projekt&quot; bei Auswahl einer USD Datei

* &amp;lbrack;USD&amp;rbrack; Neues Auswahlfenster &quot;Umfang und Varianten hinzufügen&quot;

  Wenn Sie eine USD-Datei importieren, können Sie durch Klicken auf die Schaltfläche &quot;Ändern&quot; im Fenster &quot;Neues Projekt&quot; oder &quot;Projektkonfiguration&quot; auswählen, welche Teile und Varianten einer USD-Datei importiert werden sollen.

* &amp;lbrack;USD&amp;rbrack; Option &quot;Unterteilungsebenen hinzufügen

  Beim Erstellen eines neuen Projekts mit einer USD Meshdatei, die Unterteilungen enthält, ist es möglich, die Ebene der Unterteilungen mithilfe eines Schiebereglers auszuwählen. Das Projekt wird mit dem unterteilten Mesh erstellt. Die Ebene kann über die Projektkonfiguration geändert werden.

* &amp;lbrack;USD&amp;rbrack; Importieren USD Meshs mit Skin in bestimmten Rahmen

  Wenn Sie ein neues Projekt mit einer USD Meshdatei erstellen, die eine Animation enthält, können Sie den Rahmen mithilfe eines Schiebereglers auswählen, der die eingebettete Timeline-Sequenz widerspiegelt. Der Rahmen kann über die Projektkonfiguration modifiziert werden.

* &amp;lbrack;USD&amp;rbrack;&amp;lbrack;Export&amp;rbrack; Option zum Exportieren USD Dateien hinzufügen

  Das neue Kontrollkästchen &quot;USD exportieren&quot; wurde dem Fenster &quot;Texturen exportieren&quot; hinzugefügt. Wenn diese Option aktiviert ist, können USD sowie Textur Maps mit einer beliebigen Vorlage exportiert werden.

* &amp;lbrack;USD&amp;rbrack;&amp;lbrack;Export&amp;rbrack; USD Dateiformat zum Mesh-Export hinzufügen

* &amp;lbrack;USD&amp;rbrack; Benennen Sie die vorhandene Exportvorgabe &quot;USD PBR Metal Rauheit&quot; um, um sie genauer zu benennen

  Die USD Exportvorlage, die zuvor als &quot;USD PBR Metal Rauheit&quot; bezeichnet wurde, ist weiterhin über &quot;Texturen exportieren&quot; > &quot;Ausgabevorlage&quot; > &quot;USDz&quot; (Apple AR) verfügbar.

* &amp;lbrack;Automatisch Entpackt&amp;rbrack; &quot;Ausrichtung sperren&quot; für Packing hinzufügen

  Neue Option für Einstellungen für den automatischen entpack, mit der die Ausrichtung bestehender UV-Inseln beibehalten werden kann, wenn die Funktion &quot;Packing&quot; verwendet wird. Der Zugriff darauf erfolgt über &quot;Neues Projekt&quot; > &quot;Optionen für Automatisches Entpacken&quot; > &quot;Ausrichtung der UV-Insel&quot;.

* &amp;lbrack;Physische Größe&amp;rbrack; Hinzufügen einer Einstellung zur automatischen Verwendung von Physische Größe im Fülleffekt/in der Ebene

  Eine neue Option zum automatischen Umschalten auf die Skalierung der Physische Größe wurde hinzugefügt, wenn ein Material mit eingebetteter Physische Größe verwendet wird. Sie kann pro Projekt über Neues Projekt oder über Bearbeiten > Projektkonfiguration > Physische Größe > Füllebene-Skalierung auf Physische Größe umschalten, wenn Materialien zugewiesen werden, aktiviert werden.

* &amp;lbrack;Physische Größe&amp;rbrack; Physische Größe für UV-Projektion gelegt

  Die Skalierung der Physische Größe ist jetzt für UV-Projektionen verfügbar - sie aktiviert die automatische Größenänderung für ein Material basierend auf der Physische Größe eines Meshs. Sie kann über &quot;Skalieren > Physische Größe&quot; im Fenster &quot;Füllebene&quot; oder &quot;Effekteigenschaften&quot; ausgewählt werden.

* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Abfragen der Anwendungsversion zulassen

* &amp;lbrack;Skripterstellung&amp;rbrack;&amp;lbrack;JavaScript&amp;rbrack; API zur Anpassung an neue Baking-Parameter aktualisieren

* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Baking: Bearbeiten der Parameter für das Baking

* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Baking: Baking starten/abbrechen

* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Baking: Methode der selektierten Krümmung

* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Baking: Auswahl von Bakern/UV-Kacheln

* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Baking: Baker-Einstellungen auf allen Textursätzen synchronisieren

* &amp;lbrack;SVT&amp;rbrack; Aktivieren der Unterstützung von geringer Hardware auf AMD-GPUs

  Die Hardwarebeschleunigung für das Dünn besetzte virtuelle Textur-System kann jetzt mit AMD-GPUs aktiviert werden. Diese Einstellung wird in den allgemeinen Voreinstellungen automatisch aktiviert.

* &amp;lbrack;Projektion&amp;rbrack; Parameter für zylindrische Projektion umbenennen

  Der Parameter &quot;Cylinder Cap Culling&quot; wurde in &quot;Rückseiten-Ausblendung&quot; umbenannt, um seine Wirkung besser darzustellen. Die zugehörige QuickInfo wurde entsprechend angepasst.

* &amp;lbrack;Projekt&amp;rbrack; Anwendungsversion im Projekt speichern und über Skripterstellung abrufen

  Seit Version 8.2 wird die Version der Anwendung beim Speichern in der spp-Datei gespeichert. Diese Versionsnummer kann mit der Funktion last_saved_substance_painter_version() im Projektmodul der Python-API abgerufen werden. Für Projekte, die vor 8.2 erstellt wurden, ist der zurückgegebene Wert null.

* &amp;lbrack;Import&amp;rbrack; Verbessern der allgemeinen Importzeit von 3D-Modellen

  Wir haben die allgemeine Importzeit von Meshs verbessert. Zum Beispiel die Verkürzung der Wartezeit beim Laden von High-Poly-Meshs zum Baking. Diese Optimierung gilt insbesondere für das Laden von OBJ.

**Fest:**

* &amp;lbrack;Absturz&amp;rbrack; Ändern von Kanälen bei Filtern mit bestimmtem Stapel

* &amp;lbrack;Mac&amp;rbrack;&amp;lbrack;M1&amp;rbrack; Absturz beim Erstellen einer Füllebene und Verlassen des Ebenenstapels

  Dieses Problem kann durch Aktualisieren auf Mac OS 13 (Ventura) behoben werden.

* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Absturz bei Verwendung von ui.add_dock_widget() mit falschem Typ

* &amp;blbrack;Baking&amp;rbrack; Unvollständige Fehlermeldung im Protokoll, wenn ein Baking fehlschlägt

* &amp;blbrack;Baking&amp;rbrack; Der Speicher wird nach Abschluss des Bakings nicht freigegeben

* &amp;lbrack;Engine&amp;rbrack; Texturen-Cache wird nicht aktualisiert, wenn die Effektsichtbarkeit geändert wird

* &amp;lbrack;Export&amp;rbrack; 2D-Ansicht exportiert zufällig einheitliche Map

* &amp;lbrack;Projekt&amp;rbrack; Speicherzuordnungsfehler beim Speichern eines Projekts mit großem Mesh

* &amp;lbrack;Viewport&amp;rbrack; TAA verursacht beim Malen in einigen Fällen Artefakte

**Bekannte Probleme:**

* &amp;lbrack;Farbmanagement&amp;rbrack; HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen geklemmte Farben
* &amp;lbrack;Ebenenstapel&amp;rbrack; Eingabequelle nicht pro Ebene gespeichert

### 8.2.0

*(Freigegeben: 06. Oktober 2022*)Zusammenfassung: **Hauptversion mit neuen Onboarding-Bedienfeldern (neues Begrüßungs-Bedienfeld und neues Bedienfeld), Export in SBSAR, Effekten für Ordner, mehreren Verbesserungen für die Lebensqualität und Fehlerbehebungen.**

**Hinzugefügt:**

* &amp;lbrack;Onboarding&amp;rbrack; Onboarding-Bereich zur Aufnahme neuer Benutzer

  Es wurde ein neuer Begrüßungsbildschirm hinzugefügt, wenn neue CC-Benutzer Painter zum ersten Mal öffnen.

* &amp;lbrack;Onboarding&amp;rbrack; Fenster &quot;Neue Funktionen&quot; zur Verbesserung der Auffindbarkeit neuer Funktionen

  Es wurde ein neuer Bildschirm &quot;Neue Funktionen&quot; hinzugefügt, auf dem die wichtigsten neuen Funktionen angezeigt werden. Es wird automatisch angezeigt, wenn Painter nach einem wichtigen Update zum ersten Mal geöffnet wird, und Sie können erneut auf es über Hilfe > Neue Funktionen zugreifen.

* &amp;lbrack;Onboarding&amp;rbrack; Alte Willkommensseite in &quot;Startbildschirm&quot; umbenennen

  Alter Begrüßungsbildschirm wurde in Startbildschirm umbenannt, um Verwechslungen mit dem neuen Begrüßungsbildschirm zu vermeiden.

* &amp;lbrack;UI&amp;rbrack; Beheben von Skalierungsproblemen für HD-Bildschirme

  Verbesserte Anpassung der Painter-Benutzeroberfläche auf HD-Bildschirmen mit benutzerdefinierter Anzeigeskalierung.

* &amp;lbrack;UI&amp;rbrack; Vermeiden von dauerhaften Fehlermeldungen in der Benutzeroberfläche

  Fehlermeldungen aus vorherigen Projekten werden jetzt aus der unteren Statusleiste entfernt.

* &amp;lbrack;UI&amp;rbrack; Menü &quot;Speichern&quot; überarbeiten

  Zusätzliche Speicheroptionen sind jetzt in einem Untermenü gruppiert und einige werden aus Konsistenzgründen umbenannt.

* &amp;lbrack;UI&amp;rbrack; Speichern und Exportieren/Freigeben von UI-Layouts

  Im Menü &quot;Fenster&quot; (Window) gibt es neue Aktionen, mit denen Sie das UI-Layout in Dateien speichern und neu laden können. Die Layouts &quot;Malen&quot; und &quot;Rendern&quot; werden separat gespeichert. &quot;substance_painter.ui&quot; wurde um verschiedene Funktionen erweitert, mit denen auch UI-Layouts gespeichert, zurückgesetzt und geladen werden können.

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

* &amp;blbrack;Bedienfeld &quot;Elemente&quot;&amp;blbrack; &quot;Nadel&quot; von bevorzugten Elementen, die oben im Bedienfeld &quot;Elemente&quot; angezeigt werden

  Es wurde eine neue Option zum Klicken mit der rechten Maustaste hinzugefügt, um Elemente zu bibliothekieren, mit der sie oben im Bedienfeld als Favoriten Nadel werden können. Sie können auch alle Ihre bevorzugten Assets über &quot;Gespeicherte Suchen&quot; anzeigen.

* &amp;blbrack;Bedienfeld &quot;Elemente&quot;&amp;blbrack; Elemente löschen, neu laden und umbenennen

  Kontextmenüoptionen zum Löschen, erneuten Laden und Umbenennen von Elementen in der Benutzerbibliothek wurden hinzugefügt. Sie werden direkt aus ihrem Bibliotheksspeicherort auf der Festplatte gelöscht und vom ursprünglichen Speicherort neu geladen. Elemente, die Teil eines Pakets wie .abr oder .sbsar sind, können nicht einzeln bearbeitet werden.

* &amp;lbrack;Farbauswahl&amp;rbrack; Effekt &quot;Füllmethoden für Farbauswahl&quot; definieren.

* &amp;lbrack;Ebenenstapel&amp;rbrack; Füllmethode und Deckkraft auf Filtern anwenden.

* &amp;lbrack;Ebenenstapel&amp;rbrack; Kachelung größer als 128 für Füllebene/Effekte zulassen

* &amp;lbrack;Ebenenstapel&amp;rbrack; Zylinderdeckel für zylindrische Projektion in Füllebene/Wirkung

  Bei der zylindrischen Projektion in den Eigenschaften der Füllebene haben Sie jetzt die Möglichkeit, Zylinderkappen zu entfernen.

* &amp;lbrack;Log&amp;rbrack; Fehlermeldung anzeigen, wenn beim Erstellen eines UV-Kachel-Projekts ein Mesh-Teil im Leerzeichen steht

  Es wurde eine deutlichere Fehlermeldung hinzugefügt, wenn ein UV-Kachel-Projekt nicht erstellt werden kann, da UV-Teile in Leerzeichen gefunden werden.

* &amp;lbrack;Projekt&amp;rbrack; Geben Sie beim Öffnen eines Projekts die Version in der Fehlermeldung &quot;Daten zu aktuell&quot; an.

  Wenn Sie ein Projekt öffnen, das für die Anwendung zu neu ist, wird in der Fehlermeldung jetzt die Version des Projekts angezeigt, damit Sie die richtige Anwendungsversion leichter erkennen können.

* &amp;lbrack;Viewport&amp;rbrack; Mesh von unten beleuchten

  Ein neuer Parameter für die Umgebungsausrichtung wurde unter Anzeigeeinstellungen > Kamera > Umgebungseinstellungen hinzugefügt, um die Umgebungs-Map-Beleuchtung an der Kamera auszurichten, wenn sie auf &quot;Lokal&quot; eingestellt ist.

* &amp;lbrack;Viewport&amp;rbrack; Anzeigen von R, G, B und Alpha im Viewport (Einzelanzeigemodus)

  Unter Anzeigeeinstellungen > Kanaleinstellungen > Kanalanzeige gibt es eine neue Farbkanaleinstellung, mit der nur die R-, G-, B- oder Kanalkomponente eines Viewports im Einzelanzeigemodus angezeigt werden kann.

* &amp;lbrack;Shader&amp;rbrack; Zulassen, dass Benutzerkanäle in Material-Ebenenschattierungen als RGBA festgelegt werden

  Bei der Einstellung der Kanalkonfiguration innerhalb eines Shader für die Kanalschichtung ist es nun möglich, das Textursatz des Materials so festzulegen, dass es vom Standardwert abweicht. Auf diese Weise können Benutzer-Farbkanäle anstelle von Graustufen angefordert werden.

* &amp;lbrack;Export&amp;rbrack; Exportieren von Texturen als SBSAR zulassen

  Beim Exportieren von Texturen über das Fenster Datei > Texturen exportieren kann das Dateiformat SBSAR (Substance Archive) ausgewählt werden, um sie neu zu gruppieren. Der Inhalt des SBSAR richtet sich nach der verwendeten Ausgabevorlage. Das Datenformat kann auch in den Exportvorgaben festgelegt werden. Bei Verwendung einer Hybridkonfiguration (SBSAR + Anderes Format) werden Texturen, die ein SBSAR betreffen, gruppiert, während der Rest parallel exportiert wird.

* &amp;lbrack;Export&amp;rbrack; 16-Bit-Option für EXR Dateiformat gelegt

  Beim Exportieren EXR Textur-Dateien können Sie jetzt im Fenster &quot;Exporteinstellungen&quot; die Texturen 16f Bit (halbe Fließkommazahl) oder 32f Bit (Fließkommazahl) auswählen (sowohl für Exporteinstellungen als auch Exportvorgaben). Alte Projekte und alte Exportvorgaben werden standardmäßig auf 16f Bit gesetzt, um das alte Verhalten widerzuspiegeln.

* &amp;lbrack;Python&amp;rbrack; Ereignis hinzufügen, um zu erfahren, wann Textursatz geändert werden

  Mit dem neuen &quot;substance_painter.event.TextureStateEvent&quot; kann ermittelt werden, ob ein Textursatz entweder aufgrund eines Malen-Strichs, eines hinzugefügten oder eines entfernten Kanals geändert wurde.

* &amp;lbrack;Python&amp;rbrack; Mesh-Map-Ressourcen in den Textursatz-Einstellungen abrufen und festlegen

  Neue Funktionen wurden im Modul &quot;substance_painter.project&quot; hinzugefügt, um Mesh-Map-Ressourcen abzurufen und einzurichten. Diese Funktionen können verwendet werden, um die Mesh-Map zu aktualisieren, auf die in den Textursatz-Einstellungen verwiesen wird.

* &amp;lbrack;Plugins&amp;rbrack; Option zum Abrufen anderer JS-Plug-ins entfernen

  Die Option, JavaScript-Plug-ins abzurufen, wurde entfernt, da sie auf der veralteten Freigabe-Website gehostet wurden.

* &amp;lbrack;Inhalt&amp;rbrack; Neue Roblox-Vorlage hinzufügen und Vorgabe exportieren

  Eine neue Roblox-Projektvorlage &quot;Material Variant&quot; und &quot;Surface Appearance&quot; sowie eine Exportvorgabe wurden hinzugefügt, um den Export von PBR-Texturen nach Roblox zu erleichtern. Auf die Vorlage kann über das Fenster Datei > Neues Projekt zugegriffen werden.

* Substance Engine auf die neueste Version (8.6.3) aktualisieren

* &amp;lbrack;Steam&amp;rbrack; Optimierter Build für Apple Silicon-Chipsatz (Apple M1/M2)

**Fest:**

* Absturz bei Verwendung von 16k exr

* &amp;lbrack;Absturz&amp;rbrack; Strg+Z Nach dem Löschen einer Shader-Instanz

* &amp;lbrack;Iray&amp;rbrack; IoR ist bei einigen Shadern auf 1 blockiert

* &amp;lbrack;Win&amp;rbrack;&amp;lbrack;Baking&amp;rbrack; Einige High-Poly können nicht geladen werden

* &amp;lbrack;Farbmanagement&amp;rbrack; Falscher Farbraumname in der Benutzeroberfläche mit Filtern

* &amp;lbrack;Python&amp;rbrack; Von der Importfunktion zurückgegebene Ressourcenobjekte haben keinen Typ

  Beim Importieren eines Substance-Pakets in Python gab die Funktion das Paket anstelle der Graf zurück. Das Ressourcenmodul stellt nun Funktionen und Parameter bereit, um die Graf eines Substance-Pakets abzurufen.

**Bekannte Probleme:**

* &amp;lbrack;Farbmanagement&amp;rbrack; HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen geklemmte Farben
* &amp;lbrack;Ebenenstapel&amp;rbrack; Eingabequelle nicht pro Ebene gespeichert
* &amp;lbrack;Malen&amp;rbrack; Zeitweiliges Anti-Aliasing verursacht beim Malen in einigen Fällen Artefakte
* &amp;lbrack;Export&amp;rbrack; 2D-Ansicht exportiert zufällig einheitliche Map

### 8.1.3

*(Freigegeben: 25. August 2022*)Zusammenfassung: **Geringfügige Fehlerbehebungsversion**

**Hinzugefügt:**

* Update auf Iray SDK 1.6

**Fest:**

* &amp;lbrack;Shader&amp;rbrack; Absturz mit altem fehlerhaftem Shader
* &amp;blbrack;Material-Ebenen&amp;blbrack; Material können beim erneuten Öffnen eines Projekts verschwinden

**Bekannte Probleme:**

* &amp;lbrack;Farbmanagement&amp;rbrack; HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen geklemmte Farben
* &amp;lbrack;Ebenenstapel&amp;rbrack; Eingabequelle nicht pro Ebene gespeichert
* &amp;lbrack;Absturz&amp;rbrack; Strg+Z Nach dem Löschen einer Shader-Instanz
* &amp;lbrack;Iray&amp;rbrack; IoR ist bei einigen Shadern auf 1 blockiert

### 8.1.2

*(Freigegeben: 19. Juli 2022*)Zusammenfassung: **Geringfügige Fehlerbehebungsversion**

**Hinzugefügt:**

* &amp;lbrack;Automatisch Entpackt&amp;rbrack; Neue Option &quot;Für organische Mesh optimieren&quot; zur Auswahl des Segmentierungsalgorithmus
* &amp;lbrack;Physische Größe&amp;rbrack; Einheitenoptionen in &quot;Neues Projekt&quot; und &quot;Projektkonfiguration&quot; gelegt
* &amp;lbrack;Farbmanagement&amp;rbrack; Verwenden Sie die Monitoranzeige standardmäßig, wenn Sie ACE verwenden
* &amp;lbrack;Farbmanagement&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Berücksichtigung ACE env-var-Vorgabedatei beim Erstellen eines Projekts
* &amp;lbrack;Farbmanagement&amp;rbrack; Zurücksetzen der Farbmanagement-Einstellungen im Fenster &quot;Neues Projekt&quot;, wenn sich die Konfiguration ändert
* &amp;lbrack;Farbmanagement&amp;rbrack; Zugriff auf OCIO deaktivieren, wenn env-var vorhanden ist
* &amp;lbrack;Farbmanagement&amp;rbrack; Sicheres Aktualisieren ACE Einstellungen, wenn kein Parameter mehr vorhanden ist
* Substance Engine auf Version 8.6.0 aktualisieren
* &amp;lbrack;Export&amp;rbrack; Neue GLTF-Exportvorgabe mit Versatz-Unterstützung hinzufügen
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Abrufen von Ressourceninformationen (einschließlich benutzerdefinierter Metadaten)
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Funktion zur Abfrageliste der Mesh-Namen pro Textursatz hinzufügen
* &amp;lbrack;Inhalt&amp;rbrack; Neue Misch- und Exportvorgabe hinzufügen

**Fest:**

* &amp;lbrack;MacOS&amp;rbrack; Absturz beim Starten von Iray in einigen Fällen
* &amp;Klammer;Miniaturen&amp;Klammer; Regal-Miniaturansichten werden nicht richtig geladen
* Mehrere UV-Kanäle werden ignoriert.
* &amp;lbrack;Automatisch Entpackt&amp;rbrack; Unnötige Berechnung bei der Teilung langer Inseln
* &amp;lbrack;Automatisch Entpackt&amp;rbrack; Option zur Vermeidung länglicher Inseln, die nicht berücksichtigt werden
* &amp;lbrack;Automatisch Entpackt&amp;rbrack; Verlust zusätzlicher Daten (Scheitelpunkt-Farben) beim Umpacken von UVs
* &amp;lbrack;UI&amp;rbrack; Horizontale Bildlaufleiste im Eigenschaftenfenster, wenn Farbmanagement aktiviert ist
* &amp;lbrack;Farbmanagement&amp;rbrack; OCIO Konfigurationen fehlen substance_3d_painter_standard_srgb
* &amp;lbrack;Generator&amp;rbrack; Falsche Verwendung von Benutzerdaten &quot;deaktiviert&quot;
* &amp;lbrack;Farbmanagement&amp;rbrack; Die Dropdown-Liste &quot;Nicht kompatibel&quot; im Farbraum sollte nicht anklickbar sein.
* &amp;lbrack;Farbmanagement&amp;rbrack;&amp;lbrack;Shader&amp;rbrack; sRGB override define funktioniert nicht mehr
* &amp;lbrack;Generator&amp;rbrack; Falsche Verwendung von Benutzerdaten &quot;deaktivieren&quot;
* &amp;lbrack;Ebenenstapel&amp;rbrack; Fehlerhafte Vorschauen bei UV-Kacheln-Projekten
* &amp;lbrack;Shader&amp;rbrack; Die API-Dokumentation ist mit den Bent normals nicht vollständig auf dem neuesten Stand.
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;Interoperabilität&amp;rbrack; Kann nicht mit Sonderzeichen an Stager gesendet werden
* &amp;lbrack;Inhalt&amp;rbrack; Einige Miniaturansichten von Pinselvorgaben sind leer oder zu dunkel

**Bekannte Probleme:**

* &amp;lbrack;Farbmanagement&amp;rbrack; HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen geklemmte Farben
* &amp;lbrack;Ebenenstapel&amp;rbrack; Eingabequellen werden nicht pro Ebene gespeichert
* &amp;lbrack;Absturz&amp;rbrack; Strg+Z Nach dem Löschen einer Shader-Instanz
* &amp;lbrack;Iray&amp;rbrack; IoR ist bei einigen Shadern auf 1 blockiert
* &amp;lbrack;Shader&amp;rbrack; Absturz mit altem fehlerhaftem Shader

### 8.1.1

*(Freigegeben: 28. Juni 2022*)Zusammenfassung: **Hotfix für Nebenversion**

**Hinzugefügt:**

* &amp;lbrack;Ebenenstapel&amp;rbrack; Alt-Klick auf Maske hebt Auswahl von Effekten nicht mehr auf

**Fest:**

* &amp;lbrack;Absturz&amp;rbrack; Öffnen von im Einzelansichtsmodus gespeicherten alten Projekten
* &amp;lbrack;Absturz&amp;rbrack; Generator in Eigenschaften löschen
* &amp;blbrack;Textursatz-Einstellungen&amp;rbrack; Normale/Ambient occlusion-Mischung und Height-zu-Normal-Methoden sind nicht mehr funktionsfähig
* &amp;lbrack;Export&amp;rbrack; Texturen mit Innenabständen exportieren macht schwarze Diffusionen.

**Bekannte Probleme:**

* &amp;lbrack;MacOS&amp;rbrack; Absturz beim Starten von Iray auf Monterey
* &amp;blbrack;Vorschau-Miniatur&amp;blbrack; Vereinfachte Miniaturen werden nicht aktualisiert, wenn ein Anker verwendet wird
* &amp;lbrack;Farbmanagement&amp;rbrack; HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen geklemmte Farben

### 8.1.0

*(Freigegeben: 07. Juni 2022*)Zusammenfassung: **Hauptversion mit ICC-Unterstützung, Material-Skalierung auf der Grundlage von Physische Größe-Daten, neue Baker, Verbesserungen an der FarbPipette und eine Reihe zusätzlicher Inhalte**

**Hinzugefügt:**

* &amp;lbrack;Farbmanagement&amp;rbrack; Unterstützung für ICC-Profile mit Adobe Color Engine hinzufügen (ACE)
* &amp;lbrack;Farbmanagement&amp;rbrack; Unterstützung für &quot;Adobe 98 RGB&quot; als Arbeitsfarbraum für ICC hinzufügen
* &amp;lbrack;Farbmanagement&amp;rbrack; Konfigurieren von ACE/ICC-Einstellungen über eine Konfigurationsdatei zulassen
* &amp;lbrack;Farbmanagement&amp;rbrack; Zulassen, dass lineare Farbwerte im Farbwähler mit dem Legacy-Modus eingegeben werden
* &amp;lbrack;Farbmanagement&amp;rbrack; Festlegen des Farbprofils für die Farbauswahl außerhalb der Benutzeroberfläche zulassen
* &amp;lbrack;Farbmanagement&amp;rbrack; Erinnern Sie sich an den letzten im Viewport ausgewählten Anzeigewert
* &amp;lbrack;Farbmanagement&amp;rbrack;&amp;lbrack;Substance&amp;rbrack; Generatoren/Filter mit dem Farb-Management für die einwandfreie Funktion sorgen
* &amp;lbrack;Farbmanagement&amp;rbrack;&amp;lbrack;Substance&amp;rbrack; Neue Schlüsselwörter für die Farbraumüberschreibung hinzufügen $working und $standardsrgb
* &amp;lbrack;Physische Größe&amp;rbrack;&amp;lbrack;Engine&amp;rbrack; Informationen zur Physische Größe aus dem Mesh extrahieren
* &amp;lbrack;Physische Größe&amp;rbrack;&amp;lbrack;Engine&amp;rbrack; Physische Größe Berechnung
* &amp;lbrack;Physische Größe&amp;rbrack; Leg von Optionen für die Verwendung von Physische Größe in der Benutzeroberfläche
* &amp;lbrack;Physische Größe&amp;rbrack; Visuelle Helfer zum Viewport hinzufügen
* &amp;blbrack;Baking&amp;rbrack; Height-Baker hinzufügen
* &amp;blbrack;Baking&amp;rbrack; Bent normals-Baker hinzufügen
* &amp;blbrack;Baking&amp;rbrack; Deckkraft-Baker hinzufügen
* &amp;lbrack;Pipette&amp;rbrack; Neue Farbvorschau mit Pipette neben der Maus und Farb-Management
* &amp;lbrack;Pipette&amp;rbrack; Das Bedienfeld &quot;Farbwähler&quot; wird wieder an der letzten Position angezeigt, wenn es erneut geöffnet wird
* &amp;lbrack;Pipette&amp;rbrack; Ein neues Symbol für die Material-Auswahl
* &amp;lbrack;Pipette&amp;rbrack; Farb-Management der Kanalvorschau des Farbwählers
* &amp;lbrack;Pipette&amp;rbrack; Hinzufügen von Click-to-Select-Funktionen zur Pipette
* &amp;lbrack;Pipette&amp;rbrack; Kanalauswahl aktiviert nicht aktive Materialien nicht mehr
* &amp;lbrack;Pipette&amp;rbrack; Pipette mit einem Tastaturbefehl verwenden
* &amp;lbrack;Pipette&amp;rbrack; Die Pipette nimmt ggf. den entsprechenden Kanal auf.
* &amp;lbrack;Pipette&amp;rbrack; Wenn Sie den Farbwählermodus aufrufen, werden alle Tastaturbefehle deaktiviert
* &amp;lbrack;Pipette&amp;rbrack; Entfernen der automatischen Auswahl des Hexadezimalfelds
* &amp;lbrack;Pipette&amp;rbrack; Schließen Sie das Bedienfeld nicht, wenn Sie die Material-Auswahl verwenden
* &amp;lbrack;Pipette&amp;rbrack; Neuer deaktivierter Status, wenn der Kanal nicht zur Auswahl verfügbar ist
* &amp;lbrack;Export&amp;rbrack; Tangente-Attribut zum glTF-Export hinzufügen
* Substance Engine auf Version 8.4 aktualisieren
* Update Auto Entpack auf 0.9.0
* Update auf Qt 5.15.8
* Update auf Python 3.9
* &amp;lbrack;Shader&amp;rbrack; Unterstützung für Bent normals-Schattierung hinzufügen
* &amp;lbrack;MacOS&amp;rbrack; Unterstützung von 3DConnection SpaceMouse
* &amp;lbrack;Python&amp;rbrack; Dokumentieren der in der API verwendeten Python-Version
* &amp;lbrack;Inhalt&amp;rbrack; 6 neue 3D-Rauschen mit 105 Vorgaben hinzufügen
* &amp;lbrack;Inhalt&amp;rbrack; 20 neue Schmutz-Maps und 2 Stofffaltenmuster
* &amp;lbrack;Inhalt&amp;rbrack; Exportvoreinstellung &quot;Mesh-Map&quot; aktualisieren, um neue Baker zu verwenden
* &amp;lbrack;Inhalt&amp;rbrack; Die Steigung des Weichzeichners und der Verkrümmungsfilter hängen von der Auflösung des Textursatzes ab
* &amp;lbrack;Inhalt&amp;rbrack; Beispielprojekte aktualisieren, um die 3 neuen Baker zu verwenden

**Fest:**

* &amp;lbrack;glTF&amp;rbrack; glTF mit Sonderzeichen kann nicht geöffnet werden
* &amp;lbrack;Engine&amp;rbrack; Artefakte mit deaktivierter Anisotropie und SVT
* &amp;lbrack;MacOS&amp;rbrack;&amp;lbrack;M1&amp;rbrack; Intelligente Material werden nicht korrekt angezeigt
* &amp;lbrack;Mesh-Verarbeitung&amp;rbrack; Mesh können nicht aus Modeler importiert werden
* &amp;lbrack;UI&amp;rbrack; Horizontale Bildlaufleiste in neuem Projektfenster mit aktiviertem Farbmanagement
* &amp;lbrack;Farbmanagement&amp;rbrack; Im Farbwähler fehlt bei einigen OCIO der Arbeitsfarbraumwert
* &amp;lbrack;Farbmanagement&amp;rbrack; Die Pinselvorschau im Viewport ist nicht farbverwaltet
* &amp;lbrack;SpaceMouse&amp;rbrack; Pivot wird nicht sofort mit Fokusänderung aktualisiert und manchmal außerhalb des Modells
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;USD&amp;rbrack; Exportierte USD haben eine falsche Struktur
* &amp;lbrack;USD&amp;rbrack; Ambient occlusion-Problem beim Exportieren
* &amp;lbrack;Inhalt&amp;rbrack; Mesh der Miniaturansicht an das Vorschaukugel-Beispielprojekt anpassen

**Bekannte Probleme:**

* Texturen mit Innenabständen exportieren macht schwarze Diffusionen.
* Normale/Ambient occlusion-Mischung ist defekt
* &amp;lbrack;MacOS&amp;rbrack; Absturz beim Starten von Iray in seltenen Fällen
* &amp;blbrack;Vorschau-Miniatur&amp;blbrack; Vereinfachte Miniaturen werden nicht aktualisiert, wenn ein Anker verwendet wird
* &amp;lbrack;Farbmanagement&amp;rbrack; HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen geklemmte Farben

## Version 7

### 7.4.3

*(Freigegeben: 11. April 2022*)Zusammenfassung: **Bugfix mit Unterstützung von 3D-Verbindung SpaceMouse im 2D-Viewport**

**Hinzugefügt:**

* &amp;lbrack;SpaceMouse&amp;rbrack; Unterstützung von 3DConnection SpaceMouse im 2D-Viewport

**Fest:**

* &amp;Klammer;Farbwähler&amp;Klammer; Schreibzugriff im Hexadezimalfeld nicht möglich
* &amp;lbrack;Farbmanagement&amp;rbrack; Im Projektion-Modus verwendete Ressourcen werden in der Überlagerung nicht farbverwaltet
* &amp;lbrack;Farbmanagement&amp;rbrack; Fehler werden nicht im Protokoll gemeldet.
* &amp;lbrack;SpaceMouse&amp;rbrack; Generische Fehlermeldung entfernen, wenn der Benutzer keine SpaceMouse hat
* &amp;lbrack;SpaceMouse&amp;rbrack; Beim Laden eines Projekts ist der Drehpunkt immer ausgeblendet
* &amp;lbrack;Baker&amp;rbrack; Die Einstellung &quot;Durchschnittliche Normale&quot; hat keine Auswirkungen auf UV-Kachel-Projekte
* &amp;lbrack;UV-Kachel&amp;rbrack; Inaktive Überlagerungen von UV-Kacheln verschwinden beim erneuten Laden von Mesh mit verschiedenen Kacheln
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Remote-Skripterstellung ist fehlerhaft
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Mehrere Kanäle können nicht von der API abgefragt werden und es löst einen Fehler aus
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Absturz bei der Verwendung des ProjectEditionEntered-Ereignisses
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Absturz beim Aufruf von get_active_Stapel()

**Bekannte Probleme:**

* 3D-Verbindung SpaceMouse wird auf MacOS nicht unterstützt
* &amp;lbrack;UI&amp;rbrack; Horizontale Bildlaufleiste mit Farbmanagement, die in einigen Fällen in einem neuen Projektfenster angezeigt wird
* &amp;lbrack;Mac M1&amp;rbrack; Intelligente Material werden nicht korrekt angezeigt

### 7.4.2

*(Freigegeben: 08. März 2022*)Zusammenfassung: **Bugfix mit Unterstützung von Verbesserungen für 3D-Verbindung, SpaceMouse und Farbmanagement (OCIO)**

**Hinzugefügt:**

* &amp;lbrack;SpaceMouse&amp;rbrack;&amp;lbrack;Windows&amp;rbrack; Unterstützung der 3D-Verbindung SpaceMouse im 3D-Viewport für die Navigation
* &amp;lbrack;SpaceMouse&amp;rbrack;&amp;lbrack;Windows&amp;rbrack; Grundlegende Tastaturbefehle/Tasten für Pro- und Enterprise SpaceMouse-Modelle im 3D-Viewport
* &amp;lbrack;SpaceMouse&amp;rbrack;&amp;lbrack;Windows&amp;rbrack; Dediziertes Drehmittensymbol im 3D-Viewport
* &amp;lbrack;Farbmanagement&amp;rbrack; Rollen aus OCIO Konfiguration verwenden, um Standardeinstellungen zu ändern
* &amp;lbrack;Farbmanagement&amp;rbrack; Farb-Management des Eigenschaftenfensters für Farb-Widgets
* &amp;lbrack;Farbmanagement&amp;rbrack; Farb-Management des Eigenschaftenfensters für die Vorschau des Materials
* &amp;lbrack;Farbmanagement&amp;rbrack; Farbfelder in der Farbauswahl verwalten
* &amp;lbrack;Farbmanagement&amp;rbrack; Fügen Sie eine Einstellung hinzu, um den standardmäßigen sRGB-Farbraum zu definieren
* &amp;lbrack;Farbmanagement&amp;rbrack; Hinzufügen des sRGB-Standardfarbraums aus OCIO Konfiguration in der Farbwähler-Anzeigeliste
* &amp;lbrack;Farbmanagement&amp;rbrack; Verbesserungen für das Menü zum Überschreiben des Farbraums
* &amp;lbrack;Farbmanagement&amp;rbrack; Überschreiben des Umgebungs-Map-Farbraums in den Anzeigeeinstellungen zulassen
* &amp;lbrack;Farbmanagement&amp;rbrack; Farbwähler-Verläufe basierend auf aktueller Anzeige zeichnen
* &amp;lbrack;Farbmanagement&amp;rbrack; Standardmäßig HDR im Farbeditor beschränkt
* &amp;lbrack;Farbmanagement&amp;rbrack; Passthrough (keinen Farbraum) für Filter im Legacy-Modus verwenden
* &amp;lbrack;Farbmanagement&amp;rbrack; Anzeige von Farbverläufen im Farbeditor auf &amp;lbrack;0-1&amp;rbrack; beschränken Spanne
* &amp;lbrack;Farbmanagement&amp;rbrack; Anzeigeselektor in der Farbauswahl im Legacy-Modus ausblenden
* &amp;lbrack;Farbmanagement&amp;rbrack; Hex-Code für Farbwähler immer im sRGB-Farbraum
* &amp;lbrack;Farbmanagement&amp;rbrack; Deaktivieren der Farbauswahl-Dropdown-Liste für Datenkanäle
* &amp;lbrack;Optimierung&amp;rbrack; Mit &quot;Verkrümmen-Raster&quot; werden nur überdeckte UV-Kacheln neu berechnet
* &amp;lbrack;Export&amp;rbrack; Exportieren von UV-Kachel-Projekten für Sketchfab, USD und glTF zulassen
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Ändern der Tonzuordnungsfunktion zulassen

**Fest:**

* &amp;lbrack;Sketchfab&amp;rbrack; Durch die Aktualisierung des vorhandenen Modells wird am Ende ein neues Modell erstellt.
* &amp;lbrack;Sketchfab&amp;rbrack; Absturz bei der Suche nach einem zuvor aktualisierten Modell
* Absturz beim Exportieren nach USD
* Absturz beim Erstellen einer neuen Shader-Instanz in der Geometriemaske oder beim Ausblenden der Geometrie
* &amp;lbrack;Elementfenster importieren&amp;rbrack; Absturz beim Ändern des Typs von importierten Ressourcen
* Normale Mesh-Map werden bei Verwendung in Ebenenstapel invertiert
* &amp;lbrack;Substance&amp;rbrack; Der Mischmodus für Benutzerdaten wird nicht berücksichtigt.
* &amp;lbrack;Farbmanagement&amp;rbrack; Bitmaps mit einem Farbraum im Dateinamen werden als UV-Kachel importiert
* &amp;lbrack;Farbmanagement&amp;rbrack; Farbverwaltete Ausgaben von Substance Graf befinden sich im falschen Farbraum
* &amp;lbrack;Farbmanagement&amp;rbrack; Falsche Farbe mit dem Polygon-Füllwerkzeug
* &amp;lbrack;Farbmanagement&amp;rbrack; ACE Tonemapper wird im Solomodus auf Kanäle angewendet
* &amp;lbrack;Farbmanagement&amp;rbrack; Die Kugelbeleuchtung der Werkzeugvorschau ist nicht farbverwaltet
* &amp;lbrack;Farbmanagement&amp;rbrack;&amp;lbrack;Export&amp;rbrack; Konvertierte Karten werden falsch konvertiert.
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack;&amp;lbrack;Farbmanagement&amp;rbrack; Projekte, die mit einer Vorlage und OCIO Umgebungsvariablen erstellt wurden, befinden sich im Modus &quot;Veraltet&quot;
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Die JavaScript-Evaluierungsfunktion kann beim Start nicht verwendet werden.
* &amp;lbrack;3D Adobe Offer&amp;rbrack; Painter kann nicht gestartet werden, wenn Regionaleinstellungen mit Sprachen verwendet werden, die nicht standardmäßig unterstützt werden

**Bekannte Probleme:**

* 3D-Verbindung SpaceMouse wird auf MacOS nicht unterstützt
* &amp;lbrack;UI&amp;rbrack; Horizontale Bildlaufleiste mit Farbmanagement, die in einigen Fällen in einem neuen Projektfenster angezeigt wird
* &amp;lbrack;Baker&amp;rbrack; Die Einstellung &quot;Durchschnittliche Normale&quot; hat keine Auswirkungen auf UV-Kachel-Projekte
* &amp;lbrack;Mac M1&amp;rbrack; Intelligente Material werden nicht korrekt angezeigt
* &amp;lbrack;Farbmanagement&amp;rbrack; Im Projektion-Modus verwendete Ressourcen werden in der Überlagerung nicht farbverwaltet
* &amp;Klammer;Farbwähler&amp;Klammer; Schreibzugriff im Hexadezimalfeld nicht möglich

### 7.4.1

*(Freigegeben: 14. Dezember 2021*)Zusammenfassung: **Bugfix mit Farbmanagement-Verbesserungen**

**Hinzugefügt:**

* &amp;lbrack;Farbmanagement&amp;rbrack; Verwenden der Datenrolle in exportierten Dateinamen
* &amp;lbrack;Farbmanagement&amp;rbrack; Erweitern Sie den Abschnitt Farbmanagement standardmäßig, wenn OCIO in den Fenstern für neue Projekt- und Projekteinstellungen ausgewählt ist.
* &amp;lbrack;Farbmanagement&amp;rbrack; ACE Tongemapper im Legacy-Modus hinzufügen
* &amp;lbrack;Farbmanagement&amp;rbrack; Standardkonfigurationseinstellungen anpassen
* &amp;lbrack;Farbmanagement&amp;rbrack;&amp;lbrack;Export&amp;rbrack; $colorSpace in Dateinamen für Datenkanäle füllen
* &amp;lbrack;Export&amp;rbrack; UV-Kachel-Projekt in Stager exportieren
* &amp;lbrack;Interoperabilität&amp;rbrack; Nicht verfügbar für Steam- und Substance-Editionen
* &amp;lbrack;Interoperabilität&amp;rbrack; Senden eines UV-Kachel-Projekts an Stager zulassen

**Fest:**

* &amp;lbrack;MacOS&amp;rbrack;&amp;lbrack;Absturz&amp;rbrack; Painter beginnt nicht mit Catalina
* &amp;lbrack;Farbmanagement&amp;rbrack;&amp;lbrack;Absturz&amp;rbrack; Zufälliger Absturz bei der Wiedergabe mit Datentyp/Farbmanagement auf Benutzerkanal
* &amp;lbrack;Farbmanagement&amp;rbrack; Ressourcen, die als Graustufen in der Maskenanzeige verwendet werden, zeigen das neue Menü den Farbraum an
* &amp;lbrack;Farbmanagement&amp;rbrack; Benutzerkanal ist im Viewport im Legacy-Modus + Solo-Ansicht dunkler
* &amp;lbrack;Farbmanagement&amp;rbrack; Env-Map ist immer linear, wenn sie in iRay verwendet wird
* &amp;lbrack;Farbmanagement&amp;rbrack; Die Farbauswahl wählt im Legacy-Modus nicht den richtigen Wert für den Datenkanal aus
* &amp;lbrack;Farbmanagement&amp;rbrack; Farbwähler in einer Substance im Legacy-Modus funktioniert nicht
* &amp;lbrack;Farbmanagement&amp;rbrack; Wenn Sie im Viewport zwischen den Einzelkanalansichten wechseln, wird bei Verwendung des Dropdown-Menüs der richtige Farbraum angezeigt
* &amp;lbrack;Farbmanagement&amp;rbrack; Beim Export wird die falsche Konvertierung auf farbverwalteten Benutzerkanälen im Legacy-Modus angewendet.
* In der Einzelansichtsmaske erstellte Konturen werden beim Zurückwechseln zur Material-Ansicht nicht angezeigt
* &amp;lbrack;Export&amp;rbrack; Konvertierte Maps werden nicht als farbverwaltete Kanäle exportiert
* &amp;lbrack;Textursatz&amp;rbrack; QuickInfo mit dem ursprünglichen Namen fehlt auf umbenannten Benutzerkanälen
* &amp;lbrack;Steam&amp;rbrack; Dateien fehlen beim Überprüfen der Dateiintegrität mit Steam

**Bekannte Probleme:**

* &amp;lbrack;Mac M1&amp;rbrack; Intelligente Material werden nicht korrekt angezeigt

### 7.4.0

*(Freigegeben: 24. November 2021*)Zusammenfassung: **Hauptversion. Einführung der ersten Farbmanagement-Version, Abdocken der 2D- oder 3D-Ansicht, neue Option für den automatischen entpack von UV zum Vermeiden von länglichen Inseln, Aufruf von JavaScript-Funktionen von der Python-API und neuer Inhalt**

**Hinzugefügt:**

* &amp;lbrack;Farbmanagement&amp;rbrack; Unterstützung des Farbmanagements OpenColorIO Version 2
* &amp;lbrack;Farbmanagement&amp;rbrack; Hinzufügen von Farbmanagementeinstellungen zu Projekteinstellungen
* &amp;lbrack;Farbmanagement&amp;rbrack; Warnfenster zu Farbmanagement-Konfigurationsänderungen beim Öffnen eines Projekts
* &amp;lbrack;Farbmanagement&amp;rbrack; Fehlermeldung anzeigen, wenn eine ungültige OCIO Konfigurationsdatei ausgewählt ist
* &amp;lbrack;Farbmanagement&amp;rbrack; Überschreiben der Konfiguration mit OCIO Umgebungsvariable zulassen
* &amp;lbrack;Farbmanagement&amp;rbrack; Mehrere OCIO sind standardmäßig in die Anwendung integriert.
* &amp;lbrack;Farbmanagement&amp;rbrack; Extrahieren des Farbraumnamens aus dem importierten Bitmap-Dateinamen
* &amp;lbrack;Farbmanagement&amp;rbrack; Überschreiben des Farbraums mit einem Farbraum aus der Konfiguration im Eigenschaftenfenster zulassen
* &amp;lbrack;Farbmanagement&amp;rbrack; Hinzufügen von Farbmanagementoptionen in den Textursatz-Einstellungen
* &amp;lbrack;Farbmanagement&amp;rbrack;&amp;lbrack;Viewport&amp;rbrack; Erlaubt das separate Farbmanagement für 2D- und 3D-Ansichten.
* &amp;lbrack;Farbmanagement&amp;rbrack; Umgebungs-Map laden und in den Arbeitsfarbraum konvertieren
* &amp;lbrack;Farbmanagement&amp;rbrack; Anpassen des Farbwählers und des Editors mit dem aktuellen Farbraum
* &amp;lbrack;Farbmanagement&amp;rbrack; Auswahl des transformieren Farbraums für die Anzeige im Viewport über ein neues Dropdown-Menü zulassen
* &amp;lbrack;Farbmanagement&amp;rbrack; Anzeige mit Iray-Rendering-Ergebnissen transformieren anwenden
* &amp;lbrack;Farbmanagement&amp;rbrack; Exportieren von Texturen mit unterschiedlichen Farbräumen
* &amp;lbrack;Farbmanagement&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Anwenden von Farbmanagementeinstellungen aus der Umgebungsvariablen (OCIO) auf neue Projekte
* &amp;lbrack;Viewport&amp;rbrack; Abdocken des 2D- oder 3D-Viewports zulassen
* &amp;lbrack;Automatisch Entpackt&amp;rbrack; Neue Option zur Vermeidung länglicher Inseln
* &amp;lbrack;Skripterstellung Python&amp;rbrack; Aufrufen von JavaScript-Funktionen über die Python-API
* &amp;lbrack;Neues Projektfenster&amp;rbrack; Reduzieren des Abschnitts &quot;Importierte Karten&quot;
* &amp;lbrack;Projektion&amp;rbrack;&amp;lbrack;Verkrümmen&amp;rbrack; Option zum Ausblenden von Normalen in den Verkrümmen-Einstellungen
* &amp;lbrack;Inhalt&amp;rbrack; 11 neue Schmutz Maps
* &amp;lbrack;Inhalt&amp;rbrack; 8 neue Werkzeugvorgaben (Reißverschluss, Spannschnur, Glitter)
* &amp;lbrack;Inhalt&amp;rbrack; 8 neue Materialien (Narbe, Hosentasche, ...)
* &amp;lbrack;Inhalt&amp;rbrack; 1 neuer Generator (aufblasen Schrumpfwarp)

**Bekannte Probleme:**

* &amp;lbrack;Mac M1&amp;rbrack; Intelligente Material werden nicht korrekt angezeigt
* &amp;lbrack;Farbmanagement&amp;rbrack;&amp;lbrack;Absturz&amp;rbrack; Zufälliger Absturz bei der Wiedergabe mit Datentyp/Farbmanagement auf Benutzerkanal
* &amp;lbrack;Farbmanagement&amp;rbrack; Die Farbauswahl wählt im Legacy-Modus nicht den richtigen Wert für den Datenkanal aus
* &amp;lbrack;Farbmanagement&amp;rbrack;&amp;lbrack;Iray&amp;rbrack; Speichern des Renderings auf EXR oder TIFF, während das Farbmanagement im Viewport aktiviert ist, wird immer linear gespeichert
* &amp;lbrack;Farbmanagement&amp;rbrack; Ressourcen, die als Graustufen in einer Maske verwendet werden, zeigen das falsche Menü &quot;Farbraum&quot; an
* &amp;lbrack;Farbmanagement&amp;rbrack;&amp;lbrack;Iray&amp;rbrack; Env-Map ist immer linear, wenn sie in Iray verwendet wird
* &amp;lbrack;Farbmanagement&amp;rbrack;&amp;lbrack;Export&amp;rbrack; Konvertierte Karten werden nicht als Farbmanagement-Kanäle exportiert
* &amp;lbrack;Farbmanagement&amp;rbrack;&amp;lbrack;Export&amp;rbrack; Der Export ignoriert, wenn der Benutzerkanal farbverwaltet ist oder nicht im Legacy-Modus ausgeführt wird

### 7.3.1

*(Freigegeben: 24. November 2021*)Zusammenfassung: **Bugfix**

**Hinzugefügt:**

* &amp;lbrack;Projektion&amp;rbrack; Skalierung sollte nur im Objektbereich funktionieren

**Fest:**

* &amp;lbrack;Mac M1&amp;rbrack; Material-Ebene funktioniert nicht
* &amp;lbrack;Mac M1&amp;rbrack;&amp;lbrack;Projektion&amp;rbrack; Verkrümmen funktioniert nicht
* Micro-Details werden nicht richtig angezeigt
* &amp;lbrack;Projektion&amp;rbrack;&amp;lbrack;Absturz&amp;rbrack; Wechseln in den Verzerrungsmodus mit einer Ebene, die mit einer früheren Version erstellt wurde
* &amp;lbrack;Projektion&amp;rbrack;&amp;lbrack;Verkrümmen&amp;rbrack; Spiegeln funktioniert nicht, wenn die Transformation auf Welt-Raum eingestellt ist
* &amp;lbrack;Projektion&amp;rbrack;&amp;lbrack;Verkrümmen&amp;rbrack; Die Option &quot;Teilen&quot; bleibt ausgewählt, nachdem das Teilen abgeschlossen ist
* &amp;lbrack;Projektion&amp;rbrack;&amp;lbrack;UV&amp;rbrack; Drehpunkt wird beim Spiegeln der Projektion zurückgesetzt
* &amp;lbrack;Filter&amp;rbrack; Baking Die Beleuchtungsumgebung ändert sich beim erneuten Laden oder Ändern eines Parameters
* &amp;lbrack;Interoperabilität&amp;rbrack; Nicht verfügbar für Steam- und Substance-Editionen
* &amp;lbrack;Interoperabilität&amp;rbrack; Die Schaltfläche &quot;3D-Assets im Marketplace durchsuchen&quot; sollte immer CCD auf der Registerkarte &quot;Stock &amp; Marketplace 3D&quot; öffnen.

**Bekannte Probleme:**

* &amp;lbrack;Mac M1&amp;rbrack; Intelligente Material werden nicht korrekt angezeigt

### 7.3.0

*(Freigegeben: 13. Oktober 2021*)Zusammenfassung: **Hauptversion. Es enthält eine neue 3D-Verkrümmungsfunktion, eine neue zylindrische Projektion, Projektionen am Farbwähler, neue Funktionen in der Python-API und Fehlerbehebungen**

**Hinzugefügt:**

* &amp;lbrack;Projektion&amp;rbrack;&amp;lbrack;Verkrümmen&amp;rbrack; 3D-Verkrümmung als neue Projektion gelegt
* &amp;lbrack;Projektion&amp;rbrack;&amp;lbrack;Verkrümmen&amp;rbrack; Aufklebermodus für Alphas, Texturen und Prozedurale per Drag &amp; Drop im Viewport zulassen
* &amp;lbrack;Projektion&amp;rbrack;&amp;lbrack;Verkrümmen&amp;rbrack; Verkrümmen-Projektion mit Aufkleber-Tastaturbefehl (ALT) verwenden
* &amp;lbrack;Projektion&amp;rbrack;&amp;lbrack;Verkrümmen&amp;rbrack;&amp;lbrack;Werkzeugleiste&amp;rbrack; Transformieren der Verformung als Ganzes oder pro Scheitelpunkt
* &amp;lbrack;Projektion&amp;rbrack;&amp;lbrack;Verkrümmen&amp;rbrack;&amp;lbrack;Werkzeugleiste&amp;rbrack; Raster-Punkte mit geteilter Verkrümmung in Querrichtung, horizontal oder vertikal hinzufügen
* &amp;lbrack;Projektion&amp;rbrack;&amp;lbrack;Verkrümmen&amp;rbrack;&amp;lbrack;Werkzeugleiste&amp;rbrack; Dediziertes Menü zum Zurücksetzen von Aktionen
* &amp;lbrack;Projektion&amp;rbrack;&amp;lbrack;Verkrümmen&amp;rbrack;&amp;lbrack;Werkzeugleiste&amp;rbrack; Option zum automatischen Anpassen der Tangenten beim Verschieben von Punkten
* &amp;lbrack;Projektion&amp;rbrack;&amp;lbrack;Verkrümmen&amp;rbrack;&amp;lbrack;Werkzeugleiste&amp;rbrack; Spezielles Menü für die Raster-Edition (Größe, Reset, Farbe und Handle-Größe)
* &amp;lbrack;Projektion&amp;rbrack;&amp;lbrack;Verkrümmen&amp;rbrack; Neuer Tastatur-Tastaturbefehl zum Schalten des Warp-Editionsmodus für ganze Scheitelpunkt (UMSCHALT+V)
* &amp;lbrack;Projektion&amp;rbrack;&amp;lbrack;Verkrümmen&amp;rbrack; Klicken + Strg ermöglicht den Wechsel zwischen Oberflächenwerkzeug und anderen Werkzeugen
* &amp;lbrack;Projektion&amp;rbrack;&amp;lbrack;Zylindrisch&amp;rbrack; Leg der zylindrischen Projektion
* &amp;lbrack;Projektion&amp;rbrack;&amp;lbrack;Werkzeugleiste&amp;rbrack; Einstellungen für Manipulator gruppieren (Größe, Raster, Winkelschritte)
* &amp;Klammer;Farbwähler&amp;Klammer; Neue Benutzeroberfläche für den Farbwähler
* &amp;Klammer;Farbwähler&amp;Klammer; sRGB-Werte in Farbwähler-Widgets verwenden
* &amp;Klammer;Farbwähler&amp;Klammer; Farbfelder speichern und löschen
* &amp;Klammer;Farbwähler&amp;Klammer; Pipette zugänglich von Farbe und normalen Slots
* &amp;Klammer;Farbwähler&amp;Klammer; Bearbeiten dynamischer Farben zwischen 0 und 255 Werten zulassen
* &amp;Klammer;Farbwähler&amp;Klammer; Einheitlicher HSV-/RGB-Status in der gesamten App
* &amp;Klammer;Farbwähler&amp;Klammer; Das Fenster &quot;Farbwähler&quot; ist halbpersistent.
* &amp;Klammer;Farbwähler&amp;Klammer; Durch Drücken von Esc wird das Farbauswahlfenster geschlossen.
* Leistungsverbesserung für UI-Interaktion und beim Malen
* &amp;lbrack;Engine&amp;rbrack; Update auf die neue Substance Engine-Version (8.3.0)
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Erlaubt das erneute Laden des Meshs des aktuellen Projekts
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Aktualisieren von Ressourcen in Projekten zulassen
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Festlegen und Abfragen der Auflösung von UV-Kacheln zulassen
* &amp;lbrack;Interoperabilität&amp;rbrack; Nicht verfügbar für Steam- und Substance-Editionen
* &amp;lbrack;Interoperabilität&amp;rbrack; Mehrere Ressourcen von Bridge erhalten

**Fest:**

* Der Farbwähler zeigt nicht die richtige Farbe an
* &amp;blbrack;Baking&amp;rbrack; Textursatz-Listen sind nicht korrekt angeordnet
* &amp;lbrack;FBX import&amp;rbrack; 3ds Max-Gruppen-Pivot-Transformationen werden nicht berücksichtigt
* &amp;lbrack;Substance Engine&amp;rbrack; Absturz beim Importieren von beschädigtem SBSAR
* &amp;lbrack;MacOS&amp;rbrack; Projektkonfigurationsoption in verschiedenen Sprachen ist nicht vorhanden
* Automatische Speicherung kann Painter während langer Prozesse einfrieren

**Bekannte Probleme:**

* &amp;lbrack;Projektion&amp;rbrack;&amp;lbrack;Verkrümmen&amp;rbrack; Die Option &quot;Teilen&quot; bleibt ausgewählt, nachdem das Teilen abgeschlossen ist
* &amp;lbrack;Projektion&amp;rbrack;&amp;lbrack;Verkrümmen&amp;rbrack; Spiegeln funktioniert nicht, wenn die Transformation auf Welt-Raum eingestellt ist
* &amp;lbrack;Projektion&amp;rbrack;&amp;lbrack;Verkrümmen&amp;rbrack; Artefaktlinien zwischen Patches in seltenen Fällen
* &amp;lbrack;Projektion&amp;rbrack;&amp;lbrack;UV&amp;rbrack; Drehpunkt wird beim Spiegeln der Projektion zurückgesetzt
* &amp;lbrack;Mac M1&amp;rbrack; Intelligente Material werden nicht korrekt angezeigt
* &amp;lbrack;M1&amp;rbrack;&amp;lbrack;Regression&amp;rbrack; Material-Ebene funktioniert nicht

### 7.2.3

*(Freigegeben: 24. August 2021*)Zusammenfassung: **Nebenversion, Bugfix**

**Hinzugefügt:**

* &amp;lbrack;Libraries&amp;rbrack; Hinzufügen einer Möglichkeit zum Ausschließen unerwünschter Dateien vom Durchsuchen

**Fest:**

* &amp;lbrack;Win&amp;rbrack; Mehrere Bildschirme und Schlafprobleme
* &amp;lbrack;MacOS&amp;rbrack;&amp;lbrack;Absturz&amp;rbrack; Wechseln des Shader bei Verwendung von Effekten
* &amp;lbrack;Viewport&amp;rbrack; Im Vollvorschaumodus wird der Pinselcursor nicht mehr ohne Alpha angezeigt
* &amp;lbrack;UI&amp;rbrack; Winkel-Widget wechselt in die falsche Richtung
* &amp;lbrack;Ebenenstapel&amp;rbrack; Viele Unterordner erstellen sehr lange Einfrieren
* &amp;lbrack;Iray&amp;rbrack; Verschiedene Ansichten in Iray und OpenGL: Sichtbar, wenn nicht funktionierend
* &amp;lbrack;Iray&amp;rbrack; Brechungsindex wird nicht berücksichtigt und erscheint nicht in den mdl-Eigenschaften
* &amp;lbrack;JavaScript&amp;rbrack; ShowExportDialog() gibt niemals true zurück.
* Kann keine MTL aus Adobe Stock lesen

### 7.2.2

*(Freigegeben: 27. Juli 2021*)Zusammenfassung: **Nebenversion, Bugfix**

**Hinzugefügt:**

* Aktualisieren Sie die Version der AMD-Treiberanforderungen

**Fest:**

* &amp;lbrack;Mac M1&amp;rbrack; Falsche Speichererkennung
* &amp;lbrack;Export&amp;rbrack; Sehr lange Pfade werden nicht richtig angezeigt

**Bekannte Probleme:**

* &amp;lbrack;Inhalt&amp;rbrack; Veraltete Shader der Beispiele

### 7.2.1

*(Freigegeben: 02. Juli 2021*)Zusammenfassung: **Nebenversion, Hotfix**

**Hinzugefügt:**

* &amp;lbrack;Interop&amp;rbrack; Fügen Sie einen QuickInfo hinzu, um zu informieren, dass das Senden von UV-Kachel-Projekten an Stager noch nicht unterstützt wird.
* &amp;lbrack;Plugin&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Aktualisierung des Livelink-Symbols

**Fest:**

* &amp;lbrack;Nvidia&amp;rbrack; Treiberversion ab 30 gilt als veraltet
* &amp;lbrack;Libraries&amp;rbrack; Der Status des Bedienfelds &quot;Elemente&quot; wird nur gespeichert, wenn ein Projekt geöffnet ist
* &amp;lbrack;Libraries&amp;rbrack; Neue gespeicherte Suche behält Schlüsselwort aus alter gespeicherter Suche bei
* &amp;lbrack;Baker&amp;rbrack;&amp;lbrack;UVTiles&amp;rbrack; ID-Map pro MeshID berücksichtigen ebenfalls UV-Kacheln
* &amp;lbrack;Export&amp;rbrack; gLTF-Dateien importieren keine Scheitelpunkt-Farbe
* &amp;lbrack;Iray&amp;rbrack; Einige QuickInfos fehlen
* &amp;lbrack;Interop&amp;rbrack; An Stager senden ist nicht immer deaktiviert, wenn Stager nicht erkannt wird
* &amp;lbrack;Ressourcenaktualisierung&amp;rbrack; Photoshop-Pinselmaker kann nicht aktualisiert werden
* &amp;lbrack;Inhalt&amp;rbrack; Generator für Glasfaserkantenverschleiß ist defekt

### 7.2.0

*(Freigegeben: 23. Juni 2021*)Zusammenfassung: **Die Hauptversion bietet eine Aktualisierung des Bedienfelds &quot;Elemente&quot;, einen neuen Shader mit Zugriff auf neue Kanäle und Parameter, eine allgemeine Aktualisierung der Benutzeroberfläche, einige dringend angeforderte Leistungsverbesserungen, erweiterte Sprachunterstützung und vieles mehr!**

**Hinzugefügt:**

* &amp;lbrack;Libraries&amp;rbrack; Neues Bedienfeld &quot;Element&quot;, um das Regal zu ersetzen
* &amp;lbrack;Libraries&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Neues Bedienfeld &quot;Elemente&quot;
* &amp;lbrack;Libraries&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Ändern der standardmäßigen Ausrichtung und Benutzeroberfläche des Bedienfelds &quot;Elemente&quot;
* &amp;lbrack;Libraries&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Listenansichtsoption in Bibliothek einfügen
* &amp;lbrack;Libraries&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Neue Breadcrumbs-Navigation im Bedienfeld &quot;Elemente&quot;
* &amp;lbrack;Libraries&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Beim Auswählen einer gespeicherten Suche &quot;Alle Bibliotheken&quot; auswählen
* &amp;lbrack;Libraries&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Wählen Sie &quot;Alle Bibliotheken&quot;, wenn die Auswahl aller Ordner aufgehoben wird.
* &amp;lbrack;Libraries&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Neues Tag für Partikel-Pinsel
* &amp;lbrack;Libraries&amp;rbrack;&amp;lbrack;UI&amp;rbrack; &quot;Regal&quot; durch &quot;Alle Bibliotheken&quot; in der gesamten App ersetzt
* &amp;lbrack;Libraries&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Ausblenden leerer Ordner zulassen
* &amp;lbrack;Libraries&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Standardbenutzerbibliothek sollte sichtbar sein, auch wenn sie leer ist
* &amp;lbrack;Libraries&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Neue Filterung-Methode über Symbole des Elementtyps
* &amp;lbrack;Libraries&amp;rbrack; Tastaturbefehl &quot;STRG&quot;, um mehrere Elementtypen auszuwählen
* &amp;lbrack;Libraries&amp;rbrack; Neue Umgebungsvariable zur Steuerung des Speicherbudgets für die Elementvorschau
* &amp;lbrack;Libraries&amp;rbrack;&amp;lbrack;Content&amp;rbrack; Neue Umgebungs-Map
* &amp;lbrack;Libraries&amp;rbrack;&amp;lbrack;Content&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Versatz auf Standard-Materialien rendern
* &amp;lbrack;Libraries&amp;rbrack;&amp;lbrack;Content&amp;rbrack; Adobe Standard Material-Shader (ASM) als Standard für die Vorschauerstellung festlegen
* &amp;lbrack;Libraries&amp;rbrack;&amp;lbrack;Content&amp;rbrack;&amp;lbrack;ASM&amp;rbrack; Neue Projektvorlagen für neuen ASM-Shader
* &amp;lbrack;Libraries&amp;rbrack;&amp;lbrack;Thumbnail&amp;rbrack; Verwenden der neuen Studio 6-Umgebungs-Map
* &amp;lbrack;Libraries&amp;rbrack;&amp;lbrack;Thumbnail&amp;rbrack; Miniaturansicht in Ressource lesen, anstatt sie zu generieren
* &amp;lbrack;Libraries&amp;rbrack;&amp;lbrack;Thumbnail&amp;rbrack; Versatz zur Miniaturbildgenerierung hinzufügen
* &amp;blbrack;Textursatz-Einstellungen&amp;rbrack;
* &amp;lbrack;Textursatz-Einstellungen&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Leg eines neuen Heights zur normalen Konvertierungsmethode
* &amp;lbrack;Textursatz-Einstellungen&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Überarbeitung der Organisation der Benutzeroberfläche der Kanäle
* &amp;blbrack;Textursatz-Einstellungen&amp;rbrack; Obergrenze für Benutzerkanäle auf 16 Kanäle erhöht
* &amp;lbrack;Textursatz-Einstellungen&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Geben Sie an, welche Kanäle mit dem aktuell ausgewählten Shader kompatibel sind.
* &amp;lbrack;Shader&amp;rbrack;&amp;lbrack;ASM&amp;rbrack; Neuer Adobe Standard Material-Shader
* &amp;lbrack;Shader&amp;rbrack;&amp;lbrack;ASM&amp;rbrack; Zusätzliche Unterstützung für Anisotropie, Clear Coat, Volumenstreuung, Specular edge color und Glanz
* &amp;lbrack;Shader&amp;rbrack;&amp;lbrack;ASM&amp;rbrack; Ändern der Farbwerte der Standardkanäle
* &amp;lbrack;Shader&amp;rbrack;&amp;lbrack;ASM&amp;rbrack;&amp;lbrack;Export&amp;rbrack; Aktualisierte Exportvorlage Adobe Dimension zu Adobe Substance 3D Stager
* &amp;lbrack;Shader&amp;rbrack;&amp;lbrack;ASM&amp;rbrack; Beschriftungen und QuickInfos für Shader- und MDL-Parameter hinzugefügt
* &amp;lbrack;Shader&amp;rbrack;&amp;lbrack;ASM&amp;rbrack; Sichtbarkeit der Farbe der Streuung in der 2D-Ansicht, auch wenn SSS nicht unterstützt wird
* &amp;lbrack;Shader&amp;rbrack;&amp;lbrack;ASM&amp;rbrack;&amp;lbrack;Iray&amp;rbrack; Unterstützung von ASM-Shader in Iray mit neuer MDL
* &amp;lbrack;Shader&amp;rbrack;&amp;lbrack;ASM&amp;rbrack;&amp;lbrack;Iray&amp;rbrack; Aktualisierte Volumenstreuung in veraltetem PBR-Spezifikationsglanz und beschichtet
* &amp;lbrack;Shader&amp;rbrack;&amp;lbrack;ASM&amp;rbrack;&amp;lbrack;Content&amp;rbrack; Standard-SSS-Typ für Beispiele geändert
* &amp;lbrack;Shader&amp;rbrack;&amp;lbrack;ASM&amp;rbrack; Dokumentation für ASM-API hinzugefügt
* &amp;lbrack;Shader&amp;rbrack;&amp;lbrack;ASM&amp;rbrack; Shader optimieren, um nicht verwendete Kanäle zu ignorieren
* &amp;lbrack;Shader&amp;rbrack; Leg neuer Textursatz-Kanäle
* &amp;lbrack;Shader&amp;rbrack; Verbesserte Volumenstreuung
* &amp;lbrack;Shader&amp;rbrack; Neue Shader-Parameter für einige Shader ausgeblendet
* &amp;lbrack;Shader&amp;rbrack; Sichtbar, wenn für Shader-Parameter
* &amp;lbrack;Performance&amp;rbrack;
* &amp;lbrack;Libraries&amp;rbrack; Verbesserungen beim Laden der Ressourcenvorschau und bei der Rechenleistung
* &amp;lbrack;Engine&amp;rbrack; Verbesserte Malleistung
* &amp;lbrack;Automatisch Entpackt&amp;rbrack;
* &amp;lbrack;Automatisch Entpackt&amp;rbrack; Leistungsverbesserungen bei Packing
* &amp;lbrack;Automatisch Entpackt&amp;rbrack; Automatisch entpackt, kompatibel mit dem Arbeitsablauf für die UV-Kachel
* &amp;lbrack;Automatisches Entpacken&amp;rbrack; Neue Option zur Positionierung von UVs entsprechend der Ausrichtung des Meshs
* &amp;lbrack;Andere&amp;rbrack;
* &amp;lbrack;Einstellungen&amp;rbrack; Standardzoomrichtung geändert
* &amp;lbrack;UI&amp;rbrack; Allgemeine Aktualisierung der Benutzeroberfläche
* &amp;lbrack;UI&amp;rbrack; Überarbeitung des Hilfemenüs
* &amp;lbrack;UI&amp;rbrack; Symbol &quot;Umkehren ersetzen&quot;
* &amp;lbrack;UI&amp;rbrack;&amp;lbrack;Plugin&amp;rbrack; Symbol &quot;Ersetzen&quot; für den Link &quot;Plug-in dcc&quot;
* &amp;lbrack;UI&amp;rbrack;&amp;lbrack;AMD&amp;rbrack; Erforderliche Mindestversion aktualisieren und Popup-Nachricht
* &amp;lbrack;Ebenenstapel&amp;rbrack; Neue Ebene innerhalb des ausgewählten leeren Ordners erstellen
* Python-Dokumentation aktualisieren
* &amp;lbrack;Branding&amp;rbrack;
* &amp;lbrack;Branding&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Der Anwendungsname wurde in Adobe Substance 3D Painter aktualisiert
* &amp;lbrack;Branding&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Eigenständige Version auf &quot;Substance Edition&quot; aktualisiert
* &amp;lbrack;Branding&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Name, Installationspfad, Paket und Symbole der aktualisierten ausführbaren Datei der Anwendung
* &amp;lbrack;Branding&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Standardbibliothek und Pfad umbenannt
* &amp;lbrack;Branding&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Aktualisiertes Info-Fenster
* &amp;lbrack;Branding&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Aktualisierter Begrüßungsbildschirm
* &amp;lbrack;Branding&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Versionsnummer nach Jahr entfernt
* &amp;lbrack;Lokalisierung&amp;rbrack; Neue Übersetzungen in Deutsch, Französisch und vereinfachtem Chinesisch
* &amp;lbrack;Interoperabilität&amp;rbrack; Nicht verfügbar für Steam- und Substance-Editionen
* &amp;lbrack;Interoperabilität&amp;rbrack; Interoperabilität mit Adobe Ecosystem: Designer, Sampler, Stager und Bridge
* &amp;lbrack;Interoperabilität&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Element aus Designer empfangen und aktualisieren
* &amp;lbrack;Interoperabilität&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Element aus Sampler erhalten
* &amp;lbrack;Interoperabilität&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Element an Stager senden
* &amp;lbrack;Interoperabilität&amp;rbrack;&amp;lbrack;UI&amp;rbrack; In Adobe Bridge anzeigen
* &amp;lbrack;Interoperabilität&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Schneller Zugriff auf Adobe von 3D-Elementen
* &amp;lbrack;Interoperabilität&amp;rbrack; Neue Verwendungs-Tags von sbsar
* &amp;lbrack;Interoperabilität&amp;rbrack; Umgang mit empfangenen Elementtypen
* &amp;lbrack;Interoperabilität&amp;rbrack; Elemente, die von Adobe Substance 3D Designer oder Adobe Substance 3D Sampler empfangen werden, werden in der vom Benutzer standardmäßig ausgewählten Bibliothek gespeichert
* &amp;lbrack;Interoperabilität&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Neues Symbol in der linken Symbolleiste zum Senden an Stager oder Photoshop

**Fest:**

* &amp;Klammer;Tablet&amp;Klammer; Geringe Leistung beim Malen mit Druck
* &amp;Klammer;Tablet&amp;Klammer; Problem auf Tablets mit Schiebereglern
* &amp;lbrack;Absturz&amp;rbrack; Nicht übereinstimmender Name zwischen Textursatz-Liste und Exporter
* &amp;lbrack;Absturz&amp;rbrack;&amp;lbrack;Libraries&amp;rbrack; Doppelklicken Sie auf eine Unterbibliothek
* &amp;lbrack;Libraries&amp;rbrack; Problem beim Durchsuchen von Bibliotheksverzeichnissen
* &amp;lbrack;Libraries&amp;rbrack; Die Befehlszeile &quot;Generierung der Vorschau erzwingen&quot; funktioniert nicht wie erwartet
* &amp;lbrack;Libraries&amp;rbrack;&amp;lbrack;Content&amp;rbrack; Der Baking geführt Lichtumgebungsfilter ist standardmäßig schwarz
* &amp;lbrack;Linux&amp;rbrack;&amp;lbrack;MacOS&amp;rbrack;&amp;lbrack;Mesh&amp;rbrack exportieren; glTF kann nicht importiert werden, wenn es unter Linux/MacOS erstellt wurde
* &amp;lbrack;Linux&amp;rbrack; Das Ziehen und Ablegen einer Datei in das Bedienfeld &quot;Elemente&quot; kann zu einem Absturz führen
* &amp;lbrack;Automatisches Entpacken&amp;rbrack; Automatisches Entpacken ist auch dann verfügbar, wenn kein Mesh zum erneuten Laden ausgewählt wurde
* &amp;blbrack;Partikeln&amp;rbrack; Falsche Partikel mit Schwerkraft
* &amp;lbrack;Ebenenstapel&amp;rbrack; Ebenen-Histogramm kann nur Luminanz mit einigen Kanälen verwenden
* &amp;lbrack;Geometrie-Maske&amp;rbrack; Kontextmenü auf einem Ordner, wenn das Bearbeiten der Geometriemaske nicht funktioniert
* &amp;lbrack;Projektion&amp;rbrack; Naht mit sphärische Projektion &amp; bilinearer Filterung
* &amp;blbrack;UV-Kacheln&amp;rbrack; Maske in Datei exportieren exportiert nur Kachel 0, 0
* &amp;lbrack;Mesh&amp;rbrack; exportieren FBX Mesh-Export ist leer
* &amp;lbrack;Iray&amp;rbrack; Normalen-Map wird beim Rendern in neuen Projekten nicht berücksichtigt
* &amp;lbrack;Speichern&amp;rbrack; Probleme auf freigegebenen Laufwerken speichern
* &amp;blbrack;Baking&amp;rbrack; Beim erneuten Erstellen eines Meshs mit geänderten Parametern wird eine Warnung angezeigt
* &amp;lbrack;Baking&amp;rbrack;&amp;lbrack;Regression&amp;rbrack; Falsches Ergebnis, wenn der globale Begrenzungsrahmen des hohen Poly-Meshs den Ursprung der Szene nicht enthält
* &amp;lbrack;Python&amp;rbrack; Benutzerdefinierte Benutzerbibliotheken werden nicht berücksichtigt

**Bekannte Probleme:**

* &amp;lbrack;Libraries&amp;rbrack; Gespeicherte Suchvorgänge werden nicht gespeichert, wenn kein Projekt geöffnet wird
* &amp;lbrack;NVIDIA&amp;rbrack; Meldung für veralteten Treiber, selbst wenn der Treiber auf dem neuesten Stand ist

### 7.1.1 (2021.1.1)

*(Freigegeben: 23. März 2021*)Zusammenfassung: **Nebenversion, Bugfix mit der Möglichkeit, Hexadezimalwerte in den Farbwähler einzugeben**

**Hinzugefügt:**

* &amp;lbrack;Log&amp;rbrack; Benutzer über inkompatible AMD-GPU-Treiber warnen
* &amp;Klammer;Farbwähler&amp;Klammer; Eingabe von Hexadezimalwerten zulassen

**Fest:**

* &amp;lbrack;Baker&amp;rbrack; Einbruch der Leistung
* &amp;lbrack;Geometrie-Maske&amp;rbrack; Alt-Klick auf den Namen des Meshs kann zu einem Absturz führen
* &amp;lbrack;Engine&amp;rbrack; Beim Malen wird nicht die gesamte Ansicht aktualisiert, wenn dies erforderlich ist
* &amp;lbrack;Ebenenstapel&amp;rbrack; Auswahl bleibt nach dem Ändern des Shader hängen
* &amp;lbrack;MacOS&amp;rbrack;&amp;lbrack;Farbwähler&amp;rbrack; Die Farbe ist etwas anders als die ausgewählte
* &amp;lbrack;Export&amp;rbrack; Bei Verwendung des PSD-Dateiformats wird nicht eine Datei pro UV-Kachel generiert
* &amp;lbrack;Skripterstellung&amp;rbrack;&amp;lbrack;Javascript&amp;rbrack; alg.mapexport.getPathsExportDocumentMaps() gibt nicht alle Werte zurück
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Deaktivierte Plug-ins werden beim erneuten Öffnen von Painter wieder aktiviert

### 7.1.0 (2021.1.0)

*(Freigegeben: 28. Januar 2021*)Zusammenfassung: **Hauptversion, neue Geometriemaske, mit der Teile der UV-Kachel ausgewählt und Malen werden können, Kopier-/Einfügeeffekte im Ebenenstapel, verbesserte Geometriemaske, Aktualisierung von Iray, Bakern, Substance Engine und neuen Inhalten**

**Hinzugefügt:**

* Neue Geometriemaske und Malen ausgewählter Teile der Geometrie
* &amp;lbrack;Geometrie-Maske&amp;rbrack; Malen ausgewählter Geometrieteile nach Mesh-Namen zulassen
* &amp;lbrack;Geometrie-Maske&amp;rbrack; Rechteckige Auswahl in beiden Viewporten
* &amp;lbrack;Geometrie-Maske&amp;rbrack; Ausgeschlossene Geometrie auf einer Ebene ausblenden/ignorieren
* &amp;lbrack;Geometriemaske&amp;rbrack;&amp;lbrack;Eigenschaften&amp;rbrack; Schnellauswahl für Kontrollkästchen durch Klicken und Ziehen
* &amp;lbrack;Geometry Mask&amp;rbrack;&amp;lbrack;Properties&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Alle einschließen/ausschließen mit einer Dropdown-Liste im Eigenschaftenfenster
* &amp;lbrack;Geometriemaske&amp;rbrack;&amp;lbrack;Eigenschaften&amp;rbrack; Schnelles Auswählen eines Elements in einer Liste mit ALT+LINKSKLICK
* &amp;lbrack;Geometriemaske&amp;rbrack;&amp;lbrack;Eigenschaften&amp;rbrack; Überlagerung in Viewporten, wenn der Mauszeiger über Mesh-Namen/-UV-Kacheln im Eigenschaftenfenster bewegt wird
* &amp;lbrack;Geometriemaske&amp;rbrack;&amp;lbrack;Ebenenstapel&amp;rbrack; Hinzufügen von Kopier-/Einfügeoptionen zur Geometriemaske
* &amp;lbrack;Geometrie-Maske&amp;rbrack; Neues Symbol für die Schaltfläche &quot;Ausgeschlossene Geometrie ausblenden/ignorieren&quot;
* &amp;lbrack;Geometrie-Maske&amp;rbrack; Neue QuickInfo für Ausgeschlossene Geometrie ausblenden/ignorieren
* &amp;lbrack;Geometrie-Maske&amp;rbrack; Tastaturbefehl ALT+H drücken, um die Schaltfläche &quot;Ausgeschlossene Geometrie ignorieren&quot; ein- oder auszublenden
* &amp;lbrack;UV-Kacheln&amp;rbrack;&amp;lbrack;Ebenenstapel&amp;rbrack; Vorschau der neuen Füllebene-Kugel für UV-Kacheln und vereinfachten Modus
* &amp;lbrack;UV-Kacheln&amp;rbrack;&amp;lbrack;Ebenenstapel&amp;rbrack; UV-Kachel-Maske leicht verlassen
* &amp;lbrack;UV-Kacheln&amp;rbrack;&amp;lbrack;Textursatz Liste&amp;rbrack; Geben Sie eine Beschreibung pro UV-Kachel an.
* &amp;lbrack;UV-Kacheln&amp;rbrack;&amp;lbrack;Textursatz-Einstellungen&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Zwei neue Abschnittstitel im Dropdown-Menü zum Ändern der Auflösung der UV-Kachel
* &amp;lbrack;UV-Kacheln&amp;rbrack;&amp;lbrack;Viewport&amp;rbrack; UV-Kachel-Maske beenden, wenn ein Material in den Viewport gezogen wird
* &amp;lbrack;Ebenenstapel&amp;rbrack; Optionen zum Kopieren/Einfügen für Effekte hinzufügen
* &amp;lbrack;Ebenenstapel&amp;rbrack; Kopieren/Einfügen von Effekten von einem Textursatz in einen anderen zulassen
* &amp;lbrack;Ebenenstapel&amp;rbrack; Mehrfachauswahl von Effekten zulassen
* &amp;lbrack;Ebenenstapel&amp;rbrack; Optionen zum Kopieren/Einfügen als Tastaturbefehle für Ebeneneffekte hinzufügen
* &amp;lbrack;Ebenenstapel&amp;rbrack; Automatisches Umschalten zwischen Maske und Inhalt beim Ziehen von Effekten auf eine andere Ebene
* &amp;lbrack;Ebenenstapel&amp;rbrack; Beim Einfügen einer Maske aus einer anderen Ebene automatisch eine Maske erstellen
* &amp;lbrack;Ebenenstapel&amp;rbrack; Hinzufügen von Aktionen zum Verschieben von Effekten im Kontextmenü des jeweiligen Effekts
* &amp;lbrack;Ebenenstapel&amp;rbrack; Ziehen und Ablegen von Effekten von einer Ebene auf eine andere zulassen
* &amp;lbrack;Ebenenstapel&amp;rbrack; Wenn Elemente in einen Ordner gezogen werden, werden sie oben im Ordner abgelegt.
* Iray auf Version 2020.1.0 aktualisieren
* &amp;lbrack;Baker&amp;rbrack; Baker auf Version 2.5.4 aktualisieren
* &amp;lbrack;Baker&amp;rbrack; Einzelne UV-Kacheln im Fenster &quot;Baking-Fortschritt&quot; anzeigen
* &amp;lbrack;Baker&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Ermöglicht das schnelle Baking des aktuellen Textursatzes mit einer neuen Schaltfläche
* &amp;lbrack;Baker&amp;rbrack; Benutzer können mit ALT+LINKSKLICK schnell einen der Baker auswählen
* Substance Engine auf Version 8.0.8 aktualisieren
* &amp;lbrack;Substance Engine&amp;rbrack; Unterstützung der Standardfarbe in neuen .sbsar-Dateien
* &amp;lbrack;Automatisch Entpackt&amp;rbrack; Leistungssteigerung
* &amp;lbrack;Export&amp;rbrack; Fügen Sie visuelles Feedback hinzu, um anzuzeigen, welche Auflösung der UV-Kachel vom Projektstandard abweicht
* &amp;lbrack;Export&amp;rbrack; Szene-Größenfaktor zur exportierten Shader-JSON-Datei hinzufügen
* &amp;lbrack;Sprache&amp;rbrack; Hinzufügen von japanischen Übersetzungen
* &amp;lbrack;UI&amp;rbrack; Info-Fenster mit Versionierung interner Abhängigkeiten aktualisieren
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Verwalten von Regal-Ressourcen zulassen
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Benachrichtigen, wenn ein Projekt zum Baking und Exportieren bereit ist
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Erlaubt zu wissen, wann ein Regal das Crawlen von Ressourcen auf der Festplatte abgeschlossen hat
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Abfragen der Liste der UV-Kacheln pro Textursatz zulassen
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Zuweisen einer benutzerdefinierten Vorschau zu Regal-Ressourcen zulassen
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Verwalten benutzerdefinierter Regal zulassen
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Hinzufügen eines Methodenindex in jedem Untermodul in der Dokumentation
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Neuer Stil für die Dokumentation
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Verbesserung der Ressourcen und Dokumentation des Regals
* &amp;lbrack;Inhalt&amp;rbrack; Drei neue Werkzeugvorgaben zum Nähen
* &amp;lbrack;Regal&amp;rbrack; Entfernen Sie vorübergehend &quot;Auf Substance share exportieren&quot;, während Sie zur neuen Substance share-Plattform wechseln.

**Fest:**

* Absturz bei Monitoren mit unterschiedlichen Auflösungen
* Absturz im Substance Engine mit einigen seltenen Projekten
* Die Aktualisierung des Viewports schlägt beim Wechseln von Ebenen mit &quot;Ausgeschlossene Geometrie ausblenden/ignorieren&quot; fehl.
* &amp;lbrack;2D-Ansicht&amp;rbrack; 2D-Viewport kann in einigen Projekten fehlen
* &amp;blbrack;Baking&amp;rbrack; &quot;Nach Mesh suchen&quot; ignoriert Teile des Objekts.
* &amp;lbrack;Ebenenstapel&amp;rbrack; Durch Klicken auf einen Ebeneneffekt wird der Ordner geöffnet.
* &amp;lbrack;Geometrie-Maske&amp;rbrack; UV-Kachel wird immer noch in der Maske gezählt, auch wenn der Mesh ohne sie erneut importiert wird
* &amp;lbrack;Geometrie-Maske&amp;rbrack; Das Kontextmenü im Viewport bietet nicht die richtigen Werkzeuge
* &amp;lbrack;Engine&amp;rbrack; Erhebliche Verzögerungen bei bestimmten Projekten
* &amp;lbrack;Skripterstellung&amp;rbrack; Hohe Latenz bei JSON-Remote-POST-Anforderungen unter Windows
* &amp;lbrack;Linux&amp;rbrack; Die VRAM-Menge wird bei bestimmten integrierten GPUs nicht ordnungsgemäß erkannt.
* &amp;lbrack;Automatisch Entpackt&amp;rbrack; Absturz oder lange entpack an einigen Projekten

## Version 6

### 6.2.2 (2020.2.2)

*(Freigegeben: 28. September 2020 (1})Zusammenfassung:**Nebenversion, Bugfix mit einigen Funktionen in der Python-API***

**Hinzugefügt:**

* &amp;lbrack;Performance&amp;rbrack; Nicht alle UV-Kacheln bei Verwendung der Farb-ID berechnen
* &amp;lbrack;Baker&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Anzeigen von Textursatz-Beschreibungen
* &amp;lbrack;Baker&amp;rbrack; Speichern von Baking-Einstellungen zulassen
* &amp;lbrack;Baker&amp;rbrack; Hinzufügen aller reduzierten/aller erweiterten Optionen zur Registerkarte &quot;Auswahl&quot;
* &amp;lbrack;Textursatz Liste&amp;rbrack; Beschreibung ausblenden, wenn leer
* &amp;lbrack;UV-Kacheln&amp;rbrack;&amp;lbrack;Textursatz Liste&amp;rbrack; Klicken auf UV-Kachel sollte Liste erweitern/reduzieren
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Horizontale Änderung der Größe des Bedienfelds &quot;Textursatz-Liste&quot; zulassen
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Konsistenter QuickInfo-Text für UV-Kacheln und Textursatz-Arbeitsablauf mit nicht ausgewählten Texturen
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Verwenden von Exportvorgaben zum Exportieren von Texturen zulassen
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Hinzufügen eines Änderungsprotokolls in der Dokumentation
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Zulassen, dass alle verfügbaren Kanäle auf einem bestimmten Stapel abgefragt werden
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Verbesserungen an der Konsolenbenutzeroberfläche

**Fest:**

* &amp;lbrack;AMD&amp;rbrack; Falsche Erkennung veralteter Treiberversionen
* Absturz beim erneuten Importieren eines Meshs mit unterschiedlichem UV-Kacheln-Layout in einigen Fällen
* Absturz bei der Verwendung von Partikeln mit UDIM auf sehr schweren Meshs
* &amp;blbrack;UV-Kacheln&amp;rbrack; Absturz beim Exportieren eines Meshs mit Versatz-Informationen in einigen Fällen
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;Absturz&amp;rbrack; Das Exportieren von 2D-Ansichten im PSD-Format kann einen Absturz verursachen
* Das Importieren von Bildern als Sequenzen beim Erstellen eines Projekts funktioniert nicht
* Engine in einer Endlosschleife
* &amp;lbrack;Tastaturbefehl&amp;rbrack; Kamera dreht sich immer im einrasten Modus, wenn Tastenkombinationen im einrasten Modus geändert werden
* Mesh werden immer automatisch entpackt, wenn sie erneut importiert werden, auch wenn die Option deaktiviert ist
* &amp;lbrack;Textursatz Liste&amp;rbrack; Das Textfeld &quot;Beschreibung&quot; ist während der Edition manchmal nicht vollständig sichtbar.
* &amp;lbrack;Textursatz Liste&amp;rbrack; Dropdown-Menü zum Ein-/Ausblenden von Textursätzen ist nicht vollständig sichtbar
* &amp;lbrack;Textursatz Liste&amp;rbrack; Wenn Sie auf das Augensymbol klicken, sollten Sie nicht den Namen des Textursatzes bearbeiten eingeben.
* &amp;blbrack;Textursatz-Einstellungen&amp;rbrack; Durch Entfernen eines Kanals wird auch der darunter liegende Kanal entfernt
* &amp;lbrack;Export&amp;rbrack; Alle einschließen und Alle zurücksetzen berücksichtigt keine UV-Kacheln
* &amp;lbrack;Baker&amp;rbrack; Während des Bakings werden nicht ausgewählte Baker angezeigt
* Die Behebungsaktualisierung wird bei durch Baking erzeugte Map als Eingabe nicht berücksichtigt
* &amp;lbrack;UV-Kacheln&amp;rbrack;&amp;lbrack;Viewport&amp;rbrack; 3D-Viewport friert ein, wenn Intelligente Material nach einem UV-Kachel mit ausgewählter Ordnermaske hinzugefügt wird
* &amp;lbrack;UV-Kacheln&amp;rbrack;&amp;lbrack;Viewport&amp;rbrack; Drahtgitter ist immer noch für ausgeblendete Kacheln mit dem Modus &quot;Malen durch&quot; sichtbar
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;Sketchfab&amp;rbrack; Probleme mit dem Abonnementtyp &quot;Plus&quot;
* &amp;lbrack;Sketchfab&amp;rbrack; Das Kontrollkästchen &quot;Dieses Asset ist privat&quot; wird nach dem Kontowechsel nicht angezeigt
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;Content&amp;rbrack; Verwackelte Pinselvorgaben können zu Leistungsproblemen führen.
* &amp;lbrack;Plugin Photoshop&amp;rbrack; Meldung im Protokoll: nicht kompatibel mit dem UV-Kachel-Workflow
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; PYTHONPATH env var verhindert den Start der Anwendung
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Typo in der Python-Dokumentation

### 6.2.1 (2020.2.1)

*(Freigegeben: 29. Juli 2020 (1})Zusammenfassung:**Nebenversion, Hotfix***

**Hinzugefügt:**

* Umgebungsvariable &quot;SUBSTANCE_PAINTER_VRAM_BUDGET&quot; hinzufügen, um den GPU-VRam-Betrag zu überschreiben
* &amp;lbrack;UV-Kacheln&amp;rbrack;&amp;lbrack;Leistung&amp;rbrack; Nicht alle UV-Kacheln berechnen, wenn das Polygon-Füllwerkzeug verwendet wird

**Fest:**

* &amp;lbrack;Iray&amp;rbrack; &quot;Rendering speichern&quot; gibt einen Fehler zurück, der zu einem schwarzen Bild führt
* &amp;lbrack;Linux&amp;rbrack; Absturz nach dem Begrüßungsbildschirm unter CentOS 7.3
* &amp;lbrack;Linux&amp;rbrack; Die VRAM-Menge wird bei bestimmten Konfigurationen nicht richtig erkannt.
* &amp;lbrack;Absturz&amp;rbrack; Öffnen eines Projekts mit dem Namen des duplizierten Textursatzes
* &amp;lbrack;Engine&amp;rbrack; Problem mit Cache-Invalidierung beim Ändern einer Maske
* &amp;lbrack;Textursatz Liste&amp;rbrack; Falscher Schrifteffekt, wenn Textursatz deaktiviert ist

**Bekannte Probleme:**

* &amp;lbrack;Textursatz Liste&amp;rbrack; Beschreibung kann nicht ausgeblendet werden
* &amp;lbrack;Textursatz Liste&amp;rbrack; UI-Probleme
* &amp;lbrack;Iray&amp;rbrack; PSD-Rendering wird nicht geöffnet
* &amp;lbrack;Plugin Photoshop&amp;rbrack; Nicht kompatibel mit dem Arbeitsablauf für UV-Kacheln

### 6.2.0 (2020.2.0)

*(Freigegeben: 23. Juli 2020 (1})Zusammenfassung:**Hauptversion mit neuem Arbeitsablauf für UV-Kacheln, Malen über UV-Kacheln hinweg und Leistungsverbesserung***

**Hinzugefügt:**

* UV-Kacheln (UDIM)
* &amp;blbrack;UV-Kacheln&amp;rbrack; Malen über UV-Kacheln
* &amp;blbrack;UV-Kacheln&amp;rbrack; Auswahl zwischen neuem und veraltetem Arbeitsablauf für UV-Kacheln zulassen
* &amp;blbrack;UV-Kacheln&amp;rbrack; Importieren von Bildsequenzen für UDIM/UV-Kacheln als Ressource
* &amp;blbrack;UV-Kacheln&amp;rbrack; Liste der UV-Kacheln pro Textursatz im Fenster &quot;Liste der Textursatz&quot; hinzufügen
* &amp;blbrack;UV-Kacheln&amp;rbrack; Ermöglichen der gleichzeitigen Bearbeitung mehrerer UV-Kacheln in den Textursatz-Einstellungen
* &amp;lbrack;UV-Kacheln&amp;rbrack;&amp;lbrack;2D-Ansicht&amp;rbrack; UV-Kacheln als Raster anzeigen
* &amp;lbrack;UV-Kacheln&amp;rbrack;&amp;lbrack;2D-Ansicht&amp;rbrack; Neue Viewport-Schaltfläche zum Anzeigen oder Ausblenden von Informationen zu UV-Kacheln
* &amp;blbrack;UV-Kacheln&amp;rbrack; Beim UV-Kachel von Projekten standardmäßig auf Ein Kanal umstellen
* &amp;blbrack;UV-Kacheln&amp;rbrack; Neue Schaltfläche in der kontextabhängigen Symbolleiste, um maskierte UV-Kacheln beim Malen zu ignorieren
* &amp;lbrack;UV-Kacheln&amp;rbrack;&amp;lbrack;Ebenenstapel&amp;rbrack; Neue Ebenenstapel-Symbole zur Leistungsverbesserung
* &amp;lbrack;UV-Kacheln&amp;rbrack;&amp;lbrack;Ebenenstapel&amp;rbrack; Verbessern der Symbole &quot;Malen und Füllen&quot; in der Symbolleiste
* &amp;lbrack;UV-Kachel&amp;rbrack;&amp;lbrack;2D-Ansicht&amp;rbrack; Mehrere UV-Kacheln gleichzeitig ein- oder ausschließen (Linksklick, Strg + Linksklick)
* &amp;blbrack;UV-Kachel mask&amp;rbrack; Neue Ebenenmaske zum Einschließen, Ausschließen von Kacheln pro UV-Kachel mit neuem Symbol
* &amp;lbrack;UV-Kachel&amp;rbrack;&amp;lbrack;Ebenenstapel&amp;rbrack; Anzahl der UV-Kacheln im Maskensymbol für UV-Kacheln anzeigen, wenn nicht alle eingeschlossen sind
* &amp;lbrack;UV-Kachel&amp;rbrack;&amp;lbrack;2D/3D-Ansicht&amp;rbrack; Einen Hover-Effekt hinzufügen, um UV-Kacheln unter dem Cursor darzustellen.
* &amp;lbrack;UV-Kacheln&amp;rbrack;&amp;lbrack;Baker&amp;rbrack; Auswahl und Baking bestimmter UV-Kacheln zulassen
* &amp;lbrack;UV-Kacheln&amp;rbrack;&amp;lbrack;Baker&amp;rbrack; Hinzufügen von Auswahloptionen für Textursatz/UV-Kacheln
* &amp;lbrack;UV-Kacheln&amp;rbrack;&amp;lbrack;Baker&amp;rbrack; Kontextmenüoption zum Auswählen von UV-Kacheln innerhalb eines Textursatzes
* &amp;lbrack;UV-Kacheln&amp;rbrack;&amp;lbrack;Baker&amp;rbrack; Schnellauswahl im Textursatz/in den UV-Kacheln durch Ziehen ermöglichen
* &amp;lbrack;UV-Kacheln&amp;rbrack;&amp;lbrack;Baker&amp;rbrack; Ersetzen Sie die Schaltflächen &quot;Alle&quot; und &quot;Keine&quot; in Mesh-Map durch explizitere Auswahloptionen
* &amp;lbrack;UV-Kacheln&amp;rbrack;&amp;lbrack;Baker&amp;rbrack; Anzahl der zu Baking führend Texturen anzeigen
* &amp;lbrack;UV-Kacheln&amp;rbrack;&amp;lbrack;Exportieren&amp;rbrack; Auswahl und Export bestimmter UV-Kacheln zulassen
* &amp;lbrack;UV-Kacheln&amp;rbrack;&amp;lbrack;Exportieren&amp;rbrack; UV-Kacheln durch Ziehen mit der Maus schnell auswählen
* &amp;lbrack;UV-Kacheln&amp;rbrack;&amp;lbrack;Exportieren&amp;rbrack; Hinzufügen von Dropdown-Menüoptionen für UV-Kacheln
* &amp;lbrack;UV-Kacheln&amp;rbrack;&amp;lbrack;Exportieren&amp;rbrack; Deaktivieren einiger Exportvorgaben, wenn sie nicht mit UV-Kacheln funktionieren (Adobe Dimension, Sketchfab, glTF, USD)
* &amp;lbrack;UV-Kacheln&amp;rbrack;&amp;lbrack;Inhalt&amp;rbrack; Exportvorgaben zur Verwendung des neuen Tags $udim aktualisieren
* &amp;blbrack;UV-Kacheln&amp;rbrack; Verbessern der Fehlerberichterstattung beim Importieren von Meshs mit überlappenden UV-Inseln
* &amp;blbrack;UV-Kacheln&amp;rbrack; In Iray kompatible UV-Kacheln
* &amp;lbrack;UV-Kacheln&amp;rbrack;&amp;lbrack;Scripting&amp;rbrack; Hinzufügen einer UV-Kachel-Exportdokumentation zu Python-Dokumenten
* Leistung
* &amp;lbrack;Performance&amp;rbrack; Neue Schaltfläche in der kontextabhängigen Symbolleiste zum Anhalten der Berechnung von Enginen bei der Arbeit (UMSCHALT+ESC)
* &amp;lbrack;Performance&amp;rbrack; Schnelleres Öffnen von Projekten durch Verzögerung der Textursatz-Cache-Berechnung
* &amp;lbrack;Performance&amp;rbrack; Warten Sie nicht, bis die Mesh-Map beim Öffnen des Projekts geladen sind
* &amp;lbrack;Performance&amp;rbrack;&amp;lbrack;2D/3D-Ansicht&amp;rbrack; Maskenkanal im Viewport nicht berechnen, wenn er nicht verwendet wird
* &amp;lbrack;Performance&amp;rbrack; Anwendung nicht blockieren, wenn Mesh-Map in den Viewporten geladen werden
* &amp;lbrack;Performance&amp;rbrack; Verbessern der inkrementellen Speichergeschwindigkeit beim Speichern eines Projekts
* &amp;lbrack;Performance&amp;rbrack;&amp;lbrack;Bakers&amp;rbrack; Ändern Sie die Standardeinstellungen für die Ausdehnung, um die Speicherzeit und die Projektgröße zu verbessern
* &amp;lbrack;Performance&amp;rbrack;&amp;lbrack;Bakers&amp;rbrack; Wechsel zu Graustufen auf bestimmten Bakern, um Zeit und Projektgröße zu sparen
* &amp;lbrack;Performance&amp;rbrack;&amp;lbrack;Export&amp;rbrack; Verbessern der Engine-Performance, um Texturen schneller exportieren zu können
* &amp;lbrack;Performance&amp;rbrack;&amp;lbrack;Export&amp;rbrack; Verbessern der Reaktionsfähigkeit beim Öffnen des Exportdialogs mit vielen Textursätzen
* &amp;lbrack;Performance&amp;rbrack;&amp;lbrack;Export&amp;rbrack; Verbessern Sie die Leistung beim Wechsel zur Registerkarte &quot;Exportliste&quot;.
* &amp;lbrack;Performance&amp;rbrack;&amp;lbrack;Iray&amp;rbrack; Iray-Startzeit reduzieren
* Sonstige
* &amp;lbrack;Baker&amp;rbrack; Hinzufügen von Auswahloptionen für Textursatz
* Shader-Instanzen-Management auf Textursatz-Einstellungen verschieben
* &amp;lbrack;2D/3D-Ansicht&amp;rbrack; Nachricht am unteren Rand des Viewports hinzufügen, um anzuzeigen, welcher Maskentyp bearbeitet wird
* &amp;lbrack;Ebenenstapel&amp;rbrack; Neue Option in den Einstellungen, um zwischen alten und neuen Miniaturansichten zu wechseln
* &amp;lbrack;Ebenenstapel&amp;rbrack; Visuelles Feedback hinzufügen, um den Ladezustand der Miniaturen anzuzeigen
* &amp;lbrack;Proj&amp;rbrack; Neue Projektion &quot;Fill (Match Per UV-Tile)&quot; zum Laden von Bildsequenzen
* &amp;lbrack;Proj&amp;rbrack; Ändern Sie in bestimmten Fällen den Modus &quot;Füllebenen-Projektion&quot; in &quot;Füllen (entspricht pro UV-Kachel)&quot;
* &amp;lbrack;Inhalt&amp;rbrack; Optimierung der Kohlevergaserleistung zur Verbesserung der Pinselvorgabe
* Iray auf Version 2020.0.0 aktualisieren
* &amp;lbrack;Export&amp;rbrack; Deaktivieren der Registerkarte &quot;Exportliste&quot;, wenn nichts ausgewählt ist
* Automatisch Entpackt
* &amp;lbrack;Automatisch Entpackt&amp;rbrack; Verbesserung der Erfolgsrate des automatischen entpack-Prozesses
* &amp;lbrack;Automatisch Entpackt&amp;rbrack; Verbesserte Parametrisierung zur Erhöhung der Geschwindigkeit und Stabilität

**Fest:**

* &amp;lbrack;Alembic&amp;rbrack; Facetten werden beim Importieren von Dateien ignoriert
* &amp;lbrack;Alembic&amp;rbrack; Unendliche Ladezeit mit bestimmten Dateien
* &amp;lbrack;Import&amp;rbrack; Eine falsche UDIM-Bildsequenz wird importiert, wenn nur die Dateierweiterung unterschiedlich ist
* &amp;lbrack;Absturz&amp;rbrack; Der Versuch, ein Projekt zu öffnen, das durch einen anderen Prozess gesperrt ist, führt zu einem Absturz
* &amp;lbrack;Projektion&amp;rbrack; Artefakte an dupliziertem Mesh bei Verwendung von triplanare Projektion
* &amp;lbrack;Export&amp;rbrack; Emissive-Kanal wird nicht mit USD exportiert
* &amp;lbrack;Inhalt&amp;rbrack; Intelligente Material &quot;Charcoal&quot; enthält Malen-Striche

**Bekannte Probleme:**

* &amp;lbrack;Textursatz Liste&amp;rbrack; Beschreibung kann nicht ausgeblendet werden
* &amp;lbrack;Textursatz Liste&amp;rbrack; UI-Probleme

### 6.1.3 (2020.1.3)

*(Freigegeben: 16. Juni 2020 (1})Zusammenfassung:**Bugfix***

**Hinzugefügt:**

* &amp;lbrack;Export&amp;rbrack; Versatz-Einstellungen in der JSON-Datei für Shader-Parameter hinzufügen

**Fest:**

* &amp;lbrack;Absturz&amp;rbrack;&amp;lbrack;Engine&amp;rbrack; Absturz beim Löschen und Ersetzen vorhandener Kanäle
* &amp;lbrack;Absturz&amp;rbrack; Ändern des Shaders nach dem Malen einer Maske in einer Material-Ebene
* &amp;lbrack;Absturz&amp;rbrack;&amp;lbrack;Engine&amp;rbrack; Absturz mit einigen umfangreichen Projekten
* &amp;lbrack;Baker&amp;rbrack; Die Zuordnung nach Name funktioniert nicht mit aus zBrush exportierten OBJ
* &amp;lbrack;Versatz&amp;rbrack;&amp;lbrack;SVT&amp;rbrack; Texturen werden beim Öffnen des Projekts nicht angezeigt, wenn der Versatz aktiviert ist
* &amp;lbrack;Export&amp;rbrack; Einige Texturen werden in einheitlichem Grau exportiert
* &amp;lbrack;Export&amp;rbrack; Deaktivierte Textursatz sollten nicht für Dimension- und Sketchfab-Exportvorgaben exportiert werden
* &amp;lbrack;Skripterstellung&amp;rbrack;&amp;lbrack;JavaScript&amp;rbrack; Absturz bei der Verwendung der JavaScript-API, um auf die Exportkonfiguration im onProjectOpened-Ereignis zuzugreifen
* &amp;lbrack;Skripterstellung&amp;rbrack;&amp;lbrack;Javascript&amp;rbrack; onExportFinished() wird nach einem Export nicht aufgerufen

### 6.1.2 (2020.1.2)

*(Freigegeben: 28. Mai 2020*)Zusammenfassung: **Bugfix mit Substance Engine- und Baker-Update**

**Hinzugefügt:**

* &amp;lbrack;Baker&amp;rbrack; Aktualisieren Sie auf die neueste Version
* &amp;lbrack;Baker&amp;rbrack; Neue Sampling-Methode in den Bakern Ambient occlusion, Krümmung, Thickness
* Aktualisieren Sie auf die neueste Version von Substance Engine
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Erstellen der ResourceID für Projektressourcen zulassen
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Abfragen von Kanalinformationen zulassen
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; Hinzufügen von DryRun- und Callback-Funktionen zur Simulation des Textur-Exports

**Fest:**

* &amp;lbrack;Baker&amp;rbrack; Falsche Normalen im Welt-Raum-Normale-Baker mit einer Tangente-Normalen-Map in bestimmten Fällen
* &amp;lbrack;Baker&amp;rbrack; Fehler beim Baking von Ambient occlusion mit Optix, wenn kein hohes Poly
* &amp;lbrack;Dynamische Pinselstriche&amp;rbrack; Verzögerung beim Laden eines bestimmten Textursatzes
* &amp;lbrack;Export&amp;rbrack; Sollte die deaktivierten Textursätze nicht für USD exportieren, glTF
* &amp;lbrack;Skripterstellung&amp;rbrack;&amp;lbrack;JavaScript&amp;rbrack; Die Baker-Einstellungen für neue Krümmungen können nicht bearbeitet werden.
* &amp;lbrack;Skripterstellung&amp;rbrack;&amp;lbrack;JavaScript&amp;rbrack; alg.texturesets.addChannel() gibt in einigen Fällen keinen Fehler zurück
* &amp;lbrack;Skripterstellung&amp;rbrack;&amp;lbrack;JavaScript&amp;rbrack; Typo in der JavaScript-API-Dokumentation für setProjectExportOptions()
* &amp;lbrack;Skripterstellung&amp;rbrack;&amp;lbrack;JavaScript&amp;rbrack; Immer alle Textursatz exportieren
* &amp;lbrack;Scripting&amp;rbrack;&amp;lbrack;Python&amp;rbrack; sys.executable gibt einen Pfad zu python.exe anstelle von Substance Painter zurück
* Textur-Cache nicht kompatibel mit Mac OS und Windows/Linux
* &amp;lbrack;Livelink UE4&amp;rbrack; Nur das letzte Material wird für alle Textursatz in einem kombinierten Mesh verwendet.

**Bekannte Probleme:**

* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;Dimension&amp;rbrack;&amp;lbrack;Skecthfab&amp;rbrack; Die deaktivierten Textursatz sollten nicht exportiert werden
* &amp;lbrack;Absturz&amp;rbrack; Shader nach dem Malen einer Maske in einer Material-Ebene ändern

### 6.1.1 (2020.1.1)

*(Freigegeben: 05. Mai 2020*)Zusammenfassung: **Hotfix**

**Hinzugefügt:**

* &amp;lbrack;Export&amp;rbrack; Visuelles Feedback des überschriebenen Status für TextureSet

**Fest:**

* &amp;lbrack;Export&amp;rbrack; Exporter-Fenstergröße ist auf einem Spezialauflösungsmonitor zu groß und kann nicht geändert werden
* &amp;lbrack;Export&amp;rbrack; Optionen werden nach dem Export nicht gespeichert
* &amp;lbrack;Export&amp;rbrack; Absturz oder kann nicht mit einer Exportvorgabe vom Cache exportiert werden
* &amp;lbrack;Export&amp;rbrack; Wenn Sie den Export abbrechen, wird eine unerwartete zusätzliche leere Map generiert.
* &amp;lbrack;Export&amp;rbrack; Vorgabeeinstellungen für den virtuellen Export korrigieren
* &amp;lbrack;Python&amp;rbrack; PYTHONPATH env var wird nicht berücksichtigt
* &amp;lbrack;Python&amp;rbrack;&amp;lbrack;Export&amp;rbrack; Wenn Sie den Export über Python abbrechen, wird ein Ausnahmefehler zurückgegeben
* &amp;lbrack;Python&amp;rbrack;&amp;lbrack;Export&amp;rbrack; export_project_Texturen falsches Ergebnis mit psd-Dateiformat
* &amp;lbrack;Baker&amp;rbrack; Absturz unter Linux mit GPU-Raytracing

**Bekannte Probleme:**

* &amp;lbrack;JavaScript&amp;rbrack; Die Baker-Einstellungen für neue Krümmungen können nicht bearbeitet werden.
* &amp;lbrack;JavaScript&amp;rbrack;&amp;lbrack;Export&amp;rbrack; Immer alle Textursatz exportieren
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;USD&amp;rbrack; Die deaktivierten Textursatz sollten nicht exportiert werden
* &amp;lbrack;Absturz&amp;rbrack; Shader nach dem Malen einer Maske in einer Material-Ebene ändern

### 6.1.0 (2020.1.0)

*(Freigegeben: 22. April 2020 (1})Zusammenfassung:**Hauptversion mit neuer Textur und neuem Mesh-Exporter (mit Versatz und Tessellation), aktualisiertem UV mit mehr Steuerelementen, neuen Bakern, neuer Python-API für die Skripterstellung, besserer UX für die Decal-entpackte und neuem Inhalt***

**Hinzugefügt:**

* Exporter &quot;Neue Textur und neuer Mesh&quot;
* &amp;lbrack;Export&amp;rbrack; Neue Exporter-Oberfläche
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;Export tab&amp;rbrack; Auswahl der pro Textursatz exportierten Kartenkanäle zulassen
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;Export tab&amp;rbrack; Ändern der Textursatz-Größe für alle Textursatz in einer Aktion zulassen
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;Export tab&amp;rbrack; Andere Vorlagen pro Textursatz zulassen (außer USD, glTF, Sketchfab und Dimension)
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;Export tab&amp;rbrack; Schnelle Aktivierung und Deaktivierung von Karten und Textursätze
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;Export tab&amp;rbrack; Exportauflösung 8192x8192 nicht mehr experimentell
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;Export tab&amp;rbrack; Ändern des Dateiformats und der Bittiefe pro Map zulassen
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;Export tab&amp;rbrack; Zurücksetzen auf die Werte der Standardparameter zulassen
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;Export tab&amp;rbrack; Speichern von Einstellungen ohne Export zulassen
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;Ausgabevorlagen tab&amp;rbrack; Registerkarte &quot;Konfiguration&quot; in Registerkarte &quot;Ausgabevorlagen&quot; umbenennen
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;Ausgabevorlagen tab&amp;rbrack; Definition von Dateiformat und Bittiefe pro voreingestellter Map zulassen
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;Liste der Exporte tab&amp;rbrack; Neue Vorschauregisterkarte zum Zusammenfassen und Anzeigen des Exportvorgangs
* &amp;lbrack;Mesh&amp;rbrack; importieren/exportieren Optimierte Performance beim Importieren/Exportieren der Zeit
* &amp;lbrack;Mesh&amp;rbrack; exportieren Exportieren von Mesh in FBX
* &amp;lbrack;Mesh&amp;rbrack; exportieren Mesh mit Versatz und Tessellation exportieren
* &amp;lbrack;Mesh&amp;rbrack;&amp;lbrack;UI&amp;rbrack; exportieren Neue Einstellungen für die Neuberechnung des normalen Scheitelpunkt, Anwendung der Triangulation
* &amp;lbrack;Mesh&amp;rbrack; exportieren Exportieren der ursprünglichen Mesh-Topologie mit neuen UVs, die durch automatischen entpack generiert werden
* Automatischer entpack mit weiteren Steuerelementen wurde aktualisiert
* &amp;lbrack;UV Entpack&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Einstellung hinzufügen, um den automatischen entpack von UV im neuen Projektfenster zu aktivieren
* &amp;lbrack;UV Entpack&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Neue Optionen zum Steuern der entpackend Schritte (Nähte, entpack, Packing)
* &amp;lbrack;UV Entpack&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Beibehaltung bestehender entpackend Nähte/entpackend/Packings
* &amp;lbrack;UV Entpack&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Neue Optionen zur vollständigen Neuberechnung entpackend Schritte
* &amp;lbrack;UV Entpack&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Neue Option zur Steuerung der Randgröße (keine, kleine, mittlere und große)
* Neue Baker
* &amp;lbrack;Baker&amp;rbrack; Alte Krümmung durch neue Krümmung aus dem Mesh ersetzen
* &amp;lbrack;Baker&amp;rbrack; Option &quot;Match by Name&quot; hinzufügen, um die Rückseite im Baker &quot;Ambient occlusion&quot; zu ignorieren
* &amp;lbrack;Baker&amp;rbrack; Option &quot;Boden-Ebene hinzufügen&quot; im Baker &quot;Ambient occlusion&quot;
* Neue Python-API für die Skripterstellung (3.7.6)
* &amp;lbrack;Python&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Neues Skriptmenü für Python
* &amp;lbrack;Python&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Neue Python-Dokumentation im Hilfemenü
* &amp;lbrack;Python&amp;rbrack; Leg der Substance Painter-Pythonmodule: substance_painter, alg, display, project.setting, project, texturesets, ui
* &amp;lbrack;Python&amp;rbrack; Leg des neuen Python-Moduls &quot;substance_painter&quot;
* &amp;lbrack;Python&amp;rbrack; Neues Python-Untermodul gelegt: alg, display, log, project, resource, texturesets, ui
* &amp;lbrack;Python&amp;rbrack; Listener für Projektänderungen
* &amp;lbrack;Python&amp;rbrack; Neue Beispiele in der Python-Dokumentation
* &amp;lbrack;JavaScript&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Menü &quot;Plug-ins&quot; durch JavaScript ersetzt
* &amp;lbrack;Viewport&amp;rbrack; Erstellen einer Aufkleberressource durch Ziehen/Ablegen + ALT aus dem Regal zulassen, wenn eine Projektion aus dem Aufkleber erstellt wird
* Neue Inhalte
* &amp;lbrack;Inhalt&amp;rbrack; 5 neue Aufkleber Materialien von Substance Source
* &amp;lbrack;Inhalt&amp;rbrack; Hinzufügen neuer Projektvorlagen und Exportieren von Vorgaben für den Maxwell-Renderer
* &amp;lbrack;Inhalt&amp;rbrack; Projektvorlage für Keyshot 9-Export hinzufügen
* &amp;lbrack;Inhalt&amp;rbrack; Die Exportvorgabe von Keyshot 9 zur Unterstützung von Versatz und emissive aktualisieren
* &amp;lbrack;Inhalt&amp;rbrack;&amp;lbrack;Exporter&amp;rbrack; Aktualisierung aller Exportvorgaben, um die neuesten Versionen von Game-Enginen und Renderern abzugleichen
* &amp;lbrack;Inhalt&amp;rbrack;&amp;lbrack;Exporter&amp;rbrack; Exportvoreinstellungsdateien aktualisieren, um neue Format- und Dithering-Einstellungen zu verwenden
* &amp;lbrack;Inhalt&amp;rbrack; Neue Vorlagen und Shader zur Unterstützung von VRay Material (VRayMtl)
* &amp;lbrack;Ebenenstapel&amp;rbrack; Löschen von Ebeneneffekten über das Papierkorbsymbol oder den Tastaturbefehl &quot;Löschen&quot; über die Tastatur zulassen
* Plug-in-Substance Source entfernen (Launcher mit &quot;Senden an&quot;-Funktion verwenden)
* &amp;lbrack;Windows&amp;rbrack; Keine TDR-Warnung auf High-End-GPUs anzeigen

**Fest:**

* Übersetzungsprobleme im Dialogfeld &quot;Neue Projektdatei&quot;
* &amp;lbrack;Baker&amp;rbrack; Die Einstellung &quot;Vorverarbeitete Szene speichern&quot; funktioniert nicht mehr
* &amp;lbrack;Planare Projektion&amp;rbrack; Projektion funktioniert nicht bei Meshs mit sich wiederholenden UVs
* &amp;lbrack;Aufkleber&amp;rbrack; Verhaltensunterschiede im Normalkanal bei Verwendung verschiedener Modi zur Projektion der Füllebene
* &amp;lbrack;Verwischen&amp;rbrack;&amp;lbrack;Klon&amp;rbrack; Beim Malen in einer Maske kann ein Artefakt angezeigt werden
* &amp;lbrack;Engine&amp;rbrack; Absturz mit bestimmtem Ebeneninhalt
* &amp;lbrack;Engine&amp;rbrack; Zufälliger Absturz beim Malen in einigen Fällen
* &amp;lbrack;Ankerpunkt&amp;rbrack; Der Verweis auf eine leere Maske gibt immer Weiß zurück.
* &amp;lbrack;Export&amp;rbrack; Ebene, die in bestimmten Stapel-Konfigurationen nicht berücksichtigt wurde
* &amp;lbrack;Mesh&amp;rbrack; exportieren Export mit Pfad, der Sonderzeichen enthält, nicht möglich
* &amp;lbrack;Mesh&amp;rbrack; exportieren glTF-Dateien können beim Export aus Linux oder MacOS nicht gelesen werden
* &amp;lbrack;Mesh&amp;rbrack; importieren Das erneute Importieren von DAE, PLY oder glTF funktioniert nicht wie beabsichtigt

**Bekannte Probleme:**

* &amp;lbrack;Skripterstellung&amp;rbrack;&amp;lbrack;JavaScript&amp;rbrack; Die Baker-Einstellungen für neue Krümmungen können nicht bearbeitet werden.
* &amp;lbrack;Baker&amp;rbrack; Absturz unter Linux mit GPU-Raytracing
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;USD&amp;rbrack; Die deaktivierten Textursatz sollten nicht exportiert werden
* &amp;lbrack;Absturz&amp;rbrack; Shader nach dem Malen einer Maske in einer Material-Ebene ändern

## Version 5

### 5.3.3 (2019.3.3)

*(Freigegeben: 06. Februar 2020*)Zusammenfassung: **Bugfix mit Upgrade auf Iray 2019.3**

**Hinzugefügt:**

* Upgrade auf Iray 2019.3
* &amp;lbrack;Log&amp;rbrack; Veraltetes BIOS für Ryzen-CPU anzeigen, was beim Baking zu Abstürzen führt
* &amp;lbrack;ABR&amp;rbrack; ABR-Alphas nach Regal extrahieren

**Fest:**

* &amp;lbrack;Baker&amp;rbrack; Baking schlägt fehl, wenn der High-Poly-Mesh keine UVs enthält
* &amp;lbrack;Linux&amp;rbrack; Benutzerdefinierte Mauskürzel werden nicht gespeichert
* &amp;Klammer;Pinsel&amp;Klammer; Die Kontur verschwindet mit einigen Alpha-Formen
* &amp;Klammer;Tablet&amp;Klammer; Fehlerhafte Erkennung beim Verschieben von Schiebereglern
* &amp;blbrack;Shortcuts&amp;rbrack; Mit &quot;Strg+Alt+Mausklick&quot; kann kein Tastaturbefehl eingerichtet werden
* &amp;lbrack;Regal&amp;rbrack; Die Ressourcen-QuickInfo wird bei Verwendung eines Stift-Tablets nicht angezeigt
* &amp;lbrack;2D-Ansicht&amp;rbrack;&amp;lbrack;Export&amp;rbrack; Die Voreinstellung &quot;2D-Ansicht&quot; berücksichtigt nicht die normalen Informationen.
* Einfrieren beim Malen in UV-Ausrichtung mit bestimmten Pinseln
* Malen unter einem Filter erzeugt Artefakt auf dem laufenden Strich
* &amp;lbrack;Viewport&amp;rbrack; Falscher Texturen-Cache im Viewport nach dem erneuten Importieren eines Meshs
* &amp;lbrack;Absturz&amp;rbrack; Fehler beim Speichern nach dem Export in Photoshop
* &amp;lbrack;Absturz&amp;rbrack; Schreiben spezieller Symbole im Präfix beim Importieren von Ressourcen
* &amp;lbrack;Absturz&amp;rbrack; Klicken Sie in den Ankerpunkt-Eigenschaften auf die Referenz
* &amp;lbrack;Ankerpunkte&amp;rbrack; Kanal wird nicht aktualisiert, wenn ein Filter zwischen Ankerpunkt und Referenz vorhanden ist
* Iray-URL-Link im Hilfemenü funktioniert nicht

**Bekannte Probleme:**

* &amp;lbrack;UV Entpack&amp;rbrack; Die Verarbeitung von Meshs mit hohem Poly-Anteil kann lange dauern
* &amp;lbrack;UV Entpack&amp;rbrack; Scheitelpunkt an exakt denselben Koordinaten werden zusammengeführt
* &amp;lbrack;UV Entpack&amp;rbrack; UV-Generierung kann in seltenen Fällen auf bestimmten Mesh-Komponenten fehlschlagen
* &amp;lbrack;UV Entpack&amp;rbrack; Uneinheitliches oder stark verzerrtes Textilverhältnis in einer einzigen UV-Insel in einigen Fällen
* &amp;lbrack;UV Entpack&amp;rbrack; Nicht einheitliches Textilverhältnis zwischen Textursätzen
* &amp;lbrack;UV Entpack&amp;rbrack; Die erzeugte UV-Insel kann sehr lang sein und in manchen Fällen nicht in den UV-Raum passen
* &amp;lbrack;UV Entpack&amp;rbrack; Degenerierte Flächen oder nicht dreieckige Mesh-Flächen mit kleinen oder überlappenden Kanten werden möglicherweise nicht in UV entpackt

### 5.3.2 (2019.3.2)

*(Freigegeben: 21. Januar 2020 (1})Zusammenfassung:**Bugfix***

**Fest:**

* Beim Öffnen eines Projekts, das im Einzelkanalmodus gespeichert wurde, wird der Mesh nicht angezeigt
* Viewport wird beim Malen unter einer Ebene mit dem Kopierwerkzeug nicht immer aktualisiert

**Bekannte Probleme:**

* &amp;lbrack;Baker&amp;rbrack; Absturz im Zusammenhang mit Multithreading auf Ryzen-CPUs
* &amp;lbrack;UV Entpack&amp;rbrack; Die Verarbeitung von Meshs mit hohem Poly-Anteil kann lange dauern
* &amp;lbrack;UV Entpack&amp;rbrack; Scheitelpunkt an exakt denselben Koordinaten werden zusammengeführt
* &amp;lbrack;UV Entpack&amp;rbrack; UV-Generierung kann in seltenen Fällen auf bestimmten Mesh-Komponenten fehlschlagen
* &amp;lbrack;UV Entpack&amp;rbrack; Uneinheitliches oder stark verzerrtes Textilverhältnis in einer einzigen UV-Insel in einigen Fällen
* &amp;lbrack;UV Entpack&amp;rbrack; Nicht einheitliches Textilverhältnis zwischen Textursätzen
* &amp;lbrack;UV Entpack&amp;rbrack; Die erzeugte UV-Insel kann sehr lang sein und in manchen Fällen nicht in den UV-Raum passen
* &amp;lbrack;UV Entpack&amp;rbrack; Degenerierte Flächen oder nicht dreieckige Mesh-Flächen mit kleinen oder überlappenden Kanten werden möglicherweise nicht in UV entpackt

### 5.3.1 (2019.3.1)

*(Freigegeben: 20. Dezember 2019*)Zusammenfassung: **Hotfix**

**Fest:**

* Absturz bei der Arbeit an Meshs mit bestimmten UV-Projektionen
* &amp;lbrack;ABR&amp;rbrack; Absturz beim Wechseln zwischen Photoshop-Vorgaben
* &amp;lbrack;Linux&amp;rbrack; Substance Painter kann unter CentOS 7.4 aufgrund eines libGLX-Abhängigkeitsproblems nicht gestartet werden
* &amp;lbrack;Baker&amp;rbrack; Absturz beim Baking nach Verwendung von &quot;Datei&quot; > &quot;Bereinigen&quot;
* &amp;lbrack;Baker&amp;rbrack; Baking-Fortschrittsdialog friert nach Abbruch ein
* &amp;lbrack;Baker&amp;rbrack; Baking von Mesh nach dem Exportieren von Texturen funktioniert nicht
* &amp;lbrack;Baker&amp;rbrack; Verwenden von &quot;Nach Name abgleichen&quot; mit schwarzen Mesh-Map
* &amp;lbrack;Baker&amp;rbrack; Käfig wird nicht berücksichtigt
* &amp;lbrack;Regal&amp;rbrack; Das Importieren von PSD-Dateien führt zu fehlerhaften Bildern
* &amp;lbrack;Beispiel&amp;rbrack; &quot;Matte&quot;-Beispielprojekt hat fehlerhafte Kameras und falsche Exportvorgabe

**Bekannte Probleme:**

* &amp;lbrack;Baker&amp;rbrack; Absturz im Zusammenhang mit Multithreading auf Ryzen-CPUs
* &amp;lbrack;UV Entpack&amp;rbrack; Die Verarbeitung von Meshs mit hohem Poly-Anteil kann lange dauern
* &amp;lbrack;UV Entpack&amp;rbrack; Scheitelpunkt an exakt denselben Koordinaten werden zusammengeführt
* &amp;lbrack;UV Entpack&amp;rbrack; UV-Generierung kann in seltenen Fällen auf bestimmten Mesh-Komponenten fehlschlagen
* &amp;lbrack;UV Entpack&amp;rbrack; Uneinheitliches oder stark verzerrtes Textilverhältnis in einer einzigen UV-Insel in einigen Fällen
* &amp;lbrack;UV Entpack&amp;rbrack; Nicht einheitliches Textilverhältnis zwischen Textursätzen
* &amp;lbrack;UV Entpack&amp;rbrack; Die erzeugte UV-Insel kann sehr lang sein und in manchen Fällen nicht in den UV-Raum passen
* &amp;lbrack;UV Entpack&amp;rbrack; Degenerierte Flächen oder nicht dreieckige Mesh-Flächen mit kleinen oder überlappenden Kanten werden möglicherweise nicht in UV entpackt

### 5.3.0 (2019.3.0)

*(Freigegeben: 17. Dezember 2019*)Zusammenfassung: **Hauptversion mit Verbesserung der Benutzererfahrung beim Handmalen, Arbeiten mit Tablets, automatischem UV entpack in der Beta-Version (0.3.0) und verschiedenen neuen Inhalten zum Handmalen**

**Hinzugefügt:**

* Integration von Automatic UV entpack 0.3.0 in Substance Painter
* &amp;lbrack;UV entpack&amp;rbrack; Automatische UV entpackend im Substance Painter, wenn keine UVs oder partielle UVs vorhanden sind
* &amp;lbrack;UV entpack&amp;rbrack; Eine globale Einstellung zum Aktivieren und Deaktivieren
* &amp;lbrack;UV entpack&amp;rbrack; In Protokolldatei gemeldete Version
* &amp;lbrack;UV entpack&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Anzeige des Fortschritts beim Entpack der UV
* &amp;lbrack;UI&amp;rbrack; Neue Einstellungen in der kontextabhängigen Symbolleiste zum Auswählen der Pinselvorschau: Vollständige Vorschau, Pinselkontur und Fadenkreuz
* &amp;lbrack;Werkzeug&amp;rbrack; Neuer erweiterter Mischmodus im Alpha-Bereich: Aufhellen (Maximal) zusätzlich zu Normal
* &amp;lbrack;Ebenenstapel&amp;rbrack; Gammakorrekturoption pro Ebene für Alpha oder Maske (Kontextmenü)
* &amp;lbrack;Ebenenstapel&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Symbol &quot;i&quot; hinzufügen, wenn Alpha-Ebene gamma-korrigiert wurde
* &amp;lbrack;Tablet&amp;rbrack;&amp;lbrack;Tool&amp;rbrack; Gelegt Mindestdruck für Größe und Durchfluss
* &amp;lbrack;Tablet&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Neue Einstellung in der kontextabhängigen Symbolleiste, um den Kurvendruck auszuwählen: linear, easy-in, easy-in-out
* &amp;lbrack;Tablet&amp;rbrack;&amp;lbrack;UX&amp;rbrack; Strg- + Alt-Taste + Klicken zum Bildlauf hinzufügen
* Photoshop-Pinselvorgaben importieren (ABR-Format)
* &amp;lbrack;ABR&amp;rbrack; Unterstützen von Shape-Parametern
* &amp;lbrack;ABR&amp;rbrack; Unterstützung von Parametern für die Formdynamik
* &amp;lbrack;ABR&amp;rbrack; Support-Übertragungsparameter
* &amp;lbrack;ABR&amp;rbrack; Unterstützung von Streuungsparametern
* &amp;lbrack;ABR&amp;rbrack;&amp;lbrack;Dynamischen Pinselstriche&amp;rbrack; Rundheit und Spiegelung unterstützen
* &amp;lbrack;ABR&amp;rbrack;&amp;lbrack;Regal&amp;rbrack; Leg der Pinselordnerstruktur im Filtereditor
* &amp;lbrack;ABR&amp;rbrack;&amp;lbrack;Regal&amp;rbrack; Photoshop-Symbol zu Miniaturansichten hinzufügen
* &amp;lbrack;ABR&amp;rbrack;&amp;lbrack;Regal&amp;rbrack; Liste nicht unterstützter Parameter in der detaillierten Miniaturansicht der ABR hinzufügen
* &amp;lbrack;Tool&amp;rbrack;&amp;lbrack;Dynamischen Pinselstriche&amp;rbrack; Neue dynamische Stricheinstellung zur Steuerung der Anzahl der zu erzeugenden Zufallszahlen
* &amp;lbrack;Tool&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Neue Verteilungs- und Achse-Einstellungen für Streuungs-Jitter hinzufügen
* &amp;lbrack;Tastaturbefehl&amp;rbrack; Füge Strg+Umschalt+B hinzu, um das Baking-Fenster zu öffnen.
* &amp;lbrack;UI&amp;rbrack;&amp;lbrack;Menu&amp;rbrack; Eintrag im Menü &quot;Bearbeiten&quot; hinzufügen, um das Baking zu öffnen
* &amp;lbrack;UI&amp;rbrack;&amp;lbrack;Einstellungen&amp;rbrack; Verbesserung der Ausrichtung der Liste der Tastaturbefehle
* &amp;lbrack;UI&amp;rbrack; Drucksteuerelemente (Größe und Fluss) durch Schaltflächen zum Ein- und Ausschalten ersetzen
* &amp;lbrack;Viewport&amp;rbrack; Separates Fokussieren von 2D- und 3D-Viewport zulassen
* Update auf QT 5.12.5
* &amp;lbrack;UI&amp;rbrack; Ladevorgang des Meshs anzeigen
* &amp;lbrack;Substance&amp;rbrack; Zusätzliche Unterstützung für nicht geklemmten und weichen Bereich mit Schiebereglern
* &amp;lbrack;Substance&amp;rbrack; Präzision der Substance-Parameter auf bis zu 6 Dezimalstellen erhöhen
* &amp;lbrack;Substance&amp;rbrack; Berücksichtigung des durch einen Parameter definierten Schritts
* &amp;lbrack;Substance&amp;rbrack; Optimieren der dynamischen Konturgenerierung mit Unterstützung von Bedingungen in Benutzerdaten
* &amp;lbrack;Substance&amp;rbrack; Graphausgabe als Maske für alle Kanäle über Benutzerdaten festlegen
* &amp;lbrack;Inhalt&amp;rbrack; Update &#39;Mat&#39; Beispielprojekt mit Versatz-freundlicher Topologie, neuer ID-Map und neuen Kameras
* &amp;lbrack;Inhalt&amp;rbrack; 3 neue Filter (MatFx) integrieren: Comic-Buch, Aquarell, Öl-Malen (inspiriert von der Arbeit von Emrecan Cubukcu)
* &amp;lbrack;Inhalt&amp;rbrack; 102 Photoshop-Pinselvorgaben aus den Packs von Kyle T. Webster integrieren
* &amp;lbrack;Inhalt&amp;rbrack; 18 neue Pinselvorgaben integrieren: Malen Roller Arrow, Malen Roller Warning text, Charcoal Fine und mehr
* &amp;lbrack;Inhalt&amp;rbrack; 9 neue Alphas integrieren: Brush Maker Malen Roller, Brush Maker Photoshop, Pinselmuster und mehr
* &amp;lbrack;Inhalt&amp;rbrack; 2 neue Werkzeugvorgaben integrieren: Gouache Dense und Gouache Faded
* &amp;lbrack;Inhalt&amp;rbrack; 1 neuen Generator integrieren : UV-Checker (UV-Inseln und Nähte hervorheben)
* &amp;lbrack;Inhalt&amp;rbrack; 2 neue Exportvorgaben integrieren: Keyshot 9+ und Spark AR Studio
* &amp;lbrack;Inhalt&amp;rbrack; 1 neue Projektvorlage integrieren : Spark AR Studio (Facebook)

**Fest:**

* &amp;Klammer;Tablet&amp;Klammer; Das Rückgängigmachen von Stiftstrichen (Strg+Z) hinkt mehr hinterher als das Rückgängigmachen von Mausstrichen
* &amp;Klammer;Tablet&amp;Klammer; Anfangs- und Enddruck werden beim Zeichnen einer Geraden nicht berücksichtigt
* &amp;Klammer;Tablet&amp;Klammer; Erster Stempel wird zweimal gezeichnet, wenn eine gerade Linie verwendet wird
* &amp;Klammer;Tablet&amp;Klammer; Verbesserte Unterstützung für Huion-Tablet-Tastaturbefehle
* &amp;Klammer;Tablet&amp;Klammer; Verbesserte Unterstützung für Huion-Stift-Schaltflächen
* &amp;Klammer;Tablet&amp;Klammer; Versatz zwischen der Pinselvorschau und dem gezeichneten Stempel
* &amp;Klammer;Tablet&amp;Klammer; Verknüpfungen zum Ändern von Pinseln mit Stift führen in seltenen Fällen zu geringer Leistung
* &amp;Klammer;Tablet&amp;Klammer; Verzögerung beim Malen auf einer bestimmten Ebene
* Unscharfe Texturen können in seltenen Fällen beim Wechseln des Viewport auftreten
* &amp;lbrack;UI&amp;rbrack;&amp;lbrack;Substance&amp;rbrack; Bildeingaben werden nicht immer angezeigt
* Beim Bereinigen werden keine Vorgaben aus dem Regal entfernt, die in ein Projekt importiert wurden
* &amp;lbrack;Werkzeug&amp;rbrack;&amp;lbrack;Dynamischer Strich&amp;rbrack; Leistungsproblem beim Anpassen der Stempelzyklusanzahl
* Aktualisierungsprobleme beim Malen im 3D/2D-Viewport in seltenen Fällen
* Wenn Sie einen sehr langen Pinselstrich zeichnen, kann dies zum Einfrieren führen
* &amp;lbrack;Werkzeug&amp;rbrack; Leistungsproblem beim Malen mit bestimmten Dynamischen Pinselstrichen
* &amp;lbrack;UI&amp;rbrack; Kontextsymbolleiste zeigt weiterhin Pinseleigenschaften an, wenn ein Ordner ausgewählt wird
* Werte für die Achse der Symmetrie werden nicht zurückgesetzt
* Import von EXR Texturen mit Fließkommawerten sind komplett schwarz
* Alt+Klicken auf einen Kanal zum Isolieren funktioniert nicht für Filter und Generator
* &amp;lbrack;Export&amp;rbrack; Spezifische Projekt-Absturz beim Exportieren
* &amp;lbrack;Substance&amp;rbrack; Falscher Standardwert in der Dropdown-Liste, wenn der Parameter von Visible If ausgeblendet ist
* &amp;lbrack;Shader&amp;rbrack; Kanäle, die über Material-Ebenen definiert werden, werden in der Benutzeroberfläche nicht gleich sortiert
* &amp;lbrack;Regal&amp;rbrack; Vorgabenmetadaten werden nicht auf dem Datenträger gespeichert

**Bekannte Probleme:**

* &amp;lbrack;UV Entpack&amp;rbrack; Die Verarbeitung von Meshs mit hohem Poly-Anteil kann lange dauern
* &amp;lbrack;UV Entpack&amp;rbrack; Scheitelpunkt an exakt denselben Koordinaten werden zusammengeführt
* &amp;lbrack;UV Entpack&amp;rbrack; UV-Generierung kann in seltenen Fällen auf bestimmten Mesh-Komponenten fehlschlagen
* &amp;lbrack;UV Entpack&amp;rbrack; Uneinheitliches oder stark verzerrtes Textilverhältnis in einer einzigen UV-Insel in einigen Fällen
* &amp;lbrack;UV Entpack&amp;rbrack; Nicht einheitliches Textilverhältnis zwischen Textursätzen
* &amp;lbrack;UV Entpack&amp;rbrack; Die erzeugte UV-Insel kann sehr lang sein und in manchen Fällen nicht in den UV-Raum passen
* &amp;lbrack;UV Entpack&amp;rbrack; Degenerierte Flächen oder nicht dreieckige Mesh-Flächen mit kleinen oder überlappenden Kanten werden möglicherweise nicht in UV entpackt
* Das Metamat-Beispiel hat einige Probleme mit importierten Kameras

### 5.2.3 (2019.2.3)

*(Freigegeben: 23. Oktober 2019*)Zusammenfassung: **Bugfix-Version**

**Hinzugefügt:**

* &amp;lbrack;Textursatz Liste&amp;rbrack; Schaltfläche &quot;Hinzufügen&quot; zum schnellen Aktivieren/Deaktivieren des Fokusmodus
* &amp;lbrack;Log&amp;rbrack; Windows 10-Versionsnummer in die Protokolldatei einfügen
* Aktualisieren Sie auf die neueste Version von Substance Engine
* &amp;lbrack;MacOS&amp;rbrack; Die Software wurde notariell beglaubigt, um die neuen Verteilungsanforderungen von MacOS Catalina zu erfüllen

**Fest:**

* &amp;lbrack;Plugin&amp;rbrack; Plug-In-Quelle funktioniert nicht
* &amp;lbrack;MacOS&amp;rbrack;&amp;lbrack;Shader&amp;rbrack; Mac OS 10.14.5 und AMD: Material-Ebenen funktionieren nicht wie vorgesehen

**Bekannte Probleme:**

* Alembic-Dateien mit Unterteilungen können nicht importiert werden
* Seltene Absturz beim Importieren einiger Alembic-Dateien
* Benutzeroberfläche reagiert beim Baking führ mit DXR auf Pascal-GPUs vorübergehend nicht

### 5.2.2 (2019.2.2)

*(Freigegeben: 20. September 2019*)Zusammenfassung: **Bugfix-Version**

**Fest:**

* Das Importieren von Ressourcen durch Skripterstellung kann zu einem Absturz führen
* &amp;lbrack;Plugin&amp;rbrack; Das Herunterladen des Materials von der Quelle kann zu einem Absturz führen

**Bekannte Probleme:**

* Alembic-Dateien mit Unterteilungen können nicht importiert werden
* Seltene Absturz beim Importieren einiger Alembic-Dateien
* Benutzeroberfläche reagiert beim Baking führ mit DXR auf Pascal-GPUs vorübergehend nicht

### 5.2.1 (2019.2.1)

*(Freigegeben: 17. September 2019 (1})Zusammenfassung:**Bugfix-Version***

**Fest:**

* &amp;lbrack;Mac&amp;rbrack;&amp;lbrack;USD&amp;rbrack; Exportierte USDZ-Dateien aus MacOS können nicht geöffnet werden
* &amp;lbrack;Textursatz&amp;rbrack; Es ist nicht möglich, einen Textursatz mit dem ALT-Modifikator zu isolieren
* &amp;lbrack;Regal&amp;rbrack; Vorgaben, Intelligente Materialien und Intelligente Masken werden beim Beenden der Anwendung immer geändert
* &amp;lbrack;Ebenenstapel&amp;rbrack; Effekt kann nach dem Löschen eines anderen Effekts nicht ausgewählt werden
* Flackern bei Verwendung eines Schiebereglers im Bedienfeld &quot;Werkzeugeigenschaften&quot;
* Absturz beim Exportieren von Vorgaben in Regal
* Absturz beim Exportieren einer Vorgabe mit zu wenig Speicherplatz
* Absturz beim Erstellen einer Vorgabe mit zu wenig Speicherplatz

**Bekannte Probleme:**

* Alembic-Dateien mit Unterteilungen können nicht importiert werden
* Seltene Absturz beim Importieren einiger Alembic-Dateien
* Benutzeroberfläche reagiert beim Baking führ mit DXR auf Pascal-GPUs vorübergehend nicht

### 5.2.0 (2019.2.0)

*(Freigegeben: 25. Juli 2019*)Zusammenfassung: **Hauptversion mit Leistungsaktualisierungen der Baker und einem neuen Vorvisualisierungsmodus + neuem Inhalt**

**Hinzugefügt:**

* &amp;lbrack;Baker&amp;rbrack; Neue Unterstützung für GPU-Raytracing mit DXR und OptiX (Ambient occlusion, Thickness)
* &amp;lbrack;Baker&amp;rbrack; Optimierungen und Beschleunigungen für CPU-Raytracing
* &amp;lbrack;Baker&amp;rbrack;&amp;lbrack;vis mode&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Neuer Baking-Visualisierungsmodus im Viewport
* &amp;lbrack;Baker&amp;rbrack;&amp;lbrack;Voreinstellungen&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Neue Baking-Option zum Aktivieren/Deaktivieren von GPU-Raytracing
* &amp;lbrack;Baker&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Überarbeitung des Dialogfelds &quot;Fortschrittsleiste&quot;
* &amp;lbrack;Baker&amp;rbrack; Verbesserung von Warn- und Fehlermeldungen
* &amp;lbrack;Baker&amp;rbrack; Reaktionsfähigeres Abbrechen des Bakings zulassen
* &amp;lbrack;Baker&amp;rbrack; Baking-Fenster nach Klicken auf &quot;Abbrechen&quot; erneut öffnen
* &amp;lbrack;Proj&amp;rbrack;&amp;lbrack;UX&amp;rbrack; Verbesserte Verwendbarkeit des Manipulators der Drehung
* &amp;lbrack;Einstellungen&amp;rbrack; Option zur Leistungssteigerung durch Reduzierung der Viewport-Auflösung für HDPI-Bildschirme
* &amp;lbrack;Skripterstellung&amp;rbrack; Ändern der Textursatz auflösung
* &amp;lbrack;Skripterstellung&amp;rbrack; Ausgewählten Textursatz abrufen
* &amp;lbrack;Skripterstellung&amp;rbrack; Auswahl eines Textursatzes durch den Benutzer zulassen
* &amp;lbrack;Skripterstellung&amp;rbrack; Funktion, um zu erfahren, wann die Auswahl des Textursatzes geändert wurde
* &amp;lbrack;Regal&amp;rbrack; 40 neue intelligente Materialien hinzugefügt
* &amp;lbrack;Regal&amp;rbrack; 20 neue intelligente Masken hinzugefügt

**Fest:**

* &amp;lbrack;Ebenenstapel&amp;rbrack; Einfrieren der Benutzeroberfläche bei Mehrfachauswahl von Ebenen
* &amp;lbrack;Ebenenstapel&amp;rbrack; Beim Gruppieren vieler Ebenen wird die Benutzeroberfläche länger als gewöhnlich fixiert.
* &amp;lbrack;Ebenenstapel&amp;rbrack; In einigen Fällen können eine Ebene und ein Effekt gleichzeitig ausgewählt werden.
* In Malwerkzeugen verwendete Substance-Graf werden nicht mit der richtigen Auflösung generiert
* &amp;lbrack;Baker&amp;rbrack; Die Schaltfläche &quot;Alle Textursatz Baking geführt&quot; ist nicht deaktiviert, wenn keine Baker ausgewählt sind
* &amp;lbrack;MacOS&amp;rbrack; Warnmeldung zur Tessellation deaktivieren
* Bei Verwendung mit einer Projektion hat das Maskierungswerkzeug keine Vorschau.
* Absturz und beschädigte Projekte beim Speichern mit zu wenig Speicherplatz
* &amp;lbrack;Regal&amp;rbrack; Absturz beim Importieren einer Ressource auf dem Datenträger über ein Regal mit nicht genügend Speicherplatz
* &amp;lbrack;Regal&amp;rbrack; Absturz beim Wiederherstellen der Sitzungsvorgabe
* &amp;lbrack;Regal&amp;rbrack; Das Importieren einer Vorgabe mit einem Namen, der mit einem Leerzeichen endet, führt zu einem Absturz
* &amp;lbrack;Regal&amp;rbrack; Das Importieren einer Ressource mit einem Präfix, das mit einem leeren Leerzeichen endet, führt zu einem Absturz

**Bekannte Probleme:**

* Alembic-Dateien mit Unterteilungen können nicht importiert werden
* Seltene Absturz beim Importieren einiger Alembic-Dateien
* Benutzeroberfläche reagiert beim Baking führ mit DXR auf Pascal-GPUs vorübergehend nicht

### 5.1.3 (2019.1.3)

*(Freigegeben: 1. Juli 2019 (1})Zusammenfassung:**Bugfix mit 2 neuen Funktionen***

**Hinzugefügt:**

* Geben Sie das VRam-Budget über eine Befehlszeile (z. B. —vram-budget 4096)
* &amp;lbrack;QML&amp;rbrack; Leg von wrapMode und elide-Eigenschaften von QML-Schaltflächen und -Kontrollkästchen

**Fest:**

* &quot;Pfad folgen&quot; funktioniert nicht immer
* Kanalzuordnung funktioniert nicht mit SBSAR, das in Ein Kanal-Steckplätzen verwendet wird
* &amp;lbrack;Ebenenstapel&amp;rbrack; Niedrige Leistung beim Scrollen mit ausgeblendeten Ebenen
* &amp;lbrack;TextureSet&amp;rbrack; Absturz beim Klicken zwischen Masken
* &amp;lbrack;SVT&amp;rbrack; Versatz wird nicht richtig angezeigt und flackert in einigen Fällen
* &amp;lbrack;Alembic&amp;rbrack; Absturz mit Mesh, der Punktnormalen anstelle von Scheitelpunkt-Normalen verwendet
* &amp;lbrack;Alembic&amp;rbrack;&amp;lbrack;Log&amp;rbrack; Berichtsfehler im Protokoll, wenn Alembic-Datei während des Imports nicht unterstützt wird

**Bekannte Probleme:**

* Alembic-Dateien mit Unterteilungen können nicht importiert werden
* Seltene Absturz beim Importieren einiger Alembic-Dateien

### 5.1.2 (2019.1.2)

*(Freigegeben: 21. Mai 2019*)Zusammenfassung: **Hotfix**

**Fest:**

* Absturz beim Auswählen von zwei Ressourcen mit einer Bildeingabe

### 5.1.1 (2019.1.1)

*(Freigegeben: 20. Mai 2019*)Zusammenfassung: **Hotfix**

**Hinzugefügt:**

* Aktualisieren Sie auf die neueste Version von Substance Engine mit der letzten Version von Substance Designer 2019.1

**Fest:**

* &amp;lbrack;Substance&amp;rbrack; Visible If wird bei Eingabebildern nicht berücksichtigt
* &amp;lbrack;SVT&amp;rbrack;&amp;lbrack;Engine&amp;rbrack; Das Ändern der Textursatz-Auflösung führt in einigen Fällen zu einem Absturz
* &amp;lbrack;Engine&amp;rbrack; In einigen Fällen werden zufällige schwarze Texturen angezeigt
* &amp;lbrack;Ebenenstapel&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Durch Umschalten einer Maske mit UMSCHALTTASTE können mehrere Ebenen gleichzeitig ausgewählt werden
* &amp;lbrack;Ebenenstapel&amp;rbrack; Deckkraft hat keine Auswirkungen auf den Malen-Effekt mit dem Mischmodus &quot;Hindurchwirken&quot;
* &amp;lbrack;Ebenenstapel&amp;rbrack; Filtereingabe &quot;Height zu Normal&quot; wird mit dem Pinselstrich des Radiergummis nicht richtig aktualisiert
* &amp;lbrack;LayersStack&amp;rbrack; Absturz beim Rückgängigmachen des Abfalls einer intelligente Maske
* Flackerndes Drahtgitter mit aktiviertem temporalem Anti-Aliasing
* &amp;lbrack;Versatz&amp;rbrack; Verzögerung bei AMD mit einigen starken Meshs
* &amp;lbrack;Windows&amp;rbrack; Absturz beim Öffnen einiger Projekte über den Datei-Explorer
* &amp;lbrack;Histogramm&amp;rbrack; Absturz beim Entfernen einer Maske mit Ankerpunkt in einigen Fällen
* Absturz bei der Vorschauerstellung in einigen seltenen Fällen
* &amp;lbrack;Absturz&amp;rbrack; Ein Projekt kann mit zu vielen Klon- und Verwischen-Werkzeugen nicht erneut geöffnet werden
* Nach dem Speichern wird in einigen Fällen kein Mesh im Materialmodi angezeigt
* &amp;lbrack;Skripterstellung&amp;rbrack; alg.mapexport.documentStructure() gibt falsche Werte für Ordner zurück

**Bekannte Probleme:**

* Durch Doppelklicken auf den Namen des Textursatzes wird dieser vor dem Umbenennungsmodus ausgewählt.

### 5.1.0 (2019.1.0)

*(Freigegeben: 23. April 2019*)Zusammenfassung: **Dynamischer Pinselstrich mit eigenem neuen Inhalt, Versatz und Tessellation in Echtzeit und Iray, Effekt &quot;Vergleichsmaske&quot;, Radiale Symmetrie, Planar und Sphärische Projektion**

**Hinzugefügt:**

* &amp;lbrack;Werkzeug&amp;rbrack; Dynamischer Strich: Substance-Variation entlang eines Pinselstrichs
* &amp;lbrack;Dynamischer Strich&amp;rbrack; Leg eines neuen Stempelindexparameters mit Optionen
* &amp;lbrack;Dynamischer Strich&amp;rbrack; $time-Parameter berücksichtigen
* &amp;lbrack;Dynamischer Strich&amp;rbrack; Neuen Parameter $randomseed pro Strich und Stempel generieren
* &amp;lbrack;Dynamischer Strich&amp;rbrack; Dynamischen Strichindex aus einer zufälligen Zahl beginnen
* &amp;lbrack;Dynamischer Strich&amp;rbrack;&amp;lbrack;Regal&amp;rbrack; Hilfe bei der Suche nach einer dynamischen Konturressource mit eigenem neuen Symbol
* Versatz und Tessellation im Echtzeit-Viewport
* Versatz und Tessellation in Iray
* &amp;lbrack;Shader-Einstellungen&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Neue Registerkarte zur Steuerung von Versatz und Tessellation
* &amp;lbrack;Ebenenstapel&amp;rbrack; Neuer Effekt &quot;Maske vergleichen&quot;: durch Vergleich zweier Kanäle eine Maske generieren
* &amp;lbrack;Ebenenstapel&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Neuer Eintrag im Rechtsklick-Menü &quot;Height mit Maskenkombination hinzufügen&quot;, um einen CompareMask-Effekt einzufügen
* &amp;lbrack;Symmetrie&amp;rbrack; Neuer Symmetrie-Modus: Radialmalerei
* &amp;Symmetrie&amp;rbrack;Einstellungen&amp;rbrack; Erweitern Sie beide Abschnitte &quot;Einstellungen&quot; und &quot;Anzeige&quot;
* &amp;lbrack;Symmetrie&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Vorschau für radiales Malen
* Leg zweier neuer Modi für die Projektion: planar und kugelförmig
* &amp;lbrack;Proj&amp;rbrack; Neuer Formzuschneidemodus für alle Projektionen
* &amp;lbrack;Proj&amp;rbrack; Planarer Modus mit neuem Manipulator: Oberflächenwerkzeug
* &amp;lbrack;Proj&amp;rbrack;&amp;lbrack;Tastaturbefehl&amp;rbrack; Tastaturbefehl UMSCHALTTASTE+W für Oberflächenwerkzeug
* &amp;lbrack;Proj&amp;rbrack; Planare Maskierung von Projektionen mit Tiefe ausblenden und Rückseiten-Ausblendung
* &amp;lbrack;Manipulator&amp;rbrack; Verbesserung des Manipulators der Drehung auf allen drei Achsen für triplanare
* &amp;lbrack;Tool&amp;rbrack;&amp;lbrack;UX&amp;rbrack; Alt-Klick auf einen Kanal fokussiert diesen Kanal (aktiviert ihn oder deaktiviert alle anderen)
* &amp;lbrack;Engine&amp;rbrack; Aktualisieren Sie auf die neueste Version von Substance Engine
* &amp;lbrack;Textursatz&amp;rbrack; Mehrfachauswahl und Änderung der Auflösung
* &amp;lbrack;Textursatz&amp;rbrack; Schnelle Aktivierung und Deaktivierung der Textursatz
* &amp;lbrack;Textursatz&amp;rbrack; Einzelne und alle Optionen zu einem neuen Menü kombinieren
* &amp;lbrack;Textursatz&amp;rbrack;&amp;lbrack;Ebenenstapel&amp;rbrack; Neues Symbol für die Aktivierung und Deaktivierung
* &amp;lbrack;Ebenenstapel&amp;rbrack;&amp;lbrack;UX&amp;rbrack; Einfügen von Effekten über den bereits ausgewählten
* &amp;lbrack;Ebenenstapel&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Auswahlstil für die Ebenenstapel-Ansicht überarbeiten
* &amp;lbrack;Ebenenstapel&amp;rbrack; Der Mischmodus für instanzierte Ebenen ist jetzt standardmäßig im Durchlaufmodus
* &amp;lbrack;Export&amp;rbrack; Option zum Aktivieren und Deaktivieren von Dithering
* &amp;lbrack;Plugin&amp;rbrack; Präzisionsmodifikator für Schieberegler unterstützen (SHIFT)
* &amp;lbrack;Plugin&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Neues Symbol für automatisches Speichern
* &amp;lbrack;Skripterstellung&amp;rbrack; Auflisten des Inhalts eines Ordners
* &amp;lbrack;Skripterstellung&amp;rbrack; Löschen von Dateien zulassen
* &amp;lbrack;Skripterstellung&amp;rbrack; Lesen aller Stapel-Informationen, einschließlich der verwendeten Ressourcen
* &amp;lbrack;Inhalt&amp;rbrack;&amp;lbrack;Dynamischer Strich&amp;rbrack; Neue Tools und Pinselvorgaben
* &amp;lbrack;Inhalt&amp;rbrack;&amp;lbrack;Dynamischer Strich&amp;rbrack; Zwei neue prozedurale Farbverläufe: Farbton und Verlaufsgenerator
* &amp;lbrack;Inhalt&amp;rbrack; 11 neue Filter: MatFx Peeling Malen, MatFx Wassertropfen und mehr
* &amp;lbrack;Inhalt&amp;rbrack; 7 neue Generatoren: &quot;Auto-Stitcher&quot;, &quot;UV-Zufallsfarbe&quot;, &quot;UV-Texeldichte&quot; und weitere Eigenschaften
* &amp;lbrack;Inhalt&amp;rbrack; 93 neue Alphas: neue Texte, Pfeile und verschiedene andere Formen
* &amp;lbrack;Inhalt&amp;rbrack; 2 neue Verfahren: Verlaufsfarbton, Verlaufsgenerator und mehr
* &amp;lbrack;Inhalt&amp;rbrack; 21 neue Tools und Pinselvorgaben für Dynamische Pinselstriche: Kiesel, Fußabdrücke, Spray und mehr
* &amp;lbrack;Inhalt&amp;rbrack; 2 Neue HDRs: Canopus Boden- und Herbstwald
* &amp;lbrack;Inhalt&amp;rbrack; Aktualisieren von Inhalten mit Kuration nach dem Zufallsprinzip in Regal
* &amp;lbrack;Inhalt&amp;rbrack; Neues Symbol mit gelegt Zufallsparameter in Regal

**Fest:**

* &amp;lbrack;Ebenen Stapel&amp;rbrack; Ebenenstapel wird unendlich lang.
* &amp;lbrack;Mac&amp;rbrack; &quot;Im Finder anzeigen&quot; kann zum Einfrieren führen
* &amp;lbrack;Skripterstellung&amp;rbrack; Einstellungen, die über die benutzerdefinierte Benutzeroberfläche gespeichert wurden, gehen verloren, wenn die Shader-Datei verschoben wird
* &amp;lbrack;Skripterstellung&amp;rbrack; Die API-Versionsnummer ist falsch und nicht aktuell.
* &amp;blase;Effekt&amp;blase; Histogramminhalt wird nicht korrekt angezeigt
* &amp;blase;Effekt&amp;blase; Histogrammeffekt wird in einigen Fällen nicht aktualisiert
* &amp;lbrack;Regal&amp;rbrack; Die Nähte sind auf dem Material &quot;Plastic Fabric Pyramide&quot; nicht richtig ausgerichtet.

**Bekannte Probleme:**

* Durch Doppelklicken auf den Namen des Textursatzes wird dieser vor dem Umbenennungsmodus ausgewählt.
* &amp;lbrack;Ebenenstapel&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Durch Umschalten einer Maske mit UMSCHALTTASTE können mehrere Ebenen gleichzeitig ausgewählt werden

## Version 4

### 4.3.3 (2018.3.3)

*(Freigegeben: 07. März 2019*)Zusammenfassung: **Bugfix**

**Hinzugefügt:**

* &amp;lbrack;Inhalt&amp;rbrack; Neue Projektvorlage integrieren: &quot;PBR - Metallische Rauheit Alpha-blend&quot;
* Die Suchreihenfolge der dynamischen Linux-Bibliothek wurde geändert, um Bibliotheken im Installationsverzeichnis Priorität einzuräumen, bevor sie auf dem System installiert werden.

**Fest:**

* Mesh verschwindet manchmal vom 3D-Viewport (drücken Sie F, um die Kamera zurückzusetzen)
* Aktualisieren des Substance Painter Sketchfab-Uploaders mit den neuen Sketchfab-Lizenztypen
* &amp;lbrack;Import&amp;rbrack;&amp;lbrack;glTF&amp;rbrack; Falsche Handhabung der Modulation der Eingabe-Textur wie in glTF-Dateien definiert
* &amp;lbrack;Import&amp;rbrack;&amp;lbrack;glTF&amp;rbrack; Boden-Ebene wird beim glTF-Import in einigen Fällen falsch angezeigt
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;USD&amp;rbrack; Deckkraft funktioniert nicht in Arkit
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;USD&amp;rbrack; ABSTURZ beim USDz-Export in einigen Fällen
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;USD&amp;rbrack; Exportieren in USD ohne Speichern führt zu Absturz
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;USD&amp;rbrack; Ungültiger Kachelung-Modus für Texturen, Unterteilungsmodus für Mesh und Ausgabetypen für Shader
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;USD&amp;rbrack; Wenig Exporte von nur einigen Textursätzen mit allen Geometrien
* &amp;lbrack;Instanz&amp;rbrack; Absturz beim Löschen einer beschädigten Instanzebene
* &amp;lbrack;Regression&amp;rbrack;&amp;lbrack;Export&amp;rbrack; Einige Maps werden nicht in die ausgewählte Bittiefe exportiert
* &amp;lbrack;Linux&amp;rbrack; Problem mit der Bibliothek libtbb.so.2

**Bekannte Probleme:**

* Einfrieren der Berechnung in einigen Fällen auf AMD VEGA-GPUs
* Problem mit Huion-Tablets mit Tastaturbefehlen unter Windows

### 4.3.2 (2018.3.2)

*(Freigegeben: 24. Januar 2019*)Zusammenfassung: **Hotfix mit neuen Funktionen (USDZ-Export- und Textur-Filterungen im Viewport)**

**Hinzugefügt:**

* &amp;lbrack;Export&amp;rbrack; Export nach USDZ zulassen
* &amp;lbrack;Viewport&amp;rbrack; Zulassen, um die Qualität der Textur in den Anzeigeeinstellungen zu steuern
* &amp;lbrack;Viewport&amp;rbrack; Die Einstellung für die MIP-Voreinstellung in den Anzeigeeinstellungen wurde hinzugefügt.
* &amp;lbrack;Viewport&amp;rbrack; Anisotrope Filterung in den Anzeigeeinstellungen hinzugefügt
* &amp;lbrack;plugins&amp;rbrack; Offizielle Plug-ins auf Substance Painter 2018 aktualisieren
* &amp;lbrack;Lizenz&amp;rbrack; Lizenz standardmäßig in einem Benutzerordner installieren

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
* &amp;lbrack;Skripterstellung&amp;rbrack; Dateipfaderstellung beim Speichern eines Projekts nicht erzwungen
* &amp;lbrack;Skripterstellung&amp;rbrack; Der Rückruf von &quot;onProjectAboutToSave()&quot; funktioniert nicht mehr
* Fehlerhafte Links im Fenster &quot;Fehler melden&quot;

**Bekannte Probleme:**

* Einfrieren der Berechnung in einigen Fällen auf AMD VEGA-GPUs
* Problem mit Huion-Tablets mit Tastaturbefehlen unter Windows

### 4.3.1 (2018.3.1)

*(Freigegeben: 06. Dezember 2018*)Zusammenfassung: **Hotfix**

**Hinzugefügt:**

* &amp;lbrack;Symmetrie&amp;rbrack;&amp;lbrack;Viewport&amp;rbrack; Die Symmetrie in der 2D-Ansicht ist wieder da und zeigt nun eine Vorschau des Klonpinsels an.

**Fest:**

* &amp;lbrack;Export&amp;rbrack; Beim Exportieren der 2D-Ansicht wird in einigen Fällen eine schwarze Textur ausgegeben
* &amp;lbrack;Iray&amp;rbrack; Normale Informationen werden im Iray falsch, nachdem eine Material-Ebene instanziiert wurde
* Nicht quadratische Textursatz können in einigen Fällen zu Absturz führen
* &amp;lbrack;Rückgängig&amp;rbrack; Mehrere Strg+Z können in einigen Fällen zufällig zu Absturz führen
* &amp;lbrack;QML&amp;rbrack; AlgScrollView kann in einigen Fällen eine Warnung im Protokoll erstellen (Bindungsschleifen).

**Bekannte Probleme:**

* Einfrieren der Berechnung in einigen Fällen auf AMD VEGA-GPUs
* Problem mit Huion-Tablets mit Tastaturbefehlen unter Windows
* Glätten und Schatten können bei gemeinsamer Verwendung zu unerwarteten Ergebnissen führen

### 4.3.0 (2018.3.0)

*(Freigegeben: 20. November 2018*)Zusammenfassung: **Viewport-Upgrades, ordnungsgemäßer Datenexport, neue UI-Helfer, ein erweitertes Symmetrie-Tool, neue 2D-Ansichten und eine enorme Leistungssteigerung**

**Hinzugefügt:**

* &amp;lbrack;Glätten&amp;rbrack;&amp;lbrack;Viewport&amp;rbrack; Neue temporale Anti-Aliasing-Filterungen für 3D-Viewport (über Anzeigeeinstellungen)
* &amp;lbrack;Export&amp;rbrack; Exportieren des Inhalts des 2D-Viewports als eine Textur
* &amp;lbrack;Export&amp;rbrack;&amp;lbrack;Dithering&amp;rbrack; Gelegt Ditheringe bei der Ausfuhr
* &amp;lbrack;Ebenenstapel&amp;rbrack; Farben auf Ebenen und Ordnern
* &amp;lbrack;Ebenenstapel&amp;rbrack; Schnelle Aktivierung und Deaktivierung mehrerer Ebenen und Effekte
* &amp;lbrack;Ebenenstapel&amp;rbrack; Einfachere Navigation für Füllmethoden dank Tasten nach oben und Mausbildlauf
* &amp;lbrack;Proj&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Zusätzlicher Dreh-Manipulator auf allen drei Achsen für Triplanar
* &amp;lbrack;proj&amp;rbrack;&amp;lbrack;Shorcuts&amp;rbrack; - und + , um die Größe des Manipulators für die UV-Projektion zu ändern
* &amp;lbrack;Shader&amp;rbrack; Kontrolle der Schichtparameter mit Kanälen im PBR-beschichteten Shader
* &amp;lbrack;Substance&amp;rbrack; Leg neuer Mesh-basierter Texturen für Filter und Generatoren
* &amp;lbrack;Symmetrie&amp;rbrack;&amp;lbrack;Viewport&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Steuern des Offsets der Symmetrie mit Manipulatoren
* &amp;lbrack;Symmetrie&amp;rbrack;&amp;lbrack;Kontextsymbolleiste&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Neues Bedienfeld &quot;Symmetrie&quot; mit Optionen
* &amp;lbrack;Symmetrie&amp;rbrack; Neuer Schnittmodus für Symmetrien-Linien
* &amp;lbrack;Symmetrie&amp;rbrack; Neuer Symmetrie-Clone-Cursor
* &amp;lbrack;Symmetrie&amp;rbrack;&amp;lbrack;Shortcuts&amp;rbrack; Q zum Ausblenden und -, + zum Ändern der Größe und Umschalttaste zum einrasten
* &amp;lbrack;Log&amp;rbrack; Fehlermeldungen verbessern, wenn Texturen nicht exportiert werden können
* &amp;lbrack;Skripterstellung&amp;rbrack; Ressourcen in den Anzeigeeinstellungen ändern oder aktualisieren
* &amp;lbrack;Skripterstellung&amp;rbrack; Erstellen oder Entfernen von Kanälen in Textursätzen zulassen
* &amp;lbrack;Content&amp;rbrack;&amp;lbrack;Shaders&amp;rbrack; Unterstützung für Anisotropie mit einem dedizierten Shader hinzufügen (pbr-metal-rau-Anisotropie-angle)
* &amp;lbrack;Inhalt&amp;rbrack; Aktualisierung der Vorschaukugel mit Anisotropie und verändertem Winkel
* &amp;lbrack;Inhalt&amp;rbrack; Aktualisierte matFx Shutline
* &amp;lbrack;Inhalt&amp;rbrack; Neuer nahtloser Fläche-Scan von Texturing.XYZ
* &amp;lbrack;Inhalt&amp;rbrack; Neue anisotrope Verfahren
* &amp;lbrack;Inhalt&amp;rbrack; Neuer Filter: Umgebung mit vorberechnete Beleuchtung
* &amp;lbrack;Inhalt&amp;rbrack; Neue Umgebungs-Map: Studio Automotive Neutral
* &amp;lbrack;Inhalt&amp;rbrack; Neue Projektvorlage: PBR - metallische Rauheit Anisotropy angle (mit Anisotropie-Kanälen)
* &amp;lbrack;Inhalt&amp;rbrack; Neue Projektvorlage: PBR - mit metallische Rauheit beschichtet
* &amp;lbrack;SVT&amp;rbrack;&amp;lbrack;Engine&amp;rbrack; Dünn besetzte virtuelle Texturen (SVT)
* &amp;lbrack;SVT&amp;rbrack;&amp;lbrack;Preferences&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Beschleunigungsoption für SVT-Hardware-Unterstützung
* &amp;lbrack;SVT&amp;rbrack;&amp;lbrack;Log&amp;rbrack; Zusätzliche Informationen zur Funktion &quot;Virtuelle Texturierung mit geringer Dichte&quot; (z. B. Festplatte in Größe)
* &amp;lbrack;SVT&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Meldungsfenster beim Start, wenn die Größe auf dem Datenträger für den Cache zu niedrig ist
* &amp;lbrack;SVT&amp;rbrack;&amp;lbrack;Preferences&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Globaler Substance Painter-Cachespeicherort
* &amp;lbrack;SVT&amp;rbrack; Neue Umgebungsvariable zur Angabe des Cachepfads des Substance Painters
* &amp;lbrack;SVT&amp;rbrack; Neue Umgebungsvariable zum Aktivieren der SVT-Hardware-Support-Beschleunigung
* &amp;lbrack;SVT&amp;rbrack; Erkennen von geringer Hardware-Unterstützung
* &amp;lbrack;SVT&amp;rbrack;&amp;lbrack;Hardware Sparse&amp;rbrack; Erhöhen der Mindesttreiberversion für Nvidia-GPU
* &amp;lbrack;SVT&amp;rbrack;&amp;lbrack;Shader&amp;rbrack;&amp;lbrack;Viewport&amp;rbrack;&amp;lbrack;UI&amp;rbrack; Benutzer warnen, wenn bei Projektöffnung Artefakte mit virtueller Texturierung mit geringer Dichte vorhanden sind

**Fest:**

* &amp;Klammer;Farbwähler&amp;Klammer; Beim Auswählen einer Farbe wird der Cursor angezeigt.
* Absturz durch das Auswählen oder Aufheben der Auswahl von Ebenen in einer bestimmten Reihenfolge kann zu Absturz führen
* Absturz beim Einfügen einer Ebene mit einer Maske als Instanz
* &amp;lbrack;Benutzerkanal&amp;rbrack;&amp;lbrack;Regression&amp;rbrack; Absturz beim Umbenennen des Benutzerkanals
* &amp;lbrack;Benutzerkanal&amp;rbrack; Graue Pinselvorschau
* &amp;lbrack;Alembic&amp;rbrack; Nur ein Textursatz aus mehreren Materialien nach dem Import
* &amp;lbrack;Engine&amp;rbrack; Die exportierte Textur unterscheidet sich vom Viewport für Pinselstempel
* &amp;lbrack;Engine&amp;rbrack; Die Umkehrung mit einem Ebeneneffekt wirkt sich nicht vollständig auf eine Textur aus
* Die Material-Auswahl wendet beim Auswählen einen Pinselstrich an
* Der Wechsel der Auflösung auf 128 x 128 px führt zu einem Absturz
* Mesh-Map-Verknüpfungen werden beim Umbrechen oder Instanziieren von Ebenen nicht ordnungsgemäß aktualisiert
* &amp;lbrack;Substance&amp;rbrack; UserData ColorSpace funktioniert nicht bei Baking geführt Mesh Normal, der als Eingabe angefordert wird
* MDL-Zuordnungskonflikt bei Verwendung mehrerer Shader-Instanzen
* &amp;lbrack;Symmetrie&amp;rbrack;&amp;lbrack;Füllebene&amp;rbrack; Symmetrie-Ebene und ihr in der Füllebene aktiver Manipulator
* &amp;lbrack;Viewport&amp;rbrack; Pivot-Punkt für Übersetzung wird nach dem Klicken nicht immer aktualisiert
* &amp;lbrack;UI&amp;rbrack; Behobene Symbole und Entfernen von Platzhaltern für HDPI-Monitore

**Bekannte Probleme:**

* Einfrieren der Berechnung in einigen Fällen auf AMD VEGA-GPUs
* Problem mit Huion-Tablets mit Tastaturbefehlen unter Windows
* Glätten und Schatten können bei gemeinsamer Verwendung zu unerwarteten Ergebnissen führen

### 4.2.3 (2018.2.3)

*(Freigegeben: 25. September 2018)*

**Fest:**

* &amp;lbrack;2D-Ansicht&amp;rbrack; Beim Erstellen eines neuen Projekts ist die 2D-Ansicht mit einigen Meshs beschädigt
* &amp;lbrack;Absturz&amp;rbrack; Der Wechsel von der UV-Projektion zur planaren Projektion führt zu einem Absturz
* &amp;lbrack;RayCollider&amp;rbrack; Mehrere Absturz durch &quot;RayCollider&quot;
* &amp;lbrack;Werkzeug&amp;rbrack; Beim Wechseln von Ebenen gehen die geänderten Pinseleigenschaften verloren
* Pinseleinstellungen werden beim Wechsel zum Radierer zurückgesetzt

**Bekannte Probleme:**

* Einfrieren der Berechnung auf AMD VEGA-GPUs
* Problem mit Huion-Tablets mit Tastaturbefehlen unter Windows

### 4.2.2 (2018.2.2)

*(Freigegeben: 11. September 2018 (1})Zusammenfassung:**Hotfix mit Inhaltsaktualisierung, neuen Skriptfunktionen und der Möglichkeit, das automatische Update zu deaktivieren***

**Hinzugefügt:**

* &amp;lbrack;Inhalt&amp;rbrack;&amp;lbrack;Regal&amp;rbrack; Hinzufügen einer Skin-Regal-Vorgabe
* &amp;lbrack;Inhalt&amp;rbrack;&amp;lbrack;Regal&amp;rbrack; Konvertierung von 19 Hautnormalen in Materialien zur Volumenstreuung
* &amp;lbrack;Skripterstellung&amp;rbrack; Erstellen einer Projektvorlage aus einem geöffneten Projekt
* &amp;lbrack;Skripterstellung&amp;rbrack; Exporteinstellungen eines geöffneten Projekts abrufen/festlegen
* &amp;lbrack;Updates&amp;rbrack; Deaktivieren des Popups &quot;Automatische Aktualisierung&quot; unter &quot;Einstellungen&quot; und &quot;Umgebungsvariable&quot;
* &amp;lbrack;Updates&amp;rbrack; Nicht bis zur nächsten Version auf dem Popup-Fenster mit veralteten Wartungsoptionen anzeigen

**Fest:**

* &amp;lbrack;Kamera&amp;rbrack; Falscher Zoom durch Wechsel von orthografisch zu Perspektive
* &amp;lbrack;Anzeige&amp;rbrack; Einige Maps werden linear anstatt sRGB angezeigt
* &amp;lbrack;Viewport&amp;rbrack; Mesh-Fokus verhält sich nicht richtig
* &amp;lbrack;2D-Ansicht&amp;rbrack; Bei einem Projekt mit beschädigter Kamera werden UVs-Schalen ausgeblendet.
* &amp;lbrack;SSS&amp;rbrack;&amp;lbrack;Tooltip&amp;rbrack; QuickInfos zu Volumenstreuungen werden im Protokoll angezeigt
* Einige Projekte können nicht in 2018.2 geöffnet werden und die Fehlermeldung kann kein Null-Substance-Paket speichern
* &amp;lbrack;Maske&amp;rbrack; Die Farbe des Malen-Werkzeugs kann beim Arbeiten in einer Maske in einigen Fällen hängen bleiben
* &amp;lbrack;Material&amp;rbrack; Karten werden in bestimmten Situationen nicht angezeigt
* &amp;lbrack;Proj&amp;rbrack;&amp;lbrack;Tools&amp;rbrack; Generatoraktiver Manipulator
* &amp;lbrack;Substance&amp;rbrack; Fehlende Substance-Parametergruppen
* &amp;lbrack;Skripterstellung&amp;rbrack; Falscher Software-Name in der Dokumentation
* &amp;lbrack;UDIM&amp;rbrack; Keine Informationen im Protokoll über UVs-Schalen auf mehreren UVs-Kacheln

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

*(Freigegeben: 02. August 2018*)Zusammenfassung: **Sommerversion, Volumenstreuung-Support, Verbesserungen bei Projektion und Füllung, Kamera-Import und -Auswahl, Alembic- und glTF-Unterstützung, Drag-and-Drop auf dem ID-Map, verbesserte Unterstützung für Substance-Formate und neue Inhalte**

**Hinzugefügt:**

* &amp;lbrack;SSS&amp;rbrack;&amp;lbrack;Viewport&amp;rbrack;&amp;lbrack;Iray&amp;rbrack; Generische Volumenstreuung
* &amp;lbrack;SSS&amp;rbrack; MDL- und Volumenstreuung-Parameter synchronisieren
* &amp;lbrack;SSS&amp;rbrack; Es wurde ein neuer Graustufenkanal mit dem Namen &quot;Streuung&quot; hinzugefügt.
* &amp;lbrack;SSS&amp;rbrack;&amp;lbrack;Shader Settings&amp;rbrack; Streutypparameter für die Volumenstreuung (Skin oder transluzent)
* &amp;lbrack;SSS&amp;rbrack;&amp;lbrack;Shader Settings&amp;rbrack; Streuskalenparameter für die Volumenstreuung
* &amp;lbrack;SSS&amp;rbrack;&amp;lbrack;Shader Settings&amp;rbrack; Farbstreuung-Parameter für Volumenstreuung
* &amp;lbrack;SSS&amp;rbrack;&amp;lbrack;Anzeigeeinstellungen&amp;rbrack; Streuung Sampleanzahl für Volumenstreuung
* &amp;lbrack;Shader&amp;rbrack;&amp;lbrack;Iray&amp;rbrack; Volumenstreuung MDL für Iray integrieren
* &amp;lbrack;Shader&amp;rbrack; Shader-Update über den Ressourcen-Updater
* &amp;lbrack;Shader&amp;rbrack; API und Dokumentation für Änderungsprotokoll aktualisieren
* &amp;lbrack;Werkzeugeigenschaften&amp;rbrack;&amp;lbrack;Proj&amp;rbrack; Neue Parameter für die triplanare Projektion
* &amp;lbrack;Viewport&amp;rbrack;&amp;lbrack;Proj&amp;rbrack; Steuern von Ansichtseigenschaften in 3D direkt mit Manipulatoren (Füllebene)
* &amp;lbrack;Shortcuts&amp;rbrack;&amp;lbrack;Proj&amp;rbrack; Neue Tastaturbefehle Q, W, E, R, T für triplanare Projektion-Manipulator
* &amp;lbrack;Viewport&amp;rbrack;&amp;lbrack;Proj&amp;rbrack; Steuern von Eigenschaften der Füllebene in 2D-Ansichten direkt über Manipulator (UV-Projektion)
* &amp;lbrack;Shortcuts&amp;rbrack;&amp;lbrack;Proj&amp;rbrack; Neuer Tastaturbefehl Q für UV-Projektion Manipulator
* &amp;lbrack;Kontextsymbolleiste&amp;rbrack;&amp;lbrack;Proj&amp;rbrack; Manipulator der triplanare Projektion steuern
* &amp;lbrack;Kontextsymbolleiste&amp;rbrack;&amp;lbrack;Proj&amp;rbrack; Manipulator der UV-Projektion steuern
* &amp;lbrack;Werkzeugeigenschaften&amp;rbrack; Kachelung der Textur mit dem Werkzeug &quot;Projektion und Schablone&quot; deaktivieren
* &amp;lbrack;Schablone&amp;rbrack; Verwenden von Nicht-quadratischen Bildern mit dem Projektion-Werkzeug/der Schablone
* &amp;lbrack;Schablone&amp;rbrack; Kachelung im Eigenschaftenfenster zulassen
* &amp;lbrack;Schablone&amp;rbrack; Der Zoom ist nicht auf einer Schablone ohne Kachelung zentriert
* &amp;blbrack;Kameras&amp;rbrack; Kameras importieren aus Maya, Max, Blender, Modo, DAE
* &amp;lbrack;Kameras&amp;rbrack;&amp;lbrack;Viewport&amp;rbrack; Auswählen und Steuern importierter Kameras in Viewport
* &amp;lbrack;Kameras&amp;rbrack;&amp;lbrack;Iray&amp;rbrack; Auswählen und Steuern importierter Kameras in Iray
* &amp;lbrack;Kameras&amp;rbrack;&amp;lbrack;UI&amp;rbrack;&amp;lbrack;Neues Projekt&amp;rbrack;&amp;lbrack;Projektkonfiguration&amp;rbrack; Kameras importieren ist standardmäßig aktiviert
* &amp;lbrack;Kameras&amp;rbrack;&amp;lbrack;Shortcuts&amp;rbrack; Hinzufügen von Tastaturbefehlen zum Wechseln zwischen Kameras
* &amp;lbrack;Kameras&amp;rbrack;&amp;lbrack;Viewport&amp;rbrack; Rahmen zu Viewport hinzufügen
* &amp;lbrack;Kameras&amp;rbrack;&amp;lbrack;Viewport-Einstellungen&amp;rbrack; Kontrolle der Deckkraft des Rahmens
* &amp;lbrack;Kameras&amp;rbrack;&amp;lbrack;Kamera&amp;rbrack; Maximale Brennweite bei 500mm
* &amp;lbrack;Kameras&amp;rbrack;&amp;lbrack;Kamera&amp;rbrack; Leg Ratio
* &amp;lbrack;Kameras&amp;rbrack;&amp;lbrack;Kamera&amp;rbrack; Option &quot;Sperren&quot; hinzufügen
* &amp;lbrack;Kameras&amp;rbrack;&amp;lbrack;Kamera&amp;rbrack; Hinzufügen einer Wiederherstellungsoption
* &amp;lbrack;Kameras&amp;rbrack;&amp;lbrack;Kamera&amp;rbrack; Attribut &quot;Fokusabstand&quot; hinzufügen
* &amp;lbrack;glTF&amp;rbrack; Importieren einer glTF-Datei
* &amp;lbrack;glTF&amp;rbrack; Importieren einer ambient occlusion-Map
* &amp;lbrack;Alembic&amp;rbrack; Alembic 1-Rahmen mit statischer Geometrie importieren
* &amp;lbrack;Regal&amp;rbrack; Ziehen Sie Materialien mithilfe von ID-Map mit einem Modifizierer (STRG/Befehlstaste) direkt auf den Mesh
* &amp;lbrack;Ebenenstapel&amp;rbrack; Automatische Erstellung von ID-Masken durch Ziehen und Ablegen von Materialien auf einem Mesh mit ID-Map
* &amp;lbrack;Ebenenstapel&amp;rbrack; Automatischer Bildlauf von Ebenen per Drag &amp; Drop über den Ebenenstapel
* &amp;lbrack;UI&amp;rbrack;&amp;lbrack;Werkzeugeigenschaften&amp;rbrack; Leg Substance&#39;s preset
* &amp;lbrack;UI&amp;rbrack;&amp;lbrack;Hilfemenü&amp;rbrack; Verbesserung des Hilfemenüs
* &amp;lbrack;UI&amp;rbrack;&amp;lbrack;Neues Projekt&amp;rbrack;&amp;lbrack;Projektkonfiguration&amp;rbrack; Neuorganisation des Fensters
* &amp;lbrack;UI&amp;rbrack;&amp;lbrack;Neues Projekt&amp;rbrack;&amp;lbrack;Projektkonfiguration&amp;rbrack; Mesh durch Datei ersetzen
* &amp;lbrack;UI&amp;rbrack;&amp;lbrack;Substance&amp;rbrack; Anzeigen von Substance-Attributen in der Benutzeroberfläche
* &amp;blbrack;Shortcuts&amp;rbrack; F4 wechselt zwischen 2D- und 3D-Ansicht
* &amp;blbrack;Shortcuts&amp;rbrack; Neue Tastaturbefehle zum Umschalten zwischen Schablone N und schnelle Maske U
* &amp;lbrack;Substance-Integration&amp;rbrack; Berücksichtigung von &#39;visible if&#39;-Anweisungen in den Substance-Parametern
* &amp;lbrack;Viewport&amp;rbrack; Schatten, die nach dem Verschieben der Kamera nicht berechnet werden müssen
* &amp;lbrack;Inhalt&amp;rbrack; Aktualisieren von MeetMat mit importierten Kameras
* &amp;lbrack;Inhalt&amp;rbrack; Beispiel mit aktivierter Volumenstreuung hinzufügen - JadeToad
* &amp;lbrack;Inhalt&amp;rbrack; Neue PBR-Projektvorlage mit aktivierter Volumenstreuung hinzufügen
* &amp;lbrack;Inhalt&amp;rbrack; Exportvorgaben wurden aktualisiert, um einen neuen Streuungskanal hinzuzufügen
* &amp;lbrack;Inhalt&amp;rbrack;&amp;lbrack;Regal&amp;rbrack; Unterstützung zusätzlicher Volumenstreuungen für: pbr-metal-rau, pbr-metal-rau-alpha-test, pbr-coated, pbr-spec-gloss
* &amp;lbrack;Inhalt&amp;rbrack;&amp;lbrack;Regal&amp;rbrack; Hinzugefügter Streuungskanal zu 5 intelligenten Materialien (Marmor und Skins)
* &amp;lbrack;Inhalt&amp;rbrack;&amp;lbrack;Regal&amp;rbrack; 1 neues Jade-Material
* &amp;lbrack;Inhalt&amp;rbrack;&amp;lbrack;Regal&amp;rbrack; 1 neues Wachs-Material

**Fest:**

* &amp;lbrack;CMD&amp;rbrack; Verschiedene Ergebnisse bei Verwendung derselben Befehlszeile mit unterschiedlichen Versionen
* &amp;lbrack;TDR&amp;rbrack; Wenn TdrLevel eingerichtet ist, sind keine Fehler im Protokoll vorhanden.
* &amp;lbrack;Baker&amp;rbrack; Ambient occlusion-Map wird gespiegelt
* &amp;lbrack;ID-Map&amp;rbrack; Absturz beim Kommissionieren außerhalb des 0-1-Bereichs
* &amp;lbrack;Iray&amp;rbrack; Absturz beim Wechseln des Textursatzes und beim Wechseln in den Malen-Modus
* &amp;lbrack;Viewport&amp;rbrack; Synchronisieren von Ablagebereichen zwischen Viewporten für Drag &amp; Drop
* &amp;lbrack;Engine&amp;rbrack; Moiré-Artefakt bei der Kachelung von Füllebenen oder beim Malen mit einem kleinen Pinsel
* &amp;lbrack;Lizenz&amp;rbrack; Prüfung auf fehlerhafte Softwareversion des Lizenzdienstes
* &amp;lbrack;Lizenz&amp;rbrack; Verarbeitung der Authentifizierungsmethode anpassen
* &amp;lbrack;API&amp;rbrack; Rufen Sie das onNewProjectCreated-Skript-API-Ereignis auf, selbst wenn Sie mit einer Vorlage erstellen.
* &amp;lbrack;Shader&amp;rbrack; Kompilierter Shader wird nicht aus dem Cache geladen, wenn die Shader-Datei nicht kompiliert wird
* &amp;lbrack;Regal&amp;rbrack; Beim Exportieren der HDR aus dem Regal wird eine Datei mit geklemmten Werten ausgegeben
* &amp;lbrack;Export&amp;rbrack; EXR-Exportklammern RGB von Farbwerten zwischen 0 und 1
* &amp;lbrack;Inhalt&amp;rbrack; Prozedurales Rauschen 3D Perlin Rauschen Fraktal ist verpixelt

**Bekannte Probleme:**

* Einfrieren der Berechnung auf AMD VEGA-GPUs
* Problem mit Huion-Tablets mit Tastaturbefehlen unter Windows

### 4.1.3 (2018.1.3)

*(Freigegeben: 28. Juni 2018)*

**Hinzugefügt:**

* &amp;lbrack;Voreinstellungen&amp;rbrack; Projekt beim Neustart von Painter speichern

**Fest:**

* &amp;lbrack;Plugin&amp;rbrack; Die Substance Source &quot;Suchen&quot; funktioniert nicht
* &amp;Intelligenten Materials&amp;rbrack; Das Importieren von Intelligente Materialien führt in einigen Fällen zu einem Absturz
* &amp;Intelligenten Materials&amp;rbrack; Das Löschen von Intelligenten Materialien führt in einigen Fällen zu einem Absturz
* &amp;lbrack;Speichern&amp;rbrack; Das Speichern führt in einigen seltenen Fällen zu einem Absturz
* &amp;lbrack;Regal&amp;rbrack; Umkehren funktioniert nicht auf Zellen 2 und Zellen 3
* &amp;lbrack;Regal&amp;rbrack; Typo in einigen Alphas
* &amp;lbrack;Regal&amp;rbrack; Einige Substance-Material werden nicht richtig gerendert

**Bekannte Probleme:**

* Einfrieren der Berechnung auf AMD VEGA-GPUs

### 4.1.2 (2018.1.2)

*(Freigegeben: 12. Juni 2018*)Zusammenfassung: **Verbesserte Wiedergabegeschwindigkeit, verbessertes Speichersystem, aktualisierte Schieberegler, aktualisierte Plug-in-API, chinesische Baking, verbesserter Abstand jetzt optional**

**Hinzugefügt:**

* &amp;lbrack;Baker&amp;rbrack; Leistungsverbesserung mit der neuen Baker-Version
* Erzwungene Anzeige von Dialogfeldern mit inkompatibler GPU
* &amp;lbrack;Speichern&amp;rbrack; Leg der neuen Funktion für kompakte Projekte (Speichermodus &quot;Voll/Kompakt&quot;)
* &amp;lbrack;Speichern&amp;rbrack; Benutzer im Fall eines Speicherfehlers informieren
* &amp;lbrack;Clean&amp;rbrack; Nächstes Speichern im Voll-/Kompaktmodus
* &amp;blase;Regler&amp;blase; Verbesserung der Präzision der Farb-/Graustufenbalken und -schieberegler
* &amp;blase;Regler&amp;blase; Hinzufügen von Nach-oben-/Nach-unten-Steuerelementen
* &amp;blase;Regler&amp;blase; Dieselbe Erkennungszone für Farb- und Graustufenbalkenschieberegler
* &amp;lbrack;Plugin&amp;rbrack; Automatisches Speichern immer im inkrementellen Modus
* &amp;lbrack;Plugin&amp;rbrack; Option zum Wechseln von Plug-ins zu einem neuen Schnittstellenstil
* &amp;lbrack;Sprache&amp;rbrack; Chinesische Übersetzung hinzufügen
* &amp;Klammer;Auffüllung&amp;Klammer; Option zum Wechseln zwischen UV- und 3D-Raum, Nachbar-Innenabständen pro Textursatz in den Textursatz-Einstellungen
* &amp;lbrack;Script&amp;rbrack; Gelegt Speichermodus: Voll/Kompakt oder inkrementell
* &amp;lbrack;Script&amp;rbrack; Aktualisieren von Skripterstellung/QML-Dokumentation
* &amp;lbrack;Log&amp;rbrack; Anzeige des Speichermodus im Protokoll (vollständig/kompakt oder inkrementell)

**Fest:**

* &amp;lbrack;Werkzeug&amp;rbrack; Bei Einkanalfüllungen transformieren der Kanalsteckplatz in einen Material-Steckplatz ein
* Absturz beim Laden eines Meshs (FBX) mit einigen Flächen, die nicht von einem Material zugewiesen wurden
* Absturz in Iray mit NVIDIA RASTER 5.2 auf einem virtuellen Computer
* Absturz beim Rückgängigmachen eines Löschens einer Materialvorgabe
* Absturz beim Laden einiger Projekte
* &amp;lbrack;Befehlszeile&amp;rbrack; Neue Befehlszeile für UDIM-Mesh, aufgeteilt nach Audio
* &amp;blbrack;Symbolleiste&amp;rbrack; Verkleinern der Symbolleiste
* &amp;lbrack;Instancing&amp;rbrack; Bitmaps können nicht auf mehreren Textursätzen instanziieren werden
* &amp;lbrack;Viewport&amp;rbrack; Die Aktualisierung ist beim Malen auf Mesh mit gekachelten UVs nicht abgeschlossen
* &amp;lbrack;Iray&amp;rbrack; Normalen-Map wird zweimal für Dielektrika angewendet
* &amp;lbrack;Regal&amp;rbrack; Typos in einigen Substance-Parametern (Alphas, Prozedurals und Matfx)
* &amp;lbrack;Regal&amp;rbrack; Typo für die Bitmap &quot;Nur autorisiertes Personal&quot;
* &amp;lbrack;Script&amp;rbrack; Die Funktion alg.shaders.Materials() funktioniert nicht mehr

**Bekannte Probleme:**

* Einfrieren der Berechnung auf AMD VEGA-GPUs

### 4.1.1 (2018.1.1)

*(Freigegeben: 03. April 2018)*

**Fest:**

* &amp;Klammer;Tablet&amp;Klammer; Problem beim Ändern der Standardinteraktionsoptionen
* &amp;lbrack;Baker&amp;rbrack; Absturz mit Assimp-Bibliothek
* &amp;lbrack;Baker&amp;rbrack; Leistungsrückgang mit A.O.-Karte
* &amp;lbrack;Iray&amp;rbrack; Die Verzerrung der Linse wird nicht auf den Alphakanal angewendet
* &amp;lbrack;Treiber&amp;rbrack; Aktualisierung der Mindestanforderungen für Treiber
* &amp;lbrack;3Dview&amp;rbrack; Normale werden auf UDIM-Meshs ohne Normale nicht korrekt generiert
* &amp;lbrack;Intel&amp;rbrack; Absturz mit Substance Painter 2018.1.0
* &amp;lbrack;Intel&amp;rbrack;&amp;lbrack;Viewport&amp;rbrack; Problem mit Innenabständen (schwarze Artefakte)

**Bekannte Probleme:**

* Einfrieren der Berechnung auf AMD VEGA-GPUs

### 4.1.0 (2018.1.0)

*(Freigegeben: 15. März 2018)*

**Hinzugefügt:**

* Neuer allgemeiner Stil (Symbole, Farbe, Verhalten)
* Neues Standardlayout
* &amp;Klammer;Tablet&amp;Klammer; Verbessertes Benutzererlebnis beim Malen
* &amp;lbrack;Hauptmenü&amp;rbrack; Sortieren Sie native Elemente zuerst in Ansichten und Symbolleisten
* &amp;lbrack;Hauptmenü&amp;rbrack; Aktionen &quot;schnelle Maske verschieben&quot; im Abschnitt &quot;Viewport&quot;
* &amp;lbrack;Hauptmenü&amp;rbrack; Rechtsklickaktionen in den Abschnitt &quot;Viewport&quot; verschieben
* &amp;lbrack;Hauptmenü&amp;rbrack; Menü &quot;Ansicht&quot; in &quot;Fenster&quot; umbenennen
* &amp;lbrack;Schnellmenü&amp;rbrack; Neue Werkzeugeigenschaften durch Rechtsklick im Viewport
* &amp;lbrack;Andocken-Widget&amp;rbrack; Neue Dock-Symbolleiste für schnelles Reduzieren/Zurückrufen
* &amp;lbrack;Anzeigeeinstellungen&amp;rbrack; Fenster &quot;Kamera- und Anzeigeeinstellungen&quot; wurde zusammengeführt
* &amp;lbrack;Ebenenstapel&amp;rbrack; Kontextmenü durch Rechtsklick
* &amp;lbrack;Ebenenstapel&amp;rbrack; Verschieben Sie jeden Effekt innerhalb derselben Ebene per Drag &amp; Drop
* &amp;blbrack;Symbolleiste&amp;rbrack; Neuanordnung der Symbolleiste und neue kontextbezogene Symbolleiste
* &amp;Klammer;Werkzeugleiste&amp;Klammer; Klonwerkzeug in zwei separate Werkzeuge teilen
* &amp;lbrack;Werkzeugeigenschaften&amp;rbrack; Hellerer Graustufenwert im Hintergrund in der Vorschau
* &amp;lbrack;Werkzeugeigenschaften&amp;rbrack; Organisation auf Registerkarten (Ausfüllen und Werkzeuge)
* &amp;lbrack;Werkzeug&amp;rbrack; Das Malergebnis entspricht der Schablone
* &amp;lbrack;Viewport&amp;rbrack; Neuer Cursor für Füllebene
* &amp;lbrack;Viewport&amp;rbrack; Einfachere Navigation und besseres Malen (höhere Rahmen-Rate)
* &amp;lbrack;Viewport&amp;rbrack; Kombinationsfeld &quot;Material-/Kanal-/Kartenauswahl&quot; im Viewport
* &amp;lbrack;Viewport&amp;rbrack; Flackern beim Drehen reduzieren (Schatten aktiviert)
* &amp;lbrack;Regal&amp;rbrack; Beim Öffnen von Painter standardmäßig Materials anzeigen
* &amp;lbrack;Regal&amp;rbrack; Ladezeitverbesserung von Substance-Texturen und Materialien (2- bis 6-mal schneller)
* &amp;lbrack;Regal&amp;rbrack; Materialien-Ordner an die Struktur einer Substance Source anpassen
* &amp;lbrack;Regal&amp;rbrack; Ziehen Sie Materialien per Drag &amp; Drop direkt auf den Mesh im Viewport
* &amp;lbrack;Regal&amp;rbrack; Neue 3D-Rauschen (Perlin, Perlin Fraktal, Simplex und Worley)
* &amp;lbrack;Regal&amp;rbrack; Neuer 3D Linear gradient-Maskengenerator mit Mesh-Position
* &amp;lbrack;Regal&amp;rbrack; Die Basis-Rauschen wurden aktualisiert, um quadratische Ausbreitung zu unterstützen
* &amp;lbrack;Regal&amp;rbrack; Neue Vorlage und Exportvoreinstellung für Lens Studio hinzugefügt (Einrasten Anwendung)
* &amp;lbrack;Regal&amp;rbrack; Intelligenten Materials und Intelligente Masken wurden aktualisiert, um die neueste Version des Maskeneditors zu verwenden (Mikrodetails)
* &amp;lbrack;Regal&amp;rbrack; Neues Beispielprojekt &quot;TilingMaterial&quot; zum Erstellen nahtloser Kachelung-Material
* &amp;lbrack;Regal&amp;rbrack; Neue Pinselvorgaben (Kalligrafie, Nass, Schraffur usw.)
* &amp;blase;Regler&amp;blase; Neue Schieberegler und Stil und Verhalten von Graustufen-/Farbbalken
* &amp;lbrack;Baker&amp;rbrack; Erlauben Sie die Verwendung des Begrenzungsrahmens für die volle Szene, um die Positionskarte zu berechnen.
* &amp;lbrack;Shader&amp;rbrack; Height Force-Parameter aus den Standard-Shader-Parametern entfernen
* &amp;lbrack;Engine&amp;rbrack; Substance Engine aktualisiert
* &amp;lbrack;Engine&amp;rbrack; Keine oder weniger Diskontinuitäten zwischen UV-Abschnitten
* &amp;lbrack;Plugins&amp;rbrack; Schnelleres Importieren von aus Substance Source heruntergeladenen Materials
* &amp;lbrack;Plugins&amp;rbrack; Alle Plug-ins entsprechend dem neuen Stil aktualisieren
* &amp;lbrack;Voreinstellungen&amp;rbrack; Automatische Vorschau der Hintergrundfarbänderungen
* &amp;lbrack;Clean&amp;rbrack; Geringeres Risiko für Projektbeschädigung
* &amp;lbrack;Open&amp;rbrack; Zeitverbesserung für das Öffnen des Projekts
* &amp;lbrack;Neues Projekt&amp;rbrack; Neues Projekt - Verbesserung der Aktualisierungszeit des Meshs
* &amp;lbrack;Speichern&amp;rbrack; Zeitersparnis bei Projekten
* &amp;lbrack;Log&amp;rbrack; Im Protokoll gemeldeter Lizenztyp
* &amp;lbrack;TextureSet&amp;rbrack; Die Schaltfläche &quot;Baking-Texturen&quot; in &quot;Baking-Mesh-Map&quot; umbenennen
* Benennen Sie &quot;Zusätzliche Maps&quot; in &quot;Mesh-Map&quot; um

**Fest:**

* &amp;lbrack;Viewport&amp;rbrack; Fehlerhafte Bewegungen bei Meshs, die viele Unterobjekte enthalten
* &amp;lbrack;Werkzeugeigenschaften&amp;rbrack; Kanal deaktiviert, wenn ein Material per Drag &amp; Drop in den Bildschlitz gezogen wird
* &amp;lbrack;Werkzeugeigenschaften&amp;rbrack; Pinselvorschau ist bei Verwisch- und Kopierwerkzeugen defekt
* &amp;lbrack;Textursatz&amp;rbrack; Die Reihenfolge der Kanäle ist falsch, wenn Vorlagen verwendet werden
* &amp;lbrack;Regal&amp;rbrack; Fehlendes Symbol für den Graustufenkonvertierungen-Generator
* &amp;lbrack;Regal&amp;rbrack; Alpha-Zeichen-Kreisnummer ist defekt (fehlende Schriftart)
* Falsche Erkennung integrierter GPUs beim Start
* &amp;lbrack;Absturz&amp;rbrack; Ziehen und Ablegen einer importierten Ressource mit dem Namen &quot;#&quot;
* &amp;lbrack;Engine&amp;rbrack; Problem mit der VRAM-Erkennung bei integrierter GPU
* &amp;lbrack;Engine&amp;rbrack; Mehrere Absturz im Substance Engine Linker behoben
* &amp;lbrack;Engine&amp;rbrack; Quadratische Artefakte bei der Änderung der Auflösung
* &amp;lbrack;Post-Effekte&amp;rbrack; Die Größe der Benutzeroberfläche ist langsam, wenn Post-Effekte aktiviert sind
* &amp;lbrack;Baker&amp;rbrack; Szene-Einheit wird bei Strahlenabstandswerten nicht korrekt eingehalten
* &amp;lbrack;Baker&amp;rbrack; AO vom Mesh Verdeckungsabstand wird unabhängig vom Eingangswert auf 1 geklemmt
* &amp;lbrack;Baker&amp;rbrack; Bei &quot;Nach Name suchen&quot; werden einige Mesh mit bestimmten Namen ignoriert
* &amp;lbrack;Baker&amp;rbrack; Die Farbe aus den Einstellungen &quot;Mesh-Polygruppe&quot; und &quot;Teilgitter-ID&quot; gibt immer ein schwarzes Bild zurück.
* &amp;lbrack;Baker&amp;rbrack; ID-Baking schlägt mit binären FBX Meshs aus Blender fehl
* &amp;lbrack;Shader&amp;rbrack; Rauschen in der 2D-Ansicht mit dota-2 und non-pbr-spec-gloss
* &amp;lbrack;Linux&amp;rbrack; Beim Baking wird nur ein CPU-Thread verwendet
* &amp;lbrack;MacOS&amp;rbrack; Absturz mit dem Pinselcursor, der sich über den Viewport bewegt

**Bekannte Probleme:**

* Einfrieren der Berechnung auf AMD VEGA-GPUs
* Verzerrungsnachbearbeitung wird beim Export in Iray nicht berücksichtigt (Alpha)

## Version 3

### 3.4.2 (2017.4.2)

*(Freigegeben: 24. Januar 2018)*

**Hinzugefügt:**

* &amp;lbrack;Export&amp;rbrack; Abrufen des Status eines Exports mit Schrittfortschritt
* &amp;lbrack;Export&amp;rbrack; Abbrechen eines Exports zulassen
* &amp;lbrack;Export&amp;rbrack; Exportieren von Texturen nach Sketchfab ohne Qualitätsverlust beim Normalen-Map
* &amp;lbrack;Export&amp;rbrack; Exportieren im glTF-Binärformat (glb)
* &amp;lbrack;Export&amp;rbrack; Größenänderung der Spalten auf der Registerkarte &quot;Konfiguration&quot; des Exportfensters zulassen
* &amp;lbrack;Shader&amp;rbrack; Hinzufügen eines Änderungsprotokolls für den Shader-API
* &amp;lbrack;Skripterstellung&amp;rbrack; Vorher- und Nachher-Rückruffunktionen beim Exportieren von Texturen hinzufügen
* &amp;lbrack;Iray&amp;rbrack; Upgrade auf SDK 2017.1 (Unterstützung für Volta-GPUs)

**Fest:**

* Absturz beim Beenden der Anwendung, bevor das Hauptfenster angezeigt wird
* &amp;lbrack;MAC&amp;rbrack; Absturz beim Laden von Graustufenkarten mit IRAY
* &amp;lbrack;MAC&amp;rbrack; VRAM Erkennung ist mit dem neuen Betriebssystem High Sierra nicht korrekt
* &amp;lbrack;Plugin&amp;rbrack; Das Herunterladen von Assets aus Substance Source funktioniert nicht mehr
* &amp;lbrack;Skripterstellung&amp;rbrack; Falsche Erkennung der Mindestversion des Plug-ins
* &amp;lbrack;Export&amp;rbrack; Nach dem Exportieren von Texturen kann die Exportvorgabe nicht gespeichert werden
* &amp;lbrack;Instancing&amp;rbrack; Problem bei Generatoren, die in einem TextureSet ohne zusätzliche Karten instanziieren wurden
* &amp;lbrack;Viewport&amp;rbrack; Dithering funktioniert nicht mit einer Auflösung über 4k
* &amp;lbrack;Viewport&amp;rbrack; 2D-Ansicht Material-Display ist mit Rauschen überzogen
* &amp;lbrack;Regal&amp;rbrack; Verbessern der Ladezeit für Regal-Vorgaben
* &amp;lbrack;Engine&amp;rbrack; Falsche Füllmethode beim Malen unter Farbauswahl

### 3.4.1 (2017.4.1)

*(Freigegeben: 15. Dezember 2017)*

**Hinzugefügt:**

* &amp;lbrack;Skripterstellung&amp;rbrack; Exportieren von Mesh über die Scripting-API
* &amp;lbrack;Import&amp;rbrack; Import nicht unterstützter Meshdateien deaktivieren (nur obj, fbx, date, play zulassen)
* &amp;lbrack;Log&amp;rbrack; Präzisere Angabe des TDR-Problems in der Protokolldatei

**Fest:**

* Absturz, wenn die Anwendung geschlossen wird, bevor das Crawlen der Ressourcen abgeschlossen ist
* Absturz beim Öffnen von Projekten mit dem Verwischen-/Klon-Werkzeug
* Absturz bei der Verwendung von &quot;redo&quot; nach einem Rückgängigmachen einer Shader-Änderung in den Anzeigeeinstellungen
* &amp;lbrack;Engine&amp;rbrack; Die Texturierung unterscheidet sich zwischen Painter 2017.2 und 2017.4
* &amp;lbrack;Viewport&amp;rbrack; Wenn Sie eine ID-Map aus einer Instanz auswählen, wird die falsche Farbe aufgenommen.
* &amp;lbrack;Export&amp;rbrack; Absturz beim Exportieren einer ungültigen Normal- oder Verdeckung-Textur
* &amp;lbrack;Export&amp;rbrack; Beim Öffnen von PSD-Dateien in Photoshop CS6 sind die Gruppen gesperrt
* &amp;lbrack;Plugin&amp;rbrack; Photoshop-Plugin ignoriert die Kanalauswahl und exportiert immer alles
* &amp;lbrack;Layers&amp;rbrack; Ankerpunkte werden beim Kopieren/Einfügen über Textursatz hinweg umgebrochen
* &amp;lbrack;Layers&amp;rbrack; Einige Ankerreferenzen können nicht wiederhergestellt werden, wenn sie beschädigt sind
* &amp;lbrack;Shader&amp;rbrack; pbr-beschichteter Parameter für sekundäre Rauheit ist defekt
* &amp;lbrack;Steam&amp;rbrack; Das Popup zur Versionsprüfung sollte beim Start nicht sichtbar sein

**Bekannte Probleme:**

* &amp;lbrack;AMD&amp;rbrack; Absturz/Einfrieren beim Malen auf einem Mesh. Kann mit einem GPU-Treiber-Update behoben werden.

### 3.4.0 (2017.4.0)

*(Freigegeben: 23. November 2017)*

**Hinzugefügt:**

* &amp;lbrack;Instancing&amp;rbrack; Parameter über Ebenen hinweg instanziieren
* &amp;lbrack;Instancing&amp;rbrack; Wechsel zwischen Quellebene und Instanz zulassen
* &amp;lbrack;Instancing&amp;rbrack; Aktion &quot;instanziieren zwischen Textursätzen&quot; hinzufügen
* &amp;lbrack;Instancing&amp;rbrack; Geben Sie im Ebenenstapel wieder eintretende Instanzen (Zyklen) an.
* &amp;lbrack;Instancing&amp;rbrack; Instanzen löschen, wenn eine Quelle entfernt wird
* &amp;lbrack;Instancing&amp;rbrack; Ankerverweise von außerhalb eines instanzierten Ordners nicht zulassen
* &amp;lbrack;UI&amp;rbrack; Den Stapel &quot;Rückgängig&quot; in ein eigenes Fenster mit dem Namen &quot;Verlauf&quot; verschieben
* &amp;lbrack;Plugin&amp;rbrack; DCC-Live-Link-Plug-in integrieren
* &amp;lbrack;Engine&amp;rbrack; Verbessern der Malleistung mit Sparse-Malerei
* &amp;lbrack;Export&amp;rbrack; Optionen für Entwürfe und Re-Exporte für Sketchfab-Exporter hinzufügen
* &amp;lbrack;Regal&amp;rbrack; Hinzufügen einer &quot;Spiegeln&quot;-Steuerung für Schriftsubstanzen
* &amp;lbrack;Regal&amp;rbrack; 20 neue Prozeduren hinzufügen - Materials
* &amp;lbrack;Regal&amp;rbrack; 40 neue Grunges Maps hinzufügen (Bitmap-basiert und prozedural)
* &amp;lbrack;Viewport&amp;rbrack; Kollisionen in der Pinselvorschau auf anderen sichtbaren Textursätzen aktivieren
* Mindestanforderungen für AMD GPU-Treiber aktualisieren

**Fest:**

* Absturz Beim Berechnen von Substance mit zu großen Auflösungen
* Absturz beim Malen mit Partikeln
* &amp;lbrack;Viewport&amp;rbrack; Falsche Specular-Spiegelung in der 2D-Ansicht mit bestimmten Meshs
* &amp;lbrack;UI&amp;rbrack; Im Verlaufsfenster werden einige unerwünschte Aktionen angezeigt

**Bekannte Probleme:**

* &amp;lbrack;Layers&amp;rbrack; Einige Ankerreferenzen können nicht wiederhergestellt werden, wenn sie beschädigt sind
* Absturz bei der Verwendung von &quot;redo&quot; nach einem Rückgängigmachen einer Shader-Änderung in den Anzeigeeinstellungen

### 3.3.3 (2017.3.3)

*(Freigegeben: 1. Dezember 2017)*

**Fest:**

* &amp;lbrack;Steam&amp;rbrack; Das Popup zur Versionsprüfung sollte beim Start nicht sichtbar sein
* &amp;lbrack;Export&amp;rbrack; Beim Öffnen von PSD-Dateien in Photoshop CS6 sind die Gruppen gesperrt

### 3.3.2 (2017.3.2)

*(Freigegeben: 20. November 2017)*

**Hinzugefügt:**

* &amp;lbrack;UI&amp;rbrack; Dialogfeld &quot;Neue Version verbessern&quot; und Änderungsprotokoll hinzufügen
* &amp;lbrack;UI&amp;rbrack; Anzeigen, ob die Wartung im Dialogfeld &quot;Neue Version&quot; abgelaufen ist
* &amp;lbrack;Lizenz&amp;rbrack; Lizenzsystem aktualisieren, um Wartungsdaten zu verarbeiten
* &amp;lbrack;Export&amp;rbrack; Adobe Standard Material in Adobe Dimension umbenennen

**Fest:**

* &amp;lbrack;Mac&amp;rbrack; Malen führt zu schwarzen Quadraten und beschädigten Texturen
* &amp;lbrack;Engine&amp;rbrack; Der Zwischenspeicher kann manchmal im Viewport verschwinden
* &amp;lbrack;Engine&amp;rbrack; Blockige Artefakte werden angezeigt, wenn der Speicherkomprimierungsauslöser aktiviert wird
* &amp;blbrack;Baking&amp;rbrack; Seltsame Fehlermeldungen beim Baking bestimmter Mesh
* &amp;lbrack;Export&amp;rbrack; PSD werden falsch geschrieben und von Photoshop nicht richtig erkannt
* &amp;lbrack;Layers&amp;rbrack; Ebenen sollten nicht projektübergreifend kopiert/eingefügt werden können.
* &amp;lbrack;Substance&amp;rbrack; UserData-Farbraum für normale Eingabe wird in einigen Fällen gespiegelt
* &amp;lbrack;Regal&amp;rbrack; Mikronormal in Generatoren gibt invertierte Krümmung aus
* &amp;lbrack;Regal&amp;rbrack; HSL beeinflussen auch den Alphakanal
* &amp;lbrack;Linux&amp;rbrack; Installation auf Centos schlägt aufgrund fehlender Abhängigkeiten fehl
* Das Installationsprogramm entfernt in bestimmten Fällen nicht alle Ressourcen aus der vorherigen Installation

### 3.3.1 (2017.3.1)

*(Freigegeben: 26. Oktober 2017)*

**Hinzugefügt:**

* &amp;lbrack;Export&amp;rbrack; Exportieren des Meshs aus einem Projekt zulassen
* &amp;lbrack;Regal&amp;rbrack; &quot;Sub-Regal&quot; aus den Registerkartentiteln entfernen
* Einstellungen für die Nachbearbeitung in Vorlagen speichern
* Die TDR-Meldung verständlicher machen
* Fenster &quot;Einstellungen&quot; verbessern, um Fehler zu melden

**Fest:**

* Absturz beim Löschen mehrerer untergeordneter Regal
* Absturz beim Wechsel von einer Ebene zu einer anderen während einer Engine-Berechnung
* &amp;lbrack;Mac&amp;rbrack; Absturz auf der Intel-GPU während der Engine-Berechnungen
* &amp;lbrack;Mac&amp;rbrack;&amp;lbrack;Viewport&amp;rbrack; Fehlerhafte Leistung, wenn Dithering aktiviert ist
* &amp;lbrack;Mac&amp;rbrack; MacOS 10.13 wird in der Protokolldatei als &quot;Unbekannte Version&quot; erkannt
* &amp;lbrack;Baker&amp;rbrack; Das Baking führ mit einem Käfig funktioniert nicht mehr
* &amp;lbrack;Layers&amp;rbrack; Strg + C Tastaturbefehl (Aktion kopieren) funktioniert nicht mehr
* &amp;lbrack;Layers&amp;rbrack; Beim Einfügen von Ebenen wird die Benutzeroberfläche mit Ankerreferenzen nicht aktualisiert
* &amp;lbrack;Anker&amp;rbrack; Duplizieren oder Kopieren/Einfügen der Ebene mit Referenzen hebt Verknüpfungen auf
* &amp;lbrack;Export&amp;rbrack; 8K-Export kann Absturz oder Deadlock-Anwendung in einigen Fällen
* &amp;lbrack;Export&amp;rbrack; Mehrere Probleme im generierten glTF-Dateiformat
* &amp;lbrack;Import&amp;rbrack; Das erneute Importieren eines Meshs mit demselben Dateinamen funktioniert nicht mehr
* &amp;lbrack;Plugin&amp;rbrack; Fenster zum automatischen Speichern wird immer über allem angezeigt
* &amp;lbrack;UI&amp;rbrack; Endlose Schleife, wenn Sie im TDR-Dialog &quot;Escape&quot; drücken
* &amp;lbrack;UI&amp;rbrack; UI zum Zurücksetzen zeigt eine zweite Titelleiste im Fenster &quot;Regal&quot; an

### 3.3.0 (2017.3.0)

*(Freigegeben: 28. September 2017)*

**Hinzugefügt:**

* &amp;lbrack;Export&amp;rbrack; Exportieren von Mesh und Texturen für Adobe Project Felix zulassen
* &amp;lbrack;Export&amp;rbrack; Export in das glTF-Dateiformat zulassen
* &amp;lbrack;Engine&amp;rbrack; Optimieren der Größe von Texturen in VRAM mithilfe der Blockkomprimierung
* &amp;lbrack;Viewport&amp;rbrack; Ziehen und Ablegen eines Meshs oder Projekts im Viewport
* &amp;lbrack;UI&amp;rbrack; Verbesserung der Warnmeldungen über TDR
* &amp;lbrack;UI&amp;rbrack; Das Protokoll sollte nur auf Anfrage angezeigt werden.
* &amp;lbrack;UI&amp;rbrack; Inhalt des Protokollfensters löschen
* &amp;lbrack;UI&amp;rbrack; Warnungen und Fehler in der Statuszeile anzeigen
* &amp;lbrack;UI&amp;rbrack; Registerkarten oben wie in Webbrowsern anzeigen
* &amp;lbrack;UI&amp;rbrack; Verbesserung des &quot;nicht bemalbaren&quot; Kontexts und der Botschaft
* &amp;lbrack;UI&amp;rbrack; Aktion &quot;Als Kopie speichern&quot; im Dateimenü hinzufügen
* &amp;lbrack;Ebene&amp;rbrack; Die Standardeinstellung für die Kachelung auf 1 festlegen
* &amp;lbrack;Regal&amp;rbrack; Verbesserter Verlaufsfilter zur Unterstützung von 10 dynamischen Farben
* &amp;lbrack;Regal&amp;rbrack; Fügen Sie ein Leerzeichen in der Standardabfrage des Mini-Regals hinzu
* &amp;lbrack;Regal&amp;rbrack; Hinzufügen einer Aktion &quot;Im Explorer öffnen&quot; für lokale Ressourcen im Regal
* &amp;lbrack;Regal&amp;rbrack; Vorlage und Shader für Adobe Material Standard hinzufügen (Project Felix)
* &amp;lbrack;Regal&amp;rbrack; Erhöhen der maximalen Kachelung auf 128 in Material-Ebenenschattierungen
* &amp;lbrack;Regal&amp;rbrack; Hinzugefügte Krümmung für Mikrodetails der Maskengenerator
* &amp;lbrack;Plugin&amp;rbrack; Plug-in zum automatischen Speichern mit anpassbarem Zeitintervall hinzufügen
* &amp;lbrack;Skripterstellung&amp;rbrack; Funktion &quot;Als Kopie speichern&quot; hinzufügen

**Fest:**

* &amp;lbrack;UI&amp;rbrack; Layout wird beim ersten Start unterbrochen
* &amp;lbrack;Export&amp;rbrack; Beim Export generierter PSD weist Formatfehler auf
* &amp;lbrack;Export&amp;rbrack; EXR exportiert immer 8-Bit-Höhen-Map
* &amp;lbrack;Export&amp;rbrack; Absturz beim Exportieren beschädigter zusätzlicher Maps
* &amp;lbrack;Import&amp;rbrack; Harte Kanten werden bei niedrigen Poly-Meshs in einigen Fällen nicht beibehalten
* &amp;lbrack;Import&amp;rbrack; Verbesserte Fehlermeldungen beim Importieren von Meshs mit Problemen
* &amp;lbrack;Baker&amp;rbrack; ID-Map-Baking schlägt fehl, wenn &quot;Nach Name abgleichen&quot; aktiviert ist
* &amp;lbrack;Viewport&amp;rbrack; Tangente-Speicherplatz wird nicht mit Bakern synchronisiert
* &amp;blase;Effekt&amp;blase; Das Zurückverschieben einer Ebene stellt die Referenz eines Ankers nicht wieder her
* &amp;blase;Effekt&amp;blase; Problem beim Aktualisieren beim Erstellen einer Verknüpfung zwischen zwei Masken mit Ankern
* &amp;blase;Effekt&amp;blase; Maskenanker über der Maske sollten nicht aufgeführt werden
* &amp;blase;Effekt&amp;blase; &quot;Alpha aus Ankerpunkten extrahieren&quot; funktioniert nicht
* &amp;lbrack;Engine&amp;rbrack; Maske kehrt sich nach dem ersten Pinselstrich um
* &amp;lbrack;Engine&amp;rbrack; Absturz beim Wechseln des Textursatzes zu einem bestimmten Projekt
* &amp;lbrack;Regal&amp;rbrack; Absturz beim Löschen einer Vorgabe, die sich in einem Projekt befindet
* &amp;lbrack;Regal&amp;rbrack; Typo in erweitertem Tri-Planarem Filter
* &amp;lbrack;Regal&amp;rbrack; MG Mask Builder AO Rauschen Scale funktioniert nicht richtig
* &amp;lbrack;Regal&amp;rbrack; Der MG-Maskenbildner verfügt über Parameter für invertierte Krümmungen
* &amp;lbrack;Regal&amp;rbrack; Importierte Alphas erzeugen eine Material-Kugelvorschau anstelle einer flachen.

### 3.2.0 (2017.2.0)

*(Freigegeben: 27. Juli 2017)*

**Hinzugefügt:**

* Ankerpunkte - Ebenen- und Maskenreferenzsystem
* &amp;lbrack;Layers&amp;rbrack; Möglichkeit, Füll- und Malen-Effekte umzubenennen
* &amp;lbrack;Plugin&amp;rbrack; Aktualisiertes Substance Source-Plug-in
* &amp;lbrack;Skripterstellung&amp;rbrack; Zulassen, dass die Auflösung des Textursatzes abgefragt wird
* &amp;lbrack;Skripterstellung&amp;rbrack; Abrufen des Status des Engine &quot;Malen&quot; zulassen
* &amp;lbrack;Performance&amp;rbrack; Verbessertes Laden von Projekten und optimiertes Pinselstempeln

**Fest:**

* &amp;lbrack;Werkzeug&amp;rbrack; Leistungsprobleme beim Anpassen von Material-Parametern
* &amp;lbrack;Engine&amp;rbrack; Verschwindende Pinselstriche bei Änderung der Auflösung (4K>2K)
* &amp;lbrack;3D-Ansicht&amp;rbrack; Tangente-Speicherplatz wird nicht mit Bakern synchronisiert
* &amp;lbrack;Regal&amp;rbrack; Der Regal-Pfad in den Benutzerdokumenten wird nicht automatisch erstellt
* &amp;lbrack;Regal&amp;rbrack; Vorgaben nach einem Update mit früheren Versionen kompatibel machen
* &amp;lbrack;Shader&amp;rbrack; Shader ohne PBR funktioniert nicht mehr
* &amp;lbrack;Baker&amp;rbrack; ID-Map-Baking schlägt fehl, wenn &quot;Nach Name abgleichen&quot; aktiviert ist
* &amp;lbrack;Beispiel&amp;rbrack; Die Namen der Meet Mat-Beispielprojekt-Textursatz sind falsch
* Beim Speichern eines Projekts vor dem Erstellen einer Vorlage werden Schreibberechtigungsfehler zurückgegeben.

### 3.1.0 (2017.1.0)

*(Freigegeben: 20. Juni 2017)*

**Hinzugefügt:**

* &amp;lbrack;Plugin&amp;rbrack; Neues Substance Source-Plug-in (ermöglicht das Herunterladen von Assets im Regal)
* &amp;lbrack;Regal&amp;rbrack; 4 Neue Schriftarten (Japanisch + vereinfachtes Chinesisch, Schreibmaschine, Segment)
* &amp;lbrack;Regal&amp;rbrack; 230 neue Alpha (Mischung aus Mustern, Pinseln und Fingerabdruckscans)
* &amp;lbrack;Regal&amp;rbrack; 50 Neue Prozedurale (Stoffmuster mittelalterlicher und zeitgenössischer Kleidung)
* &amp;lbrack;Regal&amp;rbrack; 2 neue Umgebungs-Map (Mondarrain und Villa Nova Street)
* &amp;lbrack;Regal&amp;rbrack; 9 neue Filter (MatFx Detail Edge Wear, Beschränk, HBAO, etc.)
* &amp;lbrack;Regal&amp;rbrack; Verbessertes Panorama-Umgebungs-Map
* &amp;lbrack;Regal&amp;rbrack; Neue Arnold 5-Exportvorgaben
* &amp;lbrack;Skripterstellung&amp;rbrack; Importieren von Ressourcen in das Regal zulassen

**Bekannte Probleme:**

* &amp;lbrack;Export&amp;rbrack; Die Bearbeitung einer Exportvorgabe ist sehr langsam

## Version 2

### 2.6.2

*(Freigegeben: 20. Oktober 2017)*

**Hinzugefügt:**

* &amp;lbrack;Textursatz&amp;rbrack; Löschen deaktivierter Textursatz zulassen
* &amp;lbrack;Regal&amp;rbrack; Schreiben mehrerer Benutzer in denselben Regal-Ordner zulassen
* &amp;lbrack;Skripterstellung&amp;rbrack; Ordner &quot;Plug-ins&quot; neu laden können
* &amp;lbrack;Skripterstellung&amp;rbrack; Fügen Sie eine erforderliche minimale API-Version in den Plug-in-Metadaten hinzu, um die Kompatibilität zu gewährleisten
* &amp;lbrack;Iray&amp;rbrack; Verbesserungen im Dialogfeld &quot;Bild exportieren&quot;

**Fest:**

* &amp;lbrack;Engine&amp;rbrack; Problem mit verschwundenen Strichen beim Ändern der Auflösung (4K>2K)
* &amp;lbrack;Baker&amp;rbrack; ID-Map-Baking schlägt fehl, wenn &quot;Nach Name abgleichen&quot; aktiviert ist
* &amp;lbrack;Baker&amp;rbrack; Fehlermeldungen sind nicht explizit genug
* &amp;lbrack;3D-Ansicht&amp;rbrack; Tangente-Speicherplatz wird nicht mit Bakern synchronisiert
* &amp;lbrack;Werkzeug&amp;rbrack; Schwarze Artefakte bei Verwendung des Wischfinger-Werkzeugs
* &amp;lbrack;Shader&amp;rbrack; Shader ohne PBR funktioniert nicht mehr
* &amp;lbrack;Shader&amp;rbrack; &quot;pbr-coated&quot; ist gebrochen
* &amp;lbrack;Shader&amp;rbrack; Die Rauheit von &quot;pbr-beschichtetem&quot; Shader hat keine Auswirkungen mehr
* &amp;lbrack;Shader&amp;rbrack; Spec Gloss Shader stimmt nicht mit Iray und SD überein
* &amp;lbrack;Regal&amp;rbrack; Absturz beim Laden von zwei Dateien mit demselben Namen, aber unterschiedlichen Erweiterungen
* &amp;lbrack;Regal&amp;rbrack; Die Vorgabe kann in den Regale nicht mehr bearbeitet werden
* &amp;lbrack;Regal&amp;rbrack; Für im Regal importierte Elemente kann keine benutzerdefinierte Vorschau festgelegt werden
* Aus dem Cache geladene Ressourcen verlieren ihre Nutzung
* Beim Speichern eines Projekts vor dem Erstellen einer Vorlage werden Schreibberechtigungsfehler zurückgegeben.
* Falsches Speichern des Projekts, wenn Dateiname zwei Punkte enthält
* Importieren von Dateien mit mehreren Punkten (.) im Dateinamen führt zu Problemen

### 2.6.1

*(Freigegeben: 12. Mai 2017)*

**Hinzugefügt:**

* &amp;lbrack;TextureSet&amp;rbrack; Mesh-Material nicht zu nichts zuweisen

**Fest:**

* Absturz beim Wechseln von TextureSet nach dem Ersetzen von durch Baking erzeugte Map
* Absturz beim Rückgängigmachen und Wiederholen nach dem Ändern der Füllmethode der Ebene
* Absturz oder Einfrieren bei Verwendung des Effekts &quot;Farbauswahl&quot; mit großem ID-Map
* &amp;lbrack;Export&amp;rbrack; Umbenannte Textursatz werden im Exportfenster nicht alphabetisch sortiert
* &amp;lbrack;TextureSet&amp;rbrack; Beim Zurücksetzen auf den Standardnamen wird keine Eindeutigkeit überprüft.
* &amp;lbrack;TextureSet&amp;rbrack; Umbenannter Textursatz wird nach dem erneuten Öffnen des Projekts deaktiviert
* &amp;lbrack;Regal&amp;rbrack; Fehlender Standardvorlageninhalt
* &amp;lbrack;Regal&amp;rbrack; Nicht quadratische Texturen werden als Quadrat angezeigt
* &amp;lbrack;Shader&amp;rbrack; Sobald ein Textursatz deaktiviert wurde, wird der zugehörige Shader gelöscht.
* &amp;lbrack;Skripterstellung&amp;rbrack; alg.Baking.setTextureSetBakingParameters() funktioniert nicht mehr
* &amp;lbrack;Skripterstellung&amp;rbrack; Tippfehler im Websocket-Tutorial
* &amp;lbrack;Skripterstellung&amp;rbrack; Verschiedene Probleme in AlgWidgets
* &amp;lbrack;Log&amp;rbrack; Fehlerhafte Erkennung des verfügbaren virtuellen Speichers in einigen Fällen

### 2.6.0

*(Freigegeben: 27. April 2017)*

**Hinzugefügt:**

* Neues Beispielprojekt &quot;Meet Mat&quot; hinzufügen
* &amp;lbrack;Plugin&amp;rbrack; Neues Plug-in &quot;Resources Updater&quot;
* &amp;lbrack;TextureSet&amp;rbrack; Umbenennen und Hinzufügen einer Beschreibung zu Textursätzen zulassen
* &amp;lbrack;TextureSet&amp;rbrack; Neuzuweisen von Materialien zulassen
* &amp;lbrack;TextureSet&amp;rbrack; Einstellungsschaltfläche im Textursatz-Listenfenster hinzufügen
* &amp;lbrack;TextureSet&amp;rbrack; &quot;Deaktivierte&quot; Textursatz am Ende der Liste anzeigen
* &amp;lbrack;Substance&amp;rbrack; Verwenden zusätzlicher Maps bei der aktuellen Textursatz-Auflösung, um die Leistung zu verbessern
* &amp;lbrack;Skripterstellung&amp;rbrack; Aktualisieren einer in einem Projekt verwendeten Ressource (Material, Generator usw.) zulassen
* &amp;lbrack;Skripterstellung&amp;rbrack; Hinzufügen einer Möglichkeit zum Hinzufügen/Entfernen eines Regals
* &amp;lbrack;Skripterstellung&amp;rbrack; Abfragen von Informationen aus einer Ressource in Projekten zulassen
* &amp;lbrack;Skripterstellung&amp;rbrack; Liste der verfügbaren Shelfs abrufen
* &amp;lbrack;Skripterstellung&amp;rbrack; AlgWidget-Miniaturansicht verbessern
* &amp;lbrack;Export&amp;rbrack; Deaktivieren/Aktivieren der Bittiefe je nach Dateiformatunterstützung
* &amp;lbrack;Log&amp;rbrack; Plug-in-Namen zum Drucken in der Konsole hinzufügen
* &amp;lbrack;Log&amp;rbrack; Fehler zu ausgeblendeten Textursätzen entfernen
* &quot;Begrüßungsbildschirm&quot; mit neuen Symbolen und Text für Beispiele aktualisieren

**Fest:**

* Absturz beim Aktualisieren eines Meshs in bestimmten Projekten
* &amp;lbrack;Viewport&amp;rbrack; Innenfarbe der Symmetrie-Ebene ist nicht mehr sichtbar
* &amp;lbrack;Viewport&amp;rbrack; Einige Nachbearbeitungseffekte sind aktiviert, wenn die Einzelansicht verwendet wird
* &amp;lbrack;Shaders&amp;rbrack; &quot;over_premult&quot;-Füllmethode funktioniert nicht richtig
* &amp;lbrack;Shaders&amp;rbrack; Warnung zum Alphatest mit dem Standard-Shader
* &amp;lbrack;Regal&amp;rbrack; Falsches Analysieren von Tags aus Substance
* &amp;lbrack;Regal&amp;rbrack; MatFX Rost Verwitterung funktioniert nicht richtig
* &amp;lbrack;Regal&amp;rbrack; HSL Filter ist standardmäßig für falsche Kanäle aktiviert
* &amp;lbrack;Regal&amp;rbrack; Der Scharfzeichner ist standardmäßig auf dem Height-/Normalkanal aktiviert
* &amp;lbrack;Export&amp;rbrack; Vray-Exportvorgaben verwenden keine OpenGL-Normalen-Map
* &amp;lbrack;Werkzeug&amp;rbrack; Ungenauigkeitsprobleme mit dem Klon-/Verwischen-Werkzeug erzeugen Artefakte

### 2.5.3

*(Freigegeben: 15. März 2017)*

**Fest:**

* &amp;lbrack;Baker&amp;rbrack; Absturz beim Baking führ mit bestimmten Meshs

**Bekannte Probleme:**

* &amp;lbrack;Mac&amp;rbrack; Partikeln können in einigen Fällen zu Beschädigungen der Textur führen

### 2.5.2

*(Freigegeben: 14. März 2017)*

**Fest:**

* &amp;lbrack;Werkzeug&amp;rbrack; Wacom-Tablets funktionieren unter Linux nicht
* &amp;lbrack;Werkzeug&amp;rbrack; Schwarze Artefakte bei Verwendung des Wischfinger-Werkzeugs
* &amp;lbrack;Baker&amp;rbrack; Baking schlägt fehl, wenn &quot;Nach Name abgleichen&quot; mit einem Käfig verwendet wird
* &amp;lbrack;Baker&amp;rbrack; Ambient occlusion funktioniert nicht, wenn nur mit Normalen-Map Baking geführt wird
* &amp;lbrack;Regal&amp;rbrack; Generische Filter behandeln Alpha nicht richtig (Kontrast/Luminanz, Hochpass usw.)
* &amp;lbrack;Viewport&amp;rbrack; Leistungsproblem beim Laden eines Projekts mit aktivierten Schatten
* &amp;lbrack;Viewport&amp;rbrack; Ditheringe in der 3D-Ansicht über MacOS
* &amp;lbrack;Viewport&amp;rbrack; Partikel-Vorschauen werden falsch angezeigt, wenn Farbprofil aktiviert ist
* &amp;lbrack;Iray&amp;rbrack; Absturz beim Zurückwechseln des Projekts zu OpenGL, wenn Iray nicht initialisiert werden konnte
* &amp;lbrack;Iray&amp;rbrack; Glanz wird beim Rendern von SpecGloss Shader/mdl ignoriert
* &amp;lbrack;Shader&amp;rbrack; Spec/Gloss Shader stimmt nicht mit Iray und SD überein
* &amp;lbrack;Shader&amp;rbrack; sRGB-Konvertierung anders als bei der linearen in sRGB-LUT-Konvertierung
* &amp;lbrack;Shader&amp;rbrack; Falsches Rendering beim Laden des Projekts mit veralteten Shadern
* &amp;lbrack;Shader&amp;rbrack; &quot;pbr-beschichteter&quot; Shader funktioniert nicht mehr
* &amp;lbrack;Export&amp;rbrack; Einige Kanäle werden weiterhin exportiert, auch wenn sie nicht im Textursatz vorhanden sind
* &amp;lbrack;Layers&amp;rbrack; Der Mischmodus &quot;Normalen-Map inverse detail&quot; funktioniert nicht auf Graustufenkanälen
* &amp;lbrack;UI&amp;rbrack; Problem beim &quot;Farbauswahl window&quot; mit HDPI-Monitor und Anzeigezoom bei 150 %

**Bekannte Probleme:**

* &amp;lbrack;Mac&amp;rbrack; Partikeln können in einigen Fällen zu Beschädigungen der Textur führen

### 2.5.1

*(Freigegeben: 27. Februar 2017)*

**Fest:**

* &amp;lbrack;Mac&amp;rbrack; Wacom-Tablet-Eingang in 3D und 2D-Ansicht defekt
* &amp;lbrack;Baker&amp;rbrack; Die Zuordnung nach Namen funktioniert nicht mehr
* &amp;lbrack;Baker&amp;rbrack; Die Einstellung &quot;Durchschnittliche Normale&quot; funktioniert nicht mehr
* &amp;lbrack;Iray&amp;rbrack; Falsches Rendering mit fehlendem Baking geführt Normalen-Map
* &amp;lbrack;Iray&amp;rbrack; Farbprofil verhalten sich anders als beim OpenGL-Renderer
* &amp;lbrack;Iray&amp;rbrack; Beim Exportieren des Renderings als Bitmap wird das Farbprofil nicht korrigiert.
* &amp;lbrack;Substance&amp;rbrack; Materialfilter funktionieren nicht mehr
* &amp;lbrack;Werkzeug&amp;rbrack; Die Konturdeckkraft wird nicht in Pinselvorgaben gespeichert
* &amp;lbrack;Werkzeug&amp;rbrack; Klon-Pinsel-UV-Ausrichtung funktioniert nicht mehr
* &amp;lbrack;Export&amp;rbrack; Beim Exportieren in Ganzzahl sollte der Versatz-Kanal in 0,5 zentriert sein
* &amp;lbrack;Vorlage&amp;rbrack; Absoluter Pfad wird in Vorlagen gespeichert
* &amp;lbrack;TextureSet&amp;rbrack; Die Textur des Kanals bleibt auch nach dem Entfernen des Kanals bestehen.

**Bekannte Probleme:**

* &amp;lbrack;Linux&amp;rbrack; Wacom-Tablet-Eingaben funktionieren nicht in 3D und 2D-Ansicht
* &amp;lbrack;Mac&amp;rbrack; Partikeln können in einigen Fällen zu Beschädigungen der Textur führen
* &amp;lbrack;Export&amp;rbrack; In sehr seltenen Fällen können auf AMD-GPUs schwarze Rechtecke erscheinen

### 2.5.0

*(Freigegeben: 21. Februar 2017)*

**Hinzugefügt:**

* Unterstützung für AMD Radeon Pro- und AMD FirePro-GPUs
* &amp;lbrack;Werkzeug&amp;rbrack; Unterstützung für Konturdeckkraft hinzufügen
* &amp;lbrack;Werkzeug&amp;rbrack; Fügen Sie einen Modifizierer hinzu, mit dem Sie den letzten Pinselstrich fortsetzen können
* &amp;lbrack;Iray&amp;rbrack; Update zur Unterstützung von Pascal-GPUs
* &amp;lbrack;Viewport&amp;rbrack; Unterstützung für Farbprofil hinzufügen (LUT)
* &amp;lbrack;Substance&amp;rbrack; Neues Framework integrieren (SD6-Engine)
* &amp;lbrack;UI&amp;rbrack; Liste &quot;Zuletzt verwendete Datei&quot; im Menü &quot;Datei&quot; vergrößern
* &amp;lbrack;Import&amp;rbrack; Kategorie aus Stoffen verwenden, um das Präfix im Dialogfeld &quot;Einfuhr&quot; auszufüllen
* &amp;lbrack;Baker&amp;rbrack; Baking von 8K-Texturen zulassen
* &amp;lbrack;Baker&amp;rbrack; Nicht quadratische Auflösungen können Baking geführt werden
* &amp;lbrack;Baker&amp;rbrack; Verbessern Sie den Speicherverbrauch beim Baking führ von hochpolaren Meshs
* &amp;lbrack;Regal&amp;rbrack; Regale (und Projekte) sperren, um gleichzeitige Bearbeitung zu verhindern und Beschädigungen zu vermeiden
* &amp;lbrack;Regal&amp;rbrack; Lesen Sie Kategorie und Schlüsselwörter von Stoffen, um sie für die Filterung zu verwenden
* &amp;lbrack;Regal&amp;rbrack; Ausschließen von Ressourcen vom Ergebnis einer Suchabfrage zulassen
* &amp;lbrack;Regal&amp;rbrack; Verbesserte Berechnung der Miniaturansichten
* &amp;lbrack;Regal&amp;rbrack; Einbetten von Vorgaben in Projekte zulassen
* &amp;lbrack;Regal&amp;rbrack; Schnelles Ein- und Ausblenden der Strukturansicht mit UMSCHALTTASTE
* &amp;lbrack;Regal&amp;rbrack; Speichern von Miniaturansichten zulassen, wenn Assets schreibgeschützt sind (lokaler Cache)
* &amp;lbrack;Regal&amp;rbrack; Neue Inhalte : neue Filter (transformieren, Mirror, Tri-planar usw.)
* &amp;lbrack;Regal&amp;rbrack; Neue Inhalte : neue LUTs-Profile (klassisch und künstlerisch, z. B. Film Noir, Vintage usw.)
* &amp;lbrack;Regal&amp;rbrack; Neue Inhalte : 10 neue Font-Substance zur schnellen Generierung benutzerdefinierter Texte
* &amp;lbrack;Regal&amp;rbrack; Neue Vorlagen : Unity 5 und Unreal Engine 4
* &amp;lbrack;Regal&amp;rbrack; Verbesserter HSL-Filter für mehr Künstlerfreundlichkeit
* &amp;lbrack;Shader&amp;rbrack; Unterstützung für Specular level-Kanal in PBR-Shadern hinzufügen
* &amp;lbrack;Shader&amp;rbrack; Unterstützung für Dithering in Alpha Test Shader hinzufügen
* &amp;lbrack;Shader&amp;rbrack; Unterstützung für die Zuordnung von Parallax-Verdeckungen in PBR-Shadern hinzufügen
* &amp;lbrack;Shader&amp;rbrack; Definieren einer benutzerdefinierten Benutzeroberfläche für Shader-Parameter zulassen
* &amp;lbrack;MatLayering&amp;rbrack; Neuen Maskenkanal für Material-Ebenen-Workflow erstellen
* &amp;lbrack;Skripterstellung&amp;rbrack; Schreiben von Metadaten in ein SP-Projekt zulassen
* &amp;lbrack;Skripterstellung&amp;rbrack; Exportieren mit einer bestimmten Exportvorgabe zulassen
* &amp;lbrack;Skripterstellung&amp;rbrack; Shader-Parameter als JSON abrufen
* &amp;lbrack;Skripterstellung&amp;rbrack; Unterstützung für WebSocket-Verbindungen hinzufügen
* &amp;lbrack;Skripterstellung&amp;rbrack; Shader-Instanzen können geladen werden.
* &amp;lbrack;Skripterstellung&amp;rbrack; Hinzufügen der Möglichkeit, ein neues Projekt zu erstellen
* &amp;lbrack;Skripterstellung&amp;rbrack; Abrufen der URL des in ein Projekt importierten Meshs zulassen
* &amp;lbrack;Skripterstellung&amp;rbrack; Nicht quadratisches Baking zulassen
* &amp;lbrack;Skripterstellung&amp;rbrack; Fehler beim Festlegen von Daten über die Skript-API melden
* &amp;lbrack;Substance&amp;rbrack; Benutzerdaten-Tag zum Angeben von Normalen-Map-Format hinzufügen

**Fest:**

* Absturz bei der Farbauswahl mit Stoffen
* Absturz beim Laden eines Nicht-RGBA32f-Bildes als Umgebungs-Map
* Absturz beim Malen auf AMD-GPUs
* &amp;lbrack;Mesh&amp;rbrack; OBJ Import erkennt Materialien ohne MTL-Datei nicht
* &amp;lbrack;Mesh&amp;rbrack; Die Generierung des Namens des UDIM-Textursatzes kann auf einigen Meshs falsch sein
* &amp;lbrack;UI&amp;rbrack; Schaltfläche &quot;Rückgängig/Wiederholen&quot; in Anzeigeeinstellung &quot;Fokus stehlen&quot; und Mausbildlauf anhalten
* &amp;lbrack;UI&amp;rbrack; Einige Beschriftungen werden in High-DPI falsch beschnitten
* &amp;lbrack;Ebene&amp;rbrack; Der Ersetzungsmodus für den Malen-Effekt hat ein falsches Verhalten auf der Maske.
* &amp;lbrack;Ebene&amp;rbrack; Der subtrahieren-Mischmodus verhält sich mit Alpha nicht korrekt.
* &amp;lbrack;Werkzeug&amp;rbrack; Die Pinselgröße wird in der 2D-Ansicht sehr groß, wenn auf UV-Rahmen gemalt wird
* &amp;lbrack;Werkzeug&amp;rbrack; Einrasten Gerade hat ein ungleichmäßiges Verhalten mit High-DPI.
* &amp;lbrack;Werkzeug&amp;rbrack; Die Auflösung der Schablone ist manchmal falsch
* &amp;lbrack;Baker&amp;rbrack; Die Werte für &quot;Max. Verdeckungsabstand&quot; werden festgeklemmt, wenn &quot;relativ zum Begrenzungsrahmen&quot; &quot;Aus&quot; ist.
* &amp;lbrack;Shader&amp;rbrack; Kanaldefinitionen für Stapel und automatische Parameter stimmen nicht überein
* &amp;lbrack;3D-Ansicht&amp;rbrack; Inkonsistente Anzeige des normalen Kanals abhängig von der Projekteinstellung
* &amp;lbrack;Viewport&amp;rbrack; Einige Normalen-Map haben eingeklemmte Werte, die als Artefakte erscheinen
* &amp;lbrack;Viewport&amp;rbrack; Post-Effect sind standardmäßig immer deaktiviert
* &amp;lbrack;Export&amp;rbrack; Normale Mischeinstellung ist falsch, wenn normaler Kanal fehlt
* &amp;lbrack;Export&amp;rbrack; Falsche Generierung von Texturen in einigen Fällen auf AMD-GPUs
* &amp;lbrack;Export&amp;rbrack; Shader-Parameter werden nicht ordnungsgemäß exportiert, wenn sie sich in einer Gruppe befinden
* &amp;lbrack;Export&amp;rbrack; Beim Bearbeiten einer Exportvorgabe in einem benutzerdefinierten Regal wird ein Protokollfehler ausgegeben
* &amp;lbrack;Regal&amp;rbrack; Die Filterungen in der Strukturansicht stimmen nicht genau mit dem Ordnernamen überein
* &amp;lbrack;Regal&amp;rbrack; Das Umbenennen einer Regal-Vorgabe ist schwer zu lesen
* &amp;lbrack;Regal&amp;rbrack; Im Regal importierte Shader-Ressource bleibt nach dem Neustart nicht erhalten
* &amp;lbrack;Regal&amp;rbrack; Inhalt : Werkzeugvorgabe fehlt
* &amp;lbrack;Regal&amp;rbrack; Inhalt : Tile Generator funktioniert nicht richtig
* &amp;lbrack;Regal&amp;rbrack; Inhalt : Falsche Maske auf Gummireifen-Schmutziges intelligente Material behoben
* &amp;lbrack;Regal&amp;rbrack; Inhalt : Falscher Gruppenname auf dem Material der Ledertasche wurde behoben
* &amp;lbrack;Iray&amp;rbrack; Die Hälfte der Mesh fehlt in Iray
* &amp;lbrack;Linux&amp;rbrack; Absturz beim Ziehen einer Ressource über die 3D-Ansicht
* &amp;lbrack;Mac&amp;rbrack; Die Voreinstellungen werden bei jedem Start in Sierra zurückgesetzt

**Bekannte Probleme:**

* &amp;lbrack;Export&amp;rbrack; In sehr seltenen Fällen können auf AMD-GPUs schwarze Rechtecke erscheinen
* &amp;lbrack;Iray&amp;rbrack; Farbprofil können sich manchmal seltsam verhalten

### 2.4.1

*(Freigegeben: 28. Oktober 2016)*

**Fest:**

* Absturz beim Erstellen eines Projekts mit einer Vorlage
* Absturz beim Schließen des Exportdialogfelds während eines Exports
* &amp;lbrack;Mac&amp;rbrack; Fehler beim Speichern des Projekts (Exportvorgabe kann nicht gespeichert werden)
* &amp;lbrack;Regal&amp;rbrack; Beim Erstellen einer neuen Vorgabe wird sie zweimal angezeigt
* &amp;lbrack;Regal&amp;rbrack; Vorgaben können ohne Administratorrechte nicht im schreibgeschützten Modus geladen werden.

### 2.4.0

*(Freigegeben: 27. Oktober 2016)*

**Hinzugefügt:**

* &amp;lbrack;Regal&amp;rbrack; Neue Benutzeroberfläche zum Durchsuchen von Ressourcen (Strukturansicht, Filter usw.)
* &amp;lbrack;Regal&amp;rbrack; Speichern einer Suche als Vorgabe zulassen
* &amp;lbrack;Regal&amp;rbrack; Erstellen eines neuen Fensters aus einer Vorgabe zulassen
* &amp;lbrack;Regal&amp;rbrack; Neue Benutzeroberfläche für den Import von Ressourcen
* &amp;lbrack;Regal&amp;rbrack; Kopieren Sie kein standardmäßiges allegorisches Regal im Ordner &quot;Dokumente&quot;
* &amp;lbrack;Regal&amp;rbrack; Neue Partikeln-Vorgaben : Stromkreis, elektrische Leitungen, Rokoko, Kleinvenen
* &amp;lbrack;Regal&amp;rbrack; Verbesserte Vorgaben für ältere Partikeln, um einfacher zu verwenden (z. B. &quot;Rain&quot;)
* &amp;lbrack;Regal&amp;rbrack; Neue Informationen zum Kontextmenü der Ressource hinzufügen
* &amp;lbrack;Viewport&amp;rbrack; Verbessern der Leistung beim Laden von Umgebungs-Map
* &amp;lbrack;Viewport&amp;rbrack; Unterstützung für Umgebungs-Map, die nicht die Macht von zwei sind

**Fest:**

* Absturz beim Entfernen einer Maske
* Absturz beim Malen nach dem Speichern einer Vorgabe
* Absturz mit Umgebungsunschärfe bei einigen GPUs
* Absturz beim Zuweisen einer falschen Ressource zum Mini-Regal
* &amp;lbrack;Regal&amp;rbrack; Bereinigen + Speichern - Entfernen von Tags und Metadaten für Ressourcen im Projekt
* &amp;lbrack;Regal&amp;rbrack; Beim Importieren einer Vorgabe werden ihre Ressourcen im Regal angezeigt
* &amp;lbrack;Export&amp;rbrack; Normalen-Map, die aus dem Height-Kanal generiert wird, ist niedrig
* &amp;lbrack;Export&amp;rbrack; Normal vom Mesh ist in der endgültigen Normalen-Map nicht immer vorhanden
* &amp;lbrack;Export&amp;rbrack; Ausdehnung mit Transparenz kann manchmal ohne Transparenz erfolgen
* &amp;lbrack;Skripterstellung&amp;rbrack; &quot;alg.plugin_root_directory&quot; kann einen abgeschnittenen Netzwerkpfad zurückgeben
* &amp;lbrack;TextureSet&amp;rbrack; Sperrschaltfläche ist aktiviert, wenn nicht quadratische Projekte erneut geöffnet werden

### 2.3.1

*(Freigegeben: 07. Oktober 2016)*

**Hinzugefügt:**

* &amp;lbrack;Plugin&amp;rbrack;&amp;lbrack;Photoshop&amp;rbrack; Geben Sie an, welches Material/welcher Stapel/welche Kanäle exportiert werden sollen.
* &amp;lbrack;Skripterstellung&amp;rbrack; Funktionsnamen weisen einige Inkonsistenzen auf.

**Fest:**

* &amp;lbrack;Export&amp;rbrack; Alpha kann in benutzerdefinierten Exportvorgaben verworfen werden
* &amp;lbrack;Export&amp;rbrack; Alpha erhält falsche Gamma-Konvertierung auf sRGB-Kanälen
* &amp;lbrack;Export&amp;rbrack; Nicht quadratische Dokumente werden als quadratische
* &amp;lbrack;Export&amp;rbrack; Es ist nicht möglich, zusätzliche Maps zu exportieren, wenn eine fehlt
* &amp;lbrack;Iray&amp;rbrack; Einige Parameter (z. B. &quot;emissive-Intensität&quot;) haben keine Auswirkungen
* &amp;lbrack;NVIDIA&amp;rbrack; Absturz beim Start mit NVIDIA Quadro K2200/GTX 750/760
* &amp;lbrack;AMD&amp;rbrack; Falscher Farbsatz für Miniaturen und Vorschauen
* &amp;lbrack;AMD&amp;rbrack; Einfrieren und Treiberfehler beim Öffnen neuer Dateien und Dateien
* &amp;lbrack;Log&amp;rbrack; &quot;software-version&quot; fehlt in der Protokolldatei

### 2.3.0

*(Freigegeben: 15. September 2016)*

**Hinzugefügt:**

* &amp;lbrack;Plugin&amp;rbrack; Neues Plug-in &quot;Nach Photoshop exportieren&quot; (vollständiger Ebenenstapel exportieren)
* &amp;lbrack;Export&amp;rbrack; Zulassen, dass die Breite der Auffüllung (in Pixeln oder unendlich) angegeben wird
* &amp;lbrack;Export&amp;rbrack; Festlegen des Hintergrundtyps außerhalb der UVs zulassen
* &amp;lbrack;Regal&amp;rbrack; Neues Material mit Shader-Ebenen zum Überblenden von 10 Materialien
* &amp;lbrack;Regal&amp;rbrack; Neuer Ton-Shader zur Anzeige von Details mit dem Height-/Normalkanal
* &amp;lbrack;Regal&amp;rbrack; Neuer Baking geführt Lichtfilter mit Umgebungseingabe
* &amp;lbrack;Regal&amp;rbrack; Einige Maskengenerator wurden aktualisiert, um nicht quadratische Transformationen hinzuzufügen
* &amp;lbrack;Viewport&amp;rbrack; Composited Normalen-Map (Normal+Height+Baking) zum Solomodus hinzufügen
* &amp;lbrack;Skripterstellung&amp;rbrack; Exportieren zusätzlicher Maps zulassen
* &amp;lbrack;Skripterstellung&amp;rbrack; Abfragen verfügbarer zusätzlicher Maps pro Textursatz zulassen
* &amp;lbrack;Skripterstellung&amp;rbrack; Abrufen des Kanalformats zulassen
* &amp;lbrack;Skripterstellung&amp;rbrack; Fügen Sie der Baking führend Dokumentation Beispiele hinzu
* &amp;lbrack;Skripterstellung&amp;rbrack; Abfragen der Sichtbarkeit einer Ebene zulassen
* &amp;lbrack;Skripterstellung&amp;rbrack; Füllmethode und Deckkraft der Ebene abfragen
* &amp;lbrack;Skripterstellung&amp;rbrack; Exportieren konvertierter Maps (endgültige Normalen-Map, gemischte AO usw.) zulassen
* &amp;lbrack;Substance&amp;rbrack; Benutzerdefinierte Verwendungen lesen und verbinden
* &amp;blbrack;Shortcuts&amp;rbrack; Zusatztaste (SHIFT) hinzufügen, um Solo-Modus rückwärts zu durchlaufen
* &amp;lbrack;Export&amp;rbrack; Standardexportvorgabe wurde aktualisiert, um Alpha zu deaktivieren
* &amp;lbrack;UI&amp;rbrack; Miniaturen werden jetzt nur berechnet, wenn das Engine verfügbar ist
* &amp;lbrack;UI&amp;rbrack; Anzeigen einer Erwähnung bei der Berechnung von Miniaturansichten

**Fest:**

* Absturz zu einigen alten Projekten beim Öffnen
* Absturz mit beschädigtem Textur-Kanal-Cache
* Absturz beim Mischen von mehr als 4 Materialien mit dem Material-Ebenen-Arbeitsablauf
* &amp;lbrack;UI&amp;rbrack; Tastaturbefehle funktionieren nicht, wenn die Symbolleiste ausgeblendet ist
* &amp;lbrack;UI&amp;rbrack; Iray-Werkzeugleiste ist im Ansichtsmenü mit &quot;Unbenannt&quot; beschriftet
* &amp;lbrack;UI&amp;rbrack; Plug-in-Symbolleisten werden im Menü &quot;Ansicht&quot; als &quot;Nicht geneigt&quot; bezeichnet
* &amp;lbrack;Baker&amp;rbrack; Durch Drücken der Eingabetaste beim Bearbeiten einer Baking-Einstellung wird der Baking-Prozess gestartet
* &amp;lbrack;Baker&amp;rbrack; Falsche Bereiche für einige Parameter
* &amp;lbrack;Import&amp;rbrack; Import von OBJ-Meshs aufgrund sehr großer Zahlen nicht möglich
* &amp;lbrack;Import&amp;rbrack; Einige OBJ werden mit zu vielen Unterobjekten importiert
* &amp;lbrack;Export&amp;rbrack; Kanalhintergrund wird beim Export mit Schwarz anstelle der Standardfarbe gefüllt
* &amp;lbrack;Werkzeug&amp;rbrack; Partikeln funktionieren nicht richtig, wenn der FOV-Wert zu niedrig ist
* &amp;lbrack;Werkzeug&amp;rbrack; Die Pinselvorschaufarbe ist bei Masken in untergeordneten Stapeln falsch
* &amp;lbrack;Viewport&amp;rbrack; Wenn der Pinsel in leere Bereiche in der 2D-Ansicht übergeht, wird er gigantisch
* &amp;lbrack;Viewport&amp;rbrack; Leere Pinselvorschau beim Malen mit normalen Texturen
* &amp;lbrack;Skripterstellung&amp;rbrack; Falsche Dokumentation : &quot;ao&quot; anstelle von &quot;ambientocclusion&quot; aufgeführt
* &amp;lbrack;Skripterstellung&amp;rbrack; Der mit subprocess() gestartete Prozess wird beim Schließen von Painter beendet
* &amp;lbrack;Regal&amp;rbrack; Baking geführt Beleuchtungsfilter verwenden falsche AO-Eingabe
* &amp;lbrack;MacOS&amp;rbrack; Entferntes Fire Hydrant-Projekt (inkompatibel)
* Standardprojekt wird beim Laden einer \*.spt-Datei geöffnet (anstelle von \*.spp).

**Bekannte Probleme:**

* &amp;lbrack;Plugin&amp;rbrack; Aufgrund von Photoshop können das Height und der normale Kanal nicht unverändert Kamera bewogen werden.

### 2.2.0

*(Freigegeben: 22. Juli 2016)*

**Hinzugefügt:**

* &amp;lbrack;Regal&amp;rbrack; Verbesserung des Suchsystems und der Suchanfragen
* &amp;lbrack;Regal&amp;rbrack; Hinzufügen eines Suchfelds für Mini-Regals
* &amp;lbrack;Shader&amp;rbrack; Festlegen der Schrittgenauigkeit für Schieberegler
* &amp;lbrack;Shader&amp;rbrack; Hinzufügen einer Schaltfläche &quot;Rückgängig/Wiederholen&quot; für Shader-Parameter
* &amp;lbrack;Shader&amp;rbrack; Das erneute Laden eines Shader sollte seine Parameter nicht zurücksetzen.
* &amp;lbrack;MatLayering&amp;rbrack; Unterstützung für Dynamische Materialüberlagerung und Sub-Stapel hinzufügen
* &amp;lbrack;MatLayering&amp;rbrack; JSON-Datei zum Einrichten der Shader-Einstellungen importieren
* &amp;lbrack;MatLayering&amp;rbrack; Limit für Textur-Sampler entsperren (Wechsel zu Bindless-Texturen)
* &amp;lbrack;Skripterstellung&amp;rbrack; Festlegen der Baker-Einstellungen und Starten der Berechnung zulassen
* &amp;lbrack;Substance&amp;rbrack; &quot;Verwendung&quot; für Ein-/Ausgangsverbindungen zusätzlich zu den Identifizierungen verwenden
* &amp;lbrack;Werkzeug&amp;rbrack; Auswahl des Vorschaukanals im Viewport für das Projektion-Werkzeug zulassen

**Fest:**

* Absturz beim Start, wenn sich die Substanzen im falschen Ordner befinden
* Der Absturz-Bericht funktioniert aufgrund einer falschen Protokolldatei manchmal nicht
* &amp;lbrack;Iray&amp;rbrack; Post-Effekte werden nicht aktualisiert, wenn das Iray angehalten wird
* &amp;lbrack;Iray&amp;rbrack; Autofokus-Tastaturbefehl funktioniert nicht mehr
* &amp;lbrack;Iray&amp;rbrack; Verhalten des Reglers &quot;Blende&quot; ändert sich je nach Elementgröße.
* &amp;lbrack;Layers&amp;rbrack; Der Kanal des ersten Materials ist standardmäßig nicht aktiviert, wenn alle deaktiviert sind
* &amp;lbrack;Shader&amp;rbrack; Es werden keine Fehler gedruckt, wenn ein &quot;automatischer Parameter&quot; falsch ist

**Bekannte Probleme:**

* &amp;lbrack;Mac&amp;rbrack; Grenzwert für Textur-Samples auf 16 gesperrt (GPU-Treiberproblem)

### 2.1.1

*(Freigegeben: 1. Juli 2016)*

**Hinzugefügt:**

* &amp;lbrack;Lizenz&amp;rbrack; Ändern des Speicherorts der Lizenzdatei
* &amp;lbrack;Viewport&amp;rbrack; Hinzufügen eines &quot;B&quot;-Tastaturbefehl, um zwischen weiteren Karten zu wechseln
* &amp;lbrack;Import&amp;rbrack; FBX 2016/2017 ordnungsgemäß importieren
* &amp;lbrack;Werkzeug&amp;rbrack; Entfernen von Häkchen bei Verwendung der schnelle Maske
* &amp;lbrack;Iray&amp;rbrack; Informationen zu den Abmessungen der Szene hinzufügen
* &amp;lbrack;Iray&amp;rbrack; Zulassen, dass die maximale Anzahl von Samples und die Renderzeit erhöht werden
* &amp;lbrack;UI&amp;rbrack; Ergebnis sofort aktualisieren, wenn +/- Taste auf Schiebereglern verwendet wird
* &amp;lbrack;UI&amp;rbrack; Höhere Präzision bei den Graustufen-Reglern
* &amp;lbrack;Export&amp;rbrack; Exportieren Sie keinen Alphakanal für Texturen, die nur RGB sind
* &amp;lbrack;Export&amp;rbrack; Exportvorgabe &quot;Dota 2 aktualisieren&quot;
* &amp;lbrack;Regal&amp;rbrack; Neues Muster &quot;Sechseckfliesen&quot;
* &amp;lbrack;Regal&amp;rbrack; Neues Werkzeug &quot;Verschweißt&quot;
* &amp;lbrack;Regal&amp;rbrack; Die Abschlussfilter wurden aktualisiert, um Richtungssteuerungen bereitzustellen.

**Fest:**

* &amp;lbrack;Export&amp;rbrack; PSD-Dateien mit 8 Bit können nicht exportiert werden
* &amp;lbrack;Export&amp;rbrack; 8K-Export ist bei einigen Hardware-Konfigurationen nicht verfügbar
* &amp;lbrack;Export&amp;rbrack; Das Sketchfab-Fenster ist zugeschnitten
* &amp;lbrack;Export&amp;rbrack; Falsche Rauheit in der Vorgabe für den Export von Spezifikation/Glanz
* &amp;lbrack;UI&amp;rbrack; Die Eingabe in Graustufenreglern funktioniert nicht mehr
* &amp;lbrack;UI&amp;rbrack; Es ist nicht möglich, Filter in Substance-Eingaben zu integrieren (wie Generatoren)
* &amp;lbrack;UI&amp;rbrack; Einige Regler haben ein seltsames Verhalten.
* &amp;lbrack;UI&amp;rbrack; DeltaTime +/- für Partikeln ist zu groß
* &amp;lbrack;Iray&amp;rbrack; Einige Projekte blockieren die Anwendung beim Wechsel zu Iray
* &amp;lbrack;Iray&amp;rbrack; Absturz beim Erkennen von Hardware
* &amp;lbrack;Werkzeug&amp;rbrack; Die Pinselvorschaufarbe ist im Maskenmodus falsch
* &amp;lbrack;Werkzeug&amp;rbrack; Die Werkzeugauswahl kann mit inkompatiblen Materialien verwendet werden
* &amp;lbrack;Werkzeug&amp;rbrack; Projektion-Vorschau wechselt nicht zu Diffuse mit Spec/Gloss-Workflow
* &amp;lbrack;Regal&amp;rbrack; Ändern des Standard-Shader unterbricht Smart Mats/intelligente Masken-Vorschauen
* &amp;lbrack;Regal&amp;rbrack; Einige intelligente Material haben falsche Namen.
* &amp;lbrack;Regal&amp;rbrack; Zusätzliche Alpha-Formen sind beschädigt und werden nicht geladen.
* &amp;lbrack;Viewport&amp;rbrack; Wechseln in den Modus &quot;Zusätzliche Karte&quot; zeigt zuerst &quot;andere&quot; an
* &amp;lbrack;Viewport&amp;rbrack; Viewport wechseln zurück zu &quot;Andere&quot;, wenn keine zusätzliche Map vorhanden ist
* &amp;lbrack;Absturz&amp;rbrack;&amp;lbrack;Linux&amp;rbrack; Absturz-Bericht funktioniert nicht auf Ubuntu (Steam)
* &amp;lbrack;Absturz&amp;rbrack;&amp;lbrack;Linux&amp;rbrack; Web-URL-Links funktionieren nicht auf Ubuntu (Steam)
* &amp;lbrack;Absturz&amp;rbrack;&amp;lbrack;Windows&amp;rbrack; Entfernen Sie &quot;crashwatcher&quot;, wenn Substance Painter nicht mehr ausgeführt wird.
* &amp;lbrack;Absturz&amp;rbrack;&amp;lbrack;Mac&amp;rbrack; Absturz-Berichtssystem funktioniert nicht richtig
* &amp;lbrack;Absturz&amp;rbrack; Das Importieren eines Meshs, während bereits ein Mesh importiert wurde, führt zu einem Absturz
* Textursatz beim Auswählen eines Tastaturbefehl nach einem Neustart auf nichts zurückgesetzt

### 2.1.0

*(Freigegeben: Juni 2016)*

**Hinzugefügt:**

* &amp;lbrack;UDIM&amp;rbrack; Importieren von UDIM-Kacheln aus einem Mesh als Textursatz
* &amp;lbrack;Linux&amp;rbrack; Neue Unterstützung für CentOS 6.6 und Ubuntu 12.4
* &amp;lbrack;Export&amp;rbrack; Hinzufügen einer 8K-Auflösung (experimentell)
* &amp;lbrack;Export&amp;rbrack; Auswahl der Bittiefe während des Exports zulassen
* &amp;lbrack;Baker&amp;rbrack; Baking mehrerer Textursatz gleichzeitig zulassen
* Unterstützung hochauflösender Monitore (hohe DPI-Skalierung)
* &amp;lbrack;Skripterstellung&amp;rbrack; Benutzerdefinierte Auflösung und Innenabstände pro Textur beim Export festlegen
* &amp;lbrack;Viewport&amp;rbrack; Erlaubt das Wechseln zwischen Textursatz durch Klicken auf den Mesh (über Strg+Alt+Klick)
* &amp;lbrack;Viewport&amp;rbrack; Bewegen des Mauszeigers beim Zoomen mit dem Mausrad
* &amp;lbrack;UI&amp;rbrack; Standardhintergrundfarbe und Umgebungs-Map-Anzeige aktualisieren
* &amp;lbrack;UI&amp;rbrack; QuickInfos mit Originalnamen für Benutzerkanäle hinzufügen
* &amp;lbrack;UI&amp;rbrack; Hintergrundfarbe für Kanäle ändern, die nicht umbenannt werden können
* &amp;lbrack;Werkzeug&amp;rbrack; Entfernen von Häkchen bei Verwendung der schnelle Maske
* &amp;lbrack;Shader&amp;rbrack; Erlaubt das Definieren von Gruppen für Shader-Parameter und Materialien/Masken.
* &amp;lbrack;Engine&amp;rbrack; Optimierung der Kleinstprägung
* &amp;lbrack;Schablone&amp;rbrack; W als Tastaturbefehl hinzufügen, um die Maske vorübergehend zu aktivieren bzw. zu deaktivieren
* &amp;lbrack;Regal&amp;rbrack; Kreuzschaltfläche zum Löschen des Suchfelds hinzufügen
* &amp;lbrack;Regal&amp;rbrack; Alpha mit einem Klick laden
* &amp;lbrack;Regal&amp;rbrack; Neue Exportvorgabe : Vray UDIM, Arnold UDIM, Spec/Gloss von Metal/Rough
* &amp;lbrack;Regal&amp;rbrack; Neue Alphas : geometrische Formen, Adern und Zeichen
* Namen und Version in den Eigenschaften der ausführbaren Substance Painter-Datei hinzufügen

**Fest:**

* &amp;lbrack;Substance&amp;rbrack; Es ist nicht möglich, den normalen Kanal und die zusätzliche Karte gleichzeitig zu verwenden
* &amp;lbrack;Iray&amp;rbrack; MDL-Brechung und Absorption-Einstellung funktionieren nicht
* &amp;lbrack;Iray&amp;rbrack; Originalskala der Szene wird nicht beibehalten
* &amp;lbrack;Regal&amp;rbrack; Specular/Glanz-Vorlage verwendet falschen Shader
* &amp;lbrack;Export&amp;rbrack; Bei der Standard-Exportvorgabe werden einige Maps (wie AO) nicht exportiert.
* &amp;lbrack;Viewport&amp;rbrack; Pivot-Punkt wird nicht aktualisiert, wenn Sie außerhalb der UVs in der 2D-Ansicht klicken
* &amp;lbrack;UI&amp;rbrack; Reglerwerte sind abgerundet
* &amp;lbrack;UI&amp;rbrack; Manchmal ist beim Bearbeiten der Reglerwerte der Speicherplatz sehr klein
* &amp;lbrack;Neues Projekt&amp;rbrack; Die Dropdown-Liste für Vorlagen wurde nicht korrekt aktualisiert (von 1.x auf 2.x)
* &amp;lbrack;Skripterstellung&amp;rbrack; &quot;Hover&quot;-Verhalten bei benutzerdefinierten Schaltflächen behoben
* &amp;lbrack;Mac&amp;rbrack; Durch Rückgängigmachen für ein leeres Projekt wird die Kamera gesperrt

**Bekannte Probleme:**

* Absturz-Bericht ist auf Ubuntu nicht verfügbar
* Einige URL-Schaltflächen funktionieren möglicherweise nicht. In unseren FAQs finden Sie eine Problemumgehung

### 2.0.5

*(Freigegeben: 29. April 2016)*

**Hinzugefügt:**

* &amp;lbrack;Regal&amp;rbrack; Hinzugefügte/aktualisierte Nicht-PBR-Vorlage, Shader- und Exportvoreinstellung
* &amp;lbrack;Regal&amp;rbrack; Die UE4-Exportvorgabe wurde aktualisiert und enthält jetzt auch Ambient occlusion

**Fest:**

* Absturz beim Öffnen und Speichern einiger Projekte mit beschädigten Ressourcen
* &amp;lbrack;Viewport&amp;rbrack; Drahtgitter erscheint in der 2D-Ansicht beschädigt
* &amp;lbrack;Regal&amp;rbrack; Verbesserte Performance einiger Studio-Umgebungs-Map
* &amp;lbrack;Regal&amp;rbrack; Einige Studio-Umgebungs-Map sind dupliziert.
* &amp;lbrack;Regal&amp;rbrack; Fehlendes &quot;Baking geführt Beleuchtungs-Material&quot;
* &amp;lbrack;Regal&amp;rbrack; Fehlender Generator für &quot;Graustufen-Konvertierung&quot;

### 2.0.4

*(Freigegeben: 26. April 2016)*

**Hinzugefügt:**

* Verbessern von Mesh-Kollisionen und Optimieren des Drahtgitter-Renderings
* Verbessern der Performance und des Arbeitsspeicher-Managements durch umfangreiche Projekte
* Verbessern der Schiebereglerpräzision und des Schrittmachers
* &amp;lbrack;UI&amp;rbrack; Engine nur bei der Validierung eines Schiebereglers aktualisieren (nicht bei der Eingabe eines Werts)
* &amp;lbrack;UI&amp;rbrack; Iray-Switch auf eine dedizierte Schaltfläche in der Hauptsymbolleiste bewegen (und seinen Tastaturbefehl ändern)
* &amp;lbrack;Werkzeug&amp;rbrack; Einstellung für das Quellspeicherortverhalten des Klonwerkzeugs hinzufügen
* &amp;lbrack;Shader&amp;rbrack; Lesen der Scheitelpunkt-Farben von Meshs in benutzerdefinierten Shadern zulassen
* &amp;lbrack;Skripterstellung&amp;rbrack; Liste der Textursatz, Kanäle und Ebenen abrufen
* &amp;lbrack;Skripterstellung&amp;rbrack; Helfer-Funktionen hinzufügen (URL zum Pfad, Exportpfad aus Projekt abrufen)
* &amp;lbrack;Mac&amp;rbrack; Erkennen der Mac OS-&quot;El Capitan&quot;-Version in der Protokolldatei

**Fest:**

* Absturz nach zweitem Export auf Substance share
* Absturz beim Kopieren einer Ebene zwischen Textursätzen mit Schnelle Maske-Daten.
* Einige Projekte haben einen sehr langen Updater, der viel Speicher beansprucht
* &amp;lbrack;Werkzeug&amp;rbrack; Absturz beim Auswählen einer Partikel-Vorgabe mit dem Klon-/Verwischen-Werkzeug
* &amp;lbrack;Baker&amp;rbrack; Das Laden von FBX dauert bei großen Meshs zu lange
* &amp;lbrack;Viewport&amp;rbrack; Gedehnt Umgebungs-Map auf einigen Computern
* &amp;lbrack;Viewport&amp;rbrack; Falsche Gamma-Konvertierung der Alpha-Zahl des Pinsels
* &amp;lbrack;Export&amp;rbrack; Alpha wird als Transparenz gespeichert und nicht als separater Kanal mit Tiff-Dateien.
* &amp;lbrack;Export&amp;rbrack; Normaler Kanal wird immer als OpenGL exportiert
* &amp;lbrack;Iray&amp;rbrack; Fehlende Schiebereglernamen für Iray-Einstellungen
* &amp;lbrack;Iray&amp;rbrack; Das Rendern erfolgt mit einer falschen Auflösung bei Retina/High DPI.
* &amp;lbrack;Iray&amp;rbrack; Absturz beim Skalieren der Benutzeroberfläche im Iray-Modus
* &amp;lbrack;Iray&amp;rbrack; Hohe Leistungsverlangsamung beim Rendern mit einigen niedrigen Auflösungen
* &amp;lbrack;Iray&amp;rbrack; Pause funktioniert nicht (Iray wird noch im Hintergrund berechnet)
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

* &amp;lbrack;Iray&amp;rbrack; Spezifikations-/Glanzvorlage und Shader aktualisieren, um mit Iray kompatibel zu sein
* &amp;lbrack;Export&amp;rbrack; Screenshots nach ArtStation exportieren
* &amp;lbrack;Skripterstellung&amp;rbrack; Unterstützt die Ausführung aus dem Plug-in-Verzeichnis
* &amp;lbrack;Skripterstellung&amp;rbrack; &quot;Speichern unter&quot; zulassen
* &amp;lbrack;UI&amp;rbrack; Doppelklicken auf einen Schieberegler, um den Wert zu bearbeiten
* Vela-Beispiel auf Substance share verschieben
* Neues Beispielprojekt : Kugelvorschau
* Benutzer vor einem Konflikt mit Shellerweiterungen warnen

**Fest:**

* Installation von Substance Painter 1.x durch Installationsprogramm außer Kraft gesetzt
* &amp;lbrack;UI&amp;rbrack; Das Layout der Kanalliste wurde mit Filtern unterbrochen
* &amp;lbrack;UI&amp;rbrack; Shader-Parameter werden nicht angezeigt
* &amp;lbrack;UI&amp;rbrack; Durch Ändern der Größe des Ebenenfensters wird der Inhalt falsch zugeschnitten
* &amp;lbrack;Werkzeug&amp;rbrack; Der Deckkraftkanal wird nicht immer richtig verwendet
* &amp;lbrack;Werkzeug&amp;rbrack; Verwischen/Klon funktioniert nicht mit Symmetrie
* &amp;lbrack;Werkzeug&amp;rbrack; Die Deckkraft der Pinselvorschau ist bei einigen Kanälen falsch
* &amp;lbrack;Iray&amp;rbrack; Absturz bei der Verwendung von Iray, obwohl es noch nicht erstellt wurde
* &amp;lbrack;Iray&amp;rbrack; Die Rastereinstellungsdaten aus dem Projekt können nicht geladen werden.
* &amp;lbrack;Iray&amp;rbrack; Iray kümmert sich nicht um die Einstellungsänderung, nachdem sie angehalten wurde
* &amp;lbrack;Regal&amp;rbrack; Das Importieren eines Materials in das Regal funktioniert nicht
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
* &amp;lbrack;Werkzeug&amp;rbrack; Neues Verwischen-Werkzeug zum Mischen und Verteilen von Farben
* &amp;lbrack;Werkzeug&amp;rbrack; Neues Klon-Werkzeug zum Kopieren von Teilen einer Textur
* &amp;lbrack;Werkzeug&amp;rbrack; Auswählen von Kanälen für das Verwischen-, Klon- und Radiergummi-Werkzeug zulassen
* &amp;lbrack;Ebene&amp;rbrack; Name des Substance für den Fülleffekt hinzufügen
* &amp;lbrack;Ebene&amp;rbrack; Exportieren der Maske in die Zwischenablage zulassen
* &amp;lbrack;Viewport&amp;rbrack; Zwischen Perspektive und orthografischem Modus wechseln
* &amp;lbrack;Viewport&amp;rbrack; Sichtfeld im Perspektive-Modus steuern
* &amp;lbrack;Viewport&amp;rbrack; Erlaubt das Festlegen der Tiefe des Feldabstands mit STRG + Mittelklick
* &amp;lbrack;Viewport&amp;rbrack; Lassen Sie zu ziehen und Umgebungs-Map in der 3D-Ansicht ablegen.
* &amp;lbrack;Viewport&amp;rbrack; Verbessertes Feedback bei umfangreichen Berechnungen des Engine
* &amp;lbrack;Export&amp;rbrack; Exportieren von Shader-Parametern in eine JSON-Datei zulassen
* &amp;lbrack;UI&amp;rbrack; Benutzeroberfläche mit neuen Symbolen, Farben und Layout aktualisieren
* &amp;lbrack;UI&amp;rbrack; Namen von Elementen zu Mini-Regals hinzufügen
* &amp;lbrack;UI&amp;rbrack; &quot;Kanal-Mapping&quot; standardmäßig reduzieren
* &amp;lbrack;Shader&amp;rbrack; Benutzerdefinierte Farbe für die Parameter der Shader-Textur auswählen
* &amp;lbrack;Regal&amp;rbrack; Frage beim Ziehen und Ablegen von Ressourcen nach dem Speicherort für Dateien
* &amp;lbrack;Regal&amp;rbrack; Neuer Vorschaubereich für Intelligente Material und Generatoren
* &amp;lbrack;Regal&amp;rbrack; Specular Glanz Shader hinzufügen
* &amp;lbrack;Regal&amp;rbrack; Neue Formen für harte Oberflächen
* &amp;lbrack;Regal&amp;rbrack; Neue Alphas Texturen und Formen
* &amp;lbrack;Regal&amp;rbrack; Neue Skin-Texturen
* &amp;lbrack;Regal&amp;rbrack; Neue Scan-basierte Material und Smart-Material
* &amp;lbrack;Regal&amp;rbrack; Neue intelligente Materialien und Spec/Gloss-Unterstützung von alten
* &amp;lbrack;Regal&amp;rbrack; Neue Finish-Filter für die metallic Oberflächensimulation
* &amp;lbrack;Regal&amp;rbrack; Neuer leistungsstarker Maskengenerator &quot;Maskeneditor&quot;
* &amp;lbrack;Regal&amp;rbrack; Alte Materialien überarbeitet und bereinigt
* Neues Beispielprojekt &quot;Vela&quot;

**Fest:**

* &amp;lbrack;Einstellungen&amp;rbrack; Die Drehung der Kamera und die Zoomgeschwindigkeit werden vom Projekt außer Kraft gesetzt.
* &amp;lbrack;Viewport&amp;rbrack; Genauigkeitsproblem bei der standardmäßigen normalen Textur führt zu falschen Reflexionen
* &amp;lbrack;Viewport&amp;rbrack; Vignette ist standardmäßig aktiviert
* &amp;lbrack;Viewport&amp;rbrack; Artefakte werden an den Umgebungs-Map-Rändern angezeigt (Nvidia-GPUs)
* &amp;lbrack;Viewport&amp;rbrack; Miniaturansicht im Modus &quot;Projektion/Schablone&quot; ist sehr lang zum Laden
* &amp;lbrack;Baker&amp;rbrack; Baking geführt Texturen in 16-Bit- statt in 32-Bit-Ganzzahl speichern
* &amp;lbrack;Ebene&amp;rbrack; Veraltete Stoffe werden im Stapel falsch dargestellt
* Standardfarbe und Bit-Tiefe für einige Kanäle sind falsch (z. B. : Specular, Glanz)
* Radierverhalten zum Deaktivieren der Füllmethode im Passthrough-Modus wurde korrigiert

**Bekannte Probleme:**

* Symmetrie funktioniert nicht mit dem Verwischen- und Klon-Werkzeug
* ArtStation-Export fehlt

## Version 1

### 1.7.3

*(Freigegeben: 1. März 2016)*

**Hinzugefügt:**

* &amp;lbrack;Export&amp;rbrack; Hinzufügen einer Option zum Deaktivieren der Auffüllung
* &amp;lbrack;Regal&amp;rbrack; Untergeordnete Elementhierarchie innerhalb eines Regal-Regals unterstützen

**Fest:**

* Absturz beim Speichern über einer zuvor schreibgeschützten Datei
* Absturz beim Öffnen eines zweiten Projekts
* Absturz beim Laden einiger Miniaturansichten (Regal, Ebenen oder QuickInfos)
* Die Deaktivierung von &quot;Konturpositionen auf dem Mesh beibehalten&quot; funktioniert nicht
* &amp;lbrack;Export&amp;rbrack; Die Hochskalierung von Bitmaps erfolgt mit nächstgelegenen Filterungen
* &amp;lbrack;Regal&amp;rbrack; Die Suche nach Ressourcen ist sehr langsam
* &amp;lbrack;Regal&amp;rbrack; Weichzeichnungsfilter sind nicht 16 Bit kompatibel
* &amp;lbrack;Werkzeug&amp;rbrack; Symmetrie funktioniert nicht, wenn Sie eine alte Werkzeugvorgabe laden
* Das Farbdialogfeld für den Specular-Kanal führt keine Farbraumkonvertierung durch

### 1.7.2

*(Freigegeben: 13. Januar 2016)*

**Hinzugefügt:**

* &amp;lbrack;Layers&amp;rbrack; Festlegen der Standardbearbeitung für Füllebenen zulassen

**Fest:**

* &amp;lbrack;Export&amp;rbrack; Sketchfab-Export funktioniert nicht mehr
* &amp;lbrack;Ebene&amp;rbrack; Bilineare Filterung wird auch bei &quot;Füllung&quot; ohne Transformation angewendet
* &amp;lbrack;Werkzeug&amp;rbrack; Schlechte Projektion durch Substance-Effekte mit Bildeingaben im Bewegungsmodus
* &amp;lbrack;Werkzeug&amp;rbrack; Material-Auswahl ist defekt

### 1.7.1

*(Freigegeben: 18. Dezember 2015)*

**Fest:**

* Absturz beim Wechseln des Textursatzes
* Langsame Bewegungen beim Malen

### 1.7.0

*(Freigegeben: 17. Dezember 2015)*

**Hinzugefügt:**

* &amp;lbrack;Performances&amp;rbrack; Berechnen des Inhalts von Ebenen und ihrer Miniaturansichten gleichzeitig
* &amp;lbrack;Export&amp;rbrack; Speichern Sie den Exportpfad als relativ, wenn er sich neben dem Projekt befindet
* &amp;lbrack;Layers&amp;rbrack; Neuer Mischmodus hinzugefügt : Subtrahieren und Hinzufügen/Subtrahieren
* &amp;lbrack;Layers&amp;rbrack; Neue Bilineare Filterungen des Hauptquartiers für Füllebenen
* &amp;lbrack;Shader&amp;rbrack; Legen Sie in den Voreinstellungen einen Standard-Shader für die Miniaturansichtenerstellung fest.
* &amp;lbrack;Shader&amp;rbrack; Geben Sie einen Shader pro Textursatz an
* &amp;lbrack;Shader&amp;rbrack; Texturen aus dem Regal aufnehmen
* &amp;lbrack;Werkzeug&amp;rbrack; Neues Pinselverhalten &quot;Umbrechen&quot; für das Malen
* &amp;lbrack;Werkzeug&amp;rbrack; Verbesserte Filterung und reduziertes Aliasing beim Malen
* &amp;lbrack;Werkzeug&amp;rbrack; Verbesserte Malqualität von Subpixeln
* &amp;lbrack;Werkzeug&amp;rbrack; &quot;Einfache&quot; Anzeige für Pinseleinstellungen entfernt und das Symbol zum Öffnen/Schließen des Rahmens verbessert
* &amp;lbrack;Menü&amp;rbrack; Hinzufügen von Effektsymbolen im Kontextmenü
* Vorlagenerstellung aus Projekten
* &amp;lbrack;Regal&amp;rbrack; Neue Vorlagen : PBR, Dota 2
* &amp;lbrack;Regal&amp;rbrack; Neue Exportvorgabe : Dota 2
* &amp;lbrack;Regal&amp;rbrack; Neue Shader : Dota 2, PBR Car Malen, PBR Coated, PBR Velvet
* &amp;lbrack;Regal&amp;rbrack; Neues Material : Rost und Verschleiß aus Stahl, Stilisierte Beleuchtung
* &amp;lbrack;Regal&amp;rbrack; Neue Filter : Weichzeichnen von gerichtetem, stilisiertem Licht
* &amp;lbrack;Regal&amp;rbrack; Neuer Pinsel : Standardmäßige weiche und Standardfestplatte mit einem neuen Alpha für eine bessere Steuerung der Härte
* &amp;lbrack;Regal&amp;rbrack; Neue Generatoren : 3D-Abstand und -Licht
* &amp;lbrack;Regal&amp;rbrack; Aktualisierte Pinsel mit Projektion und Rückseiten-Ausblendung des Textumbruchs (standardmäßig aktiviert)
* &amp;lbrack;Regal&amp;rbrack; Weißer Rauschen mit Pixelprozessor-Version wurde für eine schnellere Berechnung aktualisiert

**Fest:**

* &amp;lbrack;Begrüßungsbildschirm&amp;rbrack; Link &quot;Tutorials&quot; - an alte Videos senden
* &amp;lbrack;Channels&amp;rbrack; Wenn Sie &quot;Nein&quot; zur Erstellung einer Füllebene mit AO sagen, wird trotzdem die Ebene erstellt.
* &amp;lbrack;Channels&amp;rbrack; Benutzer-X-Kanalnamen werden in der Schnittstelle nicht weitergegeben
* &amp;lbrack;Viewport&amp;rbrack; Der Maskeneintrag ist in der Liste der Solokanäle leer.
* &amp;lbrack;Share&amp;rbrack; Beim Exportieren eines Alpha-Elements in die Freigabe vom SP wird eine unlesbare .image-Datei erstellt.
* &amp;lbrack;Lizenz&amp;rbrack; Aktivierung für Benutzernamen mit Nicht-ASCII-Zeichen beheben
* &amp;lbrack;Shader&amp;rbrack; Dialogfeld &quot;Farbparameter&quot; wird beim Auswählen einer Farbe ausgeblendet
* &amp;lbrack;Regal&amp;rbrack; Miniaturen werden nicht aus dem Speicher entladen, wenn sie nicht verwendet werden
* &amp;lbrack;Regal&amp;rbrack; Filter mit festem Verlauf
* &amp;lbrack;Werkzeug&amp;rbrack; Symmetrie funktioniert nicht mit Schablone/Projektion
* &amp;lbrack;Werkzeug&amp;rbrack; Falscher Name beim Erstellen einer neuen Pinselvorgabe
* Die Option &quot;Kontur beibehalten&quot; bleibt auch beim erneuten Importieren eines Meshs deaktiviert
* TDR (Driver Reset) beim Berechnen von Partikeln mit großen Abmessungen.

### 1.6.1

*(Freigegeben: 9. November 2015)*

**Fest:**

* Absturz beim Öffnen des Projekts, wenn die 2D-Ansicht sichtbar ist
* Absturz beim Erstellen einer neuen Exportvorgabe, wenn das aktuelle Regal nicht vorhanden ist
* &amp;lbrack;Werkzeug&amp;rbrack; Symbol für die Material-Auswahl kann angezeigt bleiben
* &amp;lbrack;Werkzeug&amp;rbrack; Material-Auswahl blendet den Mauszeiger aus, wenn gleichzeitig gemalt wird
* &amp;lbrack;Regal&amp;rbrack; Metadaten werden nach jedem Beenden auf die Festplatte geschrieben

### 1.6.0

*(Freigegeben: 29. Oktober 2015)*

**Hinzugefügt:**

* Offizielle Unterstützung für Windows 10
* &amp;lbrack;Substance&amp;rbrack; Substanzparametergruppen standardmäßig reduzieren
* &amp;lbrack;Substance&amp;rbrack; Neues Framework hinzufügen (Verbesserung der Pixelprozessor-Performance)
* &amp;lbrack;Viewport&amp;rbrack; Erlaubt die Deaktivierung der Anzeige der Symmetrie-Ebene im Symmetrie-Modus.
* &amp;lbrack;Viewport&amp;rbrack; Verbessern des Renderings von Schatten und der Leistung
* &amp;lbrack;Viewport&amp;rbrack; Berechnung von Schatten beim Malen anhalten
* &amp;lbrack;Viewport&amp;rbrack; Verbessern der Drahtgitter-Renderleistung
* &amp;lbrack;Engine&amp;rbrack; Verbesserte VRAM-Speicherverwaltung zur Reduzierung des Speicherplatzbedarfs
* &amp;lbrack;Engine&amp;rbrack; Verbessern der Leistungsaktualisierung auf AMD-GPUs für eine bessere Textur
* &amp;lbrack;Engine&amp;rbrack; Deaktivieren der Einstellung für die Threadoptimierung auf NVIDIA-GPUs für bessere Leistung
* &amp;blase;Effekt&amp;blase; Tag hinzufügen, um eine &quot;aufgefüllte&quot; Bildeingabe anzufordern
* &amp;lbrack;Ebene&amp;rbrack; Präzision des UV-Versatzes/der Skalierung in der Füllung erhöhen
* &amp;lbrack;Ebene&amp;rbrack; Skalierungsregler in der Füllung exponentiell machen
* &amp;lbrack;Ebene&amp;rbrack; Erlauben Sie, Materialien direkt in den Ebenenstapel zu ziehen und abzulegen.
* &amp;lbrack;Ebene&amp;rbrack; Ermöglicht das Ziehen und Ablegen von Filtern direkt in den Ebenenstapel
* &amp;lbrack;Ebene&amp;rbrack; Maskenpinselfarbe an die neu erstellte Maskenfarbe anpassen
* &amp;lbrack;Shader&amp;rbrack; Leg mehrerer Texcoords
* &amp;lbrack;Shader&amp;rbrack; Leg der Gamma-/Tonzuordnungsfunktion, um benutzerdefinierte Funktionen zu ermöglichen
* &amp;lbrack;Baker&amp;rbrack; Ändern der Standardeinstellungen des Bakers &quot;Position&quot; für die Verwendung von TriPlanar
* &amp;lbrack;Werkzeug&amp;rbrack; Benennen Sie &quot;Geometry Decal&quot; in &quot;Polygon Fill&quot; um.
* &amp;lbrack;Regal&amp;rbrack; Generatoren zur Unterstützung von TriPlanar aktualisieren : MG Metallkantenverschleiß, MG Maskenbildner, MG Glasfaser, MG Dirt
* &amp;lbrack;Regal&amp;rbrack; Aktualisieren von Materials mit neuen Einstellungen und Entfernen nicht verwendeter Materials
* &amp;lbrack;Regal&amp;rbrack; 22 neue intelligente Materialien (Kunststoff, Eisen, Stoff, Stahl und mehr)
* &amp;lbrack;Regal&amp;rbrack; Die Filter &quot;Schärfen&quot;, &quot;Weichzeichnen&quot; und &quot;Verformen&quot; mit aufgefüllten Bilddaten aktualisieren, um Nähte zu vermeiden
* &amp;lbrack;Regal&amp;rbrack; Verbessern der Verkrümmungseinstellungen für eine einfachere Verwendung
* &amp;lbrack;Regal&amp;rbrack; 2 neue prozedurale Rauschen: 3D Perlin Rauschen und 3D Worley Rauschen

**Fest:**

* &amp;lbrack;Engine&amp;rbrack; Die VRAM-Betragserkennung für die dedizierte GPU ist auf Mac falsch
* &amp;lbrack;Engine&amp;rbrack; Texturen werden im Viewport dunkler
* &amp;lbrack;Engine&amp;rbrack; Schlechte Leistung beim Malen unter mehreren Ebenen
* &amp;lbrack;Engine&amp;rbrack; Beim Öffnen des Projekts berechnete Ebenen unterscheiden sich von der zwischengespeicherten Version
* &amp;lbrack;Substance&amp;rbrack; Falsche Ergebnisse in 4K auf Mac
* &amp;lbrack;Substance&amp;rbrack; Die Parameter haben die falsche Reihenfolge.
* &amp;lbrack;Shader&amp;rbrack; Toon und verpixelte Shader sind total schwarz
* &amp;lbrack;Shader&amp;rbrack; Parameter verschwinden nach dem Ändern der env-map
* &amp;lbrack;Regal&amp;rbrack; Absturz beim Bereitstellen von PNG-Dateien im Generatorordner
* &amp;lbrack;Regal&amp;rbrack; Miniaturansichten werden mit niedriger Rauheit generiert
* &amp;lbrack;Werkzeug&amp;rbrack; Absturz bei Verwendung einer Bitmap im Pinsel-Alpha unter Windows
* &amp;lbrack;Export&amp;rbrack; Eine zusätzliche Kartenexportvorgabe exportiert jetzt eine RGB-Karte für die Position

### 1.5.7

*(Freigegeben: 24. September 2015)*

**Fest:**

* Absturz-Bericht funktioniert nicht mehr

### 1.5.6

*(Freigegeben: 21. September 2015)*

**Hinzugefügt:**

* &amp;lbrack;Regal&amp;rbrack; Verbessern der Qualität der Miniaturansichten (verwenden Sie 1K-Texturen)

**Fest:**

* &amp;lbrack;Share&amp;rbrack; Anmeldung mit einem anderen Konto nicht möglich
* &amp;lbrack;Regal&amp;rbrack; Miniaturansichten sind auf der Festplatte zu groß
* &amp;lbrack;Regal&amp;rbrack; Intelligente Materialien sind sehr langsam
* &amp;lbrack;Windows&amp;rbrack; Installation des Lizenz-Service beheben
* &amp;lbrack;Channels&amp;rbrack; Transmissive map wird standardmäßig als G8 erstellt

### 1.5.5

*(Freigegeben: 15. September 2015)*

**Hinzugefügt:**

* &amp;lbrack;Regal&amp;rbrack; Exportieren von Assets auf Substance share
* &amp;lbrack;Regal&amp;rbrack; Neue Kugelvorschau für Materialien hinzufügen
* &amp;lbrack;Regal&amp;rbrack; Verwenden Sie die Env-Karte &quot;Glasüberdachter Patio&quot; zum Generieren von Miniaturen
* &amp;lbrack;Regal&amp;rbrack; Auflösung der Miniaturbildgröße auf 512 x 512 Pixel erhöhen
* &amp;lbrack;3D-Ansicht&amp;rbrack; Umgebungsdrehungswert gelegt
* &amp;lbrack;Windows&amp;rbrack; Anwendung signieren

**Fest:**

* &amp;lbrack;Baker&amp;rbrack; Falsche Ergebnisse beim gleichzeitigen Baking von Karten
* &amp;lbrack;3D-Ansicht&amp;rbrack; Die Env-Map wird angezeigt, wenn kein Projekt geöffnet ist
* &amp;lbrack;Layers&amp;rbrack; Maskengenerator funktionieren nicht auf Ebeneninhalten
* &amp;lbrack;Layers&amp;rbrack; Sie können Malen auf ausgeblendeten Ebenen durchführen
* &amp;lbrack;Regal&amp;rbrack; Rauschen mit Dirt_5 und Dirt_6 sind identisch
* &amp;lbrack;Regal&amp;rbrack; Einige Maskengenerator sind verpixelt oder haben eine niedrige Qualität
* &amp;lbrack;Werkzeug&amp;rbrack; Falsche Gizmo-Drehung um bestimmte Winkel.
* &amp;lbrack;Werkzeug&amp;rbrack; Zu viele Kanäle führen dazu, dass die Kanalschaltflächen abgeschnitten werden
* &amp;lbrack;Werkzeug&amp;rbrack; Tastaturbefehl der Maske für Schnelle Maske umkehren funktioniert nicht
* &amp;lbrack;Export&amp;rbrack; Sketchfab: Schaltfläche &quot;Abbrechen&quot; wird nicht korrekt berücksichtigt
* &amp;lbrack;Lizenz&amp;rbrack; Aktivierung fehlgeschlagen, wenn die Lizenz nicht kopiert werden kann
* Der Framerate-Begrenzer funktioniert nicht mehr auf der Benutzeroberfläche

### 1.5.0

*(Freigegeben: 20. August 2015)*

**Hinzugefügt:**

* &amp;lbrack;Shader&amp;rbrack; Zeilennummer in Fehlermeldungen beim Kompilieren von Shader hinzufügen
* &amp;lbrack;Regal&amp;rbrack; Verbessern der Vorschauqualität von Miniaturen
* &amp;lbrack;Regal&amp;rbrack; Miniaturansichten für Intelligenten Materials automatisch erstellen
* &amp;lbrack;Werkzeug&amp;rbrack; Tastaturbefehl zur Einstellung der Härte im Stoff
* &amp;lbrack;Werkzeug&amp;rbrack; Graustufen-Widget für Geometrieaufkleber verwenden, wenn Sie sich über einer Maske befinden
* &amp;lbrack;Werkzeug&amp;rbrack; Tastaturbefehl zum Umkehren der Malen-Farbe beim Malen auf einer Graustufenkarte
* &amp;lbrack;Viewport&amp;rbrack; Anzeige des Drahtgitter und Farbänderung zulassen
* &amp;lbrack;Viewport&amp;rbrack; Hintergrund der Umgebung weichzeichnen
* &amp;blbrack;Steuerung&amp;blbrack; Hinzufügen von Drehung zu Pinselmaus-Kurzbefehlen
* &amp;lbrack;Export&amp;rbrack; Exportieren nach Sketchfab
* &amp;lbrack;Export&amp;rbrack; Erstellen von Exportvorgaben für Renderer
* &amp;lbrack;Export&amp;rbrack; Konvertierte Abbildung hinzufügen - Reflexion, F0 und 1/IOR
* &amp;lbrack;UI&amp;rbrack; Startbildschirm hinzufügen
* &amp;lbrack;UI&amp;rbrack; Standardlayout aktualisieren
* &amp;lbrack;UI&amp;rbrack; Hinzufügen fehlender QuickInfos und Umbenennen einiger Menüeinträge
* &amp;lbrack;Layers&amp;rbrack; Exportieren der aktuell ausgewählten Maske als Bitmap
* &amp;lbrack;Layers&amp;rbrack; Aktion &quot;Maske umkehren&quot; im Kontextmenü hinzufügen

**Fest:**

* &amp;lbrack;Projekt&amp;rbrack; Wenn sich die Pivot-Werte der Meshs in der FBX unterscheiden, werden die Meshs beim Importieren explodiert
* &amp;lbrack;Substance&amp;rbrack; Substance in Projektion-Tools sind in 256\*256 gesperrt
* &amp;lbrack;Layers&amp;rbrack; Absturz bei Verwendung von &quot;Maske löschen&quot;
* &amp;lbrack;Export&amp;rbrack; Falsche Gamma-Konvertierung auf sehr dunklen Texturen
* &amp;lbrack;Export&amp;rbrack; Die Positionszuordnung kann nur in Exportvorgaben als Graustufenzuordnung verwendet werden.
* &amp;lbrack;Werkzeug&amp;rbrack; Die Anfangsfarbe des Geometrie-Aufklebers ist schwarz, wenn er auf einer Maske verwendet wird
* &amp;lbrack;Werkzeug&amp;rbrack; &quot;Drehung - Tastaturbefehl&quot; funktioniert nicht, wenn keine Härte im Alpha-Wert vorhanden ist

### 1.4.2

*(Freigegeben: 15. Juli 2015)*

**Fest:**

* &amp;lbrack;Werkzeug&amp;rbrack; Absturz bei der Verwendung von Geometrieaufklebern mit schnelle Maske
* Beim Aktualisieren des Projekts von 1.4.0 auf 1.4.1 wird der gesamte Computerspeicher belegt.
* Falscher Import des alten Projektformats
* Bei benutzerdefinierten Regalen wird die gesamte Hierarchie analysiert, und Assets werden überall dupliziert.

### 1.4.1

*(Freigegeben: 23. Juni 2015)*

**Hinzugefügt:**

* &amp;lbrack;Viewport&amp;rbrack; Andocken von Fenstern nebeneinander zulassen
* &amp;blase;Effekt&amp;blase; Hinzufügen eines Hintergrunds und eines Lineals für den Ebeneneffekt
* &amp;blase;Effekt&amp;blase; Einen Malen-Effekt hinzufügen, der es ermöglicht, über andere Effekte zu arbeiten

**Fest:**

* &amp;lbrack;Regal&amp;rbrack; Miniaturgenerierung funktioniert nicht, wenn kein Projekt geöffnet ist
* &amp;lbrack;Regal&amp;rbrack; Materialvorgabe-Vorschau kann nicht generiert werden
* &amp;lbrack;Regal&amp;rbrack; Material-Vorschauen werden auf einem Mesh mit invertierten Normalen generiert
* &amp;lbrack;Regal&amp;rbrack; Miniaturen werden aufgrund einer falschen Hash-Funktion immer neu berechnet
* &amp;lbrack;Regal&amp;rbrack; Wenn Sie auf ein Substance-Material klicken, werden keine zusätzlichen Maps verbunden.
* &amp;lbrack;Werkzeug&amp;rbrack; Falscher Wert, der mit der Material-Auswahl aufgenommen wurde
* &amp;lbrack;Werkzeug&amp;rbrack; Farbwähler Viewport auswählen Cursorfarbe
* &amp;lbrack;2D-Ansicht&amp;rbrack; Sehr niedrige Framerate/Performance
* &amp;lbrack;Export&amp;rbrack; Absturz beim Öffnen des Exportfensters mit zu aktuellen Exportvorgaben.
* &amp;lbrack;Export&amp;rbrack; Height-Kanal auf Normalen-Map wird in den falschen Bereich konvertiert
* &amp;lbrack;Mac&amp;rbrack; BaseColor aus Substance-Effekten wird als Linear angezeigt
* &amp;lbrack;Mac&amp;rbrack; Widget für gerade Linien wurde auf der Retina falsch gezeichnet
* Gerade Linien können auch bei einem Loslassen des Tastaturbefehl aktiviert bleiben.
* Gerade Linien Guizmo verschwinden nach dem Drehen des Umgebungs-Map
* Ambient occlusion-Ausgänge von Stoffen werden nicht automatisch an den AO-Kanal angeschlossen
* Problem mit Lizenzkopien unter Windows mit Sonderzeichen im Benutzernamen beheben

### 1.4.0

*(Freigegeben: 10. Juni 2015)*

**Hinzugefügt:**

* &amp;lbrack;Export&amp;rbrack; Zusätzliche Maps in der Liste der verfügbaren Eingabe-Map hinzufügen
* &amp;lbrack;Regal&amp;rbrack; SBSAR-Materialien als Materialvorgaben verwenden
* &amp;lbrack;Regal&amp;rbrack; Verwenden benutzerdefinierter Bibliothekspfade zulassen
* &amp;lbrack;Regal&amp;rbrack; Die Mindestgröße ändern.
* &amp;lbrack;Regal&amp;rbrack; Neue Inhalte : 20 neue intelligente Material
* &amp;lbrack;Regal&amp;rbrack; Neue Inhalte : neuer prozeduraler Stoff (Gewebe, Mesh)
* &amp;lbrack;Regal&amp;rbrack; Aktualisierter Weichzeichnungsfilter
* Zeichnen von geraden Linien mit einer Zusatztaste
* Hinzufügen eines Ambient occlusion-Kanals und Überarbeiten des AO/Normal-Verhaltens im Ebenenstapel
* Lesen der Standardfarbe aus der Bildeingabe, die in den Substance-Benutzerdaten definiert ist
* Exportieren des Protokolls über das Hilfemenü zulassen

**Fest:**

* &amp;lbrack;Baker&amp;rbrack;&amp;lbrack;Mac&amp;rbrack; Absturz mit Normal vom Mesh Baker
* &amp;lbrack;Baker&amp;rbrack; Absturz, wenn die Käfig-Datei keine UVs enthält
* &amp;lbrack;Baker&amp;rbrack; Das Abgleichen nach Namen funktioniert nicht mit aus zBrush exportierten OBJ
* &amp;lbrack;Baker&amp;rbrack; Beim Baking mit einem Käfig wird das Baking überschrieben, wenn mehrere Textursatz und überlappende UVs verwendet werden.
* &amp;lbrack;Baker&amp;rbrack; Bestimmte OBJ führen zu schwarzen Texturen
* &amp;lbrack;Regal&amp;rbrack; Ressourcen können nicht gelesen werden, wenn sie auf schreibgeschützt festgelegt sind
* &amp;lbrack;Regal&amp;rbrack; Asset-Dateien werden in Painter geschrieben, wenn sie im Projekt verwendet wurden.
* &amp;lbrack;Regal&amp;rbrack; Durch erneutes Laden von Stoffen wird auch die Schicht aktualisiert
* &amp;lbrack;Export&amp;rbrack; Tiff exportiert 32-Bit-Bilder, die von Photoshop oder Game-Enginen nicht richtig gelesen werden können
* &amp;lbrack;Export&amp;rbrack; Standardkanalvorgaben werden immer als RGB exportiert
* &amp;lbrack;Material&amp;rbrack; Diffuse-Kanal überschreibt BaseColor-Zuordnung mit Stoffen
* &amp;lbrack;3D-Ansicht&amp;rbrack; Falsche Diffuse mit spezifischen Umgebungskarten
* &amp;lbrack;Werkzeug&amp;rbrack; Pinsel kann nicht in einen bestimmten Winkel gedreht werden
* Viewport erhält den Fokus, wenn der Mauszeiger während der Eingabe in einem Textfeld auf
* Absturz mit zu aktuellen Vorgaben für die aktuelle Version des Regals
* Absturz nach dem Ersetzen von Mesh
* Absturz beim erneuten Laden eines Stoffes mit einer anderen Anzahl von Einsatzstoffen
* FBX von Meshs aus dem Cinema4D-Import mit falschen Material-Namen

### 1.3.5

*(Freigegeben: 29. Mai 2015)*

**Hinzugefügt:**

* &amp;lbrack;Lizenz&amp;rbrack; Aktivierungsproblem, wenn eine bereits vorhandene Lizenzdatei vorhanden ist
* &amp;lbrack;Mac&amp;rbrack; Absturz beim Laden bestimmter FBX
* &amp;lbrack;Mac&amp;rbrack;&amp;lbrack;3D-Ansicht&amp;rbrack; Falsche Spiegelung für integrierte GPU
* &amp;lbrack;3D-Ansicht&amp;rbrack; Schnelle Maske-Schrift ist defekt
* &amp;lbrack;3D-Ansicht&amp;rbrack; Material-Picker macht den Viewport komplett schwarz
* Absturz nach dem Öffnen von Projekten, die in 1.3.3 erstellt wurden
* Die Vorschau des Materials ist leer, wenn Shader mit Alpha verwendet werden
* Malerei funktioniert nicht mehr an bestimmten Meshs
* Die Leistung nimmt mit bestimmten OBJ Meshs stark ab
* Benutzerkanäle werden bei Verwendung von Effekten nicht zugeordnet
* Temporäre Ordner werden beim Start nicht gesäubert

**Fest:**

* Verbesserte Berechnung des Projekts, das extrem lange geladen werden muss
* Ändern Sie das Fenster &quot;GPU-Fehlerbehebung&quot;, um verständlicher zu sein
* &amp;lbrack;Layers&amp;rbrack; Speichern Sie den Status der Verhältnissperre für Füllebenen und stellen Sie sie standardmäßig auf &quot;Ein&quot;
* &amp;lbrack;Baker&amp;rbrack; Bei der Zuordnung nach Namen wird jetzt das Suffix als Trennzeichen verwendet.

### 1.3.4

*(Freigegeben: 27. April 2015)*

**Hinzugefügt:**

* &amp;lbrack;Mac&amp;rbrack; Absturz mit Mac OS X Yosemite (10.10)
* &amp;lbrack;Mac&amp;rbrack; Vollbildmodus kann nicht beendet werden
* &amp;lbrack;Baker&amp;rbrack; Baking der Option &quot;Namensübereinstimmungen&quot; funktioniert nicht
* &amp;lbrack;Baker&amp;rbrack; Mikk-Tangente-Speicherplatz in SP funktioniert nicht mit UE4
* &amp;lbrack;Baker&amp;rbrack; ID-Baker kann die ID-Farben des Materials nicht Baking geführt haben
* &amp;lbrack;2D-Ansicht&amp;rbrack; Drahtgitter wird bei Verwendung des Geometry-Aufklebers nicht angezeigt
* &amp;lbrack;Werkzeug&amp;rbrack; Pinsel-Alphakanal wird bei Materialien als Checker anstelle von Transparenz angezeigt
* &amp;lbrack;Werkzeug&amp;rbrack; Absturz mit geometrischem Aufkleber
* &amp;lbrack;Layers&amp;rbrack; Der Steckplatz des Materials ist bei der Füllebene standardmäßig ausgeblendet
* &amp;lbrack;Export&amp;rbrack; Absturz beim Exportieren mit einer höheren Auflösung als der Textursatz
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
* &amp;lbrack;Regal&amp;rbrack; Neue Umgebungs-Map hinzufügen : Korsika Strand, Studio 05, Tornoco Studio und mehr
* &amp;lbrack;Regal&amp;rbrack; MG-Maskenbildner mit neuen Parametern aktualisieren
* &amp;lbrack;Regal&amp;rbrack; Alte Umgebungs-Map aktualisieren und kalibrieren

**Fest:**

* Absturz beim Öffnen des Exportfensters
* Drag &amp; Drop im UI-Widget ist nicht möglich, wenn abgedockt
* &quot;Nach Updates suchen&quot; funktioniert nicht
* &amp;lbrack;Layers&amp;rbrack; Wählen Sie die Maske nicht aus, wenn Sie bei gedrückter Alt-Taste darauf klicken
* &amp;lbrack;Werkzeug&amp;rbrack; Tri-planar funktioniert nicht mit dem normalen Kanal
* &amp;lbrack;3D-Ansicht&amp;rbrack; Diffuse Beleuchtung von env map ist nicht korrekt
* &amp;lbrack;3D-Ansicht&amp;rbrack; Die Berechnung der Belichtung unterscheidet sich von der in Designer
* &amp;lbrack;3D-Ansicht&amp;rbrack; Schatten sollten auf 100 % metallic Fläche nicht sichtbar sein.
* &amp;lbrack;3D-Ansicht&amp;rbrack; Mesh mit gespiegelten UVs hat gespiegelte Tangente/Binomale
* &amp;lbrack;3D-Ansicht&amp;rbrack; Schatten führen bei bestimmten Meshs zu falschen Ergebnissen
* &amp;lbrack;Baker&amp;rbrack; Ordner &quot;.alg_meta&quot;, der mit Assbin-Dateien erstellt wurde, entfernen
* &amp;lbrack;Baker&amp;rbrack; Absturz beim Baking, wenn Painter ein TextureSet gleichzeitig neu berechnet
* &amp;lbrack;Mac&amp;rbrack; Benutzeroberflächenfehler beim Starten der Anwendung

### 1.3.2

*(Freigegeben: 06. März 2015)*

**Fest:**

* &amp;lbrack;3D-Ansicht&amp;rbrack; Fehler beim erneuten Laden einer mit dem Projekt gespeicherten Env-Map.

### 1.3.1

*(Freigegeben: 05. März 2015)*

**Hinzugefügt:**

* &amp;lbrack;Baker&amp;rbrack; Fügen Sie eine zwischengespeicherte Version von Meshs mit hohem Poly-Anteil hinzu, um die Berechnung zu beschleunigen
* &amp;lbrack;Baker&amp;rbrack; Warnsymbol hinzufügen, wenn kein Mesh mit hoher Poly-Qualität geladen wird
* &amp;lbrack;Baker&amp;rbrack; Wenn kein Mesh mit hoher Poly-Qualität geladen wird, verwenden Sie stattdessen den Projekt-Mesh

**Fest:**

* &amp;lbrack;Baker&amp;rbrack; Drücken der &quot;Eingabe&quot; beim Bearbeiten des Werts eines Schiebereglers, um das Fenster zu schließen
* &amp;lbrack;Baker&amp;rbrack; Das Aktivieren/Deaktivieren eines Bakers löst ebenfalls die Schaltfläche aus.
* &amp;lbrack;Baker&amp;rbrack; Es kann nicht Baking geführt werden, wenn Sie die Schaltfläche &quot;all/none&quot; verwenden.
* &amp;lbrack;Baker&amp;rbrack; Die Sortierung der Baker-Schaltflächen ist nicht in der richtigen Reihenfolge.
* &amp;lbrack;Baker&amp;rbrack; Kontrollkästchen werden ignoriert und alle Baker werden immer verarbeitet.
* &amp;lbrack;Baker&amp;rbrack; Fortschritt der Fortschrittsleiste behoben

### 1.3.0

*(Freigegeben: 04. März 2015)*

**Hinzugefügt:**

* &amp;lbrack;Baker&amp;rbrack;&amp;lbrack;3D-Ansicht&amp;rbrack; Mikkt-Tangente-Raum-Berechnung verwenden, wenn keine Tangenten/Binormale gefunden wurden
* &amp;lbrack;Baker&amp;rbrack; Neue Baker hinzugefügt : Normal, ID, Verdeckung, Krümmung, Thickness, Position
* &amp;blase;Effekte&amp;blase; Der Stapel &quot;Effekt&quot; ist jetzt invertiert und wird von oben nach unten (wie Ebenen) angezeigt.
* &amp;blase;Effekte&amp;blase; Hinzufügen neuer Symbole auf dem Stapel des Effekts
* &amp;blase;Effekte&amp;blase; Fülloptionen im Stapel &quot;Effekt&quot; mit Füllmethode versehen
* &amp;blase;Effekte&amp;blase; Effekte umbenennen (Substance-Effekt = Filter, usw.)
* Hinzufügen einer &quot;gesperrten&quot; Datei während des Speichervorgangs
* &amp;blase;Effekte&amp;blase; Aktion &quot;Füllen&quot; im Stapel &quot;Effekt&quot; hinzufügen
* Neue Ressource hinzugefügt : Intelligente Materialien
* &amp;lbrack;Layers&amp;rbrack; Neuanordnung von Ebeneneffekten zulassen
* &amp;lbrack;Werkzeug&amp;rbrack; Planare Projektion hinzufügen
* &amp;lbrack;3D-Ansicht&amp;rbrack; Unterstützung für Schatten hinzufügen
* &amp;lbrack;3D-Ansicht&amp;rbrack; Möglichkeit, erforderliche OpenGL-Status in benutzerdefinierte Shader umzuwandeln
* &amp;lbrack;3D-Ansicht&amp;rbrack; Unterstützung für Alpha über neue Shader
* &amp;lbrack;3D-Ansicht&amp;rbrack; Shader sind jetzt versioniert und vollständig in einem Projekt gespeichert
* &amp;lbrack;3D-Ansicht&amp;rbrack; Benutzer warnen, wenn der Shader nicht mehr kompiliert wird

**Fest:**

* &amp;lbrack;Layers&amp;rbrack; Ablegen unter einem reduzierten Ordner korrigieren
* &amp;lbrack;Regal&amp;rbrack; Filterung von Inhalten in Mini-Regals korrigieren
* &amp;lbrack;Regal&amp;rbrack; Umbenennen von Kategorien und Neuanordnen von Registerkarten

### 1.2.1

*(Freigegeben: 12. Februar 2015)*

**Hinzugefügt:**

* \*.spp-Dateien können jetzt durch einen Doppelklick im Explorer geöffnet werden
* &amp;lbrack;Export&amp;rbrack; Neues Tag &quot;$project&quot; für Exportvorgaben
* &amp;lbrack;Export&amp;rbrack; Kartenliste (mit Nomenklatur) unter jedem Textursatz hinzufügen
* &amp;lbrack;Export&amp;rbrack; Schaltfläche &quot;Alle/Keine&quot; hinzufügen, um die Textursatz auszuwählen
* &amp;lbrack;Export&amp;rbrack; Leere Karten werden beim Export verworfen

**Fest:**

* &amp;lbrack;Export&amp;rbrack; Unity5-Vorgaben haben invertierte Karten
* &amp;lbrack;Export&amp;rbrack; Durch Hinzufügen eines Schrägstrichs in einem Vorgabename wird ein beschädigter Ordner erstellt.
* &amp;lbrack;Export&amp;rbrack; Height-Kanal, der in 32-Bit-Formate exportiert wird, ist falsch eingespannt
* &amp;lbrack;Export&amp;rbrack; Die Liste der Textursatz wird nicht wie im Projekt sortiert
* &amp;lbrack;Werkzeug&amp;rbrack; Rückseiten-Ausblendung funktioniert nicht mehr
* Speichern funktioniert nicht mit Sonderzeichen im Pfad

### 1.2.0

*(Freigegeben: 28. Januar 2015)*

**Hinzugefügt:**

* Neuer Normalkanal, der das Malen von Normalen-Map-Daten und das Kombinieren der Ergebnisse ermöglicht
* &amp;lbrack;Export&amp;rbrack; Neues Exportfenster mit der Möglichkeit, ein benutzerdefiniertes Packing zu erstellen und benutzerdefinierte Namen festzulegen
* Das Projektdateiformat ist jetzt eine einzelne Datei anstelle von Ordnern
* &amp;lbrack;Export&amp;rbrack; Unterstützung verschiedener Normalformate (DirectX, OpenGL)
* &amp;lbrack;Export&amp;rbrack; Erstellen einer temporären Sperrdatei während des Exports
* &amp;lbrack;Layers&amp;rbrack; Umschalt+Linksklick kann zum Umschalten einer Maske verwendet werden
* &amp;lbrack;Parameter&amp;rbrack; Legt den Farbraum am unteren Rand einer Bildeingabe bei
* &amp;lbrack;Regal&amp;rbrack; Effekt &quot;MG Mask Builder&quot; hat jetzt neue Einstellungen
* &amp;lbrack;3D-Ansicht&amp;rbrack; Ambient occlusion-Map verschließt jetzt den diffusen Beitrag, nicht den Specular

**Fest:**

* Projektion Material/Schablone Vorschau wird im Viewport nicht richtig angezeigt
* &amp;lbrack;3D-Ansicht&amp;rbrack; Tastaturbefehl-QuickInfo wird nicht angezeigt, wenn &quot;S&quot; (Schablone) Tastaturbefehl verwendet wird
* &amp;lbrack;Regal&amp;rbrack; Effekt &quot;MatFx Skin Scale&quot; hat jetzt bessere Leistung bei niedriger Auflösung
* &amp;lbrack;Export&amp;rbrack; Texturen aus dem Export werden beim Festlegen einer größeren Dokumentgröße einfach hochskaliert

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

* &amp;lbrack;Ebene&amp;rbrack; Auswählen der Ebene oben beim Öffnen eines Projekts/Wechseln zwischen Textursätzen
* Verbesserte Geschwindigkeit beim Speichern und Speichern unter mit neuem Komprimierungsalgorithmus
* Anzeige eines Fehlers beim Öffnen eines zu aktuellen Projekts für Painter

**Fest:**

* &amp;lbrack;Werkzeug&amp;rbrack; Geometry Decal produziert Speicherbeschädigungen
* &amp;Klammer;Pinsel&amp;Klammer; Es ist nicht möglich, Schwimmerwerte unter 1 für die Pinselgröße manuell einzugeben
* &amp;lbrack;Ebene&amp;rbrack; Durch das Erstellen eines Farbauswahl-Effekts wird dieser nicht in den Ebenenstapel eingefügt
* &amp;lbrack;Ebene&amp;rbrack; Wenn Sie den Mauszeiger über die Ebenen bewegen, wechselt Painter in die Taskleiste.
* &amp;lbrack;Ebene&amp;rbrack; Das Hinzufügen einer Bitmap als Maske kann zu einem Absturz führen
* GUI für den Solo-Modus mit dem Height-Kanal ist falsch
* &quot;Projekt speichern&quot; kann fehlschlagen und ein Projekt beschädigen
* Absturz beim Öffnen eines Projekts nach dem Laden eines anderen Projekts mit einem veralteten Shader

### 1.1.0

*(Freigegeben: 16. Dezember 2014)*

**Hinzugefügt:**

* &amp;blase;Effekt&amp;blase; Erstellen einer neuen Materialien-ID-Maske
* Neue gepunktete weiße/schwarze Linie für das Pinsel-Gizmo
* Neuer Parameter &quot;Winkelfolge&quot;
* Neuer Parameter &quot;Rückseiten-Ausblendung&quot;
* Neuer Parameter für die Verzögerte Mausbewegung
* &amp;lbrack;Layers&amp;rbrack; Unterstützung für Mehrfachauswahl und -verwaltung
* &amp;lbrack;Layers&amp;rbrack; Kopieren und Einfügen von einem Textursatz in einen anderen
* &amp;lbrack;Export&amp;rbrack; PSD-Format von Adobe Photoshop
* &amp;lbrack;Regal&amp;rbrack; Neues Werkzeug : Fell, Metallstiche und Reißverschluss
* &amp;lbrack;Regal&amp;rbrack; Neuer Pinsel : Schimmel, Bleistift, scharfe Linie und Stich
* &amp;lbrack;Regal&amp;rbrack; Neues Alpha : Gaußsches Rauschen, scharfe Linie, Form, Stift, Spritzen, Stich, Reißverschluss
* Verbesserte Malleistung durch Aktualisierung nur eines Teils der benötigten Texturen

**Fest:**

* &amp;lbrack;Regal&amp;rbrack; Es ist nicht möglich, einen Stoff mit Graf mit gleichen Etiketten zu laden.
* &amp;lbrack;Layers&amp;rbrack; Der Mischmodus &quot;Hindurchwirken&quot; funktioniert nicht mit Masken
* &amp;lbrack;Schablone&amp;rbrack; Skalierung in 2D-Ansicht funktioniert nicht
* Probleme und Absturz auf Mac OS Yosemite

### 1.0.2

*(Freigegeben: 9. November 2014)*

**Hinzugefügt:**

* Verbesserte Performance bei der Vorschau von Materialien mit Substanzen
* Verbesserte Leistung mit der Vorschau des Pinselstrichs beim Aktualisieren des Dokuments
* Verbesserte Leistung im Viewport mit niedrigerer Aktualisierungsrate für nicht funktionierenden Bereich
* &amp;lbrack;Post-Effekte&amp;rbrack; Verbesserte Benutzeroberfläche zum Verwalten von Einstellungen
* &amp;lbrack;Post-Effekte&amp;rbrack; Auf Standardwerte zurücksetzen
* Substance von Effekten und Ebenenoperationen im Kontextmenü
* Unterstützung für die vormultiplizierte Ein-/Ausgabe in Stoffen

**Fest:**

* &amp;lbrack;3D-Ansicht&amp;rbrack; Benutzerdefinierte Shader-Parameter werden durch einen großen Leerraum voneinander getrennt
* &amp;lbrack;Export&amp;rbrack; Fehlende sRGB-Konvertierung für Unity4-Vorgabe
* Möglicher Absturz beim Laden von FBX-Meshs
* Absturz kann beim Laden von einfachen obj-Meshs auftreten
* Die Rechenleiste bleibt beim Laden auf 100 % blockiert.
* Durch das erneute Laden eines Stoffes wird dieser in jede Kategorie verschoben
* DirectX/OpenGL-Switch defekt

### 1.0.1

*(Freigegeben: 27. Oktober 2014)*

**Hinzugefügt:**

* &amp;lbrack;Werkzeug&amp;rbrack; Verbesserte Verwendung von Material-Parametern
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
* &amp;lbrack;Export&amp;rbrack; Fügen Sie vor dem Nachbearbeiten der Diffusion eine Ausdehnung hinzu.
* Befehlszeilenargumente in SP für einfache Vorgänge
* Neue Material und Effekte
* Werkzeugvorschau (separate Echtzeitvorschau von Materialien und Bereich für Konturtests)
* Beim Starten von Painter kein Standarddokument erstellen
* &amp;lbrack;Werkzeug&amp;rbrack; Hinzufügen der Möglichkeit zum manuellen Bearbeiten eines Graustufenwerts
* Verschiedene Verbesserungen für die Schablonen (Einrasten, Reset)
* Partikeln sind jetzt Unterwerkzeuge des Malpinsels, des Radiergummis und der Projektion
* &amp;lbrack;3D-Ansicht&amp;rbrack; Baking geführt AO im Viewport-Rendering verwenden
* Teilen der Steuerelemente für Schablonen zwischen der 2D- und 3D-Ansicht
* Kleine Anpassung der Daumengröße in der Bibliothek
* Suchfelder sind für jedes Fenster spezifisch
* Anpassen der Benutzeroberfläche

**Fest:**

* &amp;lbrack;Substance&amp;rbrack; Schalter funktioniert nicht
* &amp;blbrack;Farbdialog&amp;rbrack; Farbtonverlauf nicht aktualisiert
* Mesh kann nicht aktualisiert werden, wenn der Dateiname identisch ist
* Werkzeug ist in zu kleinen Ansichten nicht sichtbar
* Das Aufkleber-Werkzeug auf dem Retina-Display funktioniert nicht richtig
* &amp;lbrack;Substance&amp;rbrack; Int1 werden als float1 angezeigt
* &amp;lbrack;Substance&amp;rbrack; Grundfarbeingabe/-ausgabe werden nicht erkannt
* &amp;lbrack;Substance&amp;rbrack; Filter können nicht neu geladen werden
* &amp;lbrack;Werkzeug&amp;rbrack; Graustufen-Widget ist immer ausgeblendet

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
* &amp;lbrack; und &amp;rbrack; Tastaturbefehle für die Pinselgröße
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
