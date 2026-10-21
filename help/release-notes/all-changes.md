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
* &lbrack;Käfig malen&rbrack; Einfache Käfig-Malen-Benutzeroberfläche erstellen
* &lbrack;Käfig malen&rbrack; Neue Optionen zur Visualisierung von Käfig
* &lbrack;Käfig malen&rbrack; Bearbeitbares Auswahl-/Füllwerkzeug
* &lbrack;Käfig malen&rbrack; Überblendung-Modus in Symbolleiste anzeigen
* &lbrack;Käfig malen&rbrack; HDR. Regler Änderungen an der Benutzeroberfläche
* &lbrack;Käfig malen&rbrack; Visualisierungs-Shader
* &lbrack;Käfig malen&rbrack; Optionen zum Zurücksetzen des Stapels
* Verbesserungen am Werkzeug &quot;Polygonfüllung&quot;
* &blbrack;Polygon Fill&rbrack; Polygon-Ausbesserung hinzufügen
* &blbrack;Polygon Fill&rbrack; Polygonschleife hinzufügen
* &blbrack;Polygon Fill&rbrack; Symmetrie-Unterstützung mit Loop/Patch
* &blbrack;Polygon Fill&rbrack; Symmetrie Edge Preview
* &blbrack;Polygon Fill&rbrack; Dreiecke mit Endlosschleifen und Partialschleifen entfernen
* &blbrack;Polygon Fill&rbrack; Drahtgitter nur für aktiven Textursatz sichtbar
* &Klammer;Polygonfüllung&Klammer; Rote Kantenmarkierung bei nicht klickbaren Dreiecken
* &Klammer;Polygonfüllung&Klammer; Deaktivieren Sie nicht die Füllmodusoptionen
* &blbrack;Polygon Fill&rbrack; Festlegen aller Kanaleigenschaften mit der Polygonfüllung zulassen
* &blbrack;Polygon Fill&rbrack; Vorherigen Strich fortsetzen funktioniert mit Polygonfüllung
* &Klammer;Polygonfüllung&Klammer; Unzulässige Cursorposition auf nicht aktiven Textursätzen anzeigen
* &blbrack;Polygon Fill&rbrack; ALT-Sofortvorschau
* &blbrack;Polygon Fill&rbrack; Tastaturbefehl für temporären Wechsel zu Polyloop (UMSCHALT+A)
* &lbrack;Viewport&rbrack; Markierung für Textursatz-/UV-Kacheln-Auswahl anzeigen
* &lbrack;Viewport&rbrack; Unterstützung für &quot;Order Independent Transparency&quot; im Echtzeit-Viewport hinzufügen
* &lbrack;Anzeigeeinstellungen&rbrack; Anzeigeeinstellungen in neuen Gruppen neu organisieren
* &lbrack;Werkzeug&rbrack; Hinzufügen von Unterstützung für das additive Mischen mit Pinselstrichen
* &lbrack;Werkzeug&rbrack; Unterstützung für additive Überblendung mit der Polygonfüllung hinzufügen
* &lbrack;USD&rbrack; Exportierte USD mit Deckkraftmap werden in Arnold transparent dargestellt
* &lbrack;Nvidia&rbrack; Fügen Sie eine Warnung zu den neuesten Nvidia-Treibern hinzu (616.56 bis 617.14)
* Neue Eingabe für &quot;Mesh_UV_Neighbor&quot;-Engine hinzufügen
* Baker auf Version 3.23.0 aktualisieren
* Substance Engine auf Version 9.6.1 aktualisieren

**Fest:**

* &blbrack;Baking&rbrack; Ambient occlusion &quot;Rückseitige ignorierung nach Mesh&quot; funktioniert nicht
* &blbrack;Baking&rbrack; &lbrack;AMD&rbrack; Gerät beim Baking führ mit hochpolaren Meshs verloren
* &lbrack;Performances&rbrack; Painter VRAM Verwendung
* &lbrack;Viewport&rbrack; Fehlende Texturen beim Öffnen von Projekten auf HDPI-Bildschirmen
* &lbrack;Werkzeug&rbrack; Füllmethode ist ausgegraut, wenn in eine Maske gemalt wird
* Temporäre Ordner werden nach dem Export im Netzwerk nicht gelöscht
* &lbrack;USD&rbrack; Die exportierte USD wird entlang der UV-Begrenzungslinien geteilt
* &lbrack;USD&rbrack; Einfrieren beim Laden von falsch geformtem USDz

### 12.1.5

Freigabedatum: **2026/09/15**

Zusammenfassung: **Nebenversion**

**Fest:**

* Das Exportieren eines Bildes aus einem Regal in ein Netzwerk funktioniert nicht mehr
* &lbrack;Generator&rbrack; Die Einstellung &quot;Textur verwenden&quot; auf &quot;false&quot; deaktiviert nicht die Verwendung der Textur-Eingabe.
* Einfrieren des Viewports beim Speichern während der Bearbeitung der 3D-Projektion
* Material-Ebenenauflösung ist zu niedrig

### 12.1.4

Freigabedatum: **2026/09/04**

Zusammenfassung: **Nebenversion**

**Fest:**

* &lbrack;Absturz&rbrack; Absturz beim Importieren oder Exportieren von Dateien, deren Dateinamen Nicht-ASCII-Zeichen enthalten

### 12.1.3

Freigabedatum: **2026/08/26**

Zusammenfassung: **Nebenversion**

**Hinzugefügt:**

* Substance Engine auf Version 9.4.6 aktualisieren

**Fest:**

* &lbrack;Graustufenwähler&rbrack; Picker bleibt nach dem Ändern des Werkzeugs geöffnet
* &Klammer;Baking&amp;Klammer verzerren; Verzerrungskorrektur bricht beim Malen und Rückgängigmachen
* &blbrack;Projektion-Werkzeug&blbrack; Viewport-Interaktion wird vom Projektion-Werkzeug blockiert
* &lbrack;Dynamischer Strich&rbrack; Fehlende dynamische Konturparameter in den Pinseleigenschaften
* Export in ein Netzwerk funktioniert nicht mehr

### 12.1.2

Freigabedatum: **2026/08/03**

Zusammenfassung: **Nebenversion**

**Fest:**

* &lbrack;Absturz&rbrack; Einige Substance können beim Rendern zu einem Absturz führen
* &lbrack;Absturz&rbrack; Mesh beim Baking erneut importieren
* &lbrack;Absturz&rbrack; Wenn die Grafikanzeige nicht initialisiert wird, kann dies zu einem Absturz führen
* &lbrack;Absturz&rbrack; Beim Exportieren von Texturen kann in einigen Fällen ein Absturz beim Aktualisieren des Protokolls auftreten
* &lbrack;Absturz&rbrack; Absturz im Baking-Modus in einigen Fällen beim Laden/Aktualisieren der Umgebungs-Map
* &blbrack;Baking&rbrack; Das erneute Starten von Baking nach dem Ändern einer Datei mit hohem Poly-Wert kann zum Einfrieren führen
* &lbrack;An Photoshop senden&rbrack; Fehler beim Exportieren der Ebenenmaske
* &lbrack;Engine&rbrack; Das Ergebnis des Ankerpunkts wird nicht zwischen einer Maske und einem Farbkanal gerendert

### 12.1.1

Freigabedatum: **2026/07/09**

Zusammenfassung: Nebenversion

Hinzugefügt:

* &Klammer;Baking&amp;Klammer verzerren; Leg des normalen Neigungsbasismodus: Mesh oder pro Dreieck
* &lbrack;Eigenschaften&rbrack; Einheitliche Farben immer auf den Standardwert ihres Kanals zurücksetzen lassen
* &lbrack;OpenPBR&rbrack; Kanäle zur Erstellung von Ausgabevorlagen im Fenster &quot;Texturen exportieren&quot; nach Kategorien neu gruppieren
* Substance Engine auf Version 9.4.5 aktualisieren

Fest:

* &lbrack;Projekt&rbrack; Das Öffnen und Speichern einiger Projekte kann länger als gewöhnlich dauern
* &lbrack;Absturz&rbrack; Das erneute Laden mehrerer Mesh kann zu einem Absturz führen
* &lbrack;Absturz&rbrack; Das Löschen eines Kanals im Maskenansichtsmodus führt zu einem Absturz
* &lbrack;Absturz&rbrack; Einige Substance können beim Rendern zu einem Absturz führen
* &lbrack;Malen Skew&rbrack; Das ausgewählte Werkzeug in Malen Skew bleibt nach dem Wechsel in den Malmodus ausgewählt
* &lbrack;Baking Allgemeine Einstellungen&rbrack; Käfig-Entfernungseinstellungen aktualisieren die Käfig-Drahtgitter- und Shader-Visualisierung nicht
* &lbrack;Engine&rbrack; UV-Auffüllmodus &quot;3D-Raum-Nachbar&quot; funktioniert nicht gut bei dünnen Dreiecken
* &lbrack;Engine&rbrack; Das Ergebnis des Ankerpunkts wird nicht zwischen einer Maske und einem Farbkanal gerendert

### 12.1.0

Freigabedatum: **2026/06/23**

Zusammenfassung: **Dieses Update ist eine Hauptversion. Es enthält Verbesserungen an Bakern mit dem Standardzustand &quot;Neues Baking&quot;, der Zeichnungs-Skew-Map, dem automatischen Reake, einer neuen Option für den automatischen entpack von UV für Mesh und OpenPBR mit fester Oberfläche. Weitere Informationen finden Sie in den vollständigen Versionshinweisen.**

**Hinzugefügt**:

* &Klammer;Baking&amp;Klammer verzerren; Malwerkzeuge verzerren
* &Klammer;Baking&amp;Klammer verzerren; Skew-Vorschau hinzufügen Shader und Skew-Richtung Vektorgrafiken beim Malen einer Skew-Map
* &Klammer;Baking&amp;Klammer verzerren; Option &quot;Kantenschutz hinzufügen&quot;
* &Klammer;Baking&amp;Klammer verzerren; Auto-Reake
* &Klammer;Baking&amp;Klammer verzerren; Benutzeroberfläche der Mesh-Map-Liste überarbeiten
* &Klammer;Baking&amp;Klammer verzerren; Mesh-Map teilen/Allgemeine Baking-Einstellungen + Allgemeine Einstellungen aus Mesh-Map-Liste verschieben (nur Grundfarbe oder Maske)
* &Klammer;Baking&amp;Klammer verzerren; Symbolleistenschaltflächen für Viewport ändern
* &Klammer;Baking&amp;Klammer verzerren; Symmetrie-Schalter für Pinsel in der oberen Symbolleiste anzeigen
* &Klammer;Baking&amp;Klammer verzerren; Umbenennungsoptionen im Menü &quot;Synchronisierung der Mesh-Map-Liste&quot;
* &Klammer;Baking&amp;Klammer verzerren; Dialogfelder &quot;Synchronisation aktualisieren&quot; und &quot;Überwachter Status&quot;
* &Klammer;Baking&amp;Klammer verzerren; Variante des Graustufen-Farbwählers erstellen
* &Klammer;Baking&amp;Klammer verzerren; Symbol &quot;Baking aktualisieren&quot;
* &lbrack;Automatisch Entpackt&rbrack; Option &quot;Festplatte integrieren&quot;
* &lbrack;OpenPBR&rbrack; Unterstützung für OpenPBR 1.1 hinzufügen
* &lbrack;OpenPBR&rbrack; OpenPBR zum Standard-Arbeitsablauf und -Shader machen
* &lbrack;OpenPBR&rbrack; Importieren von OpenPBR Materials und Texturen über USD
* &lbrack;OpenPBR&rbrack; Exportieren von OpenPBR und Texturen über USD
* &lbrack;OpenPBR&rbrack; Fenster &quot;Texturen exportieren&quot; aktualisieren, um die Namenskonvention für OpenPBR anzuzeigen
* &lbrack;OpenPBR&rbrack; Fügen Sie Dokumentationen zu Änderungen an der Support-OpenPBR hinzu
* &lbrack;OpenPBR&rbrack;&lbrack;Iray&rbrack; Neue MDL zur Unterstützung von OpenPBR 1.1 in Iray hinzufügen
* Mehrere geringfügige Verbesserungen bei USD Exporten
* &lbrack;UI&rbrack; Warnmeldung im Viewport beim Malen auf einem anderen Textursatz hinzufügen
* &lbrack;Reduzieren&rbrack; Reduzieren aller instanzierten Ebenen über Textursatz hinweg zulassen
* &amp;Textursatz&rbrack;Einstellungen&rbrack; Auswahl mehrerer Kanäle gleichzeitig über neues Fenster zulassen
* &lbrack;Verlauf&rbrack; &quot;Wert&quot; aktualisieren Eintragstext rückgängig machen, um den Parameternamen anzugeben
* &lbrack;Ebenenstapel&rbrack; Fülleffekte in Masken auf Weiß (1.0) festlegen
* &lbrack;Substance&rbrack; Neue Eingabe für &quot;Mesh_harte_Kanten_Dreieck&quot;-Engine hinzufügen
* &lbrack;Substance&rbrack; Neue Eingabe für Engine &quot;Mesh_hard_edges&quot; hinzufügen
* &lbrack;Shader&rbrack; Shader-Instanzen zum Freigeben derselben Namen verhindern
* &lbrack;Shader&rbrack; Verwenden des Shaders aus der Projektvorlage beim Importieren einer USD- oder GLTF-Datei
* Adobe Color Engine auf Version 7.0 aktualisieren
* Aktualisieren der MacOSX-Mindestversion auf 13.0 (Ventura)
* &lbrack;Inhalt&rbrack; Neue Projektvorlagen für OpenPBR
* &lbrack;Inhalt&rbrack; Aktualisieren von Beispielprojekten, um den neuen OpenPBR-Shader zu verwenden
* &lbrack;Python&rbrack; Erweitern Sie die Geometrie-Masken-API, um Einschluss- und Ausschlussmodi wie in der Benutzeroberfläche zuzulassen.

**Fest**:

* &lbrack;Absturz&rbrack;&lbrack;Mesh-Map-Einstellungen&rbrack; Einstellungen auf andere Textursatz anwenden
* &lbrack;Absturz&rbrack; Beim Baking von Krümmungen von einer Karte ohne Welt-Raum-Normale
* &lbrack;Absturz&rbrack;&lbrack;Baking&rbrack; Baking mit aktiviertem benutzerdefiniertem Käfig, aber ohne Dateiauswahl-Absturz
* &lbrack;Absturz&rbrack; AO-Baking wird abgebrochen
* &lbrack;Käfig&rbrack; Unendliche Ladung, wenn der hohe Polydateipfad ungültig ist
* &lbrack;Linux&rbrack;&lbrack;Windows&rbrack; Der Farbwähler kann ganz schwarz sein oder nicht angezeigt werden.
* &blbrack;Polygon-Füllwerkzeug&rbrack; Das Tool funktioniert nicht mit Nicht-PBR
* &lbrack;&lbrack;Malen&rbrack; Durch Löschen des Farbkanals werden zuvor gemalte Grundfarben nicht gelöscht.
* &lbrack;USD&rbrack; Shader-Instanzen werden nicht alle korrekt erkannt
* &lbrack;Substance&rbrack; Es wird nur die erste Verwendung eines Eingabe-/Ausgabeknotens berücksichtigt
* &lbrack;Shader&rbrack; Ambient occlusion wird zweimal mit Textursätzen unter Verwendung unterschiedlicher Mischmethoden aufgetragen
* &lbrack;Engine&rbrack; Normale Texturen mit leerem Blaukanal (Schwarz) können zu falschen Füllergebnissen führen.
* &lbrack;GLTF Import&rbrack; Alpha-Überblendung ist auf jedem Textursatz aktiviert
* &lbrack;GLTF Export&rbrack; Alpha-Überblendung ist beim Export immer aktiviert
* &lbrack;Export&rbrack; Doppelseitige Geometrie ist beim Importieren einer GLTF-Datei immer deaktiviert
* &lbrack;Javascript&rbrack; Das Ändern der Shader-Einstellungen trägt nicht zum Rückgängig-Verlauf bei
* &lbrack;Samples&rbrack; Volumenstreuung ist in den Anzeigeeinstellungen für Meet Mat nicht aktiviert

### 12.0.3

Freigabedatum: **2026/05/05**

Zusammenfassung: **Nebenversion**

**Hinzugefügt:**

* Baker auf Version 3.22.2 aktualisieren
* Substance Engine auf Version 9.4.3 aktualisieren
* &lbrack;Python&rbrack; Speichern eines intelligenten Materials an einem bestimmten Speicherort

**Fest:**

* &lbrack;Ubuntu&rbrack; Absturz bei der Auswahl von Material
* &lbrack;Mac&rbrack; Es wird ein Popup angezeigt, in dem Sie um Zugriff auf Daten anderer Anwendungen gebeten werden.
* &blbrack;Baking&rbrack; Artefakte können auf dem Krümmungs-Map erscheinen
* &blbrack;Baking&rbrack; Das Baking ist in manchen Fällen langsamer
* &lbrack;Verkrümmen auf Geometrie&rbrack; In einigen Fällen wird &quot;Auf Geometrie verformen&quot; deaktiviert
* &lbrack;UV-Kachel&rbrack; Der extrahierte Alpha-Wert des Ankerpunkts wird von anderen Kacheln ignoriert
* &lbrack;Python&rbrack;&lbrack;Mac&rbrack; Ausnahmen in der Python-Konsole mit SSL
* &lbrack;Python&rbrack; Painter Absturz beim Beenden mit verbleibenden Qt-Widgets

### 12.0.2

Freigabedatum: **2026/04/07**

Zusammenfassung: **Nebenversion**

**Hinzugefügt:**

* &lbrack;Farbmanagement&rbrack; Fügen Sie neue OCIO hinzu, um den Standardfarbraum des Farbwählers anzugeben
* &lbrack;Python&rbrack; Leg der Einstellungen für den automatischen entpack in der Python-API

**Fest:**

* &lbrack;Absturz&rbrack; Das Speichern bei zu wenig Speicherplatz kann zu einem Absturz oder einer Beschädigung der Projekte führen.
* &lbrack;Absturz&rbrack; &lbrack;Menüband&rbrack; Die Verwendung des Menübands kann bei einigen Projekten zu Abstürzen führen
* &lbrack;Absturz&rbrack; &blbrack;Baking&rbrack; Absturz, wenn die .assbin-Datei nicht in den Ordner geschrieben werden kann
* &lbrack;Import&rbrack; OBJ Meshs aus Stager können bei der Projekterstellung fehlschlagen
* &lbrack;Import&rbrack; OBJ fehlt in einigen Fällen die Fläche
* &lbrack;Import&rbrack; USD Mesh ohne zugewiesenes Material kann beim Importieren Absturz hinzufügen.
* &lbrack;Ausgefüllter Pfad&rbrack; Nicht von der Symmetrie betroffen
* &lbrack;Schablone&rbrack; Die Vorschau hat eine geringere Auflösung als das gemalte Ergebnis
* &lbrack;UI&rbrack; &quot;uv island&quot; wird in der QuickInfo für ID-Map-Farbquellen noch erwähnt
* &lbrack;Anzeige&rbrack; Schatten erscheinen invertiert
* &lbrack;Viewport&rbrack; Transformieren Projektion der Verkrümmung bleibt nach dem Wechsel in den Baking-Modus erhalten
* &lbrack;Verkrümmen&rbrack; Raster verschwindet, wenn die Skalierung auf der Z-Achse auf 0 eingestellt ist und &quot;Auf Geometrie verformen&quot; aktiviert ist
* &lbrack;Python&rbrack; Unerwarteter Fehler beim Hinzufügen eines Kanals mit bereichsbezogener Änderung

### 12.0.1

Freigabedatum: **2026/03/18**

Zusammenfassung: **Nebenversion**

**Fest:**

* &lbrack;Absturz&rbrack;&lbrack;Freeze&rbrack; Exportieren aus bestimmten Projekten

### 12.0.0

Freigabedatum: **2026/03/09** Zusammenfassung: **Dies ist eine Hauptversion. Diese Version enthält die Funktionen zum Reduzieren von Ebenen, Verformen der Geometrie, neue Post-Effekte, Verbesserung des neuen Projektfensters und weitere Verbesserungen.**

**Hinzugefügt**:

* &lbrack;Ebenen reduzieren&rbrack; Ebenen innerhalb des Ebenenstapels reduzieren
* &lbrack;Ebenen reduzieren&rbrack; Exportieren reduzierter Ebenen auf die Festplatte
* &lbrack;Verkrümmen auf Geometrie&rbrack; Neue Funktion für die automatische Verkrümmung in Verkrümmen-Projektionen hinzufügen
* &lbrack;Post-effects&rbrack; Post-Effekte durch neue ersetzen
* &lbrack;Post-effects&rbrack; Tonzuordnung aktualisieren
* &lbrack;Post-effects&rbrack; Neue Verwendung für Post-Effects-Elemente hinzufügen
* &lbrack;Content&rbrack;&lbrack;Post-effects&rbrack; Standard-Post-Effects-Elemente in die Bibliothek integrieren
* &lbrack;Neues Projekt&rbrack; Verbessern der Benutzeroberfläche für die Projekterstellung
* &lbrack;Neues Projekt&rbrack; Änderungen an der Funktion zum erneuten Importieren von Mesh
* &lbrack;Neues Projekt&rbrack; Öffnen von \*.geo.usd-Dateien zulassen
* &lbrack;Projektkonfiguration&rbrack; Verbessern der Benutzeroberfläche für die Projektkonfiguration
* USD auf Version 25.05 aktualisieren
* Substance Engine auf Version 9.3.4 aktualisieren
* Erhöhen der Mindesttreiber auf 25.3.1/25.Q2 für AMD-GPUs
* Update Qt auf 6.8.6
* &lbrack;Skripterstellung&rbrack; JavaScript-API auf Version 1.1.20 aktualisieren
* Aktualisieren von Python auf 3.13

**Fest:**

* &lbrack;Absturz&rbrack; Ändern der Ausgabe eines Material-Kanals in einer Maske kann Absturz verursachen
* &lbrack;Import&rbrack; EXR Texturen werden beim Importieren von USD in sRGB anstelle von linear erzwungen
* &blbrack;UV-Kacheln&rbrack; Bildsequenz mit einem einzigen Bild füllt auch andere UV-Kacheln
* &blbrack;Baking&rbrack; AO unterscheidet sich zwischen CPU- und GPU-Baking
* &lbrack;Farbmanagement&rbrack;&lbrack;MacOS&rbrack; Viewport &quot;BaseColor&quot; stimmt nicht mit dem Farbwähler überein
* &lbrack;USD&rbrack; Einheitliche Werte werden in einigen Fällen nicht importiert

## Version 11

### 11.1.3

Freigabedatum: **2026/02/12** Zusammenfassung: **Nebenversion**

**Fest**:

* &lbrack;Malen&rbrack; Schablone und Symmetrie funktionieren in einigen Fällen nicht
* &lbrack;Pfad&rbrack; Keine Aktualisierung beim Ändern des Deckkraftreglers für den Verwischungsstrich
* &lbrack;Projekt&rbrack; Malen auf einer bestimmten Geometrie nicht möglich
* &lbrack;Menüband&rbrack; Der instanziieren Pfad verschwindet, wenn die Auflösung des Textursatzes geändert wird
* &lbrack;UI&rbrack; Der Farbwähler kann sich verkleinern und in einigen Fällen verschwinden

### 11.1.2

Freigabedatum: **2026/01/13** Zusammenfassung: **Nebenversion**

**Hinzugefügt**:

* &blbrack;Baking&rbrack; Verbessern des Bakings von UV-Kacheln-Projekten durch asynchrones Speichern
* &lbrack;Shaders&rbrack; Erwähnung in Shader-API Changelog Veränderungen nach Vulkan Migration
* Update OpenEXR auf Version 3.4.4

**Fest**:

* &lbrack;Absturz&rbrack; Absturz beim Starten von Nvidia GTX 10xx
* &lbrack;Absturz&rbrack; Die Verwendung des Farbwählers auf verschiedenen Textursätzen kann beim Beenden der Anwendung zu einem Absturz führen
* &lbrack;Performance&rbrack; Leistungsproblem beim Malen im Projekt mit vielen Ebenen
* &lbrack;Performance&rbrack; Verzögerung beim Malen mit Grafiktablett-Stift
* &lbrack;UI&rbrack; Kamera-Einstellungen bleiben im Rendermodus deaktiviert (Iray)
* &lbrack;Menüband&rbrack; Pfad kann sich in einigen Fällen nach einer Ecke unerwartet überlappen
* &lbrack;Menüband&rbrack; Leistungsproblem mit UV-Kacheln
* &lbrack;Substance&rbrack;&lbrack;UI&rbrack; Bildeingaben verschwinden, wenn sie ausgeblendet werden
* &lbrack;Substance&rbrack;&lbrack;UI&rbrack; Verschachtelte Gruppen können auch dann beibehalten werden, wenn sie unter Sichtbar, wenn sie ausgeblendet sind.
* &lbrack;Baking&rbrack;&lbrack;UI&rbrack; Der Krümmung-Sampling-Radius kann nicht über 0,01 hinaus festgelegt werden
* &lbrack;Baking&rbrack;&lbrack;UI&rbrack; Max. Verdeckungsabstand kann nicht auf mehr als 1 eingestellt werden
* &blbrack;Baking&rbrack; AO-Einstellung &quot;Selbstverdeckung&quot; wird bei mehreren Textursätzen ignoriert und &quot;Niedrig&quot; steht für &quot;Hoch&quot; Baking geführt
* &blbrack;Baking&rbrack; ID-Map Baking führe keine Textfarben aus FBX im Scheitelpunkt &quot;Niedrig bis Hoch&quot;
* &lbrack;Inhalt&rbrack; Hochpassfilter führt zu ausgewaschenen Farben in farbverwalteten Kanälen

### 11.1.1

Freigabedatum: **2025/12/09** Zusammenfassung: **Nebenversion**

**Hinzugefügt**:

* &lbrack;Performance&rbrack; Verbessern der UV-Kacheln-Performance bei der Berechnung partieller Texturen
* &lbrack;Baker&rbrack; Update auf Version 3.15.4

**Fest**:

* &lbrack;Absturz&rbrack;&lbrack;MacOS&rbrack; Speichern eines Projekts aus einer früheren Version immer mit dem Absturz
* &lbrack;Absturz&rbrack; Das Schließen eines Projekts kann zu einem Absturz führen
* &lbrack;Projekt&rbrack; Fehler &quot;Die Mitgliederanzahl stimmt nicht überein&quot; beim Öffnen des Projekts, das in der vorherigen Version erstellt wurde
* &blbrack;Baking&rbrack; UV-Kacheln werden nicht mit vorherigen Baking-Ergebnissen kombiniert, sofern vorhanden.
* &blbrack;Baking&rbrack; Gerät verloren, selbst wenn Raytracing in der Nvidia GTX 10XX-Serie deaktiviert ist
* &blbrack;Baking&rbrack; AO mit Normal weist an Kanten Artefakte auf, da keine Auffüllung erfolgt.
* &blbrack;Baking&rbrack; AO-Einstellung &quot;Selbstverdeckung&quot; wird bei mehreren Textursätzen ignoriert und &quot;Namensübereinstimmung&quot; aktiviert.
* &blbrack;Baking&rbrack; ID-Map ist vollständig schwarz, wenn Scheitelpunkt-Farben bei Meshs mit hohem Poly fehlen
* &lbrack;Menüband&rbrack; QuickInfo für den Modus &quot;Alpha-Überblendung&quot; nennt den Bildschirmüberblendmodus anstelle von &quot;Linear abwedeln&quot;
* &lbrack;Pfad&rbrack; Tangenten erstellen eine unerwartete Schleife, wenn der Punkt dicht an das Pfadende verschoben wird
* &lbrack;Werkzeug&rbrack; Die Maskenvorschau funktioniert nicht, wenn die Projektion in einer Material verwendet wird
* &lbrack;Engine&rbrack; Das Malen kleiner Striche kann zu blockartigen Artefakten führen
* &lbrack;Shader&rbrack; Durch Rückgängigmachen der Erstellung von Shader-Instanzen wird sie nicht ordnungsgemäß entfernt.
* &lbrack;Export&rbrack; Alpha-Modus für GLTF-Export ist immer auf MASK festgelegt
* &lbrack;Python&rbrack; Unerwarteter Fehler beim Bearbeiten von Ebenenstapel außerhalb des umfangreichen Änderungsblocks

**Bekannte Probleme**:

* &lbrack;Menüband&rbrack; Leistungsproblem mit UV-Kacheln
* &lbrack;Menüband&rbrack; Pfad kann sich in einigen Fällen nach einer Ecke unerwartet überlappen
* &lbrack;Absturz&rbrack;&lbrack;Ribbon&rbrack; Erstellen von sehr langen Texten im Menüband kann Absturz
* &lbrack;Farbmanagement&rbrack; HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen geklemmte Farben
* &lbrack;Regression&rbrack;&lbrack;UI&rbrack; Kontextmenü ist auf HD-Bildschirmen zu klein
* &lbrack;Absturz&rbrack;&lbrack;Python&rbrack; USD Export ausgelöst durch TextureStateEvent
* &lbrack;Engine&rbrack; Malen mit dem Klon-Werkzeug in normalen Kanalverschiebungsfarben falsch
* &lbrack;Python&rbrack; Phantom-Widget wird angezeigt, weil das Skript noch funktioniert

### 11.1.0

Veröffentlichungsdatum: **2025/11/18** Zusammenfassung: **Dieses Update ist eine Hauptversion, es enthält das neue Multifunktionsleisten-Tool mit eigenem neuen Inhalt, Unterstützung von Füllebenen, Leistungsparameter für Versatz, verbesserte Physische Größe durch die aktualisierten Baker, vollständige Vulkan-Unterstützung für Windows und Linux und weitere Symmetrien.**

**Hinzugefügt**:

* Neues Bandwerkzeug
* &lbrack;Werkzeug&rbrack; Neues Werkzeug &quot;Menüband&quot; für nahtlose Pfade hinzufügen
* &lbrack;Menüband&rbrack; Tastenkombinationen für die Bandvorgabe im Eigenschaftenfenster hinzufügen
* &lbrack;Menüband&rbrack; Zulassen, dass die Deckkraft des Menübands pro Scheitelpunkt auf dem Pfad geändert wird
* &lbrack;Menüband&rbrack; Ändern der Größe des Menübands pro Scheitelpunkt auf dem Pfad zulassen
* &lbrack;Menüband&rbrack; In einer Substance definierte Anfang-/Endpunkte entfernen, wenn Pfade geschlossen sind
* &lbrack;Menüband&rbrack; Entfernen der Pfad-/Material-Vorschau im Eigenschaftenfenster für Malen-/Radiergummi-/Verwisch-Pfadwerkzeuge
* &lbrack;Menüband&rbrack; Fülloptionen für Alpha und einige Kanäle bei Selbstüberlappung hinzufügen
* Symmetrie füllen
* &lbrack;Füllen&rbrack; Unterstützung für Symmetrie zu Füllebenen und Effekten hinzufügen
* &lbrack;Fill&rbrack;&lbrack;UI&rbrack; Einstellungen für die Symmetrie von Füllebene und Effekten im Eigenschaftenfenster gelegt
* &lbrack;Füllen&rbrack; Benutzeroberfläche für Symmetrie-Einstellungen im Viewport- und Eigenschaftenfenster überarbeiten
* &lbrack;Füllen&rbrack; Normale Texturen bei Projektion im Verkrümmungsmodus korrekt neu ausrichten
* Physische Größe Versatz
* &lbrack;Versatz&rbrack; Physische Größe als Versatz verwenden
* Leistungssteigerung
* &lbrack;Performance&rbrack; Verbessern der Darstellung kleiner Pinselstriche auf großen Dreiecken
* &lbrack;Performance&rbrack; Verbessern der Shader-Kompilierungszeit
* &lbrack;Performance&rbrack; Vollständige Vulkan-Unterstützung für Windows und Linux
* &lbrack;Performance&rbrack; Aktualisierte Baker mit schnellerem GPU-Rendering und Unterstützung von AMD-Raytracing
* &lbrack;UI&rbrack; Werkzeugeigenschaften neu in Gruppen organisieren und einige standardmäßig reduzieren
* &lbrack;Engine&rbrack; Substance Engine auf Version 9.2.5 aktualisieren
* &lbrack;Substance&rbrack; Irreguläre Auflösung für Substance-Ressourcen in &quot;Extras und Füllungen&quot; gelegt
* &lbrack;Export&rbrack; Exportvoreinstellung für Mesh-Map aktualisieren, um Graustufen-Texturen zu exportieren
* Python
* &lbrack;Baking&rbrack;&lbrack;Python&rbrack; Anzeige der Änderungen im Änderungsprotokoll nach Aktualisierung der Baker
* &lbrack;Python&rbrack; Leg der Einstellungen für die Symmetrie der Füllung in Python
* Content und neue Inhalte.
* &lbrack;Inhalt&rbrack; 75 neue Werkzeugvorgaben für das Menüband-Werkzeug hinzufügen
* &lbrack;Inhalt&rbrack; Verlaufsgenerator-Ressource so aktualisieren, dass sie mit dem Menüband kompatibel ist

**Fest**:

* &lbrack;Absturz&rbrack; Laden eines anderen Projekts bei aktiviertem einrasten des Pfads kann Absturz
* &lbrack;Absturz&rbrack; Rechtsklick im Bedienfeld &quot;Pfad&quot; mit Informationen aus einer anderen Session in der Zwischenablage kann Absturz enthalten
* &lbrack;UI&rbrack; Oberfläche scrollt in den Werkzeugeigenschaften nach oben, wenn ein Pfad erstellt wird
* &lbrack;UI&rbrack; Mauszeiger verschwindet, wenn die Pfadzeigerdarstellung ausgeblendet ist
* &lbrack;Pfad&rbrack; Kopieren/Einfügen verschiedener Werkzeugeigenschaften im Bedienfeld &quot;Pfad&quot; führt zu instabilen Eigenschaften
* &lbrack;Werkzeug&rbrack; Radiergummi- und Verwischen-Werkzeugvorgaben aktualisieren nicht immer die Kanalauswahl
* &lbrack;Werkzeug&rbrack; Gemalter Wert ist grau, aber Benutzeroberfläche zeigt Weiß an, nachdem farbige Werkzeugvorgabe in die Maske geladen wurde
* &lbrack;Werkzeug&rbrack; Die aus der Maske erstellte Vorgabe behält Kanalwerte bei, die aus einer anderen Vorgabe geladen wurden.
* &lbrack;Substance&rbrack; Die in Graf definierte normale Farbraumübersteuerung wird nicht berücksichtigt
* &lbrack;Inhalt&rbrack; Die Standard-Pinselform-Ressource verwendet eine veraltete Substance

**Bekannte Probleme**:

* Shader-Instanz-Verlauf wird nicht richtig verfolgt
* &lbrack;Menüband&rbrack; Leistungsproblem mit UV-Kacheln
* &lbrack;Menüband&rbrack; Pfad kann sich in einigen Fällen nach einer Ecke unerwartet überlappen
* &lbrack;Menüband&rbrack; Tangenten erzeugen eine unerwünschte Schleife, wenn der Punkt nahe an das Pfadende verschoben wird
* &lbrack;Absturz&rbrack;&lbrack;Ribbon&rbrack; Erstellen von sehr langen Texten im Menüband kann Absturz
* &lbrack;Werkzeug&rbrack; Die Maskenvorschau funktioniert nicht, wenn die Projektion in einer Material verwendet wird
* &blbrack;Baking&rbrack; AO-Einstellung &quot;Selbstverdeckung&quot; wird bei mehreren Textursätzen ignoriert und &quot;Namensübereinstimmung&quot; ist aktiviert
* &blbrack;Baking&rbrack; AO mit Normal weist an den Kanten Artefakte auf, da die Auffüllung fehlt.
* &lbrack;Farbmanagement&rbrack; HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen geklemmte Farben
* &lbrack;Regression&rbrack;&lbrack;UI&rbrack; Kontextmenü ist auf HD-Bildschirmen zu klein
* &lbrack;Absturz&rbrack;&lbrack;Python&rbrack; USD Export ausgelöst durch TextureStateEvent
* &lbrack;Engine&rbrack; Malen mit dem Klon-Werkzeug in normalen Kanalverschiebungsfarben falsch
* &lbrack;Python&rbrack; Phantom-Widget wird angezeigt, weil das Skript noch funktioniert

### 11.0.3

Freigabedatum: **2025/08/05** Zusammenfassung: **Nebenversion**

**Hinzugefügt**:

* &lbrack;Substance 3D Assets&rbrack; Hinzufügen eines Benachrichtigungspunkts zum Bedienfeld &quot;3D-Elemente&quot;
* &lbrack;VFX Platform 2025&rbrack; Hinzufügen der ACE 2.0-Konfiguration in den Farbmanagementeinstellungen
* &lbrack;VFX Platform 2025&rbrack; Aktualisieren Sie OCIO auf Version 2.4.2
* Iray auf Version 2024.10 aktualisieren
* &lbrack;Engine&rbrack; Update auf Substance Engine v.9.2.3
* &lbrack;Nvidia&rbrack; Erhöhen der Nvidia-Mindesttreiberversion auf 572.60 (Win) und 570.169 (Linux)

**Fest**:

* &lbrack;Python&rbrack; Die Änderung des Gültigkeitsbereichs wird nicht im Verlaufsfenster angezeigt

**Bekannte Probleme**:

* &lbrack;Farbmanagement&rbrack; HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen geklemmte Farben
* &lbrack;Regression&rbrack;&lbrack;UI&rbrack; Kontextmenü ist auf HD-Bildschirmen zu klein
* &lbrack;Absturz&rbrack;&lbrack;Python&rbrack; USD Export ausgelöst durch TextureStateEvent
* &lbrack;Engine&rbrack; Malen mit dem Klon-Werkzeug in normalen Kanalverschiebungsfarben falsch
* &lbrack;Python&rbrack; Phantom-Widget wird angezeigt, weil das Skript noch funktioniert

### 11.0.2

Freigabedatum: **2025/06/10** Zusammenfassung: **Nebenversion**

**Hinzugefügt**:

* &lbrack;Mac&rbrack; Warnmeldungen zu bestimmten Betriebssystemversionen hinzufügen, die zu Artefakten führen
* &lbrack;Automatische Aktualisierung&rbrack; Kleine UX-Verbesserungen im Fehlerprotokoll &quot;Assets&quot;
* &lbrack;Automatisches Entpacken&rbrack; Update auf Version 1.3.2 mit Seaming-Verbesserungen
* &lbrack;USD&rbrack;&lbrack;FBX&rbrack; Unterstützung für mehrere UV-Satz mit wenigen Daten hinzufügen
* &lbrack;Export&rbrack; Meshs, die als FBX exportiert wurden, fehlen ihre zusätzlichen UV-Satz, wenn beim Import vorhanden waren

**Fest**:

* &lbrack;MacOS&rbrack;&lbrack;Linux&rbrack; Absturz beim Speichern auf dem Netzlaufwerk
* &lbrack;Win&rbrack;&lbrack;Tablet&rbrack; Flackern beim Schwenken
* &lbrack;SpaceMouse&rbrack; Problem beim Arbeiten mit dem Pfadwerkzeug
* &lbrack;Käfig&rbrack; Nach einem erneuten Laden des Meshs kann kein Baking ausgeführt werden
* &lbrack;Automatische Aktualisierung&rbrack; Bildsequenz wird nicht neu geladen, wenn die erste Kachel fehlt
* &lbrack;Pfad&rbrack; Benutzerdefinierte Tangente kann sich auf andere Tangenten auswirken
* &lbrack;Pfad&rbrack; Pfad wird auf dem Textursatz nicht angezeigt, wenn sich der erste Punkt auf einem anderen Textursatz befindet
* &lbrack;UI&rbrack; Einige Menüs sind nach dem Öffnen eines Projekts immer deaktiviert (z. B.: Symmetrie)
* &lbrack;Eigenschaften&rbrack; Werkzeugvorgaben mit ausgefülltem Pfadwerkzeug können nicht verwendet/geladen werden
* &lbrack;USD&rbrack; Mehrere UV-Satz werden bei Verwendung von USD nicht im benutzerdefinierten Shader erkannt.
* &lbrack;USD&rbrack; Kameras mit dem gleichen Namen werden überschrieben
* &lbrack;Export&rbrack; &quot;An Photoshop senden&quot; führt zu einem falschen Farbraum für Farb- und Graustufenergebnisse
* &lbrack;Export&rbrack; Graustufen-Kanäle mit Alpha werden als Farbe anstatt als Graustufen mit PNG-Format exportiert
* &lbrack;Export&rbrack; Exportieren des Graustufenkanals als PSD führt zu einer ungültigen/abgeschnittenen Datei
* &lbrack;Inhalt&rbrack; Der Verkrümmungsfilter im Mehrrichtungsmodus funktioniert nicht
* &lbrack;Python&rbrack; Listenfehler beim Crawlen von Ebenenstapel-Knoten kann nicht zugewiesen werden

**Bekannte Probleme**:

* &lbrack;Farbmanagement&rbrack; HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen geklemmte Farben
* &lbrack;Regression&rbrack;&lbrack;UI&rbrack; Kontextmenü ist auf HD-Bildschirmen zu klein
* &lbrack;Absturz&rbrack;&lbrack;Python&rbrack; USD Export ausgelöst durch TextureStateEvent
* &lbrack;Engine&rbrack; Malen mit dem Klon-Werkzeug in normalen Kanalverschiebungsfarben falsch
* &lbrack;Python&rbrack; Phantom-Widget wird angezeigt, weil das Skript noch funktioniert

### 11.0.1

Freigabedatum: **2025/04/10** Zusammenfassung: **Nebenversion**

Hinweis: **Die Linux CCD-Version wird auf den 29. April verschoben.**

**Hinzugefügt:**

* Update auf Qt 6.5.8
* &lbrack;Substance&rbrack; Fügen Sie eine Protokollmeldung für Filter hinzu, wenn mehrere Bildeingaben dieselbe Verwendung haben
* &lbrack;Nvidia&rbrack; Fügen Sie eine Warnung zu den neuesten Nvidia-Treibern hinzu (572.47)

**Fest:**

* &lbrack;Absturz&rbrack; Wenn Sie einen Balken mit einer Verwendung in einem Ein Kanal-Steckplatz ziehen und ablegen
* &lbrack;Absturz&rbrack;&lbrack;Pfad&rbrack; Die Option &quot;Pfadtyp ändern&quot; ist nicht ausgegraut, wenn nicht auf einen bestimmten Pfad geklickt wird
* &lbrack;Pfad füllen&rbrack; Sollte nicht in der Lage sein, Substance-Material auszuwählen
* &lbrack;Engine&rbrack; Artefakte an Pinselstrichen
* &lbrack;Engine&rbrack; Pfade können mit bestimmten Einstellungen unterbrochen werden.
* Problem mit der Dropdown-Liste für den Pipetten-Farbraum
* &lbrack;Automatische Aktualisierung&rbrack; &lbrack;Python&rbrack; Falsche Fehlermeldung bei Verwendung von ResourceID ohne Version
* &lbrack;Shader&rbrack; Absturz beim Öffnen einiger Projekte

**Bekannte Probleme:**

* &lbrack;SpaceMouse&rbrack; Problem beim Arbeiten mit dem Pfadwerkzeug
* &lbrack;Farbmanagement&rbrack; HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen geklemmte Farben
* &lbrack;Regression&rbrack;&lbrack;UI&rbrack; Kontextmenü ist auf HD-Bildschirmen zu klein
* &lbrack;Absturz&rbrack;&lbrack;Python&rbrack; USD Export ausgelöst durch TextureStateEvent
* &lbrack;Engine&rbrack; Malen mit dem Klon-Werkzeug in normalen Kanalverschiebungsfarben falsch
* &lbrack;Python&rbrack; Phantom-Widget wird angezeigt, weil das Skript noch funktioniert

### 11.0.0

Freigabedatum: **2025/03/11** Zusammenfassung: **Hauptversion, neue Funktion zur automatischen Aktualisierung, ausgefülltes Pfadwerkzeug und andere Pfadverbesserungen sowie neue Filter und eine experimentelle Generierung von automatischen Käfigen für das Baking**

**Hinzugefügt**:

* Automatische Aktualisierung
* &lbrack;Automatische Aktualisierung&rbrack; Geänderte Elemente im Bedienfeld &quot;Elemente&quot; automatisch aktualisieren
* &lbrack;Automatische Aktualisierung&rbrack; Geänderte Elemente im gesamten Projekt automatisch aktualisieren
* &lbrack;Automatische Aktualisierung&rbrack; Automatische Aktualisierung standardmäßig deaktiviert lassen
* &lbrack;Automatische Aktualisierung&rbrack; Optionale Aktualisierung, wenn die Ressourcenparameter nicht übereinstimmen (.sbsar, .glsl, .ai, .svg)
* &lbrack;Automatische Aktualisierung&rbrack; Umgebungsvariable zum Deaktivieren der automatischen Aktualisierung hinzufügen
* &lbrack;Auto-update&rbrack;&lbrack;SBSAR&rbrack; Update optional machen, wenn die Ressourcenparameter nicht übereinstimmen
* Ausgefüllter Pfad
* &lbrack;Pfad&rbrack;&lbrack;Füllen&rbrack; Neues Werkzeug zum Erstellen ausgefüllter Pfade hinzufügen
* Verbesserungen an Pfaden
* &lbrack;Pfad&rbrack; Erstellen eines zu Polygonen einrasten Pfads
* &lbrack;Pfad&rbrack; Wechseln von Pfadtypen zulassen
* &lbrack;Pfad&rbrack; Kopieren und Einfügen von Pfadmaskendaten zwischen Scheitelpunkt und Maske zulassen
* &lbrack;Pfad&rbrack; Winkel beim Erstellen eines neuen Punkts einschränken
* &lbrack;Pfad&rbrack; Zuzulassen, dass die Punkterstellung auf eine Linie beschränkt wird
* &lbrack;Pfad&rbrack; Form mit einem Klick schließen
* &lbrack;Pfad&rbrack; Anzeigen von Pfadinformationen
* &lbrack;Pfad&rbrack; Skalieren und Drehen von Pfad-Scheitelpunkten zulassen
* &lbrack;Path&rbrack;&lbrack;UX&rbrack; Gizmos für Transformation leichter zugänglich machen
* &lbrack;Pfad&rbrack; Pfadvorschau hinzufügen
* &lbrack;Pfad&rbrack; Pfadvorschau mit Umschalt + P deaktivieren
* &lbrack;Pfad&rbrack; Verbessern der Tangente Edition in der Seitenansicht
* &lbrack;Pfad&rbrack; Fokus auf einen 3D-Pfad festlegen.
* &lbrack;Pfad&rbrack; Scheitelpunkt sollten den Auswahlstatus beibehalten, wenn sie die Benutzeroberfläche aus- und wieder einschalten
* &lbrack;Pfad&rbrack; Löschen von Pfaden mit Rücktaste zulassen
* &lbrack;Pfad&rbrack; Pfadliste offen halten, wenn der Benutzer sie erweitert
* &lbrack;Pfad&rbrack;&lbrack;Ebenenstapel&rbrack; Duplikate beim Kopieren/Einfügen richtig umbenennen
* &lbrack;Pfad&rbrack; Verbesserungen an Benutzeroberfläche und QuickInfo
* Leistung
* &lbrack;Performance&rbrack; Verbessern der Viewport-Performance bei Verwendung einer hohen Tessellation
* &lbrack;Performance&rbrack; Nur den ersten Kanal für neue Füllebenen/Effekte aktivieren
* &lbrack;Performance&rbrack; Berechnung des Pinselstrichs parallelisieren
* Baking
* &blbrack;Baking&rbrack; Neue vollautomatische Option zur Generierung von Käfigen für das Baking führ mit Meshs mit hohem Poly (experimentell)
* Inhalte
* &lbrack;Inhalt&rbrack; Fügen Sie sechs neue Filter hinzu: stilisierung, quantisieren, anisotropic kuwahara, weiche Abschrägung, Richtungsabstand, Graustufen konvertierung
* &lbrack;Inhalt&rbrack; Aktualisieren von Rauschen und Grunges auf die neueste Version von Designer (mit der neuen 2D-Voronoi)
* &lbrack;Inhalt&rbrack; 3 neue Textur-Generatoren hinzufügen (Kachel-Zufallsgenerator, Triangle Grid, Scratches-Generator)
* &lbrack;Inhalt&rbrack; Vorlage für &quot;Unreales Engine umbenennen&quot; und Exportvorgaben
* Python
* &lbrack;Regal&rbrack;&lbrack;Python&rbrack; Intelligente Material oder intelligente Maske aus Python auf Festplatte speichern
* &lbrack;Python&rbrack; Hinzufügen von automatischem Baking-Käfig zur Python-API
* &lbrack;Python&rbrack; Bearbeiten von Namen und Beschreibungen von Textursätzen/UV-Kacheln zulassen
* &lbrack;Python&rbrack; Auflösungseinstellungen für Vektor- und Schriftquellen freigeben
* &lbrack;Automatische Aktualisierung&rbrack;&lbrack;Python&rbrack; Automatische Aktualisierung von Projekten in Python gelegt
* Verschiedenes
* &lbrack;Export&rbrack; Erleichtern Sie den Zugriff auf die Optionen für &quot;Senden an&quot; mit einem neuen Bedienfeld
* &lbrack;Nvidia&rbrack; Fügen Sie eine Warnung zu den neuesten Nvidia-Treibern hinzu (572.16)
* Die einrasten Winkel sollten durch die Auswahl von Objekt/Welt-Raum beeinflusst werden.
* &lbrack;Textursatz list&rbrack; UV-Kacheln benutzerdefinierten Namen hinzufügen und beim Exportieren verwenden
* Mac
* &lbrack;Mac&rbrack; Verwenden von Metal anstelle von OpenGL für das Grafik-Rendering
* &lbrack;Mac&rbrack; Drop Mac Intel-Support

**Fest**:

* &lbrack;Absturz&rbrack; Löschen der Bildeingabe
* Smart-Matte kann nicht über Ebenenstapel-Taste hinzugefügt werden
* &lbrack;Python&rbrack; Effekte für GroupLayerNode können nicht gefunden werden

**Bekannte Probleme**:

* &lbrack;Farbmanagement&rbrack; HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen geklemmte Farben
* &lbrack;Regression&rbrack;&lbrack;UI&rbrack; Kontextmenü ist auf HD-Bildschirmen zu klein
* &lbrack;Absturz&rbrack;&lbrack;Python&rbrack; USD Export ausgelöst durch TextureStateEvent
* &lbrack;MacOS Intel&rbrack; Absturz beim Importieren einiger Vorgaben
* &lbrack;Engine&rbrack; Malen mit dem Klon-Werkzeug in normalen Kanalverschiebungsfarben falsch
* &lbrack;Python&rbrack; Phantom-Widget wird angezeigt, weil das Skript noch funktioniert
* &lbrack;RedHat&rbrack; Probleme mit dem Farbwähler

## Version 10

### 10.1.2

Veröffentlichungsdatum: **2024/12/3** Zusammenfassung: **Nebenversion, Fehlerbehebungen**

**Fest**:

* &lbrack;Absturz&rbrack; Löschen der Bildeingabe
* Smart-Matte kann nicht über Ebenenstapel-Taste hinzugefügt werden
* &lbrack;Python&rbrack; Effekte für GroupLayerNode können nicht gefunden werden

**Bekannte Probleme**:

* &lbrack;Farbmanagement&rbrack; HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen geklemmte Farben
* &lbrack;Regression&rbrack;&lbrack;UI&rbrack; Kontextmenü ist auf HD-Bildschirmen zu klein
* &lbrack;Absturz&rbrack;&lbrack;Python&rbrack; USD Export ausgelöst durch TextureStateEvent
* &lbrack;MacOS Intel&rbrack; Absturz beim Importieren einiger Vorgaben
* &lbrack;Engine&rbrack; Malen mit dem Klon-Werkzeug in normalen Kanalverschiebungsfarben falsch
* &lbrack;Python&rbrack; Phantom-Widget wird angezeigt, weil das Skript noch funktioniert
* &lbrack;RedHat&rbrack; Probleme mit dem Farbwähler

### 10.1.1

Veröffentlichungsdatum: **2024/11/5** Zusammenfassung: **Nebenversion, Fehlerbehebungen**

**Hinzugefügt**:

* &lbrack;Projekt&rbrack; Aktuelles Projekt geöffnet lassen, bis die Auswahl eines neuen Projekts überprüft wurde
* &lbrack;Automatisches Entpacken&rbrack; Texeldichte ermöglicht eine bessere Aufteilung von UV-Inseln in UDIM
* &blbrack;Baking&rbrack; Mehrdeutige Kopie im Kontextmenü von Mesh-Map reparieren
* &lbrack;Verkrümmen&rbrack; Entfernen der Skalierung im Viewport für die Z-Achse (Tiefe)
* &lbrack;Import/Export&rbrack; Unterstützung nicht verwendeter Bilddateiformate entfernen
* Update Substance Engine auf 9.1.4

**Fest**:

* &lbrack;Absturz&rbrack; Nachdem Sie Ressourcen in &quot;Elemente&quot; verlagert und das Projekt gespeichert haben
* &lbrack;Absturz&rbrack; Probleme mit der Aiserver-Bibliothek
* &lbrack;Absturz&rbrack; Illustrator Server-Absturz in einigen seltenen Fällen
* &lbrack;Absturz&rbrack; Beim Beenden der Anwendung in seltenen Fällen
* Absturz-Berichte können auf einigen Computern nicht gesendet werden
* &blbrack;Baking&rbrack; Die Farbe des Scheitelpunkts ist nicht richtig gelesen
* &lbrack;UI&rbrack; Position von Fenstern und Neuerungen beim Start wurde verschoben
* &lbrack;Assimp&rbrack; Maya&#39;s StandardSurface wird im ID-Baking nicht erkannt
* &lbrack;Python&rbrack; Fehlende SSL-Bibliothek gibt einen Fehler aus
* &lbrack;Python&rbrack;&lbrack;Win&rbrack; Fehler beim Aufrufen von QColorConstants.Transparent
* &lbrack;Python&rbrack; Über Python erstellte Ebenen-Miniaturansichten werden erst aktualisiert, wenn Sie in den Ebenenstapel klicken
* &lbrack;Shader&rbrack; Fehlerhafte Verknüpfung im Shader-API-Changelog
* &lbrack;3D Assets&rbrack; OS-Proxy-Einstellungen beim Zugriff auf 3D-Elemente verwenden

**Bekannte Probleme**:

* &lbrack;Farbmanagement&rbrack; HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen geklemmte Farben
* &lbrack;Regression&rbrack;&lbrack;UI&rbrack; Kontextmenü ist auf HD-Bildschirmen zu klein
* &lbrack;Absturz&rbrack;&lbrack;Python&rbrack; USD Export ausgelöst durch TextureStateEvent
* &lbrack;MacOS Intel&rbrack; Absturz beim Importieren einiger Vorgaben
* &lbrack;Engine&rbrack; Malen mit dem Klon-Werkzeug in normalen Kanalverschiebungsfarben falsch
* &lbrack;Python&rbrack; Widget, das über ein Skript gelöscht scheint, das noch funktioniert
* &lbrack;RedHat&rbrack; Probleme mit dem Farbwähler

### 10.1.0

Freigabedatum: **2024/09/17** Zusammenfassung: **Hauptversion, neuer Inhalt: Füllbereichsmaske/Farbfilter, Stickereiaufklebefilter und sechs generische Substance-Filter, USD mit Material- und Shader-Eigenschaften importieren, Leistungsverbesserung, VFX-Plattform 2024-kompatibel und Migration auf Linux RedHat**

**Hinzugefügt**:

* &lbrack;Inhalt&rbrack; Neue Füllbereichsmaske/neuer Farbfilter hinzufügen
* &lbrack;Inhalt&rbrack; Neuen Stickerei Aufkleber Filter hinzufügen
* &lbrack;Inhalt&rbrack; Fügen Sie 6 neue generische Substance-Filter hinzu (FXAA, Vergröberungsfilter, Hochpass, Posterisierung, Glättungsschritt, Schwellenwert).
* &lbrack;USD&rbrack; Exportieren USD Ebene mit einem definierten ASM-Material
* &lbrack;USD&rbrack; USD mit Material- und Shader-Eigenschaften importieren
* &lbrack;Performance&rbrack; Optimierte Ebenenstapel-Miniaturansichten standardmäßig aktivieren
* &lbrack;Performance&rbrack; Reduzieren der Öffnungszeit von Projektdateien und des Speicherverbrauchs (Datendecodierung)
* VFX-Plattform 2024-kompatibel
* &lbrack;VFX Platform 2024&rbrack; Update auf Python 3.11
* &lbrack;VFX Platform 2024&rbrack; Update auf OpenEXR 3.2
* &lbrack;VFX Platform 2024&rbrack; &lbrack;USD&rbrack; Update OpenSubdiv 3.6.0
* &lbrack;VFX Platform 2024&rbrack;&lbrack;Farbmanagement&rbrack; Update auf OCIO 2.3.2
* &lbrack;Linux&rbrack; Migration zu Linux RedHat
* &lbrack;Linux&rbrack; Aktualisieren Sie die NVIDIA-Treibermindestversion auf 535.171.04
* &lbrack;Import&rbrack; Hinzufügen einer Option zum Spiegeln von Normalen-Map beim Importieren eines GLTF-Meshs
* &lbrack;UI&rbrack; Standardwert des Betriebssystems für die Entfernung der Erkennung von Ziehereignissen verwenden
* &lbrack;Substance Engine&rbrack; Aufrufstreifenfunktion hinzufügen, um die Symbole aus der ausführbaren Datei zu entfernen
* &lbrack;Startbildschirm&rbrack; Update auf neues Startbildschirmformat
* Substance Engine auf Version 9.1.3 aktualisieren
* &lbrack;Python&rbrack; Link zu Beispielen im Ebenenstapel-Dokumentationsmenü anzeigen
* &lbrack;JavaScript&rbrack; Javascript-Plug-ins in den Unterordner &quot;javascript/plugins&quot; verschieben

**Fest**:

* &lbrack;Illustrator&rbrack; Absturz beim Exportieren einer UV-Kachel mit .ai-Grafik in bestimmten Fällen
* &lbrack;Dynamische Pinselstriche&rbrack;&lbrack;Pfad&rbrack; Zufällig pro Strich funktioniert nicht auf einem Pfad
* &lbrack;UI&rbrack;&lbrack;Eigenschaften&rbrack; Sperre ist aktiviert, wenn die Kachelung nicht einheitlich ist
* Debug TXT-Datei wird erstellt, wenn Sie auf ein Painter-Projekt doppelklicken
* &lbrack;USD&rbrack;&lbrack;Export&rbrack; Möglicherweise fehlen einige Texturen
* &lbrack;ASM&rbrack; Farbstreuung-Kanal ignoriert metallic
* &lbrack;Inhalt&rbrack; Weichzeichnungsfilter funktioniert nicht im &quot;funktionierenden&quot; Farbraum
* &lbrack;Inhalt&rbrack; Mit dem Filter &quot;Height anpassen&quot; wird auch das Alpha der Ebene geändert.

**Bekannte Probleme**:

* &lbrack;Farbmanagement&rbrack; HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen geklemmte Farben
* &lbrack;Win&rbrack;&lbrack;Absturz&rbrack; &lbrack;ACE&rbrack; Kein Verwenden des sRGB ICE-Farbraums für die Anzeige transformieren
* &lbrack;Regression&rbrack;&lbrack;UI&rbrack; Kontextmenü ist auf HD-Bildschirmen zu klein
* &lbrack;Absturz&rbrack;&lbrack;Python&rbrack; USD Export ausgelöst durch TextureStateEvent
* &lbrack;MacOS Intel&rbrack; Absturz beim Importieren einiger Vorgaben
* &lbrack;Absturz&rbrack; Ressource verlagern und Projekt speichern
* &lbrack;Engine&rbrack; Malen mit dem Klon-Werkzeug in normalen Kanalverschiebungsfarben falsch
* &lbrack;Python&rbrack; Phantom-Widget wird angezeigt, weil das Skript noch funktioniert
* &lbrack;RedHat&rbrack; Probleme mit dem Farbwähler

### 10.0.1

Freigabedatum: **2024/06/11** Zusammenfassung: **Nebenversion, Fehlerbehebungen**

**Hinzugefügt:**

* &lbrack;Library&rbrack; Konvertieren von Substance-Schriftarten in normale Schriftdateien
* &lbrack;Illustrator&rbrack;&lbrack;SVG&rbrack; Miniaturen in der Bereichsauswahl einen hellgrauen Hintergrund geben
* &lbrack;Python&rbrack; Hinzufügen einer Funktion zur Bitmapquelle, um verfügbare Farbräume aufzulisten

**Fest**:

* &lbrack;Ebenenstapel&rbrack; Ordner immer geschlossen, wenn er in andere Ordner verschoben oder aus anderen Ordnern verschoben wird
* &lbrack;Speichern&rbrack; Die Projektdatei geht verloren, wenn das &quot;Speichern als Kopie&quot; oder das automatische Speichern in bestimmten Fällen fehlschlägt
* &lbrack;Import&rbrack; Assets mit demselben Namen, aber unterschiedlichen Erweiterungen werden überschrieben
* &lbrack;Eigenschaften&rbrack; Einstellungen fehlen, wenn Ankerpunkt in Bildeingaben verwendet wird
* &lbrack;Illustrator&rbrack; Illustrator-Dateien können nach dem Server-Absturz nicht importiert werden, ohne Painter neu zu starten
* &lbrack;Python&rbrack; Übergeordnete Instanz kann nicht mit Typ &quot;Eigenschaften&quot; festgelegt werden
* &lbrack;Python&rbrack; Das Festlegen des hohen Poly-Werts als Baking führend Parameter lädt das hohe Poly nicht
* &lbrack;Python&rbrack; Fehlermeldung für set_color_space() ist zu allgemein
* &lbrack;Python&rbrack; Mit Referenzquellen können Zyklen erstellt werden.

**Bekannte Probleme**:

* &lbrack;Farbmanagement&rbrack; HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen geklemmte Farben
* &lbrack;Regression&rbrack;&lbrack;UI&rbrack; Kontextmenü ist auf HD-Bildschirmen zu klein
* &lbrack;Absturz&rbrack;&lbrack;Python&rbrack; USD Export ausgelöst durch TextureStateEvent
* &lbrack;MacOS Intel&rbrack; Absturz beim Importieren einiger Vorgaben
* &lbrack;Illustrator&rbrack; Absturz beim Exportieren einer UV-Kachel mit .ai-Grafik in bestimmten Fällen
* &lbrack;Dynamische Pinselstriche&rbrack;&lbrack;Pfad&rbrack; Zufällig pro Strich funktioniert nicht auf einem Pfad

### 10.0.0

Freigabedatum: **2024/05/16** Zusammenfassung: **Hauptversion, Edition des Ebenenstapels mit Python-API, Lesen nativer Illustrator-Dateien, Integration von 3D-Assets und neuer Textressource**

**Hinzugefügt**:

* &lbrack;Illustrator&rbrack; Verwenden von Illustrator-Dateien mit Zeichenflächen in Painter
* &lbrack;Illustrator&rbrack;&lbrack;SVG&rbrack; Vorschauen in der Bereichsauswahl hinzufügen
* &lbrack;Substance 3D Assets&rbrack; Durchsuchen, Auswählen und Herunterladen von 3D-Elementen direkt in Painter
* &lbrack;Substance 3D Assets&rbrack;&lbrack;UI&rbrack; Neues Bedienfeld
* &lbrack;Substance 3D Assets&rbrack; Unterstützung für Umgebungs-Map und Materials
* &lbrack;Substance 3D Assets&rbrack; Ermöglicht das erneute Laden und Navigieren im und Öffnen des Speicherortordners in einem neuen Substance 3D Assets-Bedienfeld
* &lbrack;Substance 3D Assets&rbrack; Hinzufügen eines Download-Managers
* &lbrack;Textressource&rbrack; Einbettbare Schriften verwenden
* &lbrack;Textressource&rbrack; Rendern einer Schrift/eines Textes auf einem Mesh zulassen
* &lbrack;Textressource&rbrack; Schriften von Benutzern und anderen freigegebenen Pfaden im Bedienfeld &quot;Elemente&quot; mit einer neuen Kategorie anzeigen
* &lbrack;Textressource&rbrack;&lbrack;Eigenschaften&rbrack; Unterstützung für erweiterte Schrifteigenschaften hinzufügen
* &lbrack;Textressource&rbrack; Suchen/Anzeigen von Schriftarten in Mini-Regalen zulassen
* &lbrack;Textressource&rbrack; Fehlermeldung/Dialogfeld beim Importieren einer inkompatiblen Schrift hinzufügen
* Sonstiges
* &Klammer;Projektion&amp;Klammer füllen; Verbessern des Verhaltens von Skalierungs-Manipulatoren bei Verwendung kleiner Werte
* &lbrack;Manipulator&rbrack; Hinzufügen eines neuen präzisen Modus beim Drücken von STRG-Tastaturbefehl
* &lbrack;Manipulator&rbrack; Verbessern der Stabilität des Manipulators auf der Oberfläche beim Kamera beweg
* &lbrack;Export&rbrack; Hinzufügen eines Farbraumnamens in SBSAR-Ausgaben
* &lbrack;Performance&rbrack; Verbessern der Erkennungszeit von Elementen auf der Festplatte in der Bibliothek
* &lbrack;Substance&rbrack; Update auf Substance Engine Version 9.1.2
* &lbrack;Drag &amp; Drop&rbrack; Ausrichtung der Aufkleberdrehung an der Kamera beim Ablegen im Viewport
* &lbrack;Python&rbrack; Edition des Ebenenstapels
* &lbrack;Python&rbrack; Auswahl von Ebene, Effekt, Maske und Geomaske in der Benutzeroberfläche zulassen
* &lbrack;Python&rbrack; Ebenen-Mischmodi abrufen/festlegen
* &lbrack;Python&rbrack; Einstellungen für die Projektion der Füllebene abrufen/festlegen
* &lbrack;Python&rbrack; Abfragen der Substance-Material-Farbe aus einer Füllebene zulassen
* &lbrack;Python&rbrack; Abfragen und Festlegen von einheitliche Farben und Ressourcen in Ebenen und Effekten zulassen
* &lbrack;Python&rbrack; Erstellen und Bearbeiten von Textressourcen im Ebenenstapel zulassen
* &lbrack;Python&rbrack; Bearbeiten aktiver Kanäle für Ebenen und Effekte zulassen
* &lbrack;Python&rbrack; Stapelverarbeitung von Aktionen zum Rückgängigmachen/Wiederholen einzelner Vorgänge
* &lbrack;Python&rbrack; Laden/Bearbeiten von vektoriellen Quellparametern zulassen
* &lbrack;Python&rbrack; Bearbeitung von Farbegenschaften für Ebenen und Effekte mit Farbmanagement zulassen
* &lbrack;Python&rbrack; Abfragen und Erstellen von instanzierten Ebenen zulassen
* &lbrack;Python&rbrack; Hinzufügen des Effekts &quot;Farbauswahl&quot; zulassen
* &lbrack;Python&rbrack; Steuerung des Farbmanagements für Bitmapbilder zulassen
* &lbrack;Python&rbrack; Engine anhalten/fortsetzen
* &lbrack;Python&rbrack; Navigation zu gleichrangigen und übergeordneten Knoten zulassen
* &lbrack;Python&rbrack; Erstellen eines Filter-/Generatoreffekts zulassen
* &lbrack;Python&rbrack; Hinzufügen eines Ebeneneffekts zulassen
* &lbrack;Python&rbrack; Hinzufügen von intelligente Maske zu einer Ebene zulassen
* &lbrack;Python&rbrack; Erstellen/Bearbeiten von Ankerpunkten zulassen
* &lbrack;Python&rbrack; Maske auf Ebenen abrufen/festlegen
* &lbrack;Python&rbrack; Erstellen des Effekts &quot;Maske vergleichen&quot; zulassen
* &lbrack;Python&rbrack; Abfragen und Verwenden von Vorgaben aus Substance-Ressourcen zulassen
* &lbrack;Python&rbrack; Zulassen, dass Vorgaben und ihre Werte über die Funktion internal_properties für Substance-Ressourcen aufgelistet werden
* &lbrack;Python&rbrack; Auflisten vordefinierter Exportvorgaben zulassen
* &lbrack;Python&rbrack; Erlaubt das Auflisten der in der Bibliothek verfügbaren Exportvorgaben
* &lbrack;Python&rbrack; Abrufen des Inhalts von Exportvorgaben zulassen

**Fest**:

* &lbrack;Absturz&rbrack; &quot;Shader-Instanz entfernen&quot; mit Strg+Z rückgängig machen
* &lbrack;Absturz&rbrack; Erstellen einer Ebene auf leerem Stapel, wenn die letzte Auswahl ein Effekt war
* &lbrack;SVG&rbrack; Problem mit benutzerdefiniertem Wert für den zugeschnittenen Bereich
* &lbrack;Automatisches Entpacken&rbrack; Die Neuberechnung nur des Packings ohne Änderung der UV-Ausrichtung führt zu Absturz
* &blbrack;Drag &amp; Drop&rbrack; Verzögerung aufgrund externer Ressourcen wird mehrmals vorgeladen
* &lbrack;UI&rbrack; Durch Ziehen und Ablegen der Ressourcen-Miniaturansicht kann eine Warnmeldung im Ebenenstapel ausgeblendet werden
* &lbrack;Performance&rbrack; Maskierte UV-Kacheln werden noch berechnet
* &lbrack;USD&rbrack; Falsche Markierung für die Bereichsauswahl
* &lbrack;Ressource&rbrack; Bitmapbild wird beschädigt, nachdem im normalen Kanal gemalt und das Projekt gespeichert wurde
* &lbrack;USD&rbrack; Unterstützung der Bestellung von Meshs für linkshändige Scheitelpunkt
* &lbrack;Substance&rbrack; Auf die Standardeinstellung zurücksetzen, für Winkel-Widget immer wieder auf null zurücksetzen
* &lbrack;Engine&rbrack; Das Malen mit einem SVG in einer Schablone funktioniert nicht
* &lbrack;Engine&rbrack; Normalen-Map-Pinselstriche brechen nach einem Rückgängigmachen ab
* &lbrack;Inhalt&rbrack; &quot;Grafik zu Materialfilter&quot; hat falsche Alpha-Überblendung und falschen Farbraum
* &lbrack;Inhalt&rbrack; Füllmethoden auf dem Tile Generator funktionieren nicht
* &lbrack;Inhalt&rbrack; Histogramm-Scanfilter erzeugt in einigen Fällen Streifenbildung
* &lbrack;Inhalt&rbrack; Baking geführt Beleuchtungsstil berücksichtigt kein gemaltes Height
* &lbrack;Python&rbrack; Unerwarteter Fehler beim Abrufen der instanzierten Ebeneninformationen nach dem Shader-Wechsel
* &lbrack;Speichern&rbrack; Projektdatei geht verloren, wenn &quot;Speichern unter&quot; in bestimmten Fällen fehlschlägt

**Bekannte Probleme**:

* &lbrack;Farbmanagement&rbrack; HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen geklemmte Farben
* &lbrack;Absturz&rbrack;&lbrack;Linux&rbrack;&lbrack;AMD&rbrack; Ziehen und Ablegen von Ressourcen in Ebenenstapel unter Mac OS
* &lbrack;Regression&rbrack;&lbrack;UI&rbrack; Kontextmenü ist auf HD-Bildschirmen zu klein
* &lbrack;Absturz&rbrack;&lbrack;Python&rbrack; USD Export ausgelöst durch TextureStateEvent
* &lbrack;Speichern&rbrack; Die SPP-Projektdatei geht verloren, wenn &quot;Als Kopie speichern&quot; in bestimmten Fällen fehlschlägt
* &lbrack;MacOS Intel&rbrack; Absturz beim Importieren einiger Vorgaben
* &lbrack;Illustrator&rbrack; Ai-Dateien können nach dem Server-Absturz nicht importiert werden, ohne Painter neu zu starten
* &lbrack;Import&rbrack; Assets mit demselben Namen, aber unterschiedlichen Erweiterungen werden überschrieben

## Version 9

### 9.1.2

Veröffentlichungsdatum: **2024/01/30** Zusammenfassung: **Nebenversion, Fehlerbehebungen**

**Hinzugefügt**:

* &lbrack;Performance&rbrack; Verkürzung der Erstellungszeit für erste Füllebenen in neuen Projekten
* &lbrack;Performance&rbrack; Verkürzung der Ladezeit bei großen Umgebungs-Map
* &lbrack;Substance&rbrack; Speichern/Schließen von Projekten zulassen, selbst wenn Miniaturansichten generiert werden

**Fest**:

* Speichern schlägt in Projekten früherer Versionen fehl, wenn der Viewport geändert wird
* &lbrack;Absturz&rbrack; Mesh bei Verwendung von benutzerdefiniertem AO und Farbmanagement erneut importieren
* &Klammer;Projektion&amp;Klammer füllen; Durch Klicken auf den Manipulator &quot;Skalieren&quot; wird die Meldung &quot;nicht bemalbar&quot; angezeigt.
* &Klammer;Pinsel&Klammer; Malen mit UV-Ausrichtung verursacht Artefakte
* &lbrack;Ebenenstapel&rbrack; Das Umbenennen der Ebene ist langsam, wenn der Stapel sehr lang ist
* &lbrack;Ebenenstapel&rbrack; Falsche Fehlermeldung bei Verwendung eines inkompatiblen Filters in der Maske
* &lbrack;Ebenenstapel&rbrack; Die Auswahl wechselt nach dem Löschen wieder zur obersten Ebene
* &lbrack;Export&rbrack; Generierte normale Textur befindet sich immer im 3D-Raum-Nachbar-Auffüllmodus
* &lbrack;Export&rbrack; Textur Alpha wird nicht mit der Exportvorgabe 2D-Ansicht generiert
* &lbrack;Export&rbrack; SBSAR-Export hat falsche Verwendungen mit konvertierten Karten
* &lbrack;Shader&rbrack; Shader-API Changelog ist nicht auf dem neuesten Stand bei ASM

**Bekannte Probleme**:

* &lbrack;Farbmanagement&rbrack; HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen geklemmte Farben
* &lbrack;Absturz&rbrack;&lbrack;Linux&rbrack;&lbrack;AMD&rbrack; Ziehen und Ablegen von Ressourcen in Ebenenstapel unter Mac OS
* &lbrack;Regression&rbrack;&lbrack;UI&rbrack; Kontextmenü ist auf HD-Bildschirmen zu klein
* &lbrack;Absturz&rbrack;&lbrack;Python&rbrack; USD Export ausgelöst durch TextureStateEvent

### 9.1.1

Veröffentlichungsdatum: **2023/12/05** Zusammenfassung: **Nebenversion, Fehlerbehebungen und Senden an After Effects-Funktionen**

**Hinzugefügt:**

* &lbrack;Interop&rbrack; Senden eines strukturierten Meshs an After Effects zulassen (Ae 24.1)

**Fest:**

* &lbrack;Füllen&rbrack; Projektion UV-Satz zu UV-Satz liest nicht mehr als 2 UV-Satz
* &lbrack;Absturz&rbrack; 16.000 Umgebungs-Map
* &lbrack;Absturz&rbrack; Exr als Bildeingabe verwendet
* &lbrack;Absturz&rbrack; Kopieren und Einfügen von Pfaden in andere Projekte
* &lbrack;QoL&rbrack; Ziehen und Ablegen der Alpha-Ressource im Aufklebermodus erstellt UV-Projektion in der Maske
* &lbrack;Pfad&rbrack; Durch Kopieren von Pfad-Scheitelpunkten wird auch der Zielpfad beim erneuten Öffnen des Projekts umbenannt.
* &lbrack;Linux&rbrack; Die Farbauswahl kann mit mehreren Bildschirmen unterbrochen werden
* &lbrack;Automatisch Entpackt&rbrack; UI-Problem für die Texeldichtesteuerung
* &lbrack;Farbmanagement&rbrack; UI-Feedback ist sinnvoll, aber Engine ist nicht
* &lbrack;Farbmanagement&rbrack; Falsche Farbraumauswahl in der Maske mit Überschreibung der Benutzerdaten

**Bekannte Probleme:**

* &lbrack;Farbmanagement&rbrack; HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen geklemmte Farben
* &lbrack;Absturz&rbrack;&lbrack;Linux&rbrack; mit Linux Wayland auf AMD, wenn Ressourcen per Drag &amp; Drop in den Ebenenstapel gezogen werden
* &lbrack;Absturz&rbrack;&lbrack;Mac&rbrack; Anisotropische Filterung ändern unter Monterey OS
* &lbrack;Regression&rbrack;&lbrack;UI&rbrack; Kontextmenü ist auf dem HD-Bildschirm zu klein
* &lbrack;Python&rbrack; Absturz beim Exportieren von USD, die durch TextureStateEvent ausgelöst werden

### 9.1.0

Freigabedatum: **2023/11/07** Zusammenfassung: **Hauptversion mit SVG- und Transparenzunterstützung sowie Verbesserungen an Drag-and-Drop- und Pfad-Tools**

**Hinzugefügt:**

* &lbrack;SVG&rbrack; Importieren von Vektordateien zulassen (SVG)
* &lbrack;SVG&rbrack;&lbrack;UI&rbrack; Unterstützung für SVG-spezifische Eigenschaften hinzufügen
* &lbrack;SVG&rbrack; Mit dieser Option werden die Proportionen des Originalbilds beibehalten.
* &lbrack;SVG&rbrack; Automatisches Verwenden von Alpha von SVG mit Transparenz zulassen
* &lbrack;Interop&rbrack; Senden eines strukturierten Meshs an After Effects zulassen (Ae 24.1 Beta)
* &lbrack;Interop&rbrack; Hinzufügen von Einstellungen für &quot;An After Effects senden&quot;
* &lbrack;QoL&rbrack;&lbrack;Assets&rbrack;&lbrack;UI&rbrack; Element automatisch importieren, wenn es per Drag &amp; Drop in einen Benutzeroberflächensteckplatz gezogen wird
* &lbrack;QoL&rbrack; Zulassen, dass externe Elemente in den Ebenenstapel gezogen und dort abgelegt werden
* &lbrack;QoL&rbrack;&lbrack;Ebenenstapel&rbrack; Ziehen Sie Texturen per Drag &amp; Drop aus dem Bedienfeld &quot;Elemente&quot; in den Ebenenstapel
* &lbrack;QoL&rbrack;&lbrack;Viewport&rbrack; Generator ziehen und ablegen, Filter auf dem Mesh zulassen
* &lbrack;QoL&rbrack;&lbrack;Viewport&rbrack; Zulassen, dass externe Elemente auf den Mesh gezogen werden
* &lbrack;QoL&rbrack;&lbrack;Projektion&rbrack; Neuen UV-Satz zum UV-Satz-Projektion hinzufügen
* &lbrack;QoL&rbrack; Intelligente Masken in Viewport und Ebenenstapel als neue Ebenen ziehen und ablegen
* &lbrack;QoL&rbrack; Selektor für Generatoren mit mehreren Ausgaben hinzufügen, wenn er in der Maske verwendet wird
* &lbrack;QoL&rbrack; Ziehen und Ablegen von Ein Kanal-Bildern über einen Fülleffekt zulassen
* &lbrack;QoL&rbrack;&lbrack;Ebenenstapel&rbrack; Verwenden Sie STRG/ALT-Modifizierer mit Drag &amp; Drop, um anzugeben, wo/wie Effekte/Ebenen erstellt werden sollen
* &lbrack;Pfad&rbrack; Sichtbarkeit einzelner Pfade im Pfadbedienfeld ein-/ausschalten
* &lbrack;Pfad&rbrack; Verwenden von Transformations-Manipulatoren für Pfadpunkte zulassen
* &lbrack;Pfad&rbrack; Manuelles Steuern der Tangenten pro Scheitelpunkt zulassen
* &lbrack;Pfad&rbrack; Kopieren/Einfügen von Pfadeigenschaften
* &lbrack;Pfad&rbrack; Leerer Tastaturbefehl für die Tangente der Unterbrechung
* &lbrack;Shader&rbrack; Unterstützung für Deckkraft und Translucency in ASM Shader hinzufügen
* &lbrack;Shader&rbrack; Unterstützung für Absorptionsfarbe Channel mit ASM Shader hinzufügen
* &lbrack;Shader&rbrack; QuickInfos zu ASM-Shader-Parametern verbessern
* &lbrack;Shader&rbrack; Standardfarbe des Translucency-Kanals in Schwarz ändern
* &lbrack;Anzeigeeinstellungen&rbrack; Temporale Anti-Aliasing standardmäßig aktivieren
* &lbrack;Anzeigeeinstellungen&rbrack; Standardeinstellung für die Teilflächenstreuung aktivieren
* &lbrack;Substance&rbrack; Hinzufügen von Unterstützung für die ColorSpace-Eigenschaft von der Eingabe/Ausgabe durch den Graf
* &lbrack;Substance&rbrack; Substance Engine auf Version 9.0.3 aktualisieren
* &lbrack;UI&rbrack; Kontextabhängige Symbolleistenschaltfläche barrierefrei machen, selbst wenn das App-Fenster klein ist
* &lbrack;Automatisch Entpackt&rbrack; Steuert die Anzahl der UV-Kacheln mit der Texeldichte
* &blbrack;Baking&rbrack; GPU-Raytracing auf AMD-GPUs standardmäßig deaktivieren
* &lbrack;Performance&rbrack; Verlustfreie Komprimierung auf 16-Bit-Bilder anwenden, um den Projektbedarf zu verringern
* &lbrack;Python&rbrack; Ändern der standardmäßigen Kamera in der 3D-Ansicht zulassen
* &lbrack;Python&rbrack; Gelegt Möglichkeit, Mesh über Skripterstellung zu exportieren
* &lbrack;Content&rbrack;&lbrack;Samples&rbrack; Neues Beispielprojekt &quot;Französischer Restauranttisch&quot; hinzufügen
* &lbrack;Inhalt&rbrack; Alpha-Substance-Logo auf neue Version aktualisieren
* &lbrack;Inhalt&rbrack; Drei Material-Filter auf SVG anwenden (Custom Sticker, Custom Spray und Graphic to Material)

**Fest:**

* &lbrack;Absturz&rbrack; Ändern der Manipulator-Größe, wenn das Symmetrie-Werkzeug nicht verwendet wird
* &lbrack;Absturz&rbrack; &lbrack;Ebenenstapel&rbrack; Erstellen einer Ebene, wenn nichts ausgewählt ist
* &lbrack;Projekt&rbrack; Mesh-Map können beschädigt werden, nachdem nicht verwendete Ressourcen entfernt wurden.
* &lbrack;Projekt&rbrack; Ressourcenbeschädigung nach dem erneuten Importieren oder Baking des Images
* &lbrack;Assets&rbrack; Durch erneutes Laden eines Assets wird es aus den Favoriten entfernt
* &lbrack;Import&rbrack; Ressourcen können nicht importiert werden, wenn im Bedienfeld &quot;Elemente&quot; &quot;Kein Ergebnis gefunden&quot; angezeigt wird
* &lbrack;UI&rbrack; Der Pfeil der kontextbezogenen Symbolleiste wird in einigen Fällen nicht angezeigt
* &lbrack;Substance&rbrack; Schaltfläche &quot;Nebeneinander&quot; für boolesche Werte wird nicht unterstützt
* &lbrack;Ebene&rbrack; Falsche Kanalbeschriftung bei Verwendung in der Maske
* &lbrack;Export&rbrack;&lbrack;glTF&rbrack; glTF/GLB-Dateien, die aus Painter exportiert werden, haben keine Physische Größe
* &lbrack;Inhalt&rbrack; Intensität des Weichzeichnungsfilters ist auf 16 eingestellt
* &lbrack;Inhalt&rbrack; Farbabstimmungsfilter &quot;Zielfarbe&quot; Bildeingabe ist nicht sichtbar

**Bekannte Probleme:**

* &lbrack;Farbmanagement&rbrack; HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen geklemmte Farben
* &lbrack;Absturz&rbrack;&lbrack;Linux&rbrack; mit Linux Wayland auf AMD, wenn Ressourcen per Drag &amp; Drop in den Ebenenstapel gezogen werden
* &lbrack;Absturz&rbrack;&lbrack;Mac&rbrack; Anisotropische Filterung ändern unter Monterey OS
* &lbrack;Absturz&rbrack; Exr als Bildeingabe verwendet
* &lbrack;Absturz&rbrack; 16.000 Umgebungs-Map
* &lbrack;Automatisch Entpackt&rbrack; UI-Problem für die Texeldichtesteuerung
* &lbrack;Regression&rbrack;&lbrack;UI&rbrack; Kontextmenü ist auf dem HD-Bildschirm zu klein
* &lbrack;Python&rbrack; Absturz beim Exportieren von USD, die durch TextureStateEvent ausgelöst werden
* &lbrack;QoL&rbrack; Ziehen und Ablegen der Alpha-Ressource im Aufklebermodus erstellt UV-Projektion in der Maske

### 9.0.1

Freigabedatum: **2023/09/19** Zusammenfassung: **Geringfügige Fehlerbehebungsversion mit mehreren Verbesserungen**

**Hinzugefügt:**

* &lbrack;Import&rbrack; Standard-Importspeicherort im Importfenster festlegen
* &blbrack;Baking-Modus&rbrack; Parameter auf ihre Standardwerte zurücksetzen
* &blbrack;Baking&rbrack; Baking beim Erstellen eines Projekts auf Malen-Auflösung festlegen
* &lbrack;Symmetrie&rbrack; Symmetrie-spezifischen Manipulator vom Tastaturbefehl Q lösen
* &lbrack;Menü&rbrack; Option &quot;Protokoll anzeigen&quot; im Hilfemenü hinzufügen
* &lbrack;Viewport&rbrack; Verbessern der Schatten-Rendering-Geschwindigkeit
* &lbrack;Substance&rbrack; Engine auf Version 9.0.1 aktualisieren
* &lbrack;Farbmanagement&rbrack; OCIO Konfigurationsdatei kann einen beliebigen Erweiterungstyp haben
* &lbrack;Assets&rbrack; SBSAR-Ressource mit &#39;Aufkleber&#39; sollte automatisch auf Warp-Projektion gesetzt werden
* &lbrack;Pfad&rbrack; Anzeigen einer Meldung, wenn versucht wird, mit dem Pfadwerkzeug zu interagieren, während UI und Gizmos ausgeblendet sind

**Fest:**

* &lbrack;Absturz&rbrack; Alt + Ziehen im Pfadbedienfeld
* &lbrack;Ressourcen&rbrack; importieren Zufälliger Absturz beim Entfernen der zu importierenden Ressourcen
* Absturz beim Importieren einer komprimierten GLB-Datei
* Problem beim Malen auf Meshs, die UVs gemeinsam nutzen
* Mesh blinkt schwarz, wenn der Cache neu berechnet oder geladen wird
* &lbrack;Eigenschaften&rbrack; Kontextmenü zum Zurücksetzen der Parameter wird in Dropdown-Listen nicht angezeigt
* &lbrack;Ebene&rbrack; Schieberegler für Eingabe nach vorheriger Ebene gesperrt
* &lbrack;AMD&rbrack;&lbrack;Sparse&rbrack; SVT-Option, wenn aktiviert, erzeugt Artefakte
* &lbrack;Projektion&rbrack;&lbrack;Verkrümmen&rbrack; Absturz beim Doppelklicken auf Scheitelpunkte
* &lbrack;Pfad&rbrack; Benutzeroberfläche und Pfad werden im Baking-Modus angezeigt
* &lbrack;AMD&rbrack; Textur verloren, wenn mit Sicht gespielt wird
* &lbrack;Sparse&rbrack; Zu niedrige Auflösung beim Umdrehen des Meshs

**Bekannte Probleme:**

* &lbrack;Farbmanagement&rbrack; HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen geklemmte Farben

### 9.0.0

Freigabedatum: **2023/06/20** Zusammenfassung: **Hauptversion mit Malen entlang des Pfades, die 3D-Kurven, neue Basismaterialien und das Bereinigen älterer Materialien sowie neue Vorgaben für 3D-Kurven ermöglicht**

**Hinzugefügt:**

* &lbrack;Pfad&rbrack; Neue Malen entlang des Pfads hinzufügen
* &lbrack;Pfad&rbrack; Hinzufügen eines leeren Tastaturbefehls für das Pfadwerkzeug
* &lbrack;Pfad&rbrack; Hinzufügen neuer Punkte zu einem vorhandenen Pfad zulassen
* &lbrack;Pfad&rbrack; Tastaturbefehl hinzufügen, um die aktuelle Pfaderstellung zu beenden
* &lbrack;Pfad&rbrack; Bearbeiten der Pinseleigenschaften für Pfade zulassen
* &lbrack;Pfad&rbrack; Tangenten beim Platzieren eines Punkts automatisch anpassen
* &lbrack;Pfad&rbrack; Tangenten beim Verschieben eines Punkts neu berechnen
* &lbrack;Pfad&rbrack; Einrasten neu erzeugter Ankerpunkte an die Fläche eines Meshs
* &lbrack;Pfad&rbrack; Bearbeiten des Drucks pro Scheitelpunkt zulassen
* &lbrack;Pfad&rbrack; Anpassen des Drucks des neu erstellten Punkts von benachbarten Punkten
* &lbrack;Pfad&rbrack; Umwandeln von Punkten in Übergangspunkte/Eckpunkte zulassen (Tangente umbrechen)
* &lbrack;Pfad&rbrack; Verschieben eines neu hinzugefügten Punkts sofort zulassen
* &lbrack;Pfad&rbrack; Entfernen von Punkten aus vorhandenem Pfad zulassen
* &lbrack;Pfad&rbrack; Umkehren der Richtung eines Pfades zulassen
* &lbrack;Pfad&rbrack; Auswahl eines Pfads im Viewport zulassen
* &lbrack;Pfad&rbrack; Auswählen von Pfadpunkten mit dem Auswahlrechteck zulassen
* &lbrack;Pfad&rbrack; Einführung von STRG+A-Tastaturbefehlen zum Auswählen aller Punkte eines Pfades
* &lbrack;Pfad&rbrack; Schließen des Pfads zulassen
* &lbrack;Pfad&rbrack; Geben Sie die Achse &quot;Pfad nach oben&quot; in den Eigenschaften an
* &lbrack;Pfad&rbrack; Hinzufügen eines Scheitelpunkt-Steuerungsmenüs zur kontextabhängigen Symbolleiste
* &lbrack;Pfad&rbrack; Hinzufügen von Malen-/Radier-/Verwischen-Modi zum Pfadwerkzeug
* &lbrack;Pfad&rbrack; Visuelles Feedback für Pfade im Viewport erstellen
* &lbrack;Pfad&rbrack; Visuelle Anzeige der Pfadrichtung hinzufügen
* &lbrack;Pfad&rbrack; Thickness der Pfadanzeige hinzufügen
* &lbrack;Pfad&rbrack; Pfade ausblenden.
* &lbrack;Pfad&rbrack; Bedienfeld &quot;Pfad hinzufügen&quot;, um Pfade der aktuell ausgewählten Ebene aufzulisten
* &lbrack;Pfad&rbrack; Visuelles Feedback beim Bewegen des Mauszeigers über einen Pfad im Pfadbedienfeld hinzufügen
* &lbrack;Pfad&rbrack; Pfadbedienfeld anzeigen, wenn das Pfadwerkzeug ausgewählt ist
* &lbrack;Pfad&rbrack; Umbenennen, Löschen, Kopieren, Ausschneiden und Duplizieren von Pfaden im Bedienfeld &quot;Pfad&quot; zulassen
* &lbrack;Pfad&rbrack; Meldung anzeigen, wenn versucht wird, im 2D-Viewport mit dem Pfadwerkzeug zu interagieren
* &lbrack;Library&rbrack; Neue Inhalte integrieren (Pfadwerkzeuge und Basismaterialien)
* &lbrack;Dynamische Pinselstriche&rbrack; Eigenschaft &quot;Abstand&quot; für Dynamische Pinselstriche hinzufügen
* &lbrack;Dynamische Pinselstriche&rbrack; Hinzufügen von Größen- und Abstand-Eigenschaften zu Dynamischen Pinselstrichen
* &lbrack;Dynamische Pinselstriche&rbrack; Hinzufügen der Eigenschaft &quot;Anfang/Mitte/Ende&quot; für Dynamische Pinselstriche
* &lbrack;Python&rbrack;&lbrack;USD&rbrack; Leg von Projektkonfigurationsparametern für das USD
* &lbrack;Python&rbrack;&lbrack;USD&rbrack; Leg der Projekterstellungsparameter für das USD
* &lbrack;Export&rbrack;&lbrack;USD&rbrack; Projektpfadinformationen in exportierten USD hinzufügen
* &lbrack;GLTF&rbrack; Texturen in der Bibliothek beim erneuten Laden einer GLTF-Datei aktualisieren
* &lbrack;Shader&rbrack; Reduzieren von Artefakten in der Naht von UV-Inseln mit unterschiedlicher Ausrichtung
* &lbrack;Engine&rbrack; Update auf Substance Engine Version 9.0

**Fest:**

* &lbrack;Import&rbrack; Einige GLB mit Texturen erhalten keine Texturen in Painter
* &lbrack;AMD&rbrack; Artefakte an Rahmen für alle 3D-Projektion-Flächen
* &lbrack;Engine&rbrack; Texturen brechen beim Umschalten der Ebenensichtbarkeit ab
* &lbrack;Engine&rbrack; Beim Ändern des Mischmodus sind an einigen Stellen Texturen leer
* &lbrack;Engine&rbrack; Textur/Projektion ist in einigen Fällen leerer Verkrümmungsmodus
* &lbrack;Iray&rbrack; Iteration wird beim Speichern des Renderings auf 0 zurückgesetzt
* &lbrack;Log&rbrack; USD Fehlermeldung beim Ausführen von &quot;Datei&quot; > &quot;Neu&quot;

**Bekannte Probleme:**

* &lbrack;Farbmanagement&rbrack; HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen geklemmte Farben
* &lbrack;Ebenenstapel&rbrack; Eingabequelle nicht pro Ebene gespeichert

## Version 8

### 8.3.1

Freigabedatum: **2023/04/27**

**Hinzugefügt:**

* &blbrack;Baking-Modus&rbrack; Tastaturbefehl hinzufügen (leer), um den Viewport anzuzeigen/auszublenden
* &blbrack;Baking-Modus&rbrack; Bei Verwendung der Schaltfläche &quot;Baking führend Mesh ausblenden&quot; immer niedrige Poly-Werte anzeigen
* &blbrack;Baking-Modus&rbrack; Suffix für &quot;Zuordnung nach Name&quot; basierend auf aktuellem Textursatz anzeigen
* &lbrack;Import&rbrack; Unterstützung für GLTF-Binärdateien (glb) hinzufügen
* &lbrack;Textursatz list&rbrack; Menü &quot;Hinzufügen&quot; zum Auswählen oder Erstellen von Shader-Instanzen
* &lbrack;Textursatz list&rbrack; Schnelles Ändern der Auflösung von Textursatz und UV-Kachel
* &lbrack;Physische Größe&rbrack; Verbessern des Manipulator-Verhaltens bei der Verwendung von Physische Größe in UV-Projektionen
* &lbrack;UI&rbrack; &quot;Speichern unter&quot; wieder im Dateimenü anzeigen
* &lbrack;UI&rbrack; Speichern der Ansichtsauswahl (nur 2D, nur 3D, beide) im UI-Layout
* &lbrack;USD&rbrack; Weniger vage Fehlermeldung bei der Projekterstellung mit nicht unterstützten USD
* &lbrack;Python&rbrack; Hinzufügen von Baking führend Ereignissen, um den Fortschritt des Bakings zu verfolgen
* &lbrack;Python&rbrack; Abbrechen eines Baking zulassen
* &lbrack;Python&rbrack; &quot;Basierend auf Ausgabevorlage&quot; für Dateityp und Bittiefe beim Exportieren gelegt
* &lbrack;Python&rbrack; Gelegt Aktualisierungszeit für TextureStateEvent.Update

**Fest:**

* &lbrack;Absturz&rbrack; Seltener Absturz beim Schließen eines Projekts
* &lbrack;Absturz&rbrack; &blbrack;Baking&rbrack; Mesh-Map-Synchronisierung mit Height oder Krümmung für ein bestimmtes Projekt aktivieren
* &lbrack;Absturz&rbrack;&lbrack;Scripting&rbrack; Absturz beim Hinzufügen eines Materials nach dem Erstellen einer Shader-Instanz
* &blbrack;Baking-Modus&rbrack; Die AO-Intensität im neutralen Material hat keine Auswirkungen
* &blbrack;Baking-Modus&rbrack; Absturz beim Wechseln in den Baking-Modus, bevor das Modell geladen wird
* &blbrack;Baking-Modus&rbrack; Fehlermeldung &quot;Fehlende Fehlermeldung&quot; auf der Registerkarte &quot;Baking führend Prozess&quot;
* &blbrack;Baking-Modus&rbrack; Einstellungen für neutrales Material haben nach dem erneuten Importieren eines Meshs keine Auswirkungen
* &blbrack;Baking-Modus&rbrack; Viewport-Trennzeichen werden global und nicht pro Modus gespeichert.
* &blbrack;Baking-Modus&rbrack; Visualisierungsproblem: Durchschnittliche Normale verändert die Oberfläche des Käfigs nicht
* &lbrack;Farbmanagement&rbrack; Die Einstellung &quot;Farbraum automatisch erkennen&quot; ist deaktiviert, wenn OCIO env var vorhanden ist
* &lbrack;Inhalt&rbrack; Der Maskenkonturfilter weist ein Artefakt mit Height-Eingabe auf.
* &lbrack;Inhalt&rbrack; Intensitätsregler des Steigung-Weichzeichnungsfilters ist auf 1,0 geklemmt
* &lbrack;Interop&rbrack; Projekt mit GLTF kann nicht aus Sampler erstellt werden
* &lbrack;Ebenenstapel&rbrack; Der Wert für die Kachelung der Projektion wird nicht korrekt mit dem Manipulator aktualisiert
* &lbrack;Linux&rbrack; Versatz zwischen Grafiktablett-Stift und Cursor mit einem HDPI-Wert von mehr als 100 %
* &lbrack;Python&rbrack; Absturz beim erneuten Importieren eines Meshs nach dem Erstellen eines Projekts
* &lbrack;Substance&rbrack; 3D-Rauschen funktionieren nach dem erneuten Importieren eines Meshs nicht mehr
* &blbrack;UV-Kacheln&rbrack; Offset für UV-Projektion wird auf 1 geklemmt
* &lbrack;Viewport&rbrack; Visuelles Feedback zu geraden Linien ist nicht mehr sichtbar
* &lbrack;WhatsNew&rbrack; Falscher Zeilenumbruch bei Funktionstiteln

**Bekannte Probleme:**

* &lbrack;Import&rbrack; Einige GLB mit Texturen erhalten keine Texturen in Painter

### 8.3.0

*(Freigegeben: 10. Januar 2023 (1&rbrace;)Zusammenfassung:**Hauptversion mit neuem Importmodus, neuem Baking und Export von USD und Physische Größe-Unterstützung für UV-Projektion***

**Hinzugefügt:**

* &blbrack;Baking-Modus&rbrack; Neuer Baking-Modus, der dem Baking gewidmet ist

* &blbrack;Baking-Modus&rbrack; Tastaturbefehl so einstellen, dass er in den Baking-Modus auf F8 wechselt

* &blbrack;Baking-Modus&rbrack; Schaltfläche &quot;Baking hinzufügen&quot; und &quot;Abbrechen&quot; im Viewport

* &blbrack;Baking-Modus&rbrack; Hinzufügen einer Baking führend Auswahl in der Liste &quot;Textursatz&quot;

* &blbrack;Baking-Modus&rbrack; Fenster &quot;Neue Mesh-Map-Baker hinzufügen&quot;, um Baker auszuwählen

* &blbrack;Baking-Modus&rbrack; Neues Fenster &quot;Mesh-Map-Einstellungen hinzufügen&quot; zum Bearbeiten der Baking-Einstellungen

* &blbrack;Baking-Modus&rbrack; Neues Baking-Protokollfenster hinzufügen, um dem Baking zu folgen

* &blbrack;Baking-Modus&rbrack; Hinzufügen von Baking führend Parametern und Rückgängigmachen von Aktionen zum Verlaufsfenster

* &blbrack;Baking-Modus&rbrack; Breadcrumbs in den Mesh-Map-Einstellungen hinzufügen

* &blbrack;Baking-Modus&rbrack; Hinzufügen von Mesh-Map-Miniaturansichten im Fenster &quot;Mesh-Map Baker&quot;

* &blbrack;Baking-Modus&rbrack; Minimierbares Menü &quot;Visualisierungseinstellungen hinzufügen&quot; im 3D-Viewport

* &blbrack;Baking-Modus&rbrack; Hinzufügen einer Visualisierungseinstellung zum Ein-/Ausblenden des Meshs mit hoher Poly-Intensität

* &blbrack;Baking-Modus&rbrack; Visualisierungseinstellung zum Ein-/Ausblenden des Käfig-Meshs und der Drahtgitter hinzufügen

* &blbrack;Baking-Modus&rbrack; Visualisierungseinstellung hinzufügen, um den Mesh mit geringer Poly-Intensität ein- oder auszublenden

* &blbrack;Baking-Modus&rbrack; Visualisierungseinstellung hinzufügen, um harte Kanten ohne UV-Nähte als Fehler darzustellen

* &blbrack;Baking-Modus&rbrack; Im Viewport über Mesh- und Baking-Fehler informieren, wenn das Baking-Protokoll nicht angezeigt wird

* &blbrack;Baking-Modus&rbrack; Aktion zum Synchronisieren der Baker-Einstellungen auf allen Textursätzen hinzufügen

  Im Fenster &quot;Mesh-Map-Baker&quot; kann jeder Baker (sowie die allgemeinen Einstellungen) über Textursatz hinweg synchronisiert werden, indem Sie auf das Verknüpfungssymbol neben dem Namen klicken. Dadurch wird ein Fenster geöffnet, in dem Sie auswählen können, welche Textursatz dieselben Parameter verwenden sollen.

* &blbrack;Baking-Modus&rbrack; Hinzufügen von Aktionen zum Kopieren und Einfügen von Baker

  Im Fenster &quot;Mesh-Map-Baker&quot; stehen Aktionen zum Kopieren und Übergehen der einzelnen Baker-Einstellungen über Textursätze hinweg zur Verfügung, entweder über das spezielle Menü am oberen Fensterrand oder über das Kontextmenü mit der rechten Maustaste.

* &blbrack;Baking-Modus&rbrack; Schaltfläche &quot;Baking hinzufügen&quot; im Fehlerprotokoll, um von den Fehlereinstellungen nach rechts zu springen

  Wenn ein Baker fehlschlägt oder ein Mesh nicht ordnungsgemäß geladen wird, wird im Protokoll eine Fehlermeldung Baking geführt. Mit einer Schaltfläche neben der Meldung können Sie das Fenster Mesh-Map-Baker und Mesh-Map-Einstellungen ändern, um die entsprechenden Einstellungen anzuzeigen. Dies hilft dabei, die Ursache eines Problems einfacher zu isolieren, um es beheben zu können.

* &blbrack;Baking-Modus&rbrack; Menüs hinzufügen, um Textursatz und Baker zu verwalten

  Sowohl im Fenster &quot;Textursatz-Liste&quot; als auch im Fenster &quot;Mesh-Map-Baker&quot; wurde ein kleines Aktionsmenü hinzugefügt, um das Kopieren und Umkehren von Auswahlen zu unterstützen.

* &blbrack;Baking-Modus&rbrack; Baker-Auswahlliste pro Textursatz teilen

* &blbrack;Baking-Modus&rbrack; Gemeinsame Einstellungen pro Textursatz teilen

* &blbrack;Baking-Modus&rbrack; Mesh mit hoher Poly- und Käfig-Auflösung laden, ohne die Oberfläche einzufrieren

* &blbrack;Baking-Modus&rbrack; Verwenden Sie die Fortschrittsleiste des Viewports, um das Laden des Meshs anzuzeigen

* &blbrack;Baking-Modus&rbrack; Ladestatus des Meshs im Baking-Protokoll hinzufügen

* &blbrack;Baking-Modus&rbrack; Mesh im Viewport während des Bakings umkehren

* &blbrack;Baking-Modus&rbrack; Baking-Reihenfolge auf der Grundlage der Sichtbarkeit des aktuellen Viewports des Meshs festlegen

* &blbrack;Baking-Modus&rbrack; Implizit Baking führend Käfig in Viewport anzeigen

  Wenn keine benutzerdefinierte Käfig-Meshdatei verwendet wird, wird ein automatischer Käfig-Mesh generiert und im Viewport angezeigt. Die Größe basiert auf dem Parameter &quot;Max. Frontalentfernung&quot; aus den allgemeinen Einstellungen des Bakings. Mit dem Mesh &quot;Käfig&quot; wird angegeben, wie weit die Anpassung zwischen dem niedrigen und dem hohen Poly-Wert gehen wird.

* &blbrack;Baking-Modus&rbrack; Übereinstimmende Liste von Mesh-Namen für &quot;Übereinstimmender Name&quot; im Baking-Protokoll anzeigen

* &blbrack;Baking-Modus&rbrack; 3D-Material im Viewport mit neutralem Modell anzeigen

* &blbrack;Baking-Modus&rbrack; Berechnung des Engine im Baking deaktivieren

* &blbrack;Baking-Modus&rbrack; Beim Beenden der App während eines Baking wird eine Warnung angezeigt

* &lbrack;Baker&rbrack; Aktualisieren der Beschriftungen für Anti-Aliasing-Einstellungen

  Die Einstellungswerte für das Anti-Aliasing wurden in &quot;Supersampling&quot; umbenannt und mit einer expliziten Multiplikatornummer versehen, um das Verhalten zu verdeutlichen.

* &lbrack;Baker&rbrack; Aktualisieren Sie die Baker auf Version 2.5.7.

* &lbrack;USD&rbrack; Importieren und Exportieren von Universal Scene Description-Dateien (USD)

* &lbrack;USD&rbrack; Hinzufügen USD Optionen zum Fenster &quot;Neues Projekt&quot; bei Auswahl einer USD Datei

* &lbrack;USD&rbrack; Neues Auswahlfenster &quot;Umfang und Varianten hinzufügen&quot;

  Wenn Sie eine USD-Datei importieren, können Sie durch Klicken auf die Schaltfläche &quot;Ändern&quot; im Fenster &quot;Neues Projekt&quot; oder &quot;Projektkonfiguration&quot; auswählen, welche Teile und Varianten einer USD-Datei importiert werden sollen.

* &lbrack;USD&rbrack; Option &quot;Unterteilungsebenen hinzufügen

  Beim Erstellen eines neuen Projekts mit einer USD Meshdatei, die Unterteilungen enthält, ist es möglich, die Ebene der Unterteilungen mithilfe eines Schiebereglers auszuwählen. Das Projekt wird mit dem unterteilten Mesh erstellt. Die Ebene kann über die Projektkonfiguration geändert werden.

* &lbrack;USD&rbrack; Importieren USD Meshs mit Skin in bestimmten Rahmen

  Wenn Sie ein neues Projekt mit einer USD Meshdatei erstellen, die eine Animation enthält, können Sie den Rahmen mithilfe eines Schiebereglers auswählen, der die eingebettete Timeline-Sequenz widerspiegelt. Der Rahmen kann über die Projektkonfiguration modifiziert werden.

* &lbrack;USD&rbrack;&lbrack;Export&rbrack; Option zum Exportieren USD Dateien hinzufügen

  Das neue Kontrollkästchen &quot;USD exportieren&quot; wurde dem Fenster &quot;Texturen exportieren&quot; hinzugefügt. Wenn diese Option aktiviert ist, können USD sowie Textur Maps mit einer beliebigen Vorlage exportiert werden.

* &lbrack;USD&rbrack;&lbrack;Export&rbrack; USD Dateiformat zum Mesh-Export hinzufügen

* &lbrack;USD&rbrack; Benennen Sie die vorhandene Exportvorgabe &quot;USD PBR Metal Rauheit&quot; um, um sie genauer zu benennen

  Die USD Exportvorlage, die zuvor als &quot;USD PBR Metal Rauheit&quot; bezeichnet wurde, ist weiterhin über &quot;Texturen exportieren&quot; > &quot;Ausgabevorlage&quot; > &quot;USDz&quot; (Apple AR) verfügbar.

* &lbrack;Automatisch Entpackt&rbrack; &quot;Ausrichtung sperren&quot; für Packing hinzufügen

  Neue Option für Einstellungen für den automatischen entpack, mit der die Ausrichtung bestehender UV-Inseln beibehalten werden kann, wenn die Funktion &quot;Packing&quot; verwendet wird. Der Zugriff darauf erfolgt über &quot;Neues Projekt&quot; > &quot;Optionen für Automatisches Entpacken&quot; > &quot;Ausrichtung der UV-Insel&quot;.

* &lbrack;Physische Größe&rbrack; Hinzufügen einer Einstellung zur automatischen Verwendung von Physische Größe im Fülleffekt/in der Ebene

  Eine neue Option zum automatischen Umschalten auf die Skalierung der Physische Größe wurde hinzugefügt, wenn ein Material mit eingebetteter Physische Größe verwendet wird. Sie kann pro Projekt über Neues Projekt oder über Bearbeiten > Projektkonfiguration > Physische Größe > Füllebene-Skalierung auf Physische Größe umschalten, wenn Materialien zugewiesen werden, aktiviert werden.

* &lbrack;Physische Größe&rbrack; Physische Größe für UV-Projektion gelegt

  Die Skalierung der Physische Größe ist jetzt für UV-Projektionen verfügbar - sie aktiviert die automatische Größenänderung für ein Material basierend auf der Physische Größe eines Meshs. Sie kann über &quot;Skalieren > Physische Größe&quot; im Fenster &quot;Füllebene&quot; oder &quot;Effekteigenschaften&quot; ausgewählt werden.

* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Abfragen der Anwendungsversion zulassen

* &lbrack;Skripterstellung&rbrack;&lbrack;JavaScript&rbrack; API zur Anpassung an neue Baking-Parameter aktualisieren

* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Baking: Bearbeiten der Parameter für das Baking

* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Baking: Baking starten/abbrechen

* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Baking: Methode der selektierten Krümmung

* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Baking: Auswahl von Bakern/UV-Kacheln

* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Baking: Baker-Einstellungen auf allen Textursätzen synchronisieren

* &lbrack;SVT&rbrack; Aktivieren der Unterstützung von geringer Hardware auf AMD-GPUs

  Die Hardwarebeschleunigung für das Dünn besetzte virtuelle Textur-System kann jetzt mit AMD-GPUs aktiviert werden. Diese Einstellung wird in den allgemeinen Voreinstellungen automatisch aktiviert.

* &lbrack;Projektion&rbrack; Parameter für zylindrische Projektion umbenennen

  Der Parameter &quot;Cylinder Cap Culling&quot; wurde in &quot;Rückseiten-Ausblendung&quot; umbenannt, um seine Wirkung besser darzustellen. Die zugehörige QuickInfo wurde entsprechend angepasst.

* &lbrack;Projekt&rbrack; Anwendungsversion im Projekt speichern und über Skripterstellung abrufen

  Seit Version 8.2 wird die Version der Anwendung beim Speichern in der spp-Datei gespeichert. Diese Versionsnummer kann mit der Funktion last_saved_substance_painter_version() im Projektmodul der Python-API abgerufen werden. Für Projekte, die vor 8.2 erstellt wurden, ist der zurückgegebene Wert null.

* &lbrack;Import&rbrack; Verbessern der allgemeinen Importzeit von 3D-Modellen

  Wir haben die allgemeine Importzeit von Meshs verbessert. Zum Beispiel die Verkürzung der Wartezeit beim Laden von High-Poly-Meshs zum Baking. Diese Optimierung gilt insbesondere für das Laden von OBJ.

**Fest:**

* &lbrack;Absturz&rbrack; Ändern von Kanälen bei Filtern mit bestimmtem Stapel

* &lbrack;Mac&rbrack;&lbrack;M1&rbrack; Absturz beim Erstellen einer Füllebene und Verlassen des Ebenenstapels

  Dieses Problem kann durch Aktualisieren auf Mac OS 13 (Ventura) behoben werden.

* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Absturz bei Verwendung von ui.add_dock_widget() mit falschem Typ

* &blbrack;Baking&rbrack; Unvollständige Fehlermeldung im Protokoll, wenn ein Baking fehlschlägt

* &blbrack;Baking&rbrack; Der Speicher wird nach Abschluss des Bakings nicht freigegeben

* &lbrack;Engine&rbrack; Texturen-Cache wird nicht aktualisiert, wenn die Effektsichtbarkeit geändert wird

* &lbrack;Export&rbrack; 2D-Ansicht exportiert zufällig einheitliche Map

* &lbrack;Projekt&rbrack; Speicherzuordnungsfehler beim Speichern eines Projekts mit großem Mesh

* &lbrack;Viewport&rbrack; TAA verursacht beim Malen in einigen Fällen Artefakte

**Bekannte Probleme:**

* &lbrack;Farbmanagement&rbrack; HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen geklemmte Farben
* &lbrack;Ebenenstapel&rbrack; Eingabequelle nicht pro Ebene gespeichert

### 8.2.0

*(Freigegeben: 06. Oktober 2022*)Zusammenfassung: **Hauptversion mit neuen Onboarding-Bedienfeldern (neues Begrüßungs-Bedienfeld und neues Bedienfeld), Export in SBSAR, Effekten für Ordner, mehreren Verbesserungen für die Lebensqualität und Fehlerbehebungen.**

**Hinzugefügt:**

* &lbrack;Onboarding&rbrack; Onboarding-Bereich zur Aufnahme neuer Benutzer

  Es wurde ein neuer Begrüßungsbildschirm hinzugefügt, wenn neue CC-Benutzer Painter zum ersten Mal öffnen.

* &lbrack;Onboarding&rbrack; Fenster &quot;Neue Funktionen&quot; zur Verbesserung der Auffindbarkeit neuer Funktionen

  Es wurde ein neuer Bildschirm &quot;Neue Funktionen&quot; hinzugefügt, auf dem die wichtigsten neuen Funktionen angezeigt werden. Es wird automatisch angezeigt, wenn Painter nach einem wichtigen Update zum ersten Mal geöffnet wird, und Sie können erneut auf es über Hilfe > Neue Funktionen zugreifen.

* &lbrack;Onboarding&rbrack; Alte Willkommensseite in &quot;Startbildschirm&quot; umbenennen

  Alter Begrüßungsbildschirm wurde in Startbildschirm umbenannt, um Verwechslungen mit dem neuen Begrüßungsbildschirm zu vermeiden.

* &lbrack;UI&rbrack; Beheben von Skalierungsproblemen für HD-Bildschirme

  Verbesserte Anpassung der Painter-Benutzeroberfläche auf HD-Bildschirmen mit benutzerdefinierter Anzeigeskalierung.

* &lbrack;UI&rbrack; Vermeiden von dauerhaften Fehlermeldungen in der Benutzeroberfläche

  Fehlermeldungen aus vorherigen Projekten werden jetzt aus der unteren Statusleiste entfernt.

* &lbrack;UI&rbrack; Menü &quot;Speichern&quot; überarbeiten

  Zusätzliche Speicheroptionen sind jetzt in einem Untermenü gruppiert und einige werden aus Konsistenzgründen umbenannt.

* &lbrack;UI&rbrack; Speichern und Exportieren/Freigeben von UI-Layouts

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

* &blbrack;Bedienfeld &quot;Elemente&quot;&blbrack; &quot;Nadel&quot; von bevorzugten Elementen, die oben im Bedienfeld &quot;Elemente&quot; angezeigt werden

  Es wurde eine neue Option zum Klicken mit der rechten Maustaste hinzugefügt, um Elemente zu bibliothekieren, mit der sie oben im Bedienfeld als Favoriten Nadel werden können. Sie können auch alle Ihre bevorzugten Assets über &quot;Gespeicherte Suchen&quot; anzeigen.

* &blbrack;Bedienfeld &quot;Elemente&quot;&blbrack; Elemente löschen, neu laden und umbenennen

  Kontextmenüoptionen zum Löschen, erneuten Laden und Umbenennen von Elementen in der Benutzerbibliothek wurden hinzugefügt. Sie werden direkt aus ihrem Bibliotheksspeicherort auf der Festplatte gelöscht und vom ursprünglichen Speicherort neu geladen. Elemente, die Teil eines Pakets wie .abr oder .sbsar sind, können nicht einzeln bearbeitet werden.

* &lbrack;Farbauswahl&rbrack; Effekt &quot;Füllmethoden für Farbauswahl&quot; definieren.

* &lbrack;Ebenenstapel&rbrack; Füllmethode und Deckkraft auf Filtern anwenden.

* &lbrack;Ebenenstapel&rbrack; Kachelung größer als 128 für Füllebene/Effekte zulassen

* &lbrack;Ebenenstapel&rbrack; Zylinderdeckel für zylindrische Projektion in Füllebene/Wirkung

  Bei der zylindrischen Projektion in den Eigenschaften der Füllebene haben Sie jetzt die Möglichkeit, Zylinderkappen zu entfernen.

* &lbrack;Log&rbrack; Fehlermeldung anzeigen, wenn beim Erstellen eines UV-Kachel-Projekts ein Mesh-Teil im Leerzeichen steht

  Es wurde eine deutlichere Fehlermeldung hinzugefügt, wenn ein UV-Kachel-Projekt nicht erstellt werden kann, da UV-Teile in Leerzeichen gefunden werden.

* &lbrack;Projekt&rbrack; Geben Sie beim Öffnen eines Projekts die Version in der Fehlermeldung &quot;Daten zu aktuell&quot; an.

  Wenn Sie ein Projekt öffnen, das für die Anwendung zu neu ist, wird in der Fehlermeldung jetzt die Version des Projekts angezeigt, damit Sie die richtige Anwendungsversion leichter erkennen können.

* &lbrack;Viewport&rbrack; Mesh von unten beleuchten

  Ein neuer Parameter für die Umgebungsausrichtung wurde unter Anzeigeeinstellungen > Kamera > Umgebungseinstellungen hinzugefügt, um die Umgebungs-Map-Beleuchtung an der Kamera auszurichten, wenn sie auf &quot;Lokal&quot; eingestellt ist.

* &lbrack;Viewport&rbrack; Anzeigen von R, G, B und Alpha im Viewport (Einzelanzeigemodus)

  Unter Anzeigeeinstellungen > Kanaleinstellungen > Kanalanzeige gibt es eine neue Farbkanaleinstellung, mit der nur die R-, G-, B- oder Kanalkomponente eines Viewports im Einzelanzeigemodus angezeigt werden kann.

* &lbrack;Shader&rbrack; Zulassen, dass Benutzerkanäle in Material-Ebenenschattierungen als RGBA festgelegt werden

  Bei der Einstellung der Kanalkonfiguration innerhalb eines Shader für die Kanalschichtung ist es nun möglich, das Textursatz des Materials so festzulegen, dass es vom Standardwert abweicht. Auf diese Weise können Benutzer-Farbkanäle anstelle von Graustufen angefordert werden.

* &lbrack;Export&rbrack; Exportieren von Texturen als SBSAR zulassen

  Beim Exportieren von Texturen über das Fenster Datei > Texturen exportieren kann das Dateiformat SBSAR (Substance Archive) ausgewählt werden, um sie neu zu gruppieren. Der Inhalt des SBSAR richtet sich nach der verwendeten Ausgabevorlage. Das Datenformat kann auch in den Exportvorgaben festgelegt werden. Bei Verwendung einer Hybridkonfiguration (SBSAR + Anderes Format) werden Texturen, die ein SBSAR betreffen, gruppiert, während der Rest parallel exportiert wird.

* &lbrack;Export&rbrack; 16-Bit-Option für EXR Dateiformat gelegt

  Beim Exportieren EXR Textur-Dateien können Sie jetzt im Fenster &quot;Exporteinstellungen&quot; die Texturen 16f Bit (halbe Fließkommazahl) oder 32f Bit (Fließkommazahl) auswählen (sowohl für Exporteinstellungen als auch Exportvorgaben). Alte Projekte und alte Exportvorgaben werden standardmäßig auf 16f Bit gesetzt, um das alte Verhalten widerzuspiegeln.

* &lbrack;Python&rbrack; Ereignis hinzufügen, um zu erfahren, wann Textursatz geändert werden

  Mit dem neuen &quot;substance_painter.event.TextureStateEvent&quot; kann ermittelt werden, ob ein Textursatz entweder aufgrund eines Malen-Strichs, eines hinzugefügten oder eines entfernten Kanals geändert wurde.

* &lbrack;Python&rbrack; Mesh-Map-Ressourcen in den Textursatz-Einstellungen abrufen und festlegen

  Neue Funktionen wurden im Modul &quot;substance_painter.project&quot; hinzugefügt, um Mesh-Map-Ressourcen abzurufen und einzurichten. Diese Funktionen können verwendet werden, um die Mesh-Map zu aktualisieren, auf die in den Textursatz-Einstellungen verwiesen wird.

* &lbrack;Plugins&rbrack; Option zum Abrufen anderer JS-Plug-ins entfernen

  Die Option, JavaScript-Plug-ins abzurufen, wurde entfernt, da sie auf der veralteten Freigabe-Website gehostet wurden.

* &lbrack;Inhalt&rbrack; Neue Roblox-Vorlage hinzufügen und Vorgabe exportieren

  Eine neue Roblox-Projektvorlage &quot;Material Variant&quot; und &quot;Surface Appearance&quot; sowie eine Exportvorgabe wurden hinzugefügt, um den Export von PBR-Texturen nach Roblox zu erleichtern. Auf die Vorlage kann über das Fenster Datei > Neues Projekt zugegriffen werden.

* Substance Engine auf die neueste Version (8.6.3) aktualisieren

* &lbrack;Steam&rbrack; Optimierter Build für Apple Silicon-Chipsatz (Apple M1/M2)

**Fest:**

* Absturz bei Verwendung von 16k exr

* &lbrack;Absturz&rbrack; Strg+Z Nach dem Löschen einer Shader-Instanz

* &lbrack;Iray&rbrack; IoR ist bei einigen Shadern auf 1 blockiert

* &lbrack;Win&rbrack;&lbrack;Baking&rbrack; Einige High-Poly können nicht geladen werden

* &lbrack;Farbmanagement&rbrack; Falscher Farbraumname in der Benutzeroberfläche mit Filtern

* &lbrack;Python&rbrack; Von der Importfunktion zurückgegebene Ressourcenobjekte haben keinen Typ

  Beim Importieren eines Substance-Pakets in Python gab die Funktion das Paket anstelle der Graf zurück. Das Ressourcenmodul stellt nun Funktionen und Parameter bereit, um die Graf eines Substance-Pakets abzurufen.

**Bekannte Probleme:**

* &lbrack;Farbmanagement&rbrack; HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen geklemmte Farben
* &lbrack;Ebenenstapel&rbrack; Eingabequelle nicht pro Ebene gespeichert
* &lbrack;Malen&rbrack; Zeitweiliges Anti-Aliasing verursacht beim Malen in einigen Fällen Artefakte
* &lbrack;Export&rbrack; 2D-Ansicht exportiert zufällig einheitliche Map

### 8.1.3

*(Freigegeben: 25. August 2022*)Zusammenfassung: **Geringfügige Fehlerbehebungsversion**

**Hinzugefügt:**

* Update auf Iray SDK 1.6

**Fest:**

* &lbrack;Shader&rbrack; Absturz mit altem fehlerhaftem Shader
* &blbrack;Material-Ebenen&blbrack; Material können beim erneuten Öffnen eines Projekts verschwinden

**Bekannte Probleme:**

* &lbrack;Farbmanagement&rbrack; HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen geklemmte Farben
* &lbrack;Ebenenstapel&rbrack; Eingabequelle nicht pro Ebene gespeichert
* &lbrack;Absturz&rbrack; Strg+Z Nach dem Löschen einer Shader-Instanz
* &lbrack;Iray&rbrack; IoR ist bei einigen Shadern auf 1 blockiert

### 8.1.2

*(Freigegeben: 19. Juli 2022*)Zusammenfassung: **Geringfügige Fehlerbehebungsversion**

**Hinzugefügt:**

* &lbrack;Automatisch Entpackt&rbrack; Neue Option &quot;Für organische Mesh optimieren&quot; zur Auswahl des Segmentierungsalgorithmus
* &lbrack;Physische Größe&rbrack; Einheitenoptionen in &quot;Neues Projekt&quot; und &quot;Projektkonfiguration&quot; gelegt
* &lbrack;Farbmanagement&rbrack; Verwenden Sie die Monitoranzeige standardmäßig, wenn Sie ACE verwenden
* &lbrack;Farbmanagement&rbrack;&lbrack;Python&rbrack; Berücksichtigung ACE env-var-Vorgabedatei beim Erstellen eines Projekts
* &lbrack;Farbmanagement&rbrack; Zurücksetzen der Farbmanagement-Einstellungen im Fenster &quot;Neues Projekt&quot;, wenn sich die Konfiguration ändert
* &lbrack;Farbmanagement&rbrack; Zugriff auf OCIO deaktivieren, wenn env-var vorhanden ist
* &lbrack;Farbmanagement&rbrack; Sicheres Aktualisieren ACE Einstellungen, wenn kein Parameter mehr vorhanden ist
* Substance Engine auf Version 8.6.0 aktualisieren
* &lbrack;Export&rbrack; Neue GLTF-Exportvorgabe mit Versatz-Unterstützung hinzufügen
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Abrufen von Ressourceninformationen (einschließlich benutzerdefinierter Metadaten)
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Funktion zur Abfrageliste der Mesh-Namen pro Textursatz hinzufügen
* &lbrack;Inhalt&rbrack; Neue Misch- und Exportvorgabe hinzufügen

**Fest:**

* &lbrack;MacOS&rbrack; Absturz beim Starten von Iray in einigen Fällen
* &Klammer;Miniaturen&Klammer; Regal-Miniaturansichten werden nicht richtig geladen
* Mehrere UV-Kanäle werden ignoriert.
* &lbrack;Automatisch Entpackt&rbrack; Unnötige Berechnung bei der Teilung langer Inseln
* &lbrack;Automatisch Entpackt&rbrack; Option zur Vermeidung länglicher Inseln, die nicht berücksichtigt werden
* &lbrack;Automatisch Entpackt&rbrack; Verlust zusätzlicher Daten (Scheitelpunkt-Farben) beim Umpacken von UVs
* &lbrack;UI&rbrack; Horizontale Bildlaufleiste im Eigenschaftenfenster, wenn Farbmanagement aktiviert ist
* &lbrack;Farbmanagement&rbrack; OCIO Konfigurationen fehlen substance_3d_painter_standard_srgb
* &lbrack;Generator&rbrack; Falsche Verwendung von Benutzerdaten &quot;deaktiviert&quot;
* &lbrack;Farbmanagement&rbrack; Die Dropdown-Liste &quot;Nicht kompatibel&quot; im Farbraum sollte nicht anklickbar sein.
* &lbrack;Farbmanagement&rbrack;&lbrack;Shader&rbrack; sRGB override define funktioniert nicht mehr
* &lbrack;Generator&rbrack; Falsche Verwendung von Benutzerdaten &quot;deaktivieren&quot;
* &lbrack;Ebenenstapel&rbrack; Fehlerhafte Vorschauen bei UV-Kacheln-Projekten
* &lbrack;Shader&rbrack; Die API-Dokumentation ist mit den Bent normals nicht vollständig auf dem neuesten Stand.
* &lbrack;Export&rbrack;&lbrack;Interoperabilität&rbrack; Kann nicht mit Sonderzeichen an Stager gesendet werden
* &lbrack;Inhalt&rbrack; Einige Miniaturansichten von Pinselvorgaben sind leer oder zu dunkel

**Bekannte Probleme:**

* &lbrack;Farbmanagement&rbrack; HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen geklemmte Farben
* &lbrack;Ebenenstapel&rbrack; Eingabequellen werden nicht pro Ebene gespeichert
* &lbrack;Absturz&rbrack; Strg+Z Nach dem Löschen einer Shader-Instanz
* &lbrack;Iray&rbrack; IoR ist bei einigen Shadern auf 1 blockiert
* &lbrack;Shader&rbrack; Absturz mit altem fehlerhaftem Shader

### 8.1.1

*(Freigegeben: 28. Juni 2022*)Zusammenfassung: **Hotfix für Nebenversion**

**Hinzugefügt:**

* &lbrack;Ebenenstapel&rbrack; Alt-Klick auf Maske hebt Auswahl von Effekten nicht mehr auf

**Fest:**

* &lbrack;Absturz&rbrack; Öffnen von im Einzelansichtsmodus gespeicherten alten Projekten
* &lbrack;Absturz&rbrack; Generator in Eigenschaften löschen
* &blbrack;Textursatz-Einstellungen&rbrack; Normale/Ambient occlusion-Mischung und Height-zu-Normal-Methoden sind nicht mehr funktionsfähig
* &lbrack;Export&rbrack; Texturen mit Innenabständen exportieren macht schwarze Diffusionen.

**Bekannte Probleme:**

* &lbrack;MacOS&rbrack; Absturz beim Starten von Iray auf Monterey
* &blbrack;Vorschau-Miniatur&blbrack; Vereinfachte Miniaturen werden nicht aktualisiert, wenn ein Anker verwendet wird
* &lbrack;Farbmanagement&rbrack; HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen geklemmte Farben

### 8.1.0

*(Freigegeben: 07. Juni 2022*)Zusammenfassung: **Hauptversion mit ICC-Unterstützung, Material-Skalierung auf der Grundlage von Physische Größe-Daten, neue Baker, Verbesserungen an der FarbPipette und eine Reihe zusätzlicher Inhalte**

**Hinzugefügt:**

* &lbrack;Farbmanagement&rbrack; Unterstützung für ICC-Profile mit Adobe Color Engine hinzufügen (ACE)
* &lbrack;Farbmanagement&rbrack; Unterstützung für &quot;Adobe 98 RGB&quot; als Arbeitsfarbraum für ICC hinzufügen
* &lbrack;Farbmanagement&rbrack; Konfigurieren von ACE/ICC-Einstellungen über eine Konfigurationsdatei zulassen
* &lbrack;Farbmanagement&rbrack; Zulassen, dass lineare Farbwerte im Farbwähler mit dem Legacy-Modus eingegeben werden
* &lbrack;Farbmanagement&rbrack; Festlegen des Farbprofils für die Farbauswahl außerhalb der Benutzeroberfläche zulassen
* &lbrack;Farbmanagement&rbrack; Erinnern Sie sich an den letzten im Viewport ausgewählten Anzeigewert
* &lbrack;Farbmanagement&rbrack;&lbrack;Substance&rbrack; Generatoren/Filter mit dem Farb-Management für die einwandfreie Funktion sorgen
* &lbrack;Farbmanagement&rbrack;&lbrack;Substance&rbrack; Neue Schlüsselwörter für die Farbraumüberschreibung hinzufügen $working und $standardsrgb
* &lbrack;Physische Größe&rbrack;&lbrack;Engine&rbrack; Informationen zur Physische Größe aus dem Mesh extrahieren
* &lbrack;Physische Größe&rbrack;&lbrack;Engine&rbrack; Physische Größe Berechnung
* &lbrack;Physische Größe&rbrack; Leg von Optionen für die Verwendung von Physische Größe in der Benutzeroberfläche
* &lbrack;Physische Größe&rbrack; Visuelle Helfer zum Viewport hinzufügen
* &blbrack;Baking&rbrack; Height-Baker hinzufügen
* &blbrack;Baking&rbrack; Bent normals-Baker hinzufügen
* &blbrack;Baking&rbrack; Deckkraft-Baker hinzufügen
* &lbrack;Pipette&rbrack; Neue Farbvorschau mit Pipette neben der Maus und Farb-Management
* &lbrack;Pipette&rbrack; Das Bedienfeld &quot;Farbwähler&quot; wird wieder an der letzten Position angezeigt, wenn es erneut geöffnet wird
* &lbrack;Pipette&rbrack; Ein neues Symbol für die Material-Auswahl
* &lbrack;Pipette&rbrack; Farb-Management der Kanalvorschau des Farbwählers
* &lbrack;Pipette&rbrack; Hinzufügen von Click-to-Select-Funktionen zur Pipette
* &lbrack;Pipette&rbrack; Kanalauswahl aktiviert nicht aktive Materialien nicht mehr
* &lbrack;Pipette&rbrack; Pipette mit einem Tastaturbefehl verwenden
* &lbrack;Pipette&rbrack; Die Pipette nimmt ggf. den entsprechenden Kanal auf.
* &lbrack;Pipette&rbrack; Wenn Sie den Farbwählermodus aufrufen, werden alle Tastaturbefehle deaktiviert
* &lbrack;Pipette&rbrack; Entfernen der automatischen Auswahl des Hexadezimalfelds
* &lbrack;Pipette&rbrack; Schließen Sie das Bedienfeld nicht, wenn Sie die Material-Auswahl verwenden
* &lbrack;Pipette&rbrack; Neuer deaktivierter Status, wenn der Kanal nicht zur Auswahl verfügbar ist
* &lbrack;Export&rbrack; Tangente-Attribut zum glTF-Export hinzufügen
* Substance Engine auf Version 8.4 aktualisieren
* Update Auto Entpack auf 0.9.0
* Update auf Qt 5.15.8
* Update auf Python 3.9
* &lbrack;Shader&rbrack; Unterstützung für Bent normals-Schattierung hinzufügen
* &lbrack;MacOS&rbrack; Unterstützung von 3DConnection SpaceMouse
* &lbrack;Python&rbrack; Dokumentieren der in der API verwendeten Python-Version
* &lbrack;Inhalt&rbrack; 6 neue 3D-Rauschen mit 105 Vorgaben hinzufügen
* &lbrack;Inhalt&rbrack; 20 neue Schmutz-Maps und 2 Stofffaltenmuster
* &lbrack;Inhalt&rbrack; Exportvoreinstellung &quot;Mesh-Map&quot; aktualisieren, um neue Baker zu verwenden
* &lbrack;Inhalt&rbrack; Die Steigung des Weichzeichners und der Verkrümmungsfilter hängen von der Auflösung des Textursatzes ab
* &lbrack;Inhalt&rbrack; Beispielprojekte aktualisieren, um die 3 neuen Baker zu verwenden

**Fest:**

* &lbrack;glTF&rbrack; glTF mit Sonderzeichen kann nicht geöffnet werden
* &lbrack;Engine&rbrack; Artefakte mit deaktivierter Anisotropie und SVT
* &lbrack;MacOS&rbrack;&lbrack;M1&rbrack; Intelligente Material werden nicht korrekt angezeigt
* &lbrack;Mesh-Verarbeitung&rbrack; Mesh können nicht aus Modeler importiert werden
* &lbrack;UI&rbrack; Horizontale Bildlaufleiste in neuem Projektfenster mit aktiviertem Farbmanagement
* &lbrack;Farbmanagement&rbrack; Im Farbwähler fehlt bei einigen OCIO der Arbeitsfarbraumwert
* &lbrack;Farbmanagement&rbrack; Die Pinselvorschau im Viewport ist nicht farbverwaltet
* &lbrack;SpaceMouse&rbrack; Pivot wird nicht sofort mit Fokusänderung aktualisiert und manchmal außerhalb des Modells
* &lbrack;Export&rbrack;&lbrack;USD&rbrack; Exportierte USD haben eine falsche Struktur
* &lbrack;USD&rbrack; Ambient occlusion-Problem beim Exportieren
* &lbrack;Inhalt&rbrack; Mesh der Miniaturansicht an das Vorschaukugel-Beispielprojekt anpassen

**Bekannte Probleme:**

* Texturen mit Innenabständen exportieren macht schwarze Diffusionen.
* Normale/Ambient occlusion-Mischung ist defekt
* &lbrack;MacOS&rbrack; Absturz beim Starten von Iray in seltenen Fällen
* &blbrack;Vorschau-Miniatur&blbrack; Vereinfachte Miniaturen werden nicht aktualisiert, wenn ein Anker verwendet wird
* &lbrack;Farbmanagement&rbrack; HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen geklemmte Farben

## Version 7

### 7.4.3

*(Freigegeben: 11. April 2022*)Zusammenfassung: **Bugfix mit Unterstützung von 3D-Verbindung SpaceMouse im 2D-Viewport**

**Hinzugefügt:**

* &lbrack;SpaceMouse&rbrack; Unterstützung von 3DConnection SpaceMouse im 2D-Viewport

**Fest:**

* &Klammer;Farbwähler&Klammer; Schreibzugriff im Hexadezimalfeld nicht möglich
* &lbrack;Farbmanagement&rbrack; Im Projektion-Modus verwendete Ressourcen werden in der Überlagerung nicht farbverwaltet
* &lbrack;Farbmanagement&rbrack; Fehler werden nicht im Protokoll gemeldet.
* &lbrack;SpaceMouse&rbrack; Generische Fehlermeldung entfernen, wenn der Benutzer keine SpaceMouse hat
* &lbrack;SpaceMouse&rbrack; Beim Laden eines Projekts ist der Drehpunkt immer ausgeblendet
* &lbrack;Baker&rbrack; Die Einstellung &quot;Durchschnittliche Normale&quot; hat keine Auswirkungen auf UV-Kachel-Projekte
* &lbrack;UV-Kachel&rbrack; Inaktive Überlagerungen von UV-Kacheln verschwinden beim erneuten Laden von Mesh mit verschiedenen Kacheln
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Remote-Skripterstellung ist fehlerhaft
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Mehrere Kanäle können nicht von der API abgefragt werden und es löst einen Fehler aus
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Absturz bei der Verwendung des ProjectEditionEntered-Ereignisses
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Absturz beim Aufruf von get_active_Stapel()

**Bekannte Probleme:**

* 3D-Verbindung SpaceMouse wird auf MacOS nicht unterstützt
* &lbrack;UI&rbrack; Horizontale Bildlaufleiste mit Farbmanagement, die in einigen Fällen in einem neuen Projektfenster angezeigt wird
* &lbrack;Mac M1&rbrack; Intelligente Material werden nicht korrekt angezeigt

### 7.4.2

*(Freigegeben: 08. März 2022*)Zusammenfassung: **Bugfix mit Unterstützung von Verbesserungen für 3D-Verbindung, SpaceMouse und Farbmanagement (OCIO)**

**Hinzugefügt:**

* &lbrack;SpaceMouse&rbrack;&lbrack;Windows&rbrack; Unterstützung der 3D-Verbindung SpaceMouse im 3D-Viewport für die Navigation
* &lbrack;SpaceMouse&rbrack;&lbrack;Windows&rbrack; Grundlegende Tastaturbefehle/Tasten für Pro- und Enterprise SpaceMouse-Modelle im 3D-Viewport
* &lbrack;SpaceMouse&rbrack;&lbrack;Windows&rbrack; Dediziertes Drehmittensymbol im 3D-Viewport
* &lbrack;Farbmanagement&rbrack; Rollen aus OCIO Konfiguration verwenden, um Standardeinstellungen zu ändern
* &lbrack;Farbmanagement&rbrack; Farb-Management des Eigenschaftenfensters für Farb-Widgets
* &lbrack;Farbmanagement&rbrack; Farb-Management des Eigenschaftenfensters für die Vorschau des Materials
* &lbrack;Farbmanagement&rbrack; Farbfelder in der Farbauswahl verwalten
* &lbrack;Farbmanagement&rbrack; Fügen Sie eine Einstellung hinzu, um den standardmäßigen sRGB-Farbraum zu definieren
* &lbrack;Farbmanagement&rbrack; Hinzufügen des sRGB-Standardfarbraums aus OCIO Konfiguration in der Farbwähler-Anzeigeliste
* &lbrack;Farbmanagement&rbrack; Verbesserungen für das Menü zum Überschreiben des Farbraums
* &lbrack;Farbmanagement&rbrack; Überschreiben des Umgebungs-Map-Farbraums in den Anzeigeeinstellungen zulassen
* &lbrack;Farbmanagement&rbrack; Farbwähler-Verläufe basierend auf aktueller Anzeige zeichnen
* &lbrack;Farbmanagement&rbrack; Standardmäßig HDR im Farbeditor beschränkt
* &lbrack;Farbmanagement&rbrack; Passthrough (keinen Farbraum) für Filter im Legacy-Modus verwenden
* &lbrack;Farbmanagement&rbrack; Anzeige von Farbverläufen im Farbeditor auf &lbrack;0-1&rbrack; beschränken Spanne
* &lbrack;Farbmanagement&rbrack; Anzeigeselektor in der Farbauswahl im Legacy-Modus ausblenden
* &lbrack;Farbmanagement&rbrack; Hex-Code für Farbwähler immer im sRGB-Farbraum
* &lbrack;Farbmanagement&rbrack; Deaktivieren der Farbauswahl-Dropdown-Liste für Datenkanäle
* &lbrack;Optimierung&rbrack; Mit &quot;Verkrümmen-Raster&quot; werden nur überdeckte UV-Kacheln neu berechnet
* &lbrack;Export&rbrack; Exportieren von UV-Kachel-Projekten für Sketchfab, USD und glTF zulassen
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Ändern der Tonzuordnungsfunktion zulassen

**Fest:**

* &lbrack;Sketchfab&rbrack; Durch die Aktualisierung des vorhandenen Modells wird am Ende ein neues Modell erstellt.
* &lbrack;Sketchfab&rbrack; Absturz bei der Suche nach einem zuvor aktualisierten Modell
* Absturz beim Exportieren nach USD
* Absturz beim Erstellen einer neuen Shader-Instanz in der Geometriemaske oder beim Ausblenden der Geometrie
* &lbrack;Elementfenster importieren&rbrack; Absturz beim Ändern des Typs von importierten Ressourcen
* Normale Mesh-Map werden bei Verwendung in Ebenenstapel invertiert
* &lbrack;Substance&rbrack; Der Mischmodus für Benutzerdaten wird nicht berücksichtigt.
* &lbrack;Farbmanagement&rbrack; Bitmaps mit einem Farbraum im Dateinamen werden als UV-Kachel importiert
* &lbrack;Farbmanagement&rbrack; Farbverwaltete Ausgaben von Substance Graf befinden sich im falschen Farbraum
* &lbrack;Farbmanagement&rbrack; Falsche Farbe mit dem Polygon-Füllwerkzeug
* &lbrack;Farbmanagement&rbrack; ACE Tonemapper wird im Solomodus auf Kanäle angewendet
* &lbrack;Farbmanagement&rbrack; Die Kugelbeleuchtung der Werkzeugvorschau ist nicht farbverwaltet
* &lbrack;Farbmanagement&rbrack;&lbrack;Export&rbrack; Konvertierte Karten werden falsch konvertiert.
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack;&lbrack;Farbmanagement&rbrack; Projekte, die mit einer Vorlage und OCIO Umgebungsvariablen erstellt wurden, befinden sich im Modus &quot;Veraltet&quot;
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Die JavaScript-Evaluierungsfunktion kann beim Start nicht verwendet werden.
* &lbrack;3D Adobe Offer&rbrack; Painter kann nicht gestartet werden, wenn Regionaleinstellungen mit Sprachen verwendet werden, die nicht standardmäßig unterstützt werden

**Bekannte Probleme:**

* 3D-Verbindung SpaceMouse wird auf MacOS nicht unterstützt
* &lbrack;UI&rbrack; Horizontale Bildlaufleiste mit Farbmanagement, die in einigen Fällen in einem neuen Projektfenster angezeigt wird
* &lbrack;Baker&rbrack; Die Einstellung &quot;Durchschnittliche Normale&quot; hat keine Auswirkungen auf UV-Kachel-Projekte
* &lbrack;Mac M1&rbrack; Intelligente Material werden nicht korrekt angezeigt
* &lbrack;Farbmanagement&rbrack; Im Projektion-Modus verwendete Ressourcen werden in der Überlagerung nicht farbverwaltet
* &Klammer;Farbwähler&Klammer; Schreibzugriff im Hexadezimalfeld nicht möglich

### 7.4.1

*(Freigegeben: 14. Dezember 2021*)Zusammenfassung: **Bugfix mit Farbmanagement-Verbesserungen**

**Hinzugefügt:**

* &lbrack;Farbmanagement&rbrack; Verwenden der Datenrolle in exportierten Dateinamen
* &lbrack;Farbmanagement&rbrack; Erweitern Sie den Abschnitt Farbmanagement standardmäßig, wenn OCIO in den Fenstern für neue Projekt- und Projekteinstellungen ausgewählt ist.
* &lbrack;Farbmanagement&rbrack; ACE Tongemapper im Legacy-Modus hinzufügen
* &lbrack;Farbmanagement&rbrack; Standardkonfigurationseinstellungen anpassen
* &lbrack;Farbmanagement&rbrack;&lbrack;Export&rbrack; $colorSpace in Dateinamen für Datenkanäle füllen
* &lbrack;Export&rbrack; UV-Kachel-Projekt in Stager exportieren
* &lbrack;Interoperabilität&rbrack; Nicht verfügbar für Steam- und Substance-Editionen
* &lbrack;Interoperabilität&rbrack; Senden eines UV-Kachel-Projekts an Stager zulassen

**Fest:**

* &lbrack;MacOS&rbrack;&lbrack;Absturz&rbrack; Painter beginnt nicht mit Catalina
* &lbrack;Farbmanagement&rbrack;&lbrack;Absturz&rbrack; Zufälliger Absturz bei der Wiedergabe mit Datentyp/Farbmanagement auf Benutzerkanal
* &lbrack;Farbmanagement&rbrack; Ressourcen, die als Graustufen in der Maskenanzeige verwendet werden, zeigen das neue Menü den Farbraum an
* &lbrack;Farbmanagement&rbrack; Benutzerkanal ist im Viewport im Legacy-Modus + Solo-Ansicht dunkler
* &lbrack;Farbmanagement&rbrack; Env-Map ist immer linear, wenn sie in iRay verwendet wird
* &lbrack;Farbmanagement&rbrack; Die Farbauswahl wählt im Legacy-Modus nicht den richtigen Wert für den Datenkanal aus
* &lbrack;Farbmanagement&rbrack; Farbwähler in einer Substance im Legacy-Modus funktioniert nicht
* &lbrack;Farbmanagement&rbrack; Wenn Sie im Viewport zwischen den Einzelkanalansichten wechseln, wird bei Verwendung des Dropdown-Menüs der richtige Farbraum angezeigt
* &lbrack;Farbmanagement&rbrack; Beim Export wird die falsche Konvertierung auf farbverwalteten Benutzerkanälen im Legacy-Modus angewendet.
* In der Einzelansichtsmaske erstellte Konturen werden beim Zurückwechseln zur Material-Ansicht nicht angezeigt
* &lbrack;Export&rbrack; Konvertierte Maps werden nicht als farbverwaltete Kanäle exportiert
* &lbrack;Textursatz&rbrack; QuickInfo mit dem ursprünglichen Namen fehlt auf umbenannten Benutzerkanälen
* &lbrack;Steam&rbrack; Dateien fehlen beim Überprüfen der Dateiintegrität mit Steam

**Bekannte Probleme:**

* &lbrack;Mac M1&rbrack; Intelligente Material werden nicht korrekt angezeigt

### 7.4.0

*(Freigegeben: 24. November 2021*)Zusammenfassung: **Hauptversion. Einführung der ersten Farbmanagement-Version, Abdocken der 2D- oder 3D-Ansicht, neue Option für den automatischen entpack von UV zum Vermeiden von länglichen Inseln, Aufruf von JavaScript-Funktionen von der Python-API und neuer Inhalt**

**Hinzugefügt:**

* &lbrack;Farbmanagement&rbrack; Unterstützung des Farbmanagements OpenColorIO Version 2
* &lbrack;Farbmanagement&rbrack; Hinzufügen von Farbmanagementeinstellungen zu Projekteinstellungen
* &lbrack;Farbmanagement&rbrack; Warnfenster zu Farbmanagement-Konfigurationsänderungen beim Öffnen eines Projekts
* &lbrack;Farbmanagement&rbrack; Fehlermeldung anzeigen, wenn eine ungültige OCIO Konfigurationsdatei ausgewählt ist
* &lbrack;Farbmanagement&rbrack; Überschreiben der Konfiguration mit OCIO Umgebungsvariable zulassen
* &lbrack;Farbmanagement&rbrack; Mehrere OCIO sind standardmäßig in die Anwendung integriert.
* &lbrack;Farbmanagement&rbrack; Extrahieren des Farbraumnamens aus dem importierten Bitmap-Dateinamen
* &lbrack;Farbmanagement&rbrack; Überschreiben des Farbraums mit einem Farbraum aus der Konfiguration im Eigenschaftenfenster zulassen
* &lbrack;Farbmanagement&rbrack; Hinzufügen von Farbmanagementoptionen in den Textursatz-Einstellungen
* &lbrack;Farbmanagement&rbrack;&lbrack;Viewport&rbrack; Erlaubt das separate Farbmanagement für 2D- und 3D-Ansichten.
* &lbrack;Farbmanagement&rbrack; Umgebungs-Map laden und in den Arbeitsfarbraum konvertieren
* &lbrack;Farbmanagement&rbrack; Anpassen des Farbwählers und des Editors mit dem aktuellen Farbraum
* &lbrack;Farbmanagement&rbrack; Auswahl des transformieren Farbraums für die Anzeige im Viewport über ein neues Dropdown-Menü zulassen
* &lbrack;Farbmanagement&rbrack; Anzeige mit Iray-Rendering-Ergebnissen transformieren anwenden
* &lbrack;Farbmanagement&rbrack; Exportieren von Texturen mit unterschiedlichen Farbräumen
* &lbrack;Farbmanagement&rbrack;&lbrack;Python&rbrack; Anwenden von Farbmanagementeinstellungen aus der Umgebungsvariablen (OCIO) auf neue Projekte
* &lbrack;Viewport&rbrack; Abdocken des 2D- oder 3D-Viewports zulassen
* &lbrack;Automatisch Entpackt&rbrack; Neue Option zur Vermeidung länglicher Inseln
* &lbrack;Skripterstellung Python&rbrack; Aufrufen von JavaScript-Funktionen über die Python-API
* &lbrack;Neues Projektfenster&rbrack; Reduzieren des Abschnitts &quot;Importierte Karten&quot;
* &lbrack;Projektion&rbrack;&lbrack;Verkrümmen&rbrack; Option zum Ausblenden von Normalen in den Verkrümmen-Einstellungen
* &lbrack;Inhalt&rbrack; 11 neue Schmutz Maps
* &lbrack;Inhalt&rbrack; 8 neue Werkzeugvorgaben (Reißverschluss, Spannschnur, Glitter)
* &lbrack;Inhalt&rbrack; 8 neue Materialien (Narbe, Hosentasche, ...)
* &lbrack;Inhalt&rbrack; 1 neuer Generator (aufblasen Schrumpfwarp)

**Bekannte Probleme:**

* &lbrack;Mac M1&rbrack; Intelligente Material werden nicht korrekt angezeigt
* &lbrack;Farbmanagement&rbrack;&lbrack;Absturz&rbrack; Zufälliger Absturz bei der Wiedergabe mit Datentyp/Farbmanagement auf Benutzerkanal
* &lbrack;Farbmanagement&rbrack; Die Farbauswahl wählt im Legacy-Modus nicht den richtigen Wert für den Datenkanal aus
* &lbrack;Farbmanagement&rbrack;&lbrack;Iray&rbrack; Speichern des Renderings auf EXR oder TIFF, während das Farbmanagement im Viewport aktiviert ist, wird immer linear gespeichert
* &lbrack;Farbmanagement&rbrack; Ressourcen, die als Graustufen in einer Maske verwendet werden, zeigen das falsche Menü &quot;Farbraum&quot; an
* &lbrack;Farbmanagement&rbrack;&lbrack;Iray&rbrack; Env-Map ist immer linear, wenn sie in Iray verwendet wird
* &lbrack;Farbmanagement&rbrack;&lbrack;Export&rbrack; Konvertierte Karten werden nicht als Farbmanagement-Kanäle exportiert
* &lbrack;Farbmanagement&rbrack;&lbrack;Export&rbrack; Der Export ignoriert, wenn der Benutzerkanal farbverwaltet ist oder nicht im Legacy-Modus ausgeführt wird

### 7.3.1

*(Freigegeben: 24. November 2021*)Zusammenfassung: **Bugfix**

**Hinzugefügt:**

* &lbrack;Projektion&rbrack; Skalierung sollte nur im Objektbereich funktionieren

**Fest:**

* &lbrack;Mac M1&rbrack; Material-Ebene funktioniert nicht
* &lbrack;Mac M1&rbrack;&lbrack;Projektion&rbrack; Verkrümmen funktioniert nicht
* Micro-Details werden nicht richtig angezeigt
* &lbrack;Projektion&rbrack;&lbrack;Absturz&rbrack; Wechseln in den Verzerrungsmodus mit einer Ebene, die mit einer früheren Version erstellt wurde
* &lbrack;Projektion&rbrack;&lbrack;Verkrümmen&rbrack; Spiegeln funktioniert nicht, wenn die Transformation auf Welt-Raum eingestellt ist
* &lbrack;Projektion&rbrack;&lbrack;Verkrümmen&rbrack; Die Option &quot;Teilen&quot; bleibt ausgewählt, nachdem das Teilen abgeschlossen ist
* &lbrack;Projektion&rbrack;&lbrack;UV&rbrack; Drehpunkt wird beim Spiegeln der Projektion zurückgesetzt
* &lbrack;Filter&rbrack; Baking Die Beleuchtungsumgebung ändert sich beim erneuten Laden oder Ändern eines Parameters
* &lbrack;Interoperabilität&rbrack; Nicht verfügbar für Steam- und Substance-Editionen
* &lbrack;Interoperabilität&rbrack; Die Schaltfläche &quot;3D-Assets im Marketplace durchsuchen&quot; sollte immer CCD auf der Registerkarte &quot;Stock &amp; Marketplace 3D&quot; öffnen.

**Bekannte Probleme:**

* &lbrack;Mac M1&rbrack; Intelligente Material werden nicht korrekt angezeigt

### 7.3.0

*(Freigegeben: 13. Oktober 2021*)Zusammenfassung: **Hauptversion. Es enthält eine neue 3D-Verkrümmungsfunktion, eine neue zylindrische Projektion, Projektionen am Farbwähler, neue Funktionen in der Python-API und Fehlerbehebungen**

**Hinzugefügt:**

* &lbrack;Projektion&rbrack;&lbrack;Verkrümmen&rbrack; 3D-Verkrümmung als neue Projektion gelegt
* &lbrack;Projektion&rbrack;&lbrack;Verkrümmen&rbrack; Aufklebermodus für Alphas, Texturen und Prozedurale per Drag &amp; Drop im Viewport zulassen
* &lbrack;Projektion&rbrack;&lbrack;Verkrümmen&rbrack; Verkrümmen-Projektion mit Aufkleber-Tastaturbefehl (ALT) verwenden
* &lbrack;Projektion&rbrack;&lbrack;Verkrümmen&rbrack;&lbrack;Werkzeugleiste&rbrack; Transformieren der Verformung als Ganzes oder pro Scheitelpunkt
* &lbrack;Projektion&rbrack;&lbrack;Verkrümmen&rbrack;&lbrack;Werkzeugleiste&rbrack; Raster-Punkte mit geteilter Verkrümmung in Querrichtung, horizontal oder vertikal hinzufügen
* &lbrack;Projektion&rbrack;&lbrack;Verkrümmen&rbrack;&lbrack;Werkzeugleiste&rbrack; Dediziertes Menü zum Zurücksetzen von Aktionen
* &lbrack;Projektion&rbrack;&lbrack;Verkrümmen&rbrack;&lbrack;Werkzeugleiste&rbrack; Option zum automatischen Anpassen der Tangenten beim Verschieben von Punkten
* &lbrack;Projektion&rbrack;&lbrack;Verkrümmen&rbrack;&lbrack;Werkzeugleiste&rbrack; Spezielles Menü für die Raster-Edition (Größe, Reset, Farbe und Handle-Größe)
* &lbrack;Projektion&rbrack;&lbrack;Verkrümmen&rbrack; Neuer Tastatur-Tastaturbefehl zum Schalten des Warp-Editionsmodus für ganze Scheitelpunkt (UMSCHALT+V)
* &lbrack;Projektion&rbrack;&lbrack;Verkrümmen&rbrack; Klicken + Strg ermöglicht den Wechsel zwischen Oberflächenwerkzeug und anderen Werkzeugen
* &lbrack;Projektion&rbrack;&lbrack;Zylindrisch&rbrack; Leg der zylindrischen Projektion
* &lbrack;Projektion&rbrack;&lbrack;Werkzeugleiste&rbrack; Einstellungen für Manipulator gruppieren (Größe, Raster, Winkelschritte)
* &Klammer;Farbwähler&Klammer; Neue Benutzeroberfläche für den Farbwähler
* &Klammer;Farbwähler&Klammer; sRGB-Werte in Farbwähler-Widgets verwenden
* &Klammer;Farbwähler&Klammer; Farbfelder speichern und löschen
* &Klammer;Farbwähler&Klammer; Pipette zugänglich von Farbe und normalen Slots
* &Klammer;Farbwähler&Klammer; Bearbeiten dynamischer Farben zwischen 0 und 255 Werten zulassen
* &Klammer;Farbwähler&Klammer; Einheitlicher HSV-/RGB-Status in der gesamten App
* &Klammer;Farbwähler&Klammer; Das Fenster &quot;Farbwähler&quot; ist halbpersistent.
* &Klammer;Farbwähler&Klammer; Durch Drücken von Esc wird das Farbauswahlfenster geschlossen.
* Leistungsverbesserung für UI-Interaktion und beim Malen
* &lbrack;Engine&rbrack; Update auf die neue Substance Engine-Version (8.3.0)
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Erlaubt das erneute Laden des Meshs des aktuellen Projekts
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Aktualisieren von Ressourcen in Projekten zulassen
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Festlegen und Abfragen der Auflösung von UV-Kacheln zulassen
* &lbrack;Interoperabilität&rbrack; Nicht verfügbar für Steam- und Substance-Editionen
* &lbrack;Interoperabilität&rbrack; Mehrere Ressourcen von Bridge erhalten

**Fest:**

* Der Farbwähler zeigt nicht die richtige Farbe an
* &blbrack;Baking&rbrack; Textursatz-Listen sind nicht korrekt angeordnet
* &lbrack;FBX import&rbrack; 3ds Max-Gruppen-Pivot-Transformationen werden nicht berücksichtigt
* &lbrack;Substance Engine&rbrack; Absturz beim Importieren von beschädigtem SBSAR
* &lbrack;MacOS&rbrack; Projektkonfigurationsoption in verschiedenen Sprachen ist nicht vorhanden
* Automatische Speicherung kann Painter während langer Prozesse einfrieren

**Bekannte Probleme:**

* &lbrack;Projektion&rbrack;&lbrack;Verkrümmen&rbrack; Die Option &quot;Teilen&quot; bleibt ausgewählt, nachdem das Teilen abgeschlossen ist
* &lbrack;Projektion&rbrack;&lbrack;Verkrümmen&rbrack; Spiegeln funktioniert nicht, wenn die Transformation auf Welt-Raum eingestellt ist
* &lbrack;Projektion&rbrack;&lbrack;Verkrümmen&rbrack; Artefaktlinien zwischen Patches in seltenen Fällen
* &lbrack;Projektion&rbrack;&lbrack;UV&rbrack; Drehpunkt wird beim Spiegeln der Projektion zurückgesetzt
* &lbrack;Mac M1&rbrack; Intelligente Material werden nicht korrekt angezeigt
* &lbrack;M1&rbrack;&lbrack;Regression&rbrack; Material-Ebene funktioniert nicht

### 7.2.3

*(Freigegeben: 24. August 2021*)Zusammenfassung: **Nebenversion, Bugfix**

**Hinzugefügt:**

* &lbrack;Libraries&rbrack; Hinzufügen einer Möglichkeit zum Ausschließen unerwünschter Dateien vom Durchsuchen

**Fest:**

* &lbrack;Win&rbrack; Mehrere Bildschirme und Schlafprobleme
* &lbrack;MacOS&rbrack;&lbrack;Absturz&rbrack; Wechseln des Shader bei Verwendung von Effekten
* &lbrack;Viewport&rbrack; Im Vollvorschaumodus wird der Pinselcursor nicht mehr ohne Alpha angezeigt
* &lbrack;UI&rbrack; Winkel-Widget wechselt in die falsche Richtung
* &lbrack;Ebenenstapel&rbrack; Viele Unterordner erstellen sehr lange Einfrieren
* &lbrack;Iray&rbrack; Verschiedene Ansichten in Iray und OpenGL: Sichtbar, wenn nicht funktionierend
* &lbrack;Iray&rbrack; Brechungsindex wird nicht berücksichtigt und erscheint nicht in den mdl-Eigenschaften
* &lbrack;JavaScript&rbrack; ShowExportDialog() gibt niemals true zurück.
* Kann keine MTL aus Adobe Stock lesen

### 7.2.2

*(Freigegeben: 27. Juli 2021*)Zusammenfassung: **Nebenversion, Bugfix**

**Hinzugefügt:**

* Aktualisieren Sie die Version der AMD-Treiberanforderungen

**Fest:**

* &lbrack;Mac M1&rbrack; Falsche Speichererkennung
* &lbrack;Export&rbrack; Sehr lange Pfade werden nicht richtig angezeigt

**Bekannte Probleme:**

* &lbrack;Inhalt&rbrack; Veraltete Shader der Beispiele

### 7.2.1

*(Freigegeben: 02. Juli 2021*)Zusammenfassung: **Nebenversion, Hotfix**

**Hinzugefügt:**

* &lbrack;Interop&rbrack; Fügen Sie einen QuickInfo hinzu, um zu informieren, dass das Senden von UV-Kachel-Projekten an Stager noch nicht unterstützt wird.
* &lbrack;Plugin&rbrack;&lbrack;UI&rbrack; Aktualisierung des Livelink-Symbols

**Fest:**

* &lbrack;Nvidia&rbrack; Treiberversion ab 30 gilt als veraltet
* &lbrack;Libraries&rbrack; Der Status des Bedienfelds &quot;Elemente&quot; wird nur gespeichert, wenn ein Projekt geöffnet ist
* &lbrack;Libraries&rbrack; Neue gespeicherte Suche behält Schlüsselwort aus alter gespeicherter Suche bei
* &lbrack;Baker&rbrack;&lbrack;UVTiles&rbrack; ID-Map pro MeshID berücksichtigen ebenfalls UV-Kacheln
* &lbrack;Export&rbrack; gLTF-Dateien importieren keine Scheitelpunkt-Farbe
* &lbrack;Iray&rbrack; Einige QuickInfos fehlen
* &lbrack;Interop&rbrack; An Stager senden ist nicht immer deaktiviert, wenn Stager nicht erkannt wird
* &lbrack;Ressourcenaktualisierung&rbrack; Photoshop-Pinselmaker kann nicht aktualisiert werden
* &lbrack;Inhalt&rbrack; Generator für Glasfaserkantenverschleiß ist defekt

### 7.2.0

*(Freigegeben: 23. Juni 2021*)Zusammenfassung: **Die Hauptversion bietet eine Aktualisierung des Bedienfelds &quot;Elemente&quot;, einen neuen Shader mit Zugriff auf neue Kanäle und Parameter, eine allgemeine Aktualisierung der Benutzeroberfläche, einige dringend angeforderte Leistungsverbesserungen, erweiterte Sprachunterstützung und vieles mehr!**

**Hinzugefügt:**

* &lbrack;Libraries&rbrack; Neues Bedienfeld &quot;Element&quot;, um das Regal zu ersetzen
* &lbrack;Libraries&rbrack;&lbrack;UI&rbrack; Neues Bedienfeld &quot;Elemente&quot;
* &lbrack;Libraries&rbrack;&lbrack;UI&rbrack; Ändern der standardmäßigen Ausrichtung und Benutzeroberfläche des Bedienfelds &quot;Elemente&quot;
* &lbrack;Libraries&rbrack;&lbrack;UI&rbrack; Listenansichtsoption in Bibliothek einfügen
* &lbrack;Libraries&rbrack;&lbrack;UI&rbrack; Neue Breadcrumbs-Navigation im Bedienfeld &quot;Elemente&quot;
* &lbrack;Libraries&rbrack;&lbrack;UI&rbrack; Beim Auswählen einer gespeicherten Suche &quot;Alle Bibliotheken&quot; auswählen
* &lbrack;Libraries&rbrack;&lbrack;UI&rbrack; Wählen Sie &quot;Alle Bibliotheken&quot;, wenn die Auswahl aller Ordner aufgehoben wird.
* &lbrack;Libraries&rbrack;&lbrack;UI&rbrack; Neues Tag für Partikel-Pinsel
* &lbrack;Libraries&rbrack;&lbrack;UI&rbrack; &quot;Regal&quot; durch &quot;Alle Bibliotheken&quot; in der gesamten App ersetzt
* &lbrack;Libraries&rbrack;&lbrack;UI&rbrack; Ausblenden leerer Ordner zulassen
* &lbrack;Libraries&rbrack;&lbrack;UI&rbrack; Standardbenutzerbibliothek sollte sichtbar sein, auch wenn sie leer ist
* &lbrack;Libraries&rbrack;&lbrack;UI&rbrack; Neue Filterung-Methode über Symbole des Elementtyps
* &lbrack;Libraries&rbrack; Tastaturbefehl &quot;STRG&quot;, um mehrere Elementtypen auszuwählen
* &lbrack;Libraries&rbrack; Neue Umgebungsvariable zur Steuerung des Speicherbudgets für die Elementvorschau
* &lbrack;Libraries&rbrack;&lbrack;Content&rbrack; Neue Umgebungs-Map
* &lbrack;Libraries&rbrack;&lbrack;Content&rbrack;&lbrack;UI&rbrack; Versatz auf Standard-Materialien rendern
* &lbrack;Libraries&rbrack;&lbrack;Content&rbrack; Adobe Standard Material-Shader (ASM) als Standard für die Vorschauerstellung festlegen
* &lbrack;Libraries&rbrack;&lbrack;Content&rbrack;&lbrack;ASM&rbrack; Neue Projektvorlagen für neuen ASM-Shader
* &lbrack;Libraries&rbrack;&lbrack;Thumbnail&rbrack; Verwenden der neuen Studio 6-Umgebungs-Map
* &lbrack;Libraries&rbrack;&lbrack;Thumbnail&rbrack; Miniaturansicht in Ressource lesen, anstatt sie zu generieren
* &lbrack;Libraries&rbrack;&lbrack;Thumbnail&rbrack; Versatz zur Miniaturbildgenerierung hinzufügen
* &blbrack;Textursatz-Einstellungen&rbrack;
* &lbrack;Textursatz-Einstellungen&rbrack;&lbrack;UI&rbrack; Leg eines neuen Heights zur normalen Konvertierungsmethode
* &lbrack;Textursatz-Einstellungen&rbrack;&lbrack;UI&rbrack; Überarbeitung der Organisation der Benutzeroberfläche der Kanäle
* &blbrack;Textursatz-Einstellungen&rbrack; Obergrenze für Benutzerkanäle auf 16 Kanäle erhöht
* &lbrack;Textursatz-Einstellungen&rbrack;&lbrack;UI&rbrack; Geben Sie an, welche Kanäle mit dem aktuell ausgewählten Shader kompatibel sind.
* &lbrack;Shader&rbrack;&lbrack;ASM&rbrack; Neuer Adobe Standard Material-Shader
* &lbrack;Shader&rbrack;&lbrack;ASM&rbrack; Zusätzliche Unterstützung für Anisotropie, Clear Coat, Volumenstreuung, Specular edge color und Glanz
* &lbrack;Shader&rbrack;&lbrack;ASM&rbrack; Ändern der Farbwerte der Standardkanäle
* &lbrack;Shader&rbrack;&lbrack;ASM&rbrack;&lbrack;Export&rbrack; Aktualisierte Exportvorlage Adobe Dimension zu Adobe Substance 3D Stager
* &lbrack;Shader&rbrack;&lbrack;ASM&rbrack; Beschriftungen und QuickInfos für Shader- und MDL-Parameter hinzugefügt
* &lbrack;Shader&rbrack;&lbrack;ASM&rbrack; Sichtbarkeit der Farbe der Streuung in der 2D-Ansicht, auch wenn SSS nicht unterstützt wird
* &lbrack;Shader&rbrack;&lbrack;ASM&rbrack;&lbrack;Iray&rbrack; Unterstützung von ASM-Shader in Iray mit neuer MDL
* &lbrack;Shader&rbrack;&lbrack;ASM&rbrack;&lbrack;Iray&rbrack; Aktualisierte Volumenstreuung in veraltetem PBR-Spezifikationsglanz und beschichtet
* &lbrack;Shader&rbrack;&lbrack;ASM&rbrack;&lbrack;Content&rbrack; Standard-SSS-Typ für Beispiele geändert
* &lbrack;Shader&rbrack;&lbrack;ASM&rbrack; Dokumentation für ASM-API hinzugefügt
* &lbrack;Shader&rbrack;&lbrack;ASM&rbrack; Shader optimieren, um nicht verwendete Kanäle zu ignorieren
* &lbrack;Shader&rbrack; Leg neuer Textursatz-Kanäle
* &lbrack;Shader&rbrack; Verbesserte Volumenstreuung
* &lbrack;Shader&rbrack; Neue Shader-Parameter für einige Shader ausgeblendet
* &lbrack;Shader&rbrack; Sichtbar, wenn für Shader-Parameter
* &lbrack;Performance&rbrack;
* &lbrack;Libraries&rbrack; Verbesserungen beim Laden der Ressourcenvorschau und bei der Rechenleistung
* &lbrack;Engine&rbrack; Verbesserte Malleistung
* &lbrack;Automatisch Entpackt&rbrack;
* &lbrack;Automatisch Entpackt&rbrack; Leistungsverbesserungen bei Packing
* &lbrack;Automatisch Entpackt&rbrack; Automatisch entpackt, kompatibel mit dem Arbeitsablauf für die UV-Kachel
* &lbrack;Automatisches Entpacken&rbrack; Neue Option zur Positionierung von UVs entsprechend der Ausrichtung des Meshs
* &lbrack;Andere&rbrack;
* &lbrack;Einstellungen&rbrack; Standardzoomrichtung geändert
* &lbrack;UI&rbrack; Allgemeine Aktualisierung der Benutzeroberfläche
* &lbrack;UI&rbrack; Überarbeitung des Hilfemenüs
* &lbrack;UI&rbrack; Symbol &quot;Umkehren ersetzen&quot;
* &lbrack;UI&rbrack;&lbrack;Plugin&rbrack; Symbol &quot;Ersetzen&quot; für den Link &quot;Plug-in dcc&quot;
* &lbrack;UI&rbrack;&lbrack;AMD&rbrack; Erforderliche Mindestversion aktualisieren und Popup-Nachricht
* &lbrack;Ebenenstapel&rbrack; Neue Ebene innerhalb des ausgewählten leeren Ordners erstellen
* Python-Dokumentation aktualisieren
* &lbrack;Branding&rbrack;
* &lbrack;Branding&rbrack;&lbrack;UI&rbrack; Der Anwendungsname wurde in Adobe Substance 3D Painter aktualisiert
* &lbrack;Branding&rbrack;&lbrack;UI&rbrack; Eigenständige Version auf &quot;Substance Edition&quot; aktualisiert
* &lbrack;Branding&rbrack;&lbrack;UI&rbrack; Name, Installationspfad, Paket und Symbole der aktualisierten ausführbaren Datei der Anwendung
* &lbrack;Branding&rbrack;&lbrack;UI&rbrack; Standardbibliothek und Pfad umbenannt
* &lbrack;Branding&rbrack;&lbrack;UI&rbrack; Aktualisiertes Info-Fenster
* &lbrack;Branding&rbrack;&lbrack;UI&rbrack; Aktualisierter Begrüßungsbildschirm
* &lbrack;Branding&rbrack;&lbrack;UI&rbrack; Versionsnummer nach Jahr entfernt
* &lbrack;Lokalisierung&rbrack; Neue Übersetzungen in Deutsch, Französisch und vereinfachtem Chinesisch
* &lbrack;Interoperabilität&rbrack; Nicht verfügbar für Steam- und Substance-Editionen
* &lbrack;Interoperabilität&rbrack; Interoperabilität mit Adobe Ecosystem: Designer, Sampler, Stager und Bridge
* &lbrack;Interoperabilität&rbrack;&lbrack;UI&rbrack; Element aus Designer empfangen und aktualisieren
* &lbrack;Interoperabilität&rbrack;&lbrack;UI&rbrack; Element aus Sampler erhalten
* &lbrack;Interoperabilität&rbrack;&lbrack;UI&rbrack; Element an Stager senden
* &lbrack;Interoperabilität&rbrack;&lbrack;UI&rbrack; In Adobe Bridge anzeigen
* &lbrack;Interoperabilität&rbrack;&lbrack;UI&rbrack; Schneller Zugriff auf Adobe von 3D-Elementen
* &lbrack;Interoperabilität&rbrack; Neue Verwendungs-Tags von sbsar
* &lbrack;Interoperabilität&rbrack; Umgang mit empfangenen Elementtypen
* &lbrack;Interoperabilität&rbrack; Elemente, die von Adobe Substance 3D Designer oder Adobe Substance 3D Sampler empfangen werden, werden in der vom Benutzer standardmäßig ausgewählten Bibliothek gespeichert
* &lbrack;Interoperabilität&rbrack;&lbrack;UI&rbrack; Neues Symbol in der linken Symbolleiste zum Senden an Stager oder Photoshop

**Fest:**

* &Klammer;Tablet&Klammer; Geringe Leistung beim Malen mit Druck
* &Klammer;Tablet&Klammer; Problem auf Tablets mit Schiebereglern
* &lbrack;Absturz&rbrack; Nicht übereinstimmender Name zwischen Textursatz-Liste und Exporter
* &lbrack;Absturz&rbrack;&lbrack;Libraries&rbrack; Doppelklicken Sie auf eine Unterbibliothek
* &lbrack;Libraries&rbrack; Problem beim Durchsuchen von Bibliotheksverzeichnissen
* &lbrack;Libraries&rbrack; Die Befehlszeile &quot;Generierung der Vorschau erzwingen&quot; funktioniert nicht wie erwartet
* &lbrack;Libraries&rbrack;&lbrack;Content&rbrack; Der Baking geführt Lichtumgebungsfilter ist standardmäßig schwarz
* &lbrack;Linux&rbrack;&lbrack;MacOS&rbrack;&lbrack;Mesh&amp;rbrack exportieren; glTF kann nicht importiert werden, wenn es unter Linux/MacOS erstellt wurde
* &lbrack;Linux&rbrack; Das Ziehen und Ablegen einer Datei in das Bedienfeld &quot;Elemente&quot; kann zu einem Absturz führen
* &lbrack;Automatisches Entpacken&rbrack; Automatisches Entpacken ist auch dann verfügbar, wenn kein Mesh zum erneuten Laden ausgewählt wurde
* &blbrack;Partikeln&rbrack; Falsche Partikel mit Schwerkraft
* &lbrack;Ebenenstapel&rbrack; Ebenen-Histogramm kann nur Luminanz mit einigen Kanälen verwenden
* &lbrack;Geometrie-Maske&rbrack; Kontextmenü auf einem Ordner, wenn das Bearbeiten der Geometriemaske nicht funktioniert
* &lbrack;Projektion&rbrack; Naht mit sphärische Projektion &amp; bilinearer Filterung
* &blbrack;UV-Kacheln&rbrack; Maske in Datei exportieren exportiert nur Kachel 0, 0
* &lbrack;Mesh&rbrack; exportieren FBX Mesh-Export ist leer
* &lbrack;Iray&rbrack; Normalen-Map wird beim Rendern in neuen Projekten nicht berücksichtigt
* &lbrack;Speichern&rbrack; Probleme auf freigegebenen Laufwerken speichern
* &blbrack;Baking&rbrack; Beim erneuten Erstellen eines Meshs mit geänderten Parametern wird eine Warnung angezeigt
* &lbrack;Baking&rbrack;&lbrack;Regression&rbrack; Falsches Ergebnis, wenn der globale Begrenzungsrahmen des hohen Poly-Meshs den Ursprung der Szene nicht enthält
* &lbrack;Python&rbrack; Benutzerdefinierte Benutzerbibliotheken werden nicht berücksichtigt

**Bekannte Probleme:**

* &lbrack;Libraries&rbrack; Gespeicherte Suchvorgänge werden nicht gespeichert, wenn kein Projekt geöffnet wird
* &lbrack;NVIDIA&rbrack; Meldung für veralteten Treiber, selbst wenn der Treiber auf dem neuesten Stand ist

### 7.1.1 (2021.1.1)

*(Freigegeben: 23. März 2021*)Zusammenfassung: **Nebenversion, Bugfix mit der Möglichkeit, Hexadezimalwerte in den Farbwähler einzugeben**

**Hinzugefügt:**

* &lbrack;Log&rbrack; Benutzer über inkompatible AMD-GPU-Treiber warnen
* &Klammer;Farbwähler&Klammer; Eingabe von Hexadezimalwerten zulassen

**Fest:**

* &lbrack;Baker&rbrack; Einbruch der Leistung
* &lbrack;Geometrie-Maske&rbrack; Alt-Klick auf den Namen des Meshs kann zu einem Absturz führen
* &lbrack;Engine&rbrack; Beim Malen wird nicht die gesamte Ansicht aktualisiert, wenn dies erforderlich ist
* &lbrack;Ebenenstapel&rbrack; Auswahl bleibt nach dem Ändern des Shader hängen
* &lbrack;MacOS&rbrack;&lbrack;Farbwähler&rbrack; Die Farbe ist etwas anders als die ausgewählte
* &lbrack;Export&rbrack; Bei Verwendung des PSD-Dateiformats wird nicht eine Datei pro UV-Kachel generiert
* &lbrack;Skripterstellung&rbrack;&lbrack;Javascript&rbrack; alg.mapexport.getPathsExportDocumentMaps() gibt nicht alle Werte zurück
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Deaktivierte Plug-ins werden beim erneuten Öffnen von Painter wieder aktiviert

### 7.1.0 (2021.1.0)

*(Freigegeben: 28. Januar 2021*)Zusammenfassung: **Hauptversion, neue Geometriemaske, mit der Teile der UV-Kachel ausgewählt und Malen werden können, Kopier-/Einfügeeffekte im Ebenenstapel, verbesserte Geometriemaske, Aktualisierung von Iray, Bakern, Substance Engine und neuen Inhalten**

**Hinzugefügt:**

* Neue Geometriemaske und Malen ausgewählter Teile der Geometrie
* &lbrack;Geometrie-Maske&rbrack; Malen ausgewählter Geometrieteile nach Mesh-Namen zulassen
* &lbrack;Geometrie-Maske&rbrack; Rechteckige Auswahl in beiden Viewporten
* &lbrack;Geometrie-Maske&rbrack; Ausgeschlossene Geometrie auf einer Ebene ausblenden/ignorieren
* &lbrack;Geometriemaske&rbrack;&lbrack;Eigenschaften&rbrack; Schnellauswahl für Kontrollkästchen durch Klicken und Ziehen
* &lbrack;Geometry Mask&rbrack;&lbrack;Properties&rbrack;&lbrack;UI&rbrack; Alle einschließen/ausschließen mit einer Dropdown-Liste im Eigenschaftenfenster
* &lbrack;Geometriemaske&rbrack;&lbrack;Eigenschaften&rbrack; Schnelles Auswählen eines Elements in einer Liste mit ALT+LINKSKLICK
* &lbrack;Geometriemaske&rbrack;&lbrack;Eigenschaften&rbrack; Überlagerung in Viewporten, wenn der Mauszeiger über Mesh-Namen/-UV-Kacheln im Eigenschaftenfenster bewegt wird
* &lbrack;Geometriemaske&rbrack;&lbrack;Ebenenstapel&rbrack; Hinzufügen von Kopier-/Einfügeoptionen zur Geometriemaske
* &lbrack;Geometrie-Maske&rbrack; Neues Symbol für die Schaltfläche &quot;Ausgeschlossene Geometrie ausblenden/ignorieren&quot;
* &lbrack;Geometrie-Maske&rbrack; Neue QuickInfo für Ausgeschlossene Geometrie ausblenden/ignorieren
* &lbrack;Geometrie-Maske&rbrack; Tastaturbefehl ALT+H drücken, um die Schaltfläche &quot;Ausgeschlossene Geometrie ignorieren&quot; ein- oder auszublenden
* &lbrack;UV-Kacheln&rbrack;&lbrack;Ebenenstapel&rbrack; Vorschau der neuen Füllebene-Kugel für UV-Kacheln und vereinfachten Modus
* &lbrack;UV-Kacheln&rbrack;&lbrack;Ebenenstapel&rbrack; UV-Kachel-Maske leicht verlassen
* &lbrack;UV-Kacheln&rbrack;&lbrack;Textursatz Liste&rbrack; Geben Sie eine Beschreibung pro UV-Kachel an.
* &lbrack;UV-Kacheln&rbrack;&lbrack;Textursatz-Einstellungen&rbrack;&lbrack;UI&rbrack; Zwei neue Abschnittstitel im Dropdown-Menü zum Ändern der Auflösung der UV-Kachel
* &lbrack;UV-Kacheln&rbrack;&lbrack;Viewport&rbrack; UV-Kachel-Maske beenden, wenn ein Material in den Viewport gezogen wird
* &lbrack;Ebenenstapel&rbrack; Optionen zum Kopieren/Einfügen für Effekte hinzufügen
* &lbrack;Ebenenstapel&rbrack; Kopieren/Einfügen von Effekten von einem Textursatz in einen anderen zulassen
* &lbrack;Ebenenstapel&rbrack; Mehrfachauswahl von Effekten zulassen
* &lbrack;Ebenenstapel&rbrack; Optionen zum Kopieren/Einfügen als Tastaturbefehle für Ebeneneffekte hinzufügen
* &lbrack;Ebenenstapel&rbrack; Automatisches Umschalten zwischen Maske und Inhalt beim Ziehen von Effekten auf eine andere Ebene
* &lbrack;Ebenenstapel&rbrack; Beim Einfügen einer Maske aus einer anderen Ebene automatisch eine Maske erstellen
* &lbrack;Ebenenstapel&rbrack; Hinzufügen von Aktionen zum Verschieben von Effekten im Kontextmenü des jeweiligen Effekts
* &lbrack;Ebenenstapel&rbrack; Ziehen und Ablegen von Effekten von einer Ebene auf eine andere zulassen
* &lbrack;Ebenenstapel&rbrack; Wenn Elemente in einen Ordner gezogen werden, werden sie oben im Ordner abgelegt.
* Iray auf Version 2020.1.0 aktualisieren
* &lbrack;Baker&rbrack; Baker auf Version 2.5.4 aktualisieren
* &lbrack;Baker&rbrack; Einzelne UV-Kacheln im Fenster &quot;Baking-Fortschritt&quot; anzeigen
* &lbrack;Baker&rbrack;&lbrack;UI&rbrack; Ermöglicht das schnelle Baking des aktuellen Textursatzes mit einer neuen Schaltfläche
* &lbrack;Baker&rbrack; Benutzer können mit ALT+LINKSKLICK schnell einen der Baker auswählen
* Substance Engine auf Version 8.0.8 aktualisieren
* &lbrack;Substance Engine&rbrack; Unterstützung der Standardfarbe in neuen .sbsar-Dateien
* &lbrack;Automatisch Entpackt&rbrack; Leistungssteigerung
* &lbrack;Export&rbrack; Fügen Sie visuelles Feedback hinzu, um anzuzeigen, welche Auflösung der UV-Kachel vom Projektstandard abweicht
* &lbrack;Export&rbrack; Szene-Größenfaktor zur exportierten Shader-JSON-Datei hinzufügen
* &lbrack;Sprache&rbrack; Hinzufügen von japanischen Übersetzungen
* &lbrack;UI&rbrack; Info-Fenster mit Versionierung interner Abhängigkeiten aktualisieren
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Verwalten von Regal-Ressourcen zulassen
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Benachrichtigen, wenn ein Projekt zum Baking und Exportieren bereit ist
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Erlaubt zu wissen, wann ein Regal das Crawlen von Ressourcen auf der Festplatte abgeschlossen hat
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Abfragen der Liste der UV-Kacheln pro Textursatz zulassen
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Zuweisen einer benutzerdefinierten Vorschau zu Regal-Ressourcen zulassen
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Verwalten benutzerdefinierter Regal zulassen
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Hinzufügen eines Methodenindex in jedem Untermodul in der Dokumentation
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Neuer Stil für die Dokumentation
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Verbesserung der Ressourcen und Dokumentation des Regals
* &lbrack;Inhalt&rbrack; Drei neue Werkzeugvorgaben zum Nähen
* &lbrack;Regal&rbrack; Entfernen Sie vorübergehend &quot;Auf Substance share exportieren&quot;, während Sie zur neuen Substance share-Plattform wechseln.

**Fest:**

* Absturz bei Monitoren mit unterschiedlichen Auflösungen
* Absturz im Substance Engine mit einigen seltenen Projekten
* Die Aktualisierung des Viewports schlägt beim Wechseln von Ebenen mit &quot;Ausgeschlossene Geometrie ausblenden/ignorieren&quot; fehl.
* &lbrack;2D-Ansicht&rbrack; 2D-Viewport kann in einigen Projekten fehlen
* &blbrack;Baking&rbrack; &quot;Nach Mesh suchen&quot; ignoriert Teile des Objekts.
* &lbrack;Ebenenstapel&rbrack; Durch Klicken auf einen Ebeneneffekt wird der Ordner geöffnet.
* &lbrack;Geometrie-Maske&rbrack; UV-Kachel wird immer noch in der Maske gezählt, auch wenn der Mesh ohne sie erneut importiert wird
* &lbrack;Geometrie-Maske&rbrack; Das Kontextmenü im Viewport bietet nicht die richtigen Werkzeuge
* &lbrack;Engine&rbrack; Erhebliche Verzögerungen bei bestimmten Projekten
* &lbrack;Skripterstellung&rbrack; Hohe Latenz bei JSON-Remote-POST-Anforderungen unter Windows
* &lbrack;Linux&rbrack; Die VRAM-Menge wird bei bestimmten integrierten GPUs nicht ordnungsgemäß erkannt.
* &lbrack;Automatisch Entpackt&rbrack; Absturz oder lange entpack an einigen Projekten

## Version 6

### 6.2.2 (2020.2.2)

*(Freigegeben: 28. September 2020 (1&rbrace;)Zusammenfassung:**Nebenversion, Bugfix mit einigen Funktionen in der Python-API***

**Hinzugefügt:**

* &lbrack;Performance&rbrack; Nicht alle UV-Kacheln bei Verwendung der Farb-ID berechnen
* &lbrack;Baker&rbrack;&lbrack;UI&rbrack; Anzeigen von Textursatz-Beschreibungen
* &lbrack;Baker&rbrack; Speichern von Baking-Einstellungen zulassen
* &lbrack;Baker&rbrack; Hinzufügen aller reduzierten/aller erweiterten Optionen zur Registerkarte &quot;Auswahl&quot;
* &lbrack;Textursatz Liste&rbrack; Beschreibung ausblenden, wenn leer
* &lbrack;UV-Kacheln&rbrack;&lbrack;Textursatz Liste&rbrack; Klicken auf UV-Kachel sollte Liste erweitern/reduzieren
* &lbrack;Export&rbrack;&lbrack;UI&rbrack; Horizontale Änderung der Größe des Bedienfelds &quot;Textursatz-Liste&quot; zulassen
* &lbrack;Export&rbrack;&lbrack;UI&rbrack; Konsistenter QuickInfo-Text für UV-Kacheln und Textursatz-Arbeitsablauf mit nicht ausgewählten Texturen
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Verwenden von Exportvorgaben zum Exportieren von Texturen zulassen
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Hinzufügen eines Änderungsprotokolls in der Dokumentation
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Zulassen, dass alle verfügbaren Kanäle auf einem bestimmten Stapel abgefragt werden
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Verbesserungen an der Konsolenbenutzeroberfläche

**Fest:**

* &lbrack;AMD&rbrack; Falsche Erkennung veralteter Treiberversionen
* Absturz beim erneuten Importieren eines Meshs mit unterschiedlichem UV-Kacheln-Layout in einigen Fällen
* Absturz bei der Verwendung von Partikeln mit UDIM auf sehr schweren Meshs
* &blbrack;UV-Kacheln&rbrack; Absturz beim Exportieren eines Meshs mit Versatz-Informationen in einigen Fällen
* &lbrack;Export&rbrack;&lbrack;Absturz&rbrack; Das Exportieren von 2D-Ansichten im PSD-Format kann einen Absturz verursachen
* Das Importieren von Bildern als Sequenzen beim Erstellen eines Projekts funktioniert nicht
* Engine in einer Endlosschleife
* &lbrack;Tastaturbefehl&rbrack; Kamera dreht sich immer im einrasten Modus, wenn Tastenkombinationen im einrasten Modus geändert werden
* Mesh werden immer automatisch entpackt, wenn sie erneut importiert werden, auch wenn die Option deaktiviert ist
* &lbrack;Textursatz Liste&rbrack; Das Textfeld &quot;Beschreibung&quot; ist während der Edition manchmal nicht vollständig sichtbar.
* &lbrack;Textursatz Liste&rbrack; Dropdown-Menü zum Ein-/Ausblenden von Textursätzen ist nicht vollständig sichtbar
* &lbrack;Textursatz Liste&rbrack; Wenn Sie auf das Augensymbol klicken, sollten Sie nicht den Namen des Textursatzes bearbeiten eingeben.
* &blbrack;Textursatz-Einstellungen&rbrack; Durch Entfernen eines Kanals wird auch der darunter liegende Kanal entfernt
* &lbrack;Export&rbrack; Alle einschließen und Alle zurücksetzen berücksichtigt keine UV-Kacheln
* &lbrack;Baker&rbrack; Während des Bakings werden nicht ausgewählte Baker angezeigt
* Die Behebungsaktualisierung wird bei durch Baking erzeugte Map als Eingabe nicht berücksichtigt
* &lbrack;UV-Kacheln&rbrack;&lbrack;Viewport&rbrack; 3D-Viewport friert ein, wenn Intelligente Material nach einem UV-Kachel mit ausgewählter Ordnermaske hinzugefügt wird
* &lbrack;UV-Kacheln&rbrack;&lbrack;Viewport&rbrack; Drahtgitter ist immer noch für ausgeblendete Kacheln mit dem Modus &quot;Malen durch&quot; sichtbar
* &lbrack;Export&rbrack;&lbrack;Sketchfab&rbrack; Probleme mit dem Abonnementtyp &quot;Plus&quot;
* &lbrack;Sketchfab&rbrack; Das Kontrollkästchen &quot;Dieses Asset ist privat&quot; wird nach dem Kontowechsel nicht angezeigt
* &lbrack;Export&rbrack;&lbrack;Content&rbrack; Verwackelte Pinselvorgaben können zu Leistungsproblemen führen.
* &lbrack;Plugin Photoshop&rbrack; Meldung im Protokoll: nicht kompatibel mit dem UV-Kachel-Workflow
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; PYTHONPATH env var verhindert den Start der Anwendung
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Typo in der Python-Dokumentation

### 6.2.1 (2020.2.1)

*(Freigegeben: 29. Juli 2020 (1&rbrace;)Zusammenfassung:**Nebenversion, Hotfix***

**Hinzugefügt:**

* Umgebungsvariable &quot;SUBSTANCE_PAINTER_VRAM_BUDGET&quot; hinzufügen, um den GPU-VRam-Betrag zu überschreiben
* &lbrack;UV-Kacheln&rbrack;&lbrack;Leistung&rbrack; Nicht alle UV-Kacheln berechnen, wenn das Polygon-Füllwerkzeug verwendet wird

**Fest:**

* &lbrack;Iray&rbrack; &quot;Rendering speichern&quot; gibt einen Fehler zurück, der zu einem schwarzen Bild führt
* &lbrack;Linux&rbrack; Absturz nach dem Begrüßungsbildschirm unter CentOS 7.3
* &lbrack;Linux&rbrack; Die VRAM-Menge wird bei bestimmten Konfigurationen nicht richtig erkannt.
* &lbrack;Absturz&rbrack; Öffnen eines Projekts mit dem Namen des duplizierten Textursatzes
* &lbrack;Engine&rbrack; Problem mit Cache-Invalidierung beim Ändern einer Maske
* &lbrack;Textursatz Liste&rbrack; Falscher Schrifteffekt, wenn Textursatz deaktiviert ist

**Bekannte Probleme:**

* &lbrack;Textursatz Liste&rbrack; Beschreibung kann nicht ausgeblendet werden
* &lbrack;Textursatz Liste&rbrack; UI-Probleme
* &lbrack;Iray&rbrack; PSD-Rendering wird nicht geöffnet
* &lbrack;Plugin Photoshop&rbrack; Nicht kompatibel mit dem Arbeitsablauf für UV-Kacheln

### 6.2.0 (2020.2.0)

*(Freigegeben: 23. Juli 2020 (1&rbrace;)Zusammenfassung:**Hauptversion mit neuem Arbeitsablauf für UV-Kacheln, Malen über UV-Kacheln hinweg und Leistungsverbesserung***

**Hinzugefügt:**

* UV-Kacheln (UDIM)
* &blbrack;UV-Kacheln&rbrack; Malen über UV-Kacheln
* &blbrack;UV-Kacheln&rbrack; Auswahl zwischen neuem und veraltetem Arbeitsablauf für UV-Kacheln zulassen
* &blbrack;UV-Kacheln&rbrack; Importieren von Bildsequenzen für UDIM/UV-Kacheln als Ressource
* &blbrack;UV-Kacheln&rbrack; Liste der UV-Kacheln pro Textursatz im Fenster &quot;Liste der Textursatz&quot; hinzufügen
* &blbrack;UV-Kacheln&rbrack; Ermöglichen der gleichzeitigen Bearbeitung mehrerer UV-Kacheln in den Textursatz-Einstellungen
* &lbrack;UV-Kacheln&rbrack;&lbrack;2D-Ansicht&rbrack; UV-Kacheln als Raster anzeigen
* &lbrack;UV-Kacheln&rbrack;&lbrack;2D-Ansicht&rbrack; Neue Viewport-Schaltfläche zum Anzeigen oder Ausblenden von Informationen zu UV-Kacheln
* &blbrack;UV-Kacheln&rbrack; Beim UV-Kachel von Projekten standardmäßig auf Ein Kanal umstellen
* &blbrack;UV-Kacheln&rbrack; Neue Schaltfläche in der kontextabhängigen Symbolleiste, um maskierte UV-Kacheln beim Malen zu ignorieren
* &lbrack;UV-Kacheln&rbrack;&lbrack;Ebenenstapel&rbrack; Neue Ebenenstapel-Symbole zur Leistungsverbesserung
* &lbrack;UV-Kacheln&rbrack;&lbrack;Ebenenstapel&rbrack; Verbessern der Symbole &quot;Malen und Füllen&quot; in der Symbolleiste
* &lbrack;UV-Kachel&rbrack;&lbrack;2D-Ansicht&rbrack; Mehrere UV-Kacheln gleichzeitig ein- oder ausschließen (Linksklick, Strg + Linksklick)
* &blbrack;UV-Kachel mask&rbrack; Neue Ebenenmaske zum Einschließen, Ausschließen von Kacheln pro UV-Kachel mit neuem Symbol
* &lbrack;UV-Kachel&rbrack;&lbrack;Ebenenstapel&rbrack; Anzahl der UV-Kacheln im Maskensymbol für UV-Kacheln anzeigen, wenn nicht alle eingeschlossen sind
* &lbrack;UV-Kachel&rbrack;&lbrack;2D/3D-Ansicht&rbrack; Einen Hover-Effekt hinzufügen, um UV-Kacheln unter dem Cursor darzustellen.
* &lbrack;UV-Kacheln&rbrack;&lbrack;Baker&rbrack; Auswahl und Baking bestimmter UV-Kacheln zulassen
* &lbrack;UV-Kacheln&rbrack;&lbrack;Baker&rbrack; Hinzufügen von Auswahloptionen für Textursatz/UV-Kacheln
* &lbrack;UV-Kacheln&rbrack;&lbrack;Baker&rbrack; Kontextmenüoption zum Auswählen von UV-Kacheln innerhalb eines Textursatzes
* &lbrack;UV-Kacheln&rbrack;&lbrack;Baker&rbrack; Schnellauswahl im Textursatz/in den UV-Kacheln durch Ziehen ermöglichen
* &lbrack;UV-Kacheln&rbrack;&lbrack;Baker&rbrack; Ersetzen Sie die Schaltflächen &quot;Alle&quot; und &quot;Keine&quot; in Mesh-Map durch explizitere Auswahloptionen
* &lbrack;UV-Kacheln&rbrack;&lbrack;Baker&rbrack; Anzahl der zu Baking führend Texturen anzeigen
* &lbrack;UV-Kacheln&rbrack;&lbrack;Exportieren&rbrack; Auswahl und Export bestimmter UV-Kacheln zulassen
* &lbrack;UV-Kacheln&rbrack;&lbrack;Exportieren&rbrack; UV-Kacheln durch Ziehen mit der Maus schnell auswählen
* &lbrack;UV-Kacheln&rbrack;&lbrack;Exportieren&rbrack; Hinzufügen von Dropdown-Menüoptionen für UV-Kacheln
* &lbrack;UV-Kacheln&rbrack;&lbrack;Exportieren&rbrack; Deaktivieren einiger Exportvorgaben, wenn sie nicht mit UV-Kacheln funktionieren (Adobe Dimension, Sketchfab, glTF, USD)
* &lbrack;UV-Kacheln&rbrack;&lbrack;Inhalt&rbrack; Exportvorgaben zur Verwendung des neuen Tags $udim aktualisieren
* &blbrack;UV-Kacheln&rbrack; Verbessern der Fehlerberichterstattung beim Importieren von Meshs mit überlappenden UV-Inseln
* &blbrack;UV-Kacheln&rbrack; In Iray kompatible UV-Kacheln
* &lbrack;UV-Kacheln&rbrack;&lbrack;Scripting&rbrack; Hinzufügen einer UV-Kachel-Exportdokumentation zu Python-Dokumenten
* Leistung
* &lbrack;Performance&rbrack; Neue Schaltfläche in der kontextabhängigen Symbolleiste zum Anhalten der Berechnung von Enginen bei der Arbeit (UMSCHALT+ESC)
* &lbrack;Performance&rbrack; Schnelleres Öffnen von Projekten durch Verzögerung der Textursatz-Cache-Berechnung
* &lbrack;Performance&rbrack; Warten Sie nicht, bis die Mesh-Map beim Öffnen des Projekts geladen sind
* &lbrack;Performance&rbrack;&lbrack;2D/3D-Ansicht&rbrack; Maskenkanal im Viewport nicht berechnen, wenn er nicht verwendet wird
* &lbrack;Performance&rbrack; Anwendung nicht blockieren, wenn Mesh-Map in den Viewporten geladen werden
* &lbrack;Performance&rbrack; Verbessern der inkrementellen Speichergeschwindigkeit beim Speichern eines Projekts
* &lbrack;Performance&rbrack;&lbrack;Bakers&rbrack; Ändern Sie die Standardeinstellungen für die Ausdehnung, um die Speicherzeit und die Projektgröße zu verbessern
* &lbrack;Performance&rbrack;&lbrack;Bakers&rbrack; Wechsel zu Graustufen auf bestimmten Bakern, um Zeit und Projektgröße zu sparen
* &lbrack;Performance&rbrack;&lbrack;Export&rbrack; Verbessern der Engine-Performance, um Texturen schneller exportieren zu können
* &lbrack;Performance&rbrack;&lbrack;Export&rbrack; Verbessern der Reaktionsfähigkeit beim Öffnen des Exportdialogs mit vielen Textursätzen
* &lbrack;Performance&rbrack;&lbrack;Export&rbrack; Verbessern Sie die Leistung beim Wechsel zur Registerkarte &quot;Exportliste&quot;.
* &lbrack;Performance&rbrack;&lbrack;Iray&rbrack; Iray-Startzeit reduzieren
* Sonstige
* &lbrack;Baker&rbrack; Hinzufügen von Auswahloptionen für Textursatz
* Shader-Instanzen-Management auf Textursatz-Einstellungen verschieben
* &lbrack;2D/3D-Ansicht&rbrack; Nachricht am unteren Rand des Viewports hinzufügen, um anzuzeigen, welcher Maskentyp bearbeitet wird
* &lbrack;Ebenenstapel&rbrack; Neue Option in den Einstellungen, um zwischen alten und neuen Miniaturansichten zu wechseln
* &lbrack;Ebenenstapel&rbrack; Visuelles Feedback hinzufügen, um den Ladezustand der Miniaturen anzuzeigen
* &lbrack;Proj&rbrack; Neue Projektion &quot;Fill (Match Per UV-Tile)&quot; zum Laden von Bildsequenzen
* &lbrack;Proj&rbrack; Ändern Sie in bestimmten Fällen den Modus &quot;Füllebenen-Projektion&quot; in &quot;Füllen (entspricht pro UV-Kachel)&quot;
* &lbrack;Inhalt&rbrack; Optimierung der Kohlevergaserleistung zur Verbesserung der Pinselvorgabe
* Iray auf Version 2020.0.0 aktualisieren
* &lbrack;Export&rbrack; Deaktivieren der Registerkarte &quot;Exportliste&quot;, wenn nichts ausgewählt ist
* Automatisch Entpackt
* &lbrack;Automatisch Entpackt&rbrack; Verbesserung der Erfolgsrate des automatischen entpack-Prozesses
* &lbrack;Automatisch Entpackt&rbrack; Verbesserte Parametrisierung zur Erhöhung der Geschwindigkeit und Stabilität

**Fest:**

* &lbrack;Alembic&rbrack; Facetten werden beim Importieren von Dateien ignoriert
* &lbrack;Alembic&rbrack; Unendliche Ladezeit mit bestimmten Dateien
* &lbrack;Import&rbrack; Eine falsche UDIM-Bildsequenz wird importiert, wenn nur die Dateierweiterung unterschiedlich ist
* &lbrack;Absturz&rbrack; Der Versuch, ein Projekt zu öffnen, das durch einen anderen Prozess gesperrt ist, führt zu einem Absturz
* &lbrack;Projektion&rbrack; Artefakte an dupliziertem Mesh bei Verwendung von triplanare Projektion
* &lbrack;Export&rbrack; Emissive-Kanal wird nicht mit USD exportiert
* &lbrack;Inhalt&rbrack; Intelligente Material &quot;Charcoal&quot; enthält Malen-Striche

**Bekannte Probleme:**

* &lbrack;Textursatz Liste&rbrack; Beschreibung kann nicht ausgeblendet werden
* &lbrack;Textursatz Liste&rbrack; UI-Probleme

### 6.1.3 (2020.1.3)

*(Freigegeben: 16. Juni 2020 (1&rbrace;)Zusammenfassung:**Bugfix***

**Hinzugefügt:**

* &lbrack;Export&rbrack; Versatz-Einstellungen in der JSON-Datei für Shader-Parameter hinzufügen

**Fest:**

* &lbrack;Absturz&rbrack;&lbrack;Engine&rbrack; Absturz beim Löschen und Ersetzen vorhandener Kanäle
* &lbrack;Absturz&rbrack; Ändern des Shaders nach dem Malen einer Maske in einer Material-Ebene
* &lbrack;Absturz&rbrack;&lbrack;Engine&rbrack; Absturz mit einigen umfangreichen Projekten
* &lbrack;Baker&rbrack; Die Zuordnung nach Name funktioniert nicht mit aus zBrush exportierten OBJ
* &lbrack;Versatz&rbrack;&lbrack;SVT&rbrack; Texturen werden beim Öffnen des Projekts nicht angezeigt, wenn der Versatz aktiviert ist
* &lbrack;Export&rbrack; Einige Texturen werden in einheitlichem Grau exportiert
* &lbrack;Export&rbrack; Deaktivierte Textursatz sollten nicht für Dimension- und Sketchfab-Exportvorgaben exportiert werden
* &lbrack;Skripterstellung&rbrack;&lbrack;JavaScript&rbrack; Absturz bei der Verwendung der JavaScript-API, um auf die Exportkonfiguration im onProjectOpened-Ereignis zuzugreifen
* &lbrack;Skripterstellung&rbrack;&lbrack;Javascript&rbrack; onExportFinished() wird nach einem Export nicht aufgerufen

### 6.1.2 (2020.1.2)

*(Freigegeben: 28. Mai 2020*)Zusammenfassung: **Bugfix mit Substance Engine- und Baker-Update**

**Hinzugefügt:**

* &lbrack;Baker&rbrack; Aktualisieren Sie auf die neueste Version
* &lbrack;Baker&rbrack; Neue Sampling-Methode in den Bakern Ambient occlusion, Krümmung, Thickness
* Aktualisieren Sie auf die neueste Version von Substance Engine
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Erstellen der ResourceID für Projektressourcen zulassen
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Abfragen von Kanalinformationen zulassen
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Hinzufügen von DryRun- und Callback-Funktionen zur Simulation des Textur-Exports

**Fest:**

* &lbrack;Baker&rbrack; Falsche Normalen im Welt-Raum-Normale-Baker mit einer Tangente-Normalen-Map in bestimmten Fällen
* &lbrack;Baker&rbrack; Fehler beim Baking von Ambient occlusion mit Optix, wenn kein hohes Poly
* &lbrack;Dynamische Pinselstriche&rbrack; Verzögerung beim Laden eines bestimmten Textursatzes
* &lbrack;Export&rbrack; Sollte die deaktivierten Textursätze nicht für USD exportieren, glTF
* &lbrack;Skripterstellung&rbrack;&lbrack;JavaScript&rbrack; Die Baker-Einstellungen für neue Krümmungen können nicht bearbeitet werden.
* &lbrack;Skripterstellung&rbrack;&lbrack;JavaScript&rbrack; alg.texturesets.addChannel() gibt in einigen Fällen keinen Fehler zurück
* &lbrack;Skripterstellung&rbrack;&lbrack;JavaScript&rbrack; Typo in der JavaScript-API-Dokumentation für setProjectExportOptions()
* &lbrack;Skripterstellung&rbrack;&lbrack;JavaScript&rbrack; Immer alle Textursatz exportieren
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; sys.executable gibt einen Pfad zu python.exe anstelle von Substance Painter zurück
* Textur-Cache nicht kompatibel mit Mac OS und Windows/Linux
* &lbrack;Livelink UE4&rbrack; Nur das letzte Material wird für alle Textursatz in einem kombinierten Mesh verwendet.

**Bekannte Probleme:**

* &lbrack;Export&rbrack;&lbrack;Dimension&rbrack;&lbrack;Skecthfab&rbrack; Die deaktivierten Textursatz sollten nicht exportiert werden
* &lbrack;Absturz&rbrack; Shader nach dem Malen einer Maske in einer Material-Ebene ändern

### 6.1.1 (2020.1.1)

*(Freigegeben: 05. Mai 2020*)Zusammenfassung: **Hotfix**

**Hinzugefügt:**

* &lbrack;Export&rbrack; Visuelles Feedback des überschriebenen Status für TextureSet

**Fest:**

* &lbrack;Export&rbrack; Exporter-Fenstergröße ist auf einem Spezialauflösungsmonitor zu groß und kann nicht geändert werden
* &lbrack;Export&rbrack; Optionen werden nach dem Export nicht gespeichert
* &lbrack;Export&rbrack; Absturz oder kann nicht mit einer Exportvorgabe vom Cache exportiert werden
* &lbrack;Export&rbrack; Wenn Sie den Export abbrechen, wird eine unerwartete zusätzliche leere Map generiert.
* &lbrack;Export&rbrack; Vorgabeeinstellungen für den virtuellen Export korrigieren
* &lbrack;Python&rbrack; PYTHONPATH env var wird nicht berücksichtigt
* &lbrack;Python&rbrack;&lbrack;Export&rbrack; Wenn Sie den Export über Python abbrechen, wird ein Ausnahmefehler zurückgegeben
* &lbrack;Python&rbrack;&lbrack;Export&rbrack; export_project_Texturen falsches Ergebnis mit psd-Dateiformat
* &lbrack;Baker&rbrack; Absturz unter Linux mit GPU-Raytracing

**Bekannte Probleme:**

* &lbrack;JavaScript&rbrack; Die Baker-Einstellungen für neue Krümmungen können nicht bearbeitet werden.
* &lbrack;JavaScript&rbrack;&lbrack;Export&rbrack; Immer alle Textursatz exportieren
* &lbrack;Export&rbrack;&lbrack;USD&rbrack; Die deaktivierten Textursatz sollten nicht exportiert werden
* &lbrack;Absturz&rbrack; Shader nach dem Malen einer Maske in einer Material-Ebene ändern

### 6.1.0 (2020.1.0)

*(Freigegeben: 22. April 2020 (1&rbrace;)Zusammenfassung:**Hauptversion mit neuer Textur und neuem Mesh-Exporter (mit Versatz und Tessellation), aktualisiertem UV mit mehr Steuerelementen, neuen Bakern, neuer Python-API für die Skripterstellung, besserer UX für die Decal-entpackte und neuem Inhalt***

**Hinzugefügt:**

* Exporter &quot;Neue Textur und neuer Mesh&quot;
* &lbrack;Export&rbrack; Neue Exporter-Oberfläche
* &lbrack;Export&rbrack;&lbrack;Export tab&rbrack; Auswahl der pro Textursatz exportierten Kartenkanäle zulassen
* &lbrack;Export&rbrack;&lbrack;Export tab&rbrack; Ändern der Textursatz-Größe für alle Textursatz in einer Aktion zulassen
* &lbrack;Export&rbrack;&lbrack;Export tab&rbrack; Andere Vorlagen pro Textursatz zulassen (außer USD, glTF, Sketchfab und Dimension)
* &lbrack;Export&rbrack;&lbrack;Export tab&rbrack; Schnelle Aktivierung und Deaktivierung von Karten und Textursätze
* &lbrack;Export&rbrack;&lbrack;Export tab&rbrack; Exportauflösung 8192x8192 nicht mehr experimentell
* &lbrack;Export&rbrack;&lbrack;Export tab&rbrack; Ändern des Dateiformats und der Bittiefe pro Map zulassen
* &lbrack;Export&rbrack;&lbrack;Export tab&rbrack; Zurücksetzen auf die Werte der Standardparameter zulassen
* &lbrack;Export&rbrack;&lbrack;Export tab&rbrack; Speichern von Einstellungen ohne Export zulassen
* &lbrack;Export&rbrack;&lbrack;Ausgabevorlagen tab&rbrack; Registerkarte &quot;Konfiguration&quot; in Registerkarte &quot;Ausgabevorlagen&quot; umbenennen
* &lbrack;Export&rbrack;&lbrack;Ausgabevorlagen tab&rbrack; Definition von Dateiformat und Bittiefe pro voreingestellter Map zulassen
* &lbrack;Export&rbrack;&lbrack;Liste der Exporte tab&rbrack; Neue Vorschauregisterkarte zum Zusammenfassen und Anzeigen des Exportvorgangs
* &lbrack;Mesh&rbrack; importieren/exportieren Optimierte Performance beim Importieren/Exportieren der Zeit
* &lbrack;Mesh&rbrack; exportieren Exportieren von Mesh in FBX
* &lbrack;Mesh&rbrack; exportieren Mesh mit Versatz und Tessellation exportieren
* &lbrack;Mesh&rbrack;&lbrack;UI&rbrack; exportieren Neue Einstellungen für die Neuberechnung des normalen Scheitelpunkt, Anwendung der Triangulation
* &lbrack;Mesh&rbrack; exportieren Exportieren der ursprünglichen Mesh-Topologie mit neuen UVs, die durch automatischen entpack generiert werden
* Automatischer entpack mit weiteren Steuerelementen wurde aktualisiert
* &lbrack;UV Entpack&rbrack;&lbrack;UI&rbrack; Einstellung hinzufügen, um den automatischen entpack von UV im neuen Projektfenster zu aktivieren
* &lbrack;UV Entpack&rbrack;&lbrack;UI&rbrack; Neue Optionen zum Steuern der entpackend Schritte (Nähte, entpack, Packing)
* &lbrack;UV Entpack&rbrack;&lbrack;UI&rbrack; Beibehaltung bestehender entpackend Nähte/entpackend/Packings
* &lbrack;UV Entpack&rbrack;&lbrack;UI&rbrack; Neue Optionen zur vollständigen Neuberechnung entpackend Schritte
* &lbrack;UV Entpack&rbrack;&lbrack;UI&rbrack; Neue Option zur Steuerung der Randgröße (keine, kleine, mittlere und große)
* Neue Baker
* &lbrack;Baker&rbrack; Alte Krümmung durch neue Krümmung aus dem Mesh ersetzen
* &lbrack;Baker&rbrack; Option &quot;Match by Name&quot; hinzufügen, um die Rückseite im Baker &quot;Ambient occlusion&quot; zu ignorieren
* &lbrack;Baker&rbrack; Option &quot;Boden-Ebene hinzufügen&quot; im Baker &quot;Ambient occlusion&quot;
* Neue Python-API für die Skripterstellung (3.7.6)
* &lbrack;Python&rbrack;&lbrack;UI&rbrack; Neues Skriptmenü für Python
* &lbrack;Python&rbrack;&lbrack;UI&rbrack; Neue Python-Dokumentation im Hilfemenü
* &lbrack;Python&rbrack; Leg der Substance Painter-Pythonmodule: substance_painter, alg, display, project.setting, project, texturesets, ui
* &lbrack;Python&rbrack; Leg des neuen Python-Moduls &quot;substance_painter&quot;
* &lbrack;Python&rbrack; Neues Python-Untermodul gelegt: alg, display, log, project, resource, texturesets, ui
* &lbrack;Python&rbrack; Listener für Projektänderungen
* &lbrack;Python&rbrack; Neue Beispiele in der Python-Dokumentation
* &lbrack;JavaScript&rbrack;&lbrack;UI&rbrack; Menü &quot;Plug-ins&quot; durch JavaScript ersetzt
* &lbrack;Viewport&rbrack; Erstellen einer Aufkleberressource durch Ziehen/Ablegen + ALT aus dem Regal zulassen, wenn eine Projektion aus dem Aufkleber erstellt wird
* Neue Inhalte
* &lbrack;Inhalt&rbrack; 5 neue Aufkleber Materialien von Substance Source
* &lbrack;Inhalt&rbrack; Hinzufügen neuer Projektvorlagen und Exportieren von Vorgaben für den Maxwell-Renderer
* &lbrack;Inhalt&rbrack; Projektvorlage für Keyshot 9-Export hinzufügen
* &lbrack;Inhalt&rbrack; Die Exportvorgabe von Keyshot 9 zur Unterstützung von Versatz und emissive aktualisieren
* &lbrack;Inhalt&rbrack;&lbrack;Exporter&rbrack; Aktualisierung aller Exportvorgaben, um die neuesten Versionen von Game-Enginen und Renderern abzugleichen
* &lbrack;Inhalt&rbrack;&lbrack;Exporter&rbrack; Exportvoreinstellungsdateien aktualisieren, um neue Format- und Dithering-Einstellungen zu verwenden
* &lbrack;Inhalt&rbrack; Neue Vorlagen und Shader zur Unterstützung von VRay Material (VRayMtl)
* &lbrack;Ebenenstapel&rbrack; Löschen von Ebeneneffekten über das Papierkorbsymbol oder den Tastaturbefehl &quot;Löschen&quot; über die Tastatur zulassen
* Plug-in-Substance Source entfernen (Launcher mit &quot;Senden an&quot;-Funktion verwenden)
* &lbrack;Windows&rbrack; Keine TDR-Warnung auf High-End-GPUs anzeigen

**Fest:**

* Übersetzungsprobleme im Dialogfeld &quot;Neue Projektdatei&quot;
* &lbrack;Baker&rbrack; Die Einstellung &quot;Vorverarbeitete Szene speichern&quot; funktioniert nicht mehr
* &lbrack;Planare Projektion&rbrack; Projektion funktioniert nicht bei Meshs mit sich wiederholenden UVs
* &lbrack;Aufkleber&rbrack; Verhaltensunterschiede im Normalkanal bei Verwendung verschiedener Modi zur Projektion der Füllebene
* &lbrack;Verwischen&rbrack;&lbrack;Klon&rbrack; Beim Malen in einer Maske kann ein Artefakt angezeigt werden
* &lbrack;Engine&rbrack; Absturz mit bestimmtem Ebeneninhalt
* &lbrack;Engine&rbrack; Zufälliger Absturz beim Malen in einigen Fällen
* &lbrack;Ankerpunkt&rbrack; Der Verweis auf eine leere Maske gibt immer Weiß zurück.
* &lbrack;Export&rbrack; Ebene, die in bestimmten Stapel-Konfigurationen nicht berücksichtigt wurde
* &lbrack;Mesh&rbrack; exportieren Export mit Pfad, der Sonderzeichen enthält, nicht möglich
* &lbrack;Mesh&rbrack; exportieren glTF-Dateien können beim Export aus Linux oder MacOS nicht gelesen werden
* &lbrack;Mesh&rbrack; importieren Das erneute Importieren von DAE, PLY oder glTF funktioniert nicht wie beabsichtigt

**Bekannte Probleme:**

* &lbrack;Skripterstellung&rbrack;&lbrack;JavaScript&rbrack; Die Baker-Einstellungen für neue Krümmungen können nicht bearbeitet werden.
* &lbrack;Baker&rbrack; Absturz unter Linux mit GPU-Raytracing
* &lbrack;Export&rbrack;&lbrack;USD&rbrack; Die deaktivierten Textursatz sollten nicht exportiert werden
* &lbrack;Absturz&rbrack; Shader nach dem Malen einer Maske in einer Material-Ebene ändern

## Version 5

### 5.3.3 (2019.3.3)

*(Freigegeben: 06. Februar 2020*)Zusammenfassung: **Bugfix mit Upgrade auf Iray 2019.3**

**Hinzugefügt:**

* Upgrade auf Iray 2019.3
* &lbrack;Log&rbrack; Veraltetes BIOS für Ryzen-CPU anzeigen, was beim Baking zu Abstürzen führt
* &lbrack;ABR&rbrack; ABR-Alphas nach Regal extrahieren

**Fest:**

* &lbrack;Baker&rbrack; Baking schlägt fehl, wenn der High-Poly-Mesh keine UVs enthält
* &lbrack;Linux&rbrack; Benutzerdefinierte Mauskürzel werden nicht gespeichert
* &Klammer;Pinsel&Klammer; Die Kontur verschwindet mit einigen Alpha-Formen
* &Klammer;Tablet&Klammer; Fehlerhafte Erkennung beim Verschieben von Schiebereglern
* &blbrack;Shortcuts&rbrack; Mit &quot;Strg+Alt+Mausklick&quot; kann kein Tastaturbefehl eingerichtet werden
* &lbrack;Regal&rbrack; Die Ressourcen-QuickInfo wird bei Verwendung eines Stift-Tablets nicht angezeigt
* &lbrack;2D-Ansicht&rbrack;&lbrack;Export&rbrack; Die Voreinstellung &quot;2D-Ansicht&quot; berücksichtigt nicht die normalen Informationen.
* Einfrieren beim Malen in UV-Ausrichtung mit bestimmten Pinseln
* Malen unter einem Filter erzeugt Artefakt auf dem laufenden Strich
* &lbrack;Viewport&rbrack; Falscher Texturen-Cache im Viewport nach dem erneuten Importieren eines Meshs
* &lbrack;Absturz&rbrack; Fehler beim Speichern nach dem Export in Photoshop
* &lbrack;Absturz&rbrack; Schreiben spezieller Symbole im Präfix beim Importieren von Ressourcen
* &lbrack;Absturz&rbrack; Klicken Sie in den Ankerpunkt-Eigenschaften auf die Referenz
* &lbrack;Ankerpunkte&rbrack; Kanal wird nicht aktualisiert, wenn ein Filter zwischen Ankerpunkt und Referenz vorhanden ist
* Iray-URL-Link im Hilfemenü funktioniert nicht

**Bekannte Probleme:**

* &lbrack;UV Entpack&rbrack; Die Verarbeitung von Meshs mit hohem Poly-Anteil kann lange dauern
* &lbrack;UV Entpack&rbrack; Scheitelpunkt an exakt denselben Koordinaten werden zusammengeführt
* &lbrack;UV Entpack&rbrack; UV-Generierung kann in seltenen Fällen auf bestimmten Mesh-Komponenten fehlschlagen
* &lbrack;UV Entpack&rbrack; Uneinheitliches oder stark verzerrtes Textilverhältnis in einer einzigen UV-Insel in einigen Fällen
* &lbrack;UV Entpack&rbrack; Nicht einheitliches Textilverhältnis zwischen Textursätzen
* &lbrack;UV Entpack&rbrack; Die erzeugte UV-Insel kann sehr lang sein und in manchen Fällen nicht in den UV-Raum passen
* &lbrack;UV Entpack&rbrack; Degenerierte Flächen oder nicht dreieckige Mesh-Flächen mit kleinen oder überlappenden Kanten werden möglicherweise nicht in UV entpackt

### 5.3.2 (2019.3.2)

*(Freigegeben: 21. Januar 2020 (1&rbrace;)Zusammenfassung:**Bugfix***

**Fest:**

* Beim Öffnen eines Projekts, das im Einzelkanalmodus gespeichert wurde, wird der Mesh nicht angezeigt
* Viewport wird beim Malen unter einer Ebene mit dem Kopierwerkzeug nicht immer aktualisiert

**Bekannte Probleme:**

* &lbrack;Baker&rbrack; Absturz im Zusammenhang mit Multithreading auf Ryzen-CPUs
* &lbrack;UV Entpack&rbrack; Die Verarbeitung von Meshs mit hohem Poly-Anteil kann lange dauern
* &lbrack;UV Entpack&rbrack; Scheitelpunkt an exakt denselben Koordinaten werden zusammengeführt
* &lbrack;UV Entpack&rbrack; UV-Generierung kann in seltenen Fällen auf bestimmten Mesh-Komponenten fehlschlagen
* &lbrack;UV Entpack&rbrack; Uneinheitliches oder stark verzerrtes Textilverhältnis in einer einzigen UV-Insel in einigen Fällen
* &lbrack;UV Entpack&rbrack; Nicht einheitliches Textilverhältnis zwischen Textursätzen
* &lbrack;UV Entpack&rbrack; Die erzeugte UV-Insel kann sehr lang sein und in manchen Fällen nicht in den UV-Raum passen
* &lbrack;UV Entpack&rbrack; Degenerierte Flächen oder nicht dreieckige Mesh-Flächen mit kleinen oder überlappenden Kanten werden möglicherweise nicht in UV entpackt

### 5.3.1 (2019.3.1)

*(Freigegeben: 20. Dezember 2019*)Zusammenfassung: **Hotfix**

**Fest:**

* Absturz bei der Arbeit an Meshs mit bestimmten UV-Projektionen
* &lbrack;ABR&rbrack; Absturz beim Wechseln zwischen Photoshop-Vorgaben
* &lbrack;Linux&rbrack; Substance Painter kann unter CentOS 7.4 aufgrund eines libGLX-Abhängigkeitsproblems nicht gestartet werden
* &lbrack;Baker&rbrack; Absturz beim Baking nach Verwendung von &quot;Datei&quot; > &quot;Bereinigen&quot;
* &lbrack;Baker&rbrack; Baking-Fortschrittsdialog friert nach Abbruch ein
* &lbrack;Baker&rbrack; Baking von Mesh nach dem Exportieren von Texturen funktioniert nicht
* &lbrack;Baker&rbrack; Verwenden von &quot;Nach Name abgleichen&quot; mit schwarzen Mesh-Map
* &lbrack;Baker&rbrack; Käfig wird nicht berücksichtigt
* &lbrack;Regal&rbrack; Das Importieren von PSD-Dateien führt zu fehlerhaften Bildern
* &lbrack;Beispiel&rbrack; &quot;Matte&quot;-Beispielprojekt hat fehlerhafte Kameras und falsche Exportvorgabe

**Bekannte Probleme:**

* &lbrack;Baker&rbrack; Absturz im Zusammenhang mit Multithreading auf Ryzen-CPUs
* &lbrack;UV Entpack&rbrack; Die Verarbeitung von Meshs mit hohem Poly-Anteil kann lange dauern
* &lbrack;UV Entpack&rbrack; Scheitelpunkt an exakt denselben Koordinaten werden zusammengeführt
* &lbrack;UV Entpack&rbrack; UV-Generierung kann in seltenen Fällen auf bestimmten Mesh-Komponenten fehlschlagen
* &lbrack;UV Entpack&rbrack; Uneinheitliches oder stark verzerrtes Textilverhältnis in einer einzigen UV-Insel in einigen Fällen
* &lbrack;UV Entpack&rbrack; Nicht einheitliches Textilverhältnis zwischen Textursätzen
* &lbrack;UV Entpack&rbrack; Die erzeugte UV-Insel kann sehr lang sein und in manchen Fällen nicht in den UV-Raum passen
* &lbrack;UV Entpack&rbrack; Degenerierte Flächen oder nicht dreieckige Mesh-Flächen mit kleinen oder überlappenden Kanten werden möglicherweise nicht in UV entpackt

### 5.3.0 (2019.3.0)

*(Freigegeben: 17. Dezember 2019*)Zusammenfassung: **Hauptversion mit Verbesserung der Benutzererfahrung beim Handmalen, Arbeiten mit Tablets, automatischem UV entpack in der Beta-Version (0.3.0) und verschiedenen neuen Inhalten zum Handmalen**

**Hinzugefügt:**

* Integration von Automatic UV entpack 0.3.0 in Substance Painter
* &lbrack;UV entpack&rbrack; Automatische UV entpackend im Substance Painter, wenn keine UVs oder partielle UVs vorhanden sind
* &lbrack;UV entpack&rbrack; Eine globale Einstellung zum Aktivieren und Deaktivieren
* &lbrack;UV entpack&rbrack; In Protokolldatei gemeldete Version
* &lbrack;UV entpack&rbrack;&lbrack;UI&rbrack; Anzeige des Fortschritts beim Entpack der UV
* &lbrack;UI&rbrack; Neue Einstellungen in der kontextabhängigen Symbolleiste zum Auswählen der Pinselvorschau: Vollständige Vorschau, Pinselkontur und Fadenkreuz
* &lbrack;Werkzeug&rbrack; Neuer erweiterter Mischmodus im Alpha-Bereich: Aufhellen (Maximal) zusätzlich zu Normal
* &lbrack;Ebenenstapel&rbrack; Gammakorrekturoption pro Ebene für Alpha oder Maske (Kontextmenü)
* &lbrack;Ebenenstapel&rbrack;&lbrack;UI&rbrack; Symbol &quot;i&quot; hinzufügen, wenn Alpha-Ebene gamma-korrigiert wurde
* &lbrack;Tablet&rbrack;&lbrack;Tool&rbrack; Gelegt Mindestdruck für Größe und Durchfluss
* &lbrack;Tablet&rbrack;&lbrack;UI&rbrack; Neue Einstellung in der kontextabhängigen Symbolleiste, um den Kurvendruck auszuwählen: linear, easy-in, easy-in-out
* &lbrack;Tablet&rbrack;&lbrack;UX&rbrack; Strg- + Alt-Taste + Klicken zum Bildlauf hinzufügen
* Photoshop-Pinselvorgaben importieren (ABR-Format)
* &lbrack;ABR&rbrack; Unterstützen von Shape-Parametern
* &lbrack;ABR&rbrack; Unterstützung von Parametern für die Formdynamik
* &lbrack;ABR&rbrack; Support-Übertragungsparameter
* &lbrack;ABR&rbrack; Unterstützung von Streuungsparametern
* &lbrack;ABR&rbrack;&lbrack;Dynamischen Pinselstriche&rbrack; Rundheit und Spiegelung unterstützen
* &lbrack;ABR&rbrack;&lbrack;Regal&rbrack; Leg der Pinselordnerstruktur im Filtereditor
* &lbrack;ABR&rbrack;&lbrack;Regal&rbrack; Photoshop-Symbol zu Miniaturansichten hinzufügen
* &lbrack;ABR&rbrack;&lbrack;Regal&rbrack; Liste nicht unterstützter Parameter in der detaillierten Miniaturansicht der ABR hinzufügen
* &lbrack;Tool&rbrack;&lbrack;Dynamischen Pinselstriche&rbrack; Neue dynamische Stricheinstellung zur Steuerung der Anzahl der zu erzeugenden Zufallszahlen
* &lbrack;Tool&rbrack;&lbrack;UI&rbrack; Neue Verteilungs- und Achse-Einstellungen für Streuungs-Jitter hinzufügen
* &lbrack;Tastaturbefehl&rbrack; Füge Strg+Umschalt+B hinzu, um das Baking-Fenster zu öffnen.
* &lbrack;UI&rbrack;&lbrack;Menu&rbrack; Eintrag im Menü &quot;Bearbeiten&quot; hinzufügen, um das Baking zu öffnen
* &lbrack;UI&rbrack;&lbrack;Einstellungen&rbrack; Verbesserung der Ausrichtung der Liste der Tastaturbefehle
* &lbrack;UI&rbrack; Drucksteuerelemente (Größe und Fluss) durch Schaltflächen zum Ein- und Ausschalten ersetzen
* &lbrack;Viewport&rbrack; Separates Fokussieren von 2D- und 3D-Viewport zulassen
* Update auf QT 5.12.5
* &lbrack;UI&rbrack; Ladevorgang des Meshs anzeigen
* &lbrack;Substance&rbrack; Zusätzliche Unterstützung für nicht geklemmten und weichen Bereich mit Schiebereglern
* &lbrack;Substance&rbrack; Präzision der Substance-Parameter auf bis zu 6 Dezimalstellen erhöhen
* &lbrack;Substance&rbrack; Berücksichtigung des durch einen Parameter definierten Schritts
* &lbrack;Substance&rbrack; Optimieren der dynamischen Konturgenerierung mit Unterstützung von Bedingungen in Benutzerdaten
* &lbrack;Substance&rbrack; Graphausgabe als Maske für alle Kanäle über Benutzerdaten festlegen
* &lbrack;Inhalt&rbrack; Update &#39;Mat&#39; Beispielprojekt mit Versatz-freundlicher Topologie, neuer ID-Map und neuen Kameras
* &lbrack;Inhalt&rbrack; 3 neue Filter (MatFx) integrieren: Comic-Buch, Aquarell, Öl-Malen (inspiriert von der Arbeit von Emrecan Cubukcu)
* &lbrack;Inhalt&rbrack; 102 Photoshop-Pinselvorgaben aus den Packs von Kyle T. Webster integrieren
* &lbrack;Inhalt&rbrack; 18 neue Pinselvorgaben integrieren: Malen Roller Arrow, Malen Roller Warning text, Charcoal Fine und mehr
* &lbrack;Inhalt&rbrack; 9 neue Alphas integrieren: Brush Maker Malen Roller, Brush Maker Photoshop, Pinselmuster und mehr
* &lbrack;Inhalt&rbrack; 2 neue Werkzeugvorgaben integrieren: Gouache Dense und Gouache Faded
* &lbrack;Inhalt&rbrack; 1 neuen Generator integrieren : UV-Checker (UV-Inseln und Nähte hervorheben)
* &lbrack;Inhalt&rbrack; 2 neue Exportvorgaben integrieren: Keyshot 9+ und Spark AR Studio
* &lbrack;Inhalt&rbrack; 1 neue Projektvorlage integrieren : Spark AR Studio (Facebook)

**Fest:**

* &Klammer;Tablet&Klammer; Das Rückgängigmachen von Stiftstrichen (Strg+Z) hinkt mehr hinterher als das Rückgängigmachen von Mausstrichen
* &Klammer;Tablet&Klammer; Anfangs- und Enddruck werden beim Zeichnen einer Geraden nicht berücksichtigt
* &Klammer;Tablet&Klammer; Erster Stempel wird zweimal gezeichnet, wenn eine gerade Linie verwendet wird
* &Klammer;Tablet&Klammer; Verbesserte Unterstützung für Huion-Tablet-Tastaturbefehle
* &Klammer;Tablet&Klammer; Verbesserte Unterstützung für Huion-Stift-Schaltflächen
* &Klammer;Tablet&Klammer; Versatz zwischen der Pinselvorschau und dem gezeichneten Stempel
* &Klammer;Tablet&Klammer; Verknüpfungen zum Ändern von Pinseln mit Stift führen in seltenen Fällen zu geringer Leistung
* &Klammer;Tablet&Klammer; Verzögerung beim Malen auf einer bestimmten Ebene
* Unscharfe Texturen können in seltenen Fällen beim Wechseln des Viewport auftreten
* &lbrack;UI&rbrack;&lbrack;Substance&rbrack; Bildeingaben werden nicht immer angezeigt
* Beim Bereinigen werden keine Vorgaben aus dem Regal entfernt, die in ein Projekt importiert wurden
* &lbrack;Werkzeug&rbrack;&lbrack;Dynamischer Strich&rbrack; Leistungsproblem beim Anpassen der Stempelzyklusanzahl
* Aktualisierungsprobleme beim Malen im 3D/2D-Viewport in seltenen Fällen
* Wenn Sie einen sehr langen Pinselstrich zeichnen, kann dies zum Einfrieren führen
* &lbrack;Werkzeug&rbrack; Leistungsproblem beim Malen mit bestimmten Dynamischen Pinselstrichen
* &lbrack;UI&rbrack; Kontextsymbolleiste zeigt weiterhin Pinseleigenschaften an, wenn ein Ordner ausgewählt wird
* Werte für die Achse der Symmetrie werden nicht zurückgesetzt
* Import von EXR Texturen mit Fließkommawerten sind komplett schwarz
* Alt+Klicken auf einen Kanal zum Isolieren funktioniert nicht für Filter und Generator
* &lbrack;Export&rbrack; Spezifische Projekt-Absturz beim Exportieren
* &lbrack;Substance&rbrack; Falscher Standardwert in der Dropdown-Liste, wenn der Parameter von Visible If ausgeblendet ist
* &lbrack;Shader&rbrack; Kanäle, die über Material-Ebenen definiert werden, werden in der Benutzeroberfläche nicht gleich sortiert
* &lbrack;Regal&rbrack; Vorgabenmetadaten werden nicht auf dem Datenträger gespeichert

**Bekannte Probleme:**

* &lbrack;UV Entpack&rbrack; Die Verarbeitung von Meshs mit hohem Poly-Anteil kann lange dauern
* &lbrack;UV Entpack&rbrack; Scheitelpunkt an exakt denselben Koordinaten werden zusammengeführt
* &lbrack;UV Entpack&rbrack; UV-Generierung kann in seltenen Fällen auf bestimmten Mesh-Komponenten fehlschlagen
* &lbrack;UV Entpack&rbrack; Uneinheitliches oder stark verzerrtes Textilverhältnis in einer einzigen UV-Insel in einigen Fällen
* &lbrack;UV Entpack&rbrack; Nicht einheitliches Textilverhältnis zwischen Textursätzen
* &lbrack;UV Entpack&rbrack; Die erzeugte UV-Insel kann sehr lang sein und in manchen Fällen nicht in den UV-Raum passen
* &lbrack;UV Entpack&rbrack; Degenerierte Flächen oder nicht dreieckige Mesh-Flächen mit kleinen oder überlappenden Kanten werden möglicherweise nicht in UV entpackt
* Das Metamat-Beispiel hat einige Probleme mit importierten Kameras

### 5.2.3 (2019.2.3)

*(Freigegeben: 23. Oktober 2019*)Zusammenfassung: **Bugfix-Version**

**Hinzugefügt:**

* &lbrack;Textursatz Liste&rbrack; Schaltfläche &quot;Hinzufügen&quot; zum schnellen Aktivieren/Deaktivieren des Fokusmodus
* &lbrack;Log&rbrack; Windows 10-Versionsnummer in die Protokolldatei einfügen
* Aktualisieren Sie auf die neueste Version von Substance Engine
* &lbrack;MacOS&rbrack; Die Software wurde notariell beglaubigt, um die neuen Verteilungsanforderungen von MacOS Catalina zu erfüllen

**Fest:**

* &lbrack;Plugin&rbrack; Plug-In-Quelle funktioniert nicht
* &lbrack;MacOS&rbrack;&lbrack;Shader&rbrack; Mac OS 10.14.5 und AMD: Material-Ebenen funktionieren nicht wie vorgesehen

**Bekannte Probleme:**

* Alembic-Dateien mit Unterteilungen können nicht importiert werden
* Seltene Absturz beim Importieren einiger Alembic-Dateien
* Benutzeroberfläche reagiert beim Baking führ mit DXR auf Pascal-GPUs vorübergehend nicht

### 5.2.2 (2019.2.2)

*(Freigegeben: 20. September 2019*)Zusammenfassung: **Bugfix-Version**

**Fest:**

* Das Importieren von Ressourcen durch Skripterstellung kann zu einem Absturz führen
* &lbrack;Plugin&rbrack; Das Herunterladen des Materials von der Quelle kann zu einem Absturz führen

**Bekannte Probleme:**

* Alembic-Dateien mit Unterteilungen können nicht importiert werden
* Seltene Absturz beim Importieren einiger Alembic-Dateien
* Benutzeroberfläche reagiert beim Baking führ mit DXR auf Pascal-GPUs vorübergehend nicht

### 5.2.1 (2019.2.1)

*(Freigegeben: 17. September 2019 (1&rbrace;)Zusammenfassung:**Bugfix-Version***

**Fest:**

* &lbrack;Mac&rbrack;&lbrack;USD&rbrack; Exportierte USDZ-Dateien aus MacOS können nicht geöffnet werden
* &lbrack;Textursatz&rbrack; Es ist nicht möglich, einen Textursatz mit dem ALT-Modifikator zu isolieren
* &lbrack;Regal&rbrack; Vorgaben, Intelligente Materialien und Intelligente Masken werden beim Beenden der Anwendung immer geändert
* &lbrack;Ebenenstapel&rbrack; Effekt kann nach dem Löschen eines anderen Effekts nicht ausgewählt werden
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

* &lbrack;Baker&rbrack; Neue Unterstützung für GPU-Raytracing mit DXR und OptiX (Ambient occlusion, Thickness)
* &lbrack;Baker&rbrack; Optimierungen und Beschleunigungen für CPU-Raytracing
* &lbrack;Baker&rbrack;&lbrack;vis mode&rbrack;&lbrack;UI&rbrack; Neuer Baking-Visualisierungsmodus im Viewport
* &lbrack;Baker&rbrack;&lbrack;Voreinstellungen&rbrack;&lbrack;UI&rbrack; Neue Baking-Option zum Aktivieren/Deaktivieren von GPU-Raytracing
* &lbrack;Baker&rbrack;&lbrack;UI&rbrack; Überarbeitung des Dialogfelds &quot;Fortschrittsleiste&quot;
* &lbrack;Baker&rbrack; Verbesserung von Warn- und Fehlermeldungen
* &lbrack;Baker&rbrack; Reaktionsfähigeres Abbrechen des Bakings zulassen
* &lbrack;Baker&rbrack; Baking-Fenster nach Klicken auf &quot;Abbrechen&quot; erneut öffnen
* &lbrack;Proj&rbrack;&lbrack;UX&rbrack; Verbesserte Verwendbarkeit des Manipulators der Drehung
* &lbrack;Einstellungen&rbrack; Option zur Leistungssteigerung durch Reduzierung der Viewport-Auflösung für HDPI-Bildschirme
* &lbrack;Skripterstellung&rbrack; Ändern der Textursatz auflösung
* &lbrack;Skripterstellung&rbrack; Ausgewählten Textursatz abrufen
* &lbrack;Skripterstellung&rbrack; Auswahl eines Textursatzes durch den Benutzer zulassen
* &lbrack;Skripterstellung&rbrack; Funktion, um zu erfahren, wann die Auswahl des Textursatzes geändert wurde
* &lbrack;Regal&rbrack; 40 neue intelligente Materialien hinzugefügt
* &lbrack;Regal&rbrack; 20 neue intelligente Masken hinzugefügt

**Fest:**

* &lbrack;Ebenenstapel&rbrack; Einfrieren der Benutzeroberfläche bei Mehrfachauswahl von Ebenen
* &lbrack;Ebenenstapel&rbrack; Beim Gruppieren vieler Ebenen wird die Benutzeroberfläche länger als gewöhnlich fixiert.
* &lbrack;Ebenenstapel&rbrack; In einigen Fällen können eine Ebene und ein Effekt gleichzeitig ausgewählt werden.
* In Malwerkzeugen verwendete Substance-Graf werden nicht mit der richtigen Auflösung generiert
* &lbrack;Baker&rbrack; Die Schaltfläche &quot;Alle Textursatz Baking geführt&quot; ist nicht deaktiviert, wenn keine Baker ausgewählt sind
* &lbrack;MacOS&rbrack; Warnmeldung zur Tessellation deaktivieren
* Bei Verwendung mit einer Projektion hat das Maskierungswerkzeug keine Vorschau.
* Absturz und beschädigte Projekte beim Speichern mit zu wenig Speicherplatz
* &lbrack;Regal&rbrack; Absturz beim Importieren einer Ressource auf dem Datenträger über ein Regal mit nicht genügend Speicherplatz
* &lbrack;Regal&rbrack; Absturz beim Wiederherstellen der Sitzungsvorgabe
* &lbrack;Regal&rbrack; Das Importieren einer Vorgabe mit einem Namen, der mit einem Leerzeichen endet, führt zu einem Absturz
* &lbrack;Regal&rbrack; Das Importieren einer Ressource mit einem Präfix, das mit einem leeren Leerzeichen endet, führt zu einem Absturz

**Bekannte Probleme:**

* Alembic-Dateien mit Unterteilungen können nicht importiert werden
* Seltene Absturz beim Importieren einiger Alembic-Dateien
* Benutzeroberfläche reagiert beim Baking führ mit DXR auf Pascal-GPUs vorübergehend nicht

### 5.1.3 (2019.1.3)

*(Freigegeben: 1. Juli 2019 (1&rbrace;)Zusammenfassung:**Bugfix mit 2 neuen Funktionen***

**Hinzugefügt:**

* Geben Sie das VRam-Budget über eine Befehlszeile (z. B. —vram-budget 4096)
* &lbrack;QML&rbrack; Leg von wrapMode und elide-Eigenschaften von QML-Schaltflächen und -Kontrollkästchen

**Fest:**

* &quot;Pfad folgen&quot; funktioniert nicht immer
* Kanalzuordnung funktioniert nicht mit SBSAR, das in Ein Kanal-Steckplätzen verwendet wird
* &lbrack;Ebenenstapel&rbrack; Niedrige Leistung beim Scrollen mit ausgeblendeten Ebenen
* &lbrack;TextureSet&rbrack; Absturz beim Klicken zwischen Masken
* &lbrack;SVT&rbrack; Versatz wird nicht richtig angezeigt und flackert in einigen Fällen
* &lbrack;Alembic&rbrack; Absturz mit Mesh, der Punktnormalen anstelle von Scheitelpunkt-Normalen verwendet
* &lbrack;Alembic&rbrack;&lbrack;Log&rbrack; Berichtsfehler im Protokoll, wenn Alembic-Datei während des Imports nicht unterstützt wird

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

* &lbrack;Substance&rbrack; Visible If wird bei Eingabebildern nicht berücksichtigt
* &lbrack;SVT&rbrack;&lbrack;Engine&rbrack; Das Ändern der Textursatz-Auflösung führt in einigen Fällen zu einem Absturz
* &lbrack;Engine&rbrack; In einigen Fällen werden zufällige schwarze Texturen angezeigt
* &lbrack;Ebenenstapel&rbrack;&lbrack;UI&rbrack; Durch Umschalten einer Maske mit UMSCHALTTASTE können mehrere Ebenen gleichzeitig ausgewählt werden
* &lbrack;Ebenenstapel&rbrack; Deckkraft hat keine Auswirkungen auf den Malen-Effekt mit dem Mischmodus &quot;Hindurchwirken&quot;
* &lbrack;Ebenenstapel&rbrack; Filtereingabe &quot;Height zu Normal&quot; wird mit dem Pinselstrich des Radiergummis nicht richtig aktualisiert
* &lbrack;LayersStack&rbrack; Absturz beim Rückgängigmachen des Abfalls einer intelligente Maske
* Flackerndes Drahtgitter mit aktiviertem temporalem Anti-Aliasing
* &lbrack;Versatz&rbrack; Verzögerung bei AMD mit einigen starken Meshs
* &lbrack;Windows&rbrack; Absturz beim Öffnen einiger Projekte über den Datei-Explorer
* &lbrack;Histogramm&rbrack; Absturz beim Entfernen einer Maske mit Ankerpunkt in einigen Fällen
* Absturz bei der Vorschauerstellung in einigen seltenen Fällen
* &lbrack;Absturz&rbrack; Ein Projekt kann mit zu vielen Klon- und Verwischen-Werkzeugen nicht erneut geöffnet werden
* Nach dem Speichern wird in einigen Fällen kein Mesh im Materialmodi angezeigt
* &lbrack;Skripterstellung&rbrack; alg.mapexport.documentStructure() gibt falsche Werte für Ordner zurück

**Bekannte Probleme:**

* Durch Doppelklicken auf den Namen des Textursatzes wird dieser vor dem Umbenennungsmodus ausgewählt.

### 5.1.0 (2019.1.0)

*(Freigegeben: 23. April 2019*)Zusammenfassung: **Dynamischer Pinselstrich mit eigenem neuen Inhalt, Versatz und Tessellation in Echtzeit und Iray, Effekt &quot;Vergleichsmaske&quot;, Radiale Symmetrie, Planar und Sphärische Projektion**

**Hinzugefügt:**

* &lbrack;Werkzeug&rbrack; Dynamischer Strich: Substance-Variation entlang eines Pinselstrichs
* &lbrack;Dynamischer Strich&rbrack; Leg eines neuen Stempelindexparameters mit Optionen
* &lbrack;Dynamischer Strich&rbrack; $time-Parameter berücksichtigen
* &lbrack;Dynamischer Strich&rbrack; Neuen Parameter $randomseed pro Strich und Stempel generieren
* &lbrack;Dynamischer Strich&rbrack; Dynamischen Strichindex aus einer zufälligen Zahl beginnen
* &lbrack;Dynamischer Strich&rbrack;&lbrack;Regal&rbrack; Hilfe bei der Suche nach einer dynamischen Konturressource mit eigenem neuen Symbol
* Versatz und Tessellation im Echtzeit-Viewport
* Versatz und Tessellation in Iray
* &lbrack;Shader-Einstellungen&rbrack;&lbrack;UI&rbrack; Neue Registerkarte zur Steuerung von Versatz und Tessellation
* &lbrack;Ebenenstapel&rbrack; Neuer Effekt &quot;Maske vergleichen&quot;: durch Vergleich zweier Kanäle eine Maske generieren
* &lbrack;Ebenenstapel&rbrack;&lbrack;UI&rbrack; Neuer Eintrag im Rechtsklick-Menü &quot;Height mit Maskenkombination hinzufügen&quot;, um einen CompareMask-Effekt einzufügen
* &lbrack;Symmetrie&rbrack; Neuer Symmetrie-Modus: Radialmalerei
* &amp;Symmetrie&rbrack;Einstellungen&rbrack; Erweitern Sie beide Abschnitte &quot;Einstellungen&quot; und &quot;Anzeige&quot;
* &lbrack;Symmetrie&rbrack;&lbrack;UI&rbrack; Vorschau für radiales Malen
* Leg zweier neuer Modi für die Projektion: planar und kugelförmig
* &lbrack;Proj&rbrack; Neuer Formzuschneidemodus für alle Projektionen
* &lbrack;Proj&rbrack; Planarer Modus mit neuem Manipulator: Oberflächenwerkzeug
* &lbrack;Proj&rbrack;&lbrack;Tastaturbefehl&rbrack; Tastaturbefehl UMSCHALTTASTE+W für Oberflächenwerkzeug
* &lbrack;Proj&rbrack; Planare Maskierung von Projektionen mit Tiefe ausblenden und Rückseiten-Ausblendung
* &lbrack;Manipulator&rbrack; Verbesserung des Manipulators der Drehung auf allen drei Achsen für triplanare
* &lbrack;Tool&rbrack;&lbrack;UX&rbrack; Alt-Klick auf einen Kanal fokussiert diesen Kanal (aktiviert ihn oder deaktiviert alle anderen)
* &lbrack;Engine&rbrack; Aktualisieren Sie auf die neueste Version von Substance Engine
* &lbrack;Textursatz&rbrack; Mehrfachauswahl und Änderung der Auflösung
* &lbrack;Textursatz&rbrack; Schnelle Aktivierung und Deaktivierung der Textursatz
* &lbrack;Textursatz&rbrack; Einzelne und alle Optionen zu einem neuen Menü kombinieren
* &lbrack;Textursatz&rbrack;&lbrack;Ebenenstapel&rbrack; Neues Symbol für die Aktivierung und Deaktivierung
* &lbrack;Ebenenstapel&rbrack;&lbrack;UX&rbrack; Einfügen von Effekten über den bereits ausgewählten
* &lbrack;Ebenenstapel&rbrack;&lbrack;UI&rbrack; Auswahlstil für die Ebenenstapel-Ansicht überarbeiten
* &lbrack;Ebenenstapel&rbrack; Der Mischmodus für instanzierte Ebenen ist jetzt standardmäßig im Durchlaufmodus
* &lbrack;Export&rbrack; Option zum Aktivieren und Deaktivieren von Dithering
* &lbrack;Plugin&rbrack; Präzisionsmodifikator für Schieberegler unterstützen (SHIFT)
* &lbrack;Plugin&rbrack;&lbrack;UI&rbrack; Neues Symbol für automatisches Speichern
* &lbrack;Skripterstellung&rbrack; Auflisten des Inhalts eines Ordners
* &lbrack;Skripterstellung&rbrack; Löschen von Dateien zulassen
* &lbrack;Skripterstellung&rbrack; Lesen aller Stapel-Informationen, einschließlich der verwendeten Ressourcen
* &lbrack;Inhalt&rbrack;&lbrack;Dynamischer Strich&rbrack; Neue Tools und Pinselvorgaben
* &lbrack;Inhalt&rbrack;&lbrack;Dynamischer Strich&rbrack; Zwei neue prozedurale Farbverläufe: Farbton und Verlaufsgenerator
* &lbrack;Inhalt&rbrack; 11 neue Filter: MatFx Peeling Malen, MatFx Wassertropfen und mehr
* &lbrack;Inhalt&rbrack; 7 neue Generatoren: &quot;Auto-Stitcher&quot;, &quot;UV-Zufallsfarbe&quot;, &quot;UV-Texeldichte&quot; und weitere Eigenschaften
* &lbrack;Inhalt&rbrack; 93 neue Alphas: neue Texte, Pfeile und verschiedene andere Formen
* &lbrack;Inhalt&rbrack; 2 neue Verfahren: Verlaufsfarbton, Verlaufsgenerator und mehr
* &lbrack;Inhalt&rbrack; 21 neue Tools und Pinselvorgaben für Dynamische Pinselstriche: Kiesel, Fußabdrücke, Spray und mehr
* &lbrack;Inhalt&rbrack; 2 Neue HDRs: Canopus Boden- und Herbstwald
* &lbrack;Inhalt&rbrack; Aktualisieren von Inhalten mit Kuration nach dem Zufallsprinzip in Regal
* &lbrack;Inhalt&rbrack; Neues Symbol mit gelegt Zufallsparameter in Regal

**Fest:**

* &lbrack;Ebenen Stapel&rbrack; Ebenenstapel wird unendlich lang.
* &lbrack;Mac&rbrack; &quot;Im Finder anzeigen&quot; kann zum Einfrieren führen
* &lbrack;Skripterstellung&rbrack; Einstellungen, die über die benutzerdefinierte Benutzeroberfläche gespeichert wurden, gehen verloren, wenn die Shader-Datei verschoben wird
* &lbrack;Skripterstellung&rbrack; Die API-Versionsnummer ist falsch und nicht aktuell.
* &blase;Effekt&blase; Histogramminhalt wird nicht korrekt angezeigt
* &blase;Effekt&blase; Histogrammeffekt wird in einigen Fällen nicht aktualisiert
* &lbrack;Regal&rbrack; Die Nähte sind auf dem Material &quot;Plastic Fabric Pyramide&quot; nicht richtig ausgerichtet.

**Bekannte Probleme:**

* Durch Doppelklicken auf den Namen des Textursatzes wird dieser vor dem Umbenennungsmodus ausgewählt.
* &lbrack;Ebenenstapel&rbrack;&lbrack;UI&rbrack; Durch Umschalten einer Maske mit UMSCHALTTASTE können mehrere Ebenen gleichzeitig ausgewählt werden

## Version 4

### 4.3.3 (2018.3.3)

*(Freigegeben: 07. März 2019*)Zusammenfassung: **Bugfix**

**Hinzugefügt:**

* &lbrack;Inhalt&rbrack; Neue Projektvorlage integrieren: &quot;PBR - Metallische Rauheit Alpha-blend&quot;
* Die Suchreihenfolge der dynamischen Linux-Bibliothek wurde geändert, um Bibliotheken im Installationsverzeichnis Priorität einzuräumen, bevor sie auf dem System installiert werden.

**Fest:**

* Mesh verschwindet manchmal vom 3D-Viewport (drücken Sie F, um die Kamera zurückzusetzen)
* Aktualisieren des Substance Painter Sketchfab-Uploaders mit den neuen Sketchfab-Lizenztypen
* &lbrack;Import&rbrack;&lbrack;glTF&rbrack; Falsche Handhabung der Modulation der Eingabe-Textur wie in glTF-Dateien definiert
* &lbrack;Import&rbrack;&lbrack;glTF&rbrack; Boden-Ebene wird beim glTF-Import in einigen Fällen falsch angezeigt
* &lbrack;Export&rbrack;&lbrack;USD&rbrack; Deckkraft funktioniert nicht in Arkit
* &lbrack;Export&rbrack;&lbrack;USD&rbrack; ABSTURZ beim USDz-Export in einigen Fällen
* &lbrack;Export&rbrack;&lbrack;USD&rbrack; Exportieren in USD ohne Speichern führt zu Absturz
* &lbrack;Export&rbrack;&lbrack;USD&rbrack; Ungültiger Kachelung-Modus für Texturen, Unterteilungsmodus für Mesh und Ausgabetypen für Shader
* &lbrack;Export&rbrack;&lbrack;USD&rbrack; Wenig Exporte von nur einigen Textursätzen mit allen Geometrien
* &lbrack;Instanz&rbrack; Absturz beim Löschen einer beschädigten Instanzebene
* &lbrack;Regression&rbrack;&lbrack;Export&rbrack; Einige Maps werden nicht in die ausgewählte Bittiefe exportiert
* &lbrack;Linux&rbrack; Problem mit der Bibliothek libtbb.so.2

**Bekannte Probleme:**

* Einfrieren der Berechnung in einigen Fällen auf AMD VEGA-GPUs
* Problem mit Huion-Tablets mit Tastaturbefehlen unter Windows

### 4.3.2 (2018.3.2)

*(Freigegeben: 24. Januar 2019*)Zusammenfassung: **Hotfix mit neuen Funktionen (USDZ-Export- und Textur-Filterungen im Viewport)**

**Hinzugefügt:**

* &lbrack;Export&rbrack; Export nach USDZ zulassen
* &lbrack;Viewport&rbrack; Zulassen, um die Qualität der Textur in den Anzeigeeinstellungen zu steuern
* &lbrack;Viewport&rbrack; Die Einstellung für die MIP-Voreinstellung in den Anzeigeeinstellungen wurde hinzugefügt.
* &lbrack;Viewport&rbrack; Anisotrope Filterung in den Anzeigeeinstellungen hinzugefügt
* &lbrack;plugins&rbrack; Offizielle Plug-ins auf Substance Painter 2018 aktualisieren
* &lbrack;Lizenz&rbrack; Lizenz standardmäßig in einem Benutzerordner installieren

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
* &lbrack;Skripterstellung&rbrack; Dateipfaderstellung beim Speichern eines Projekts nicht erzwungen
* &lbrack;Skripterstellung&rbrack; Der Rückruf von &quot;onProjectAboutToSave()&quot; funktioniert nicht mehr
* Fehlerhafte Links im Fenster &quot;Fehler melden&quot;

**Bekannte Probleme:**

* Einfrieren der Berechnung in einigen Fällen auf AMD VEGA-GPUs
* Problem mit Huion-Tablets mit Tastaturbefehlen unter Windows

### 4.3.1 (2018.3.1)

*(Freigegeben: 06. Dezember 2018*)Zusammenfassung: **Hotfix**

**Hinzugefügt:**

* &lbrack;Symmetrie&rbrack;&lbrack;Viewport&rbrack; Die Symmetrie in der 2D-Ansicht ist wieder da und zeigt nun eine Vorschau des Klonpinsels an.

**Fest:**

* &lbrack;Export&rbrack; Beim Exportieren der 2D-Ansicht wird in einigen Fällen eine schwarze Textur ausgegeben
* &lbrack;Iray&rbrack; Normale Informationen werden im Iray falsch, nachdem eine Material-Ebene instanziiert wurde
* Nicht quadratische Textursatz können in einigen Fällen zu Absturz führen
* &lbrack;Rückgängig&rbrack; Mehrere Strg+Z können in einigen Fällen zufällig zu Absturz führen
* &lbrack;QML&rbrack; AlgScrollView kann in einigen Fällen eine Warnung im Protokoll erstellen (Bindungsschleifen).

**Bekannte Probleme:**

* Einfrieren der Berechnung in einigen Fällen auf AMD VEGA-GPUs
* Problem mit Huion-Tablets mit Tastaturbefehlen unter Windows
* Glätten und Schatten können bei gemeinsamer Verwendung zu unerwarteten Ergebnissen führen

### 4.3.0 (2018.3.0)

*(Freigegeben: 20. November 2018*)Zusammenfassung: **Viewport-Upgrades, ordnungsgemäßer Datenexport, neue UI-Helfer, ein erweitertes Symmetrie-Tool, neue 2D-Ansichten und eine enorme Leistungssteigerung**

**Hinzugefügt:**

* &lbrack;Glätten&rbrack;&lbrack;Viewport&rbrack; Neue temporale Anti-Aliasing-Filterungen für 3D-Viewport (über Anzeigeeinstellungen)
* &lbrack;Export&rbrack; Exportieren des Inhalts des 2D-Viewports als eine Textur
* &lbrack;Export&rbrack;&lbrack;Dithering&rbrack; Gelegt Ditheringe bei der Ausfuhr
* &lbrack;Ebenenstapel&rbrack; Farben auf Ebenen und Ordnern
* &lbrack;Ebenenstapel&rbrack; Schnelle Aktivierung und Deaktivierung mehrerer Ebenen und Effekte
* &lbrack;Ebenenstapel&rbrack; Einfachere Navigation für Füllmethoden dank Tasten nach oben und Mausbildlauf
* &lbrack;Proj&rbrack;&lbrack;UI&rbrack; Zusätzlicher Dreh-Manipulator auf allen drei Achsen für Triplanar
* &lbrack;proj&rbrack;&lbrack;Shorcuts&rbrack; - und + , um die Größe des Manipulators für die UV-Projektion zu ändern
* &lbrack;Shader&rbrack; Kontrolle der Schichtparameter mit Kanälen im PBR-beschichteten Shader
* &lbrack;Substance&rbrack; Leg neuer Mesh-basierter Texturen für Filter und Generatoren
* &lbrack;Symmetrie&rbrack;&lbrack;Viewport&rbrack;&lbrack;UI&rbrack; Steuern des Offsets der Symmetrie mit Manipulatoren
* &lbrack;Symmetrie&rbrack;&lbrack;Kontextsymbolleiste&rbrack;&lbrack;UI&rbrack; Neues Bedienfeld &quot;Symmetrie&quot; mit Optionen
* &lbrack;Symmetrie&rbrack; Neuer Schnittmodus für Symmetrien-Linien
* &lbrack;Symmetrie&rbrack; Neuer Symmetrie-Clone-Cursor
* &lbrack;Symmetrie&rbrack;&lbrack;Shortcuts&rbrack; Q zum Ausblenden und -, + zum Ändern der Größe und Umschalttaste zum einrasten
* &lbrack;Log&rbrack; Fehlermeldungen verbessern, wenn Texturen nicht exportiert werden können
* &lbrack;Skripterstellung&rbrack; Ressourcen in den Anzeigeeinstellungen ändern oder aktualisieren
* &lbrack;Skripterstellung&rbrack; Erstellen oder Entfernen von Kanälen in Textursätzen zulassen
* &lbrack;Content&rbrack;&lbrack;Shaders&rbrack; Unterstützung für Anisotropie mit einem dedizierten Shader hinzufügen (pbr-metal-rau-Anisotropie-angle)
* &lbrack;Inhalt&rbrack; Aktualisierung der Vorschaukugel mit Anisotropie und verändertem Winkel
* &lbrack;Inhalt&rbrack; Aktualisierte matFx Shutline
* &lbrack;Inhalt&rbrack; Neuer nahtloser Fläche-Scan von Texturing.XYZ
* &lbrack;Inhalt&rbrack; Neue anisotrope Verfahren
* &lbrack;Inhalt&rbrack; Neuer Filter: Umgebung mit vorberechnete Beleuchtung
* &lbrack;Inhalt&rbrack; Neue Umgebungs-Map: Studio Automotive Neutral
* &lbrack;Inhalt&rbrack; Neue Projektvorlage: PBR - metallische Rauheit Anisotropy angle (mit Anisotropie-Kanälen)
* &lbrack;Inhalt&rbrack; Neue Projektvorlage: PBR - mit metallische Rauheit beschichtet
* &lbrack;SVT&rbrack;&lbrack;Engine&rbrack; Dünn besetzte virtuelle Texturen (SVT)
* &lbrack;SVT&rbrack;&lbrack;Preferences&rbrack;&lbrack;UI&rbrack; Beschleunigungsoption für SVT-Hardware-Unterstützung
* &lbrack;SVT&rbrack;&lbrack;Log&rbrack; Zusätzliche Informationen zur Funktion &quot;Virtuelle Texturierung mit geringer Dichte&quot; (z. B. Festplatte in Größe)
* &lbrack;SVT&rbrack;&lbrack;UI&rbrack; Meldungsfenster beim Start, wenn die Größe auf dem Datenträger für den Cache zu niedrig ist
* &lbrack;SVT&rbrack;&lbrack;Preferences&rbrack;&lbrack;UI&rbrack; Globaler Substance Painter-Cachespeicherort
* &lbrack;SVT&rbrack; Neue Umgebungsvariable zur Angabe des Cachepfads des Substance Painters
* &lbrack;SVT&rbrack; Neue Umgebungsvariable zum Aktivieren der SVT-Hardware-Support-Beschleunigung
* &lbrack;SVT&rbrack; Erkennen von geringer Hardware-Unterstützung
* &lbrack;SVT&rbrack;&lbrack;Hardware Sparse&rbrack; Erhöhen der Mindesttreiberversion für Nvidia-GPU
* &lbrack;SVT&rbrack;&lbrack;Shader&rbrack;&lbrack;Viewport&rbrack;&lbrack;UI&rbrack; Benutzer warnen, wenn bei Projektöffnung Artefakte mit virtueller Texturierung mit geringer Dichte vorhanden sind

**Fest:**

* &Klammer;Farbwähler&Klammer; Beim Auswählen einer Farbe wird der Cursor angezeigt.
* Absturz durch das Auswählen oder Aufheben der Auswahl von Ebenen in einer bestimmten Reihenfolge kann zu Absturz führen
* Absturz beim Einfügen einer Ebene mit einer Maske als Instanz
* &lbrack;Benutzerkanal&rbrack;&lbrack;Regression&rbrack; Absturz beim Umbenennen des Benutzerkanals
* &lbrack;Benutzerkanal&rbrack; Graue Pinselvorschau
* &lbrack;Alembic&rbrack; Nur ein Textursatz aus mehreren Materialien nach dem Import
* &lbrack;Engine&rbrack; Die exportierte Textur unterscheidet sich vom Viewport für Pinselstempel
* &lbrack;Engine&rbrack; Die Umkehrung mit einem Ebeneneffekt wirkt sich nicht vollständig auf eine Textur aus
* Die Material-Auswahl wendet beim Auswählen einen Pinselstrich an
* Der Wechsel der Auflösung auf 128 x 128 px führt zu einem Absturz
* Mesh-Map-Verknüpfungen werden beim Umbrechen oder Instanziieren von Ebenen nicht ordnungsgemäß aktualisiert
* &lbrack;Substance&rbrack; UserData ColorSpace funktioniert nicht bei Baking geführt Mesh Normal, der als Eingabe angefordert wird
* MDL-Zuordnungskonflikt bei Verwendung mehrerer Shader-Instanzen
* &lbrack;Symmetrie&rbrack;&lbrack;Füllebene&rbrack; Symmetrie-Ebene und ihr in der Füllebene aktiver Manipulator
* &lbrack;Viewport&rbrack; Pivot-Punkt für Übersetzung wird nach dem Klicken nicht immer aktualisiert
* &lbrack;UI&rbrack; Behobene Symbole und Entfernen von Platzhaltern für HDPI-Monitore

**Bekannte Probleme:**

* Einfrieren der Berechnung in einigen Fällen auf AMD VEGA-GPUs
* Problem mit Huion-Tablets mit Tastaturbefehlen unter Windows
* Glätten und Schatten können bei gemeinsamer Verwendung zu unerwarteten Ergebnissen führen

### 4.2.3 (2018.2.3)

*(Freigegeben: 25. September 2018)*

**Fest:**

* &lbrack;2D-Ansicht&rbrack; Beim Erstellen eines neuen Projekts ist die 2D-Ansicht mit einigen Meshs beschädigt
* &lbrack;Absturz&rbrack; Der Wechsel von der UV-Projektion zur planaren Projektion führt zu einem Absturz
* &lbrack;RayCollider&rbrack; Mehrere Absturz durch &quot;RayCollider&quot;
* &lbrack;Werkzeug&rbrack; Beim Wechseln von Ebenen gehen die geänderten Pinseleigenschaften verloren
* Pinseleinstellungen werden beim Wechsel zum Radierer zurückgesetzt

**Bekannte Probleme:**

* Einfrieren der Berechnung auf AMD VEGA-GPUs
* Problem mit Huion-Tablets mit Tastaturbefehlen unter Windows

### 4.2.2 (2018.2.2)

*(Freigegeben: 11. September 2018 (1&rbrace;)Zusammenfassung:**Hotfix mit Inhaltsaktualisierung, neuen Skriptfunktionen und der Möglichkeit, das automatische Update zu deaktivieren***

**Hinzugefügt:**

* &lbrack;Inhalt&rbrack;&lbrack;Regal&rbrack; Hinzufügen einer Skin-Regal-Vorgabe
* &lbrack;Inhalt&rbrack;&lbrack;Regal&rbrack; Konvertierung von 19 Hautnormalen in Materialien zur Volumenstreuung
* &lbrack;Skripterstellung&rbrack; Erstellen einer Projektvorlage aus einem geöffneten Projekt
* &lbrack;Skripterstellung&rbrack; Exporteinstellungen eines geöffneten Projekts abrufen/festlegen
* &lbrack;Updates&rbrack; Deaktivieren des Popups &quot;Automatische Aktualisierung&quot; unter &quot;Einstellungen&quot; und &quot;Umgebungsvariable&quot;
* &lbrack;Updates&rbrack; Nicht bis zur nächsten Version auf dem Popup-Fenster mit veralteten Wartungsoptionen anzeigen

**Fest:**

* &lbrack;Kamera&rbrack; Falscher Zoom durch Wechsel von orthografisch zu Perspektive
* &lbrack;Anzeige&rbrack; Einige Maps werden linear anstatt sRGB angezeigt
* &lbrack;Viewport&rbrack; Mesh-Fokus verhält sich nicht richtig
* &lbrack;2D-Ansicht&rbrack; Bei einem Projekt mit beschädigter Kamera werden UVs-Schalen ausgeblendet.
* &lbrack;SSS&rbrack;&lbrack;Tooltip&rbrack; QuickInfos zu Volumenstreuungen werden im Protokoll angezeigt
* Einige Projekte können nicht in 2018.2 geöffnet werden und die Fehlermeldung kann kein Null-Substance-Paket speichern
* &lbrack;Maske&rbrack; Die Farbe des Malen-Werkzeugs kann beim Arbeiten in einer Maske in einigen Fällen hängen bleiben
* &lbrack;Material&rbrack; Karten werden in bestimmten Situationen nicht angezeigt
* &lbrack;Proj&rbrack;&lbrack;Tools&rbrack; Generatoraktiver Manipulator
* &lbrack;Substance&rbrack; Fehlende Substance-Parametergruppen
* &lbrack;Skripterstellung&rbrack; Falscher Software-Name in der Dokumentation
* &lbrack;UDIM&rbrack; Keine Informationen im Protokoll über UVs-Schalen auf mehreren UVs-Kacheln

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

* &lbrack;SSS&rbrack;&lbrack;Viewport&rbrack;&lbrack;Iray&rbrack; Generische Volumenstreuung
* &lbrack;SSS&rbrack; MDL- und Volumenstreuung-Parameter synchronisieren
* &lbrack;SSS&rbrack; Es wurde ein neuer Graustufenkanal mit dem Namen &quot;Streuung&quot; hinzugefügt.
* &lbrack;SSS&rbrack;&lbrack;Shader Settings&rbrack; Streutypparameter für die Volumenstreuung (Skin oder transluzent)
* &lbrack;SSS&rbrack;&lbrack;Shader Settings&rbrack; Streuskalenparameter für die Volumenstreuung
* &lbrack;SSS&rbrack;&lbrack;Shader Settings&rbrack; Farbstreuung-Parameter für Volumenstreuung
* &lbrack;SSS&rbrack;&lbrack;Anzeigeeinstellungen&rbrack; Streuung Sampleanzahl für Volumenstreuung
* &lbrack;Shader&rbrack;&lbrack;Iray&rbrack; Volumenstreuung MDL für Iray integrieren
* &lbrack;Shader&rbrack; Shader-Update über den Ressourcen-Updater
* &lbrack;Shader&rbrack; API und Dokumentation für Änderungsprotokoll aktualisieren
* &lbrack;Werkzeugeigenschaften&rbrack;&lbrack;Proj&rbrack; Neue Parameter für die triplanare Projektion
* &lbrack;Viewport&rbrack;&lbrack;Proj&rbrack; Steuern von Ansichtseigenschaften in 3D direkt mit Manipulatoren (Füllebene)
* &lbrack;Shortcuts&rbrack;&lbrack;Proj&rbrack; Neue Tastaturbefehle Q, W, E, R, T für triplanare Projektion-Manipulator
* &lbrack;Viewport&rbrack;&lbrack;Proj&rbrack; Steuern von Eigenschaften der Füllebene in 2D-Ansichten direkt über Manipulator (UV-Projektion)
* &lbrack;Shortcuts&rbrack;&lbrack;Proj&rbrack; Neuer Tastaturbefehl Q für UV-Projektion Manipulator
* &lbrack;Kontextsymbolleiste&rbrack;&lbrack;Proj&rbrack; Manipulator der triplanare Projektion steuern
* &lbrack;Kontextsymbolleiste&rbrack;&lbrack;Proj&rbrack; Manipulator der UV-Projektion steuern
* &lbrack;Werkzeugeigenschaften&rbrack; Kachelung der Textur mit dem Werkzeug &quot;Projektion und Schablone&quot; deaktivieren
* &lbrack;Schablone&rbrack; Verwenden von Nicht-quadratischen Bildern mit dem Projektion-Werkzeug/der Schablone
* &lbrack;Schablone&rbrack; Kachelung im Eigenschaftenfenster zulassen
* &lbrack;Schablone&rbrack; Der Zoom ist nicht auf einer Schablone ohne Kachelung zentriert
* &blbrack;Kameras&rbrack; Kameras importieren aus Maya, Max, Blender, Modo, DAE
* &lbrack;Kameras&rbrack;&lbrack;Viewport&rbrack; Auswählen und Steuern importierter Kameras in Viewport
* &lbrack;Kameras&rbrack;&lbrack;Iray&rbrack; Auswählen und Steuern importierter Kameras in Iray
* &lbrack;Kameras&rbrack;&lbrack;UI&rbrack;&lbrack;Neues Projekt&rbrack;&lbrack;Projektkonfiguration&rbrack; Kameras importieren ist standardmäßig aktiviert
* &lbrack;Kameras&rbrack;&lbrack;Shortcuts&rbrack; Hinzufügen von Tastaturbefehlen zum Wechseln zwischen Kameras
* &lbrack;Kameras&rbrack;&lbrack;Viewport&rbrack; Rahmen zu Viewport hinzufügen
* &lbrack;Kameras&rbrack;&lbrack;Viewport-Einstellungen&rbrack; Kontrolle der Deckkraft des Rahmens
* &lbrack;Kameras&rbrack;&lbrack;Kamera&rbrack; Maximale Brennweite bei 500mm
* &lbrack;Kameras&rbrack;&lbrack;Kamera&rbrack; Leg Ratio
* &lbrack;Kameras&rbrack;&lbrack;Kamera&rbrack; Option &quot;Sperren&quot; hinzufügen
* &lbrack;Kameras&rbrack;&lbrack;Kamera&rbrack; Hinzufügen einer Wiederherstellungsoption
* &lbrack;Kameras&rbrack;&lbrack;Kamera&rbrack; Attribut &quot;Fokusabstand&quot; hinzufügen
* &lbrack;glTF&rbrack; Importieren einer glTF-Datei
* &lbrack;glTF&rbrack; Importieren einer ambient occlusion-Map
* &lbrack;Alembic&rbrack; Alembic 1-Rahmen mit statischer Geometrie importieren
* &lbrack;Regal&rbrack; Ziehen Sie Materialien mithilfe von ID-Map mit einem Modifizierer (STRG/Befehlstaste) direkt auf den Mesh
* &lbrack;Ebenenstapel&rbrack; Automatische Erstellung von ID-Masken durch Ziehen und Ablegen von Materialien auf einem Mesh mit ID-Map
* &lbrack;Ebenenstapel&rbrack; Automatischer Bildlauf von Ebenen per Drag &amp; Drop über den Ebenenstapel
* &lbrack;UI&rbrack;&lbrack;Werkzeugeigenschaften&rbrack; Leg Substance&#39;s preset
* &lbrack;UI&rbrack;&lbrack;Hilfemenü&rbrack; Verbesserung des Hilfemenüs
* &lbrack;UI&rbrack;&lbrack;Neues Projekt&rbrack;&lbrack;Projektkonfiguration&rbrack; Neuorganisation des Fensters
* &lbrack;UI&rbrack;&lbrack;Neues Projekt&rbrack;&lbrack;Projektkonfiguration&rbrack; Mesh durch Datei ersetzen
* &lbrack;UI&rbrack;&lbrack;Substance&rbrack; Anzeigen von Substance-Attributen in der Benutzeroberfläche
* &blbrack;Shortcuts&rbrack; F4 wechselt zwischen 2D- und 3D-Ansicht
* &blbrack;Shortcuts&rbrack; Neue Tastaturbefehle zum Umschalten zwischen Schablone N und schnelle Maske U
* &lbrack;Substance-Integration&rbrack; Berücksichtigung von &#39;visible if&#39;-Anweisungen in den Substance-Parametern
* &lbrack;Viewport&rbrack; Schatten, die nach dem Verschieben der Kamera nicht berechnet werden müssen
* &lbrack;Inhalt&rbrack; Aktualisieren von MeetMat mit importierten Kameras
* &lbrack;Inhalt&rbrack; Beispiel mit aktivierter Volumenstreuung hinzufügen - JadeToad
* &lbrack;Inhalt&rbrack; Neue PBR-Projektvorlage mit aktivierter Volumenstreuung hinzufügen
* &lbrack;Inhalt&rbrack; Exportvorgaben wurden aktualisiert, um einen neuen Streuungskanal hinzuzufügen
* &lbrack;Inhalt&rbrack;&lbrack;Regal&rbrack; Unterstützung zusätzlicher Volumenstreuungen für: pbr-metal-rau, pbr-metal-rau-alpha-test, pbr-coated, pbr-spec-gloss
* &lbrack;Inhalt&rbrack;&lbrack;Regal&rbrack; Hinzugefügter Streuungskanal zu 5 intelligenten Materialien (Marmor und Skins)
* &lbrack;Inhalt&rbrack;&lbrack;Regal&rbrack; 1 neues Jade-Material
* &lbrack;Inhalt&rbrack;&lbrack;Regal&rbrack; 1 neues Wachs-Material

**Fest:**

* &lbrack;CMD&rbrack; Verschiedene Ergebnisse bei Verwendung derselben Befehlszeile mit unterschiedlichen Versionen
* &lbrack;TDR&rbrack; Wenn TdrLevel eingerichtet ist, sind keine Fehler im Protokoll vorhanden.
* &lbrack;Baker&rbrack; Ambient occlusion-Map wird gespiegelt
* &lbrack;ID-Map&rbrack; Absturz beim Kommissionieren außerhalb des 0-1-Bereichs
* &lbrack;Iray&rbrack; Absturz beim Wechseln des Textursatzes und beim Wechseln in den Malen-Modus
* &lbrack;Viewport&rbrack; Synchronisieren von Ablagebereichen zwischen Viewporten für Drag &amp; Drop
* &lbrack;Engine&rbrack; Moiré-Artefakt bei der Kachelung von Füllebenen oder beim Malen mit einem kleinen Pinsel
* &lbrack;Lizenz&rbrack; Prüfung auf fehlerhafte Softwareversion des Lizenzdienstes
* &lbrack;Lizenz&rbrack; Verarbeitung der Authentifizierungsmethode anpassen
* &lbrack;API&rbrack; Rufen Sie das onNewProjectCreated-Skript-API-Ereignis auf, selbst wenn Sie mit einer Vorlage erstellen.
* &lbrack;Shader&rbrack; Kompilierter Shader wird nicht aus dem Cache geladen, wenn die Shader-Datei nicht kompiliert wird
* &lbrack;Regal&rbrack; Beim Exportieren der HDR aus dem Regal wird eine Datei mit geklemmten Werten ausgegeben
* &lbrack;Export&rbrack; EXR-Exportklammern RGB von Farbwerten zwischen 0 und 1
* &lbrack;Inhalt&rbrack; Prozedurales Rauschen 3D Perlin Rauschen Fraktal ist verpixelt

**Bekannte Probleme:**

* Einfrieren der Berechnung auf AMD VEGA-GPUs
* Problem mit Huion-Tablets mit Tastaturbefehlen unter Windows

### 4.1.3 (2018.1.3)

*(Freigegeben: 28. Juni 2018)*

**Hinzugefügt:**

* &lbrack;Voreinstellungen&rbrack; Projekt beim Neustart von Painter speichern

**Fest:**

* &lbrack;Plugin&rbrack; Die Substance Source &quot;Suchen&quot; funktioniert nicht
* &amp;Intelligenten Materials&rbrack; Das Importieren von Intelligente Materialien führt in einigen Fällen zu einem Absturz
* &amp;Intelligenten Materials&rbrack; Das Löschen von Intelligenten Materialien führt in einigen Fällen zu einem Absturz
* &lbrack;Speichern&rbrack; Das Speichern führt in einigen seltenen Fällen zu einem Absturz
* &lbrack;Regal&rbrack; Umkehren funktioniert nicht auf Zellen 2 und Zellen 3
* &lbrack;Regal&rbrack; Typo in einigen Alphas
* &lbrack;Regal&rbrack; Einige Substance-Material werden nicht richtig gerendert

**Bekannte Probleme:**

* Einfrieren der Berechnung auf AMD VEGA-GPUs

### 4.1.2 (2018.1.2)

*(Freigegeben: 12. Juni 2018*)Zusammenfassung: **Verbesserte Wiedergabegeschwindigkeit, verbessertes Speichersystem, aktualisierte Schieberegler, aktualisierte Plug-in-API, chinesische Baking, verbesserter Abstand jetzt optional**

**Hinzugefügt:**

* &lbrack;Baker&rbrack; Leistungsverbesserung mit der neuen Baker-Version
* Erzwungene Anzeige von Dialogfeldern mit inkompatibler GPU
* &lbrack;Speichern&rbrack; Leg der neuen Funktion für kompakte Projekte (Speichermodus &quot;Voll/Kompakt&quot;)
* &lbrack;Speichern&rbrack; Benutzer im Fall eines Speicherfehlers informieren
* &lbrack;Clean&rbrack; Nächstes Speichern im Voll-/Kompaktmodus
* &blase;Regler&blase; Verbesserung der Präzision der Farb-/Graustufenbalken und -schieberegler
* &blase;Regler&blase; Hinzufügen von Nach-oben-/Nach-unten-Steuerelementen
* &blase;Regler&blase; Dieselbe Erkennungszone für Farb- und Graustufenbalkenschieberegler
* &lbrack;Plugin&rbrack; Automatisches Speichern immer im inkrementellen Modus
* &lbrack;Plugin&rbrack; Option zum Wechseln von Plug-ins zu einem neuen Schnittstellenstil
* &lbrack;Sprache&rbrack; Chinesische Übersetzung hinzufügen
* &Klammer;Auffüllung&Klammer; Option zum Wechseln zwischen UV- und 3D-Raum, Nachbar-Innenabständen pro Textursatz in den Textursatz-Einstellungen
* &lbrack;Script&rbrack; Gelegt Speichermodus: Voll/Kompakt oder inkrementell
* &lbrack;Script&rbrack; Aktualisieren von Skripterstellung/QML-Dokumentation
* &lbrack;Log&rbrack; Anzeige des Speichermodus im Protokoll (vollständig/kompakt oder inkrementell)

**Fest:**

* &lbrack;Werkzeug&rbrack; Bei Einkanalfüllungen transformieren der Kanalsteckplatz in einen Material-Steckplatz ein
* Absturz beim Laden eines Meshs (FBX) mit einigen Flächen, die nicht von einem Material zugewiesen wurden
* Absturz in Iray mit NVIDIA RASTER 5.2 auf einem virtuellen Computer
* Absturz beim Rückgängigmachen eines Löschens einer Materialvorgabe
* Absturz beim Laden einiger Projekte
* &lbrack;Befehlszeile&rbrack; Neue Befehlszeile für UDIM-Mesh, aufgeteilt nach Audio
* &blbrack;Symbolleiste&rbrack; Verkleinern der Symbolleiste
* &lbrack;Instancing&rbrack; Bitmaps können nicht auf mehreren Textursätzen instanziieren werden
* &lbrack;Viewport&rbrack; Die Aktualisierung ist beim Malen auf Mesh mit gekachelten UVs nicht abgeschlossen
* &lbrack;Iray&rbrack; Normalen-Map wird zweimal für Dielektrika angewendet
* &lbrack;Regal&rbrack; Typos in einigen Substance-Parametern (Alphas, Prozedurals und Matfx)
* &lbrack;Regal&rbrack; Typo für die Bitmap &quot;Nur autorisiertes Personal&quot;
* &lbrack;Script&rbrack; Die Funktion alg.shaders.Materials() funktioniert nicht mehr

**Bekannte Probleme:**

* Einfrieren der Berechnung auf AMD VEGA-GPUs

### 4.1.1 (2018.1.1)

*(Freigegeben: 03. April 2018)*

**Fest:**

* &Klammer;Tablet&Klammer; Problem beim Ändern der Standardinteraktionsoptionen
* &lbrack;Baker&rbrack; Absturz mit Assimp-Bibliothek
* &lbrack;Baker&rbrack; Leistungsrückgang mit A.O.-Karte
* &lbrack;Iray&rbrack; Die Verzerrung der Linse wird nicht auf den Alphakanal angewendet
* &lbrack;Treiber&rbrack; Aktualisierung der Mindestanforderungen für Treiber
* &lbrack;3Dview&rbrack; Normale werden auf UDIM-Meshs ohne Normale nicht korrekt generiert
* &lbrack;Intel&rbrack; Absturz mit Substance Painter 2018.1.0
* &lbrack;Intel&rbrack;&lbrack;Viewport&rbrack; Problem mit Innenabständen (schwarze Artefakte)

**Bekannte Probleme:**

* Einfrieren der Berechnung auf AMD VEGA-GPUs

### 4.1.0 (2018.1.0)

*(Freigegeben: 15. März 2018)*

**Hinzugefügt:**

* Neuer allgemeiner Stil (Symbole, Farbe, Verhalten)
* Neues Standardlayout
* &Klammer;Tablet&Klammer; Verbessertes Benutzererlebnis beim Malen
* &lbrack;Hauptmenü&rbrack; Sortieren Sie native Elemente zuerst in Ansichten und Symbolleisten
* &lbrack;Hauptmenü&rbrack; Aktionen &quot;schnelle Maske verschieben&quot; im Abschnitt &quot;Viewport&quot;
* &lbrack;Hauptmenü&rbrack; Rechtsklickaktionen in den Abschnitt &quot;Viewport&quot; verschieben
* &lbrack;Hauptmenü&rbrack; Menü &quot;Ansicht&quot; in &quot;Fenster&quot; umbenennen
* &lbrack;Schnellmenü&rbrack; Neue Werkzeugeigenschaften durch Rechtsklick im Viewport
* &lbrack;Andocken-Widget&rbrack; Neue Dock-Symbolleiste für schnelles Reduzieren/Zurückrufen
* &lbrack;Anzeigeeinstellungen&rbrack; Fenster &quot;Kamera- und Anzeigeeinstellungen&quot; wurde zusammengeführt
* &lbrack;Ebenenstapel&rbrack; Kontextmenü durch Rechtsklick
* &lbrack;Ebenenstapel&rbrack; Verschieben Sie jeden Effekt innerhalb derselben Ebene per Drag &amp; Drop
* &blbrack;Symbolleiste&rbrack; Neuanordnung der Symbolleiste und neue kontextbezogene Symbolleiste
* &Klammer;Werkzeugleiste&Klammer; Klonwerkzeug in zwei separate Werkzeuge teilen
* &lbrack;Werkzeugeigenschaften&rbrack; Hellerer Graustufenwert im Hintergrund in der Vorschau
* &lbrack;Werkzeugeigenschaften&rbrack; Organisation auf Registerkarten (Ausfüllen und Werkzeuge)
* &lbrack;Werkzeug&rbrack; Das Malergebnis entspricht der Schablone
* &lbrack;Viewport&rbrack; Neuer Cursor für Füllebene
* &lbrack;Viewport&rbrack; Einfachere Navigation und besseres Malen (höhere Rahmen-Rate)
* &lbrack;Viewport&rbrack; Kombinationsfeld &quot;Material-/Kanal-/Kartenauswahl&quot; im Viewport
* &lbrack;Viewport&rbrack; Flackern beim Drehen reduzieren (Schatten aktiviert)
* &lbrack;Regal&rbrack; Beim Öffnen von Painter standardmäßig Materials anzeigen
* &lbrack;Regal&rbrack; Ladezeitverbesserung von Substance-Texturen und Materialien (2- bis 6-mal schneller)
* &lbrack;Regal&rbrack; Materialien-Ordner an die Struktur einer Substance Source anpassen
* &lbrack;Regal&rbrack; Ziehen Sie Materialien per Drag &amp; Drop direkt auf den Mesh im Viewport
* &lbrack;Regal&rbrack; Neue 3D-Rauschen (Perlin, Perlin Fraktal, Simplex und Worley)
* &lbrack;Regal&rbrack; Neuer 3D Linear gradient-Maskengenerator mit Mesh-Position
* &lbrack;Regal&rbrack; Die Basis-Rauschen wurden aktualisiert, um quadratische Ausbreitung zu unterstützen
* &lbrack;Regal&rbrack; Neue Vorlage und Exportvoreinstellung für Lens Studio hinzugefügt (Einrasten Anwendung)
* &lbrack;Regal&rbrack; Intelligenten Materials und Intelligente Masken wurden aktualisiert, um die neueste Version des Maskeneditors zu verwenden (Mikrodetails)
* &lbrack;Regal&rbrack; Neues Beispielprojekt &quot;TilingMaterial&quot; zum Erstellen nahtloser Kachelung-Material
* &lbrack;Regal&rbrack; Neue Pinselvorgaben (Kalligrafie, Nass, Schraffur usw.)
* &blase;Regler&blase; Neue Schieberegler und Stil und Verhalten von Graustufen-/Farbbalken
* &lbrack;Baker&rbrack; Erlauben Sie die Verwendung des Begrenzungsrahmens für die volle Szene, um die Positionskarte zu berechnen.
* &lbrack;Shader&rbrack; Height Force-Parameter aus den Standard-Shader-Parametern entfernen
* &lbrack;Engine&rbrack; Substance Engine aktualisiert
* &lbrack;Engine&rbrack; Keine oder weniger Diskontinuitäten zwischen UV-Abschnitten
* &lbrack;Plugins&rbrack; Schnelleres Importieren von aus Substance Source heruntergeladenen Materials
* &lbrack;Plugins&rbrack; Alle Plug-ins entsprechend dem neuen Stil aktualisieren
* &lbrack;Voreinstellungen&rbrack; Automatische Vorschau der Hintergrundfarbänderungen
* &lbrack;Clean&rbrack; Geringeres Risiko für Projektbeschädigung
* &lbrack;Open&rbrack; Zeitverbesserung für das Öffnen des Projekts
* &lbrack;Neues Projekt&rbrack; Neues Projekt - Verbesserung der Aktualisierungszeit des Meshs
* &lbrack;Speichern&rbrack; Zeitersparnis bei Projekten
* &lbrack;Log&rbrack; Im Protokoll gemeldeter Lizenztyp
* &lbrack;TextureSet&rbrack; Die Schaltfläche &quot;Baking-Texturen&quot; in &quot;Baking-Mesh-Map&quot; umbenennen
* Benennen Sie &quot;Zusätzliche Maps&quot; in &quot;Mesh-Map&quot; um

**Fest:**

* &lbrack;Viewport&rbrack; Fehlerhafte Bewegungen bei Meshs, die viele Unterobjekte enthalten
* &lbrack;Werkzeugeigenschaften&rbrack; Kanal deaktiviert, wenn ein Material per Drag &amp; Drop in den Bildschlitz gezogen wird
* &lbrack;Werkzeugeigenschaften&rbrack; Pinselvorschau ist bei Verwisch- und Kopierwerkzeugen defekt
* &lbrack;Textursatz&rbrack; Die Reihenfolge der Kanäle ist falsch, wenn Vorlagen verwendet werden
* &lbrack;Regal&rbrack; Fehlendes Symbol für den Graustufenkonvertierungen-Generator
* &lbrack;Regal&rbrack; Alpha-Zeichen-Kreisnummer ist defekt (fehlende Schriftart)
* Falsche Erkennung integrierter GPUs beim Start
* &lbrack;Absturz&rbrack; Ziehen und Ablegen einer importierten Ressource mit dem Namen &quot;#&quot;
* &lbrack;Engine&rbrack; Problem mit der VRAM-Erkennung bei integrierter GPU
* &lbrack;Engine&rbrack; Mehrere Absturz im Substance Engine Linker behoben
* &lbrack;Engine&rbrack; Quadratische Artefakte bei der Änderung der Auflösung
* &lbrack;Post-Effekte&rbrack; Die Größe der Benutzeroberfläche ist langsam, wenn Post-Effekte aktiviert sind
* &lbrack;Baker&rbrack; Szene-Einheit wird bei Strahlenabstandswerten nicht korrekt eingehalten
* &lbrack;Baker&rbrack; AO vom Mesh Verdeckungsabstand wird unabhängig vom Eingangswert auf 1 geklemmt
* &lbrack;Baker&rbrack; Bei &quot;Nach Name suchen&quot; werden einige Mesh mit bestimmten Namen ignoriert
* &lbrack;Baker&rbrack; Die Farbe aus den Einstellungen &quot;Mesh-Polygruppe&quot; und &quot;Teilgitter-ID&quot; gibt immer ein schwarzes Bild zurück.
* &lbrack;Baker&rbrack; ID-Baking schlägt mit binären FBX Meshs aus Blender fehl
* &lbrack;Shader&rbrack; Rauschen in der 2D-Ansicht mit dota-2 und non-pbr-spec-gloss
* &lbrack;Linux&rbrack; Beim Baking wird nur ein CPU-Thread verwendet
* &lbrack;MacOS&rbrack; Absturz mit dem Pinselcursor, der sich über den Viewport bewegt

**Bekannte Probleme:**

* Einfrieren der Berechnung auf AMD VEGA-GPUs
* Verzerrungsnachbearbeitung wird beim Export in Iray nicht berücksichtigt (Alpha)

## Version 3

### 3.4.2 (2017.4.2)

*(Freigegeben: 24. Januar 2018)*

**Hinzugefügt:**

* &lbrack;Export&rbrack; Abrufen des Status eines Exports mit Schrittfortschritt
* &lbrack;Export&rbrack; Abbrechen eines Exports zulassen
* &lbrack;Export&rbrack; Exportieren von Texturen nach Sketchfab ohne Qualitätsverlust beim Normalen-Map
* &lbrack;Export&rbrack; Exportieren im glTF-Binärformat (glb)
* &lbrack;Export&rbrack; Größenänderung der Spalten auf der Registerkarte &quot;Konfiguration&quot; des Exportfensters zulassen
* &lbrack;Shader&rbrack; Hinzufügen eines Änderungsprotokolls für den Shader-API
* &lbrack;Skripterstellung&rbrack; Vorher- und Nachher-Rückruffunktionen beim Exportieren von Texturen hinzufügen
* &lbrack;Iray&rbrack; Upgrade auf SDK 2017.1 (Unterstützung für Volta-GPUs)

**Fest:**

* Absturz beim Beenden der Anwendung, bevor das Hauptfenster angezeigt wird
* &lbrack;MAC&rbrack; Absturz beim Laden von Graustufenkarten mit IRAY
* &lbrack;MAC&rbrack; VRAM Erkennung ist mit dem neuen Betriebssystem High Sierra nicht korrekt
* &lbrack;Plugin&rbrack; Das Herunterladen von Assets aus Substance Source funktioniert nicht mehr
* &lbrack;Skripterstellung&rbrack; Falsche Erkennung der Mindestversion des Plug-ins
* &lbrack;Export&rbrack; Nach dem Exportieren von Texturen kann die Exportvorgabe nicht gespeichert werden
* &lbrack;Instancing&rbrack; Problem bei Generatoren, die in einem TextureSet ohne zusätzliche Karten instanziieren wurden
* &lbrack;Viewport&rbrack; Dithering funktioniert nicht mit einer Auflösung über 4k
* &lbrack;Viewport&rbrack; 2D-Ansicht Material-Display ist mit Rauschen überzogen
* &lbrack;Regal&rbrack; Verbessern der Ladezeit für Regal-Vorgaben
* &lbrack;Engine&rbrack; Falsche Füllmethode beim Malen unter Farbauswahl

### 3.4.1 (2017.4.1)

*(Freigegeben: 15. Dezember 2017)*

**Hinzugefügt:**

* &lbrack;Skripterstellung&rbrack; Exportieren von Mesh über die Scripting-API
* &lbrack;Import&rbrack; Import nicht unterstützter Meshdateien deaktivieren (nur obj, fbx, date, play zulassen)
* &lbrack;Log&rbrack; Präzisere Angabe des TDR-Problems in der Protokolldatei

**Fest:**

* Absturz, wenn die Anwendung geschlossen wird, bevor das Crawlen der Ressourcen abgeschlossen ist
* Absturz beim Öffnen von Projekten mit dem Verwischen-/Klon-Werkzeug
* Absturz bei der Verwendung von &quot;redo&quot; nach einem Rückgängigmachen einer Shader-Änderung in den Anzeigeeinstellungen
* &lbrack;Engine&rbrack; Die Texturierung unterscheidet sich zwischen Painter 2017.2 und 2017.4
* &lbrack;Viewport&rbrack; Wenn Sie eine ID-Map aus einer Instanz auswählen, wird die falsche Farbe aufgenommen.
* &lbrack;Export&rbrack; Absturz beim Exportieren einer ungültigen Normal- oder Verdeckung-Textur
* &lbrack;Export&rbrack; Beim Öffnen von PSD-Dateien in Photoshop CS6 sind die Gruppen gesperrt
* &lbrack;Plugin&rbrack; Photoshop-Plugin ignoriert die Kanalauswahl und exportiert immer alles
* &lbrack;Layers&rbrack; Ankerpunkte werden beim Kopieren/Einfügen über Textursatz hinweg umgebrochen
* &lbrack;Layers&rbrack; Einige Ankerreferenzen können nicht wiederhergestellt werden, wenn sie beschädigt sind
* &lbrack;Shader&rbrack; pbr-beschichteter Parameter für sekundäre Rauheit ist defekt
* &lbrack;Steam&rbrack; Das Popup zur Versionsprüfung sollte beim Start nicht sichtbar sein

**Bekannte Probleme:**

* &lbrack;AMD&rbrack; Absturz/Einfrieren beim Malen auf einem Mesh. Kann mit einem GPU-Treiber-Update behoben werden.

### 3.4.0 (2017.4.0)

*(Freigegeben: 23. November 2017)*

**Hinzugefügt:**

* &lbrack;Instancing&rbrack; Parameter über Ebenen hinweg instanziieren
* &lbrack;Instancing&rbrack; Wechsel zwischen Quellebene und Instanz zulassen
* &lbrack;Instancing&rbrack; Aktion &quot;instanziieren zwischen Textursätzen&quot; hinzufügen
* &lbrack;Instancing&rbrack; Geben Sie im Ebenenstapel wieder eintretende Instanzen (Zyklen) an.
* &lbrack;Instancing&rbrack; Instanzen löschen, wenn eine Quelle entfernt wird
* &lbrack;Instancing&rbrack; Ankerverweise von außerhalb eines instanzierten Ordners nicht zulassen
* &lbrack;UI&rbrack; Den Stapel &quot;Rückgängig&quot; in ein eigenes Fenster mit dem Namen &quot;Verlauf&quot; verschieben
* &lbrack;Plugin&rbrack; DCC-Live-Link-Plug-in integrieren
* &lbrack;Engine&rbrack; Verbessern der Malleistung mit Sparse-Malerei
* &lbrack;Export&rbrack; Optionen für Entwürfe und Re-Exporte für Sketchfab-Exporter hinzufügen
* &lbrack;Regal&rbrack; Hinzufügen einer &quot;Spiegeln&quot;-Steuerung für Schriftsubstanzen
* &lbrack;Regal&rbrack; 20 neue Prozeduren hinzufügen - Materials
* &lbrack;Regal&rbrack; 40 neue Grunges Maps hinzufügen (Bitmap-basiert und prozedural)
* &lbrack;Viewport&rbrack; Kollisionen in der Pinselvorschau auf anderen sichtbaren Textursätzen aktivieren
* Mindestanforderungen für AMD GPU-Treiber aktualisieren

**Fest:**

* Absturz Beim Berechnen von Substance mit zu großen Auflösungen
* Absturz beim Malen mit Partikeln
* &lbrack;Viewport&rbrack; Falsche Specular-Spiegelung in der 2D-Ansicht mit bestimmten Meshs
* &lbrack;UI&rbrack; Im Verlaufsfenster werden einige unerwünschte Aktionen angezeigt

**Bekannte Probleme:**

* &lbrack;Layers&rbrack; Einige Ankerreferenzen können nicht wiederhergestellt werden, wenn sie beschädigt sind
* Absturz bei der Verwendung von &quot;redo&quot; nach einem Rückgängigmachen einer Shader-Änderung in den Anzeigeeinstellungen

### 3.3.3 (2017.3.3)

*(Freigegeben: 1. Dezember 2017)*

**Fest:**

* &lbrack;Steam&rbrack; Das Popup zur Versionsprüfung sollte beim Start nicht sichtbar sein
* &lbrack;Export&rbrack; Beim Öffnen von PSD-Dateien in Photoshop CS6 sind die Gruppen gesperrt

### 3.3.2 (2017.3.2)

*(Freigegeben: 20. November 2017)*

**Hinzugefügt:**

* &lbrack;UI&rbrack; Dialogfeld &quot;Neue Version verbessern&quot; und Änderungsprotokoll hinzufügen
* &lbrack;UI&rbrack; Anzeigen, ob die Wartung im Dialogfeld &quot;Neue Version&quot; abgelaufen ist
* &lbrack;Lizenz&rbrack; Lizenzsystem aktualisieren, um Wartungsdaten zu verarbeiten
* &lbrack;Export&rbrack; Adobe Standard Material in Adobe Dimension umbenennen

**Fest:**

* &lbrack;Mac&rbrack; Malen führt zu schwarzen Quadraten und beschädigten Texturen
* &lbrack;Engine&rbrack; Der Zwischenspeicher kann manchmal im Viewport verschwinden
* &lbrack;Engine&rbrack; Blockige Artefakte werden angezeigt, wenn der Speicherkomprimierungsauslöser aktiviert wird
* &blbrack;Baking&rbrack; Seltsame Fehlermeldungen beim Baking bestimmter Mesh
* &lbrack;Export&rbrack; PSD werden falsch geschrieben und von Photoshop nicht richtig erkannt
* &lbrack;Layers&rbrack; Ebenen sollten nicht projektübergreifend kopiert/eingefügt werden können.
* &lbrack;Substance&rbrack; UserData-Farbraum für normale Eingabe wird in einigen Fällen gespiegelt
* &lbrack;Regal&rbrack; Mikronormal in Generatoren gibt invertierte Krümmung aus
* &lbrack;Regal&rbrack; HSL beeinflussen auch den Alphakanal
* &lbrack;Linux&rbrack; Installation auf Centos schlägt aufgrund fehlender Abhängigkeiten fehl
* Das Installationsprogramm entfernt in bestimmten Fällen nicht alle Ressourcen aus der vorherigen Installation

### 3.3.1 (2017.3.1)

*(Freigegeben: 26. Oktober 2017)*

**Hinzugefügt:**

* &lbrack;Export&rbrack; Exportieren des Meshs aus einem Projekt zulassen
* &lbrack;Regal&rbrack; &quot;Sub-Regal&quot; aus den Registerkartentiteln entfernen
* Einstellungen für die Nachbearbeitung in Vorlagen speichern
* Die TDR-Meldung verständlicher machen
* Fenster &quot;Einstellungen&quot; verbessern, um Fehler zu melden

**Fest:**

* Absturz beim Löschen mehrerer untergeordneter Regal
* Absturz beim Wechsel von einer Ebene zu einer anderen während einer Engine-Berechnung
* &lbrack;Mac&rbrack; Absturz auf der Intel-GPU während der Engine-Berechnungen
* &lbrack;Mac&rbrack;&lbrack;Viewport&rbrack; Fehlerhafte Leistung, wenn Dithering aktiviert ist
* &lbrack;Mac&rbrack; MacOS 10.13 wird in der Protokolldatei als &quot;Unbekannte Version&quot; erkannt
* &lbrack;Baker&rbrack; Das Baking führ mit einem Käfig funktioniert nicht mehr
* &lbrack;Layers&rbrack; Strg + C Tastaturbefehl (Aktion kopieren) funktioniert nicht mehr
* &lbrack;Layers&rbrack; Beim Einfügen von Ebenen wird die Benutzeroberfläche mit Ankerreferenzen nicht aktualisiert
* &lbrack;Anker&rbrack; Duplizieren oder Kopieren/Einfügen der Ebene mit Referenzen hebt Verknüpfungen auf
* &lbrack;Export&rbrack; 8K-Export kann Absturz oder Deadlock-Anwendung in einigen Fällen
* &lbrack;Export&rbrack; Mehrere Probleme im generierten glTF-Dateiformat
* &lbrack;Import&rbrack; Das erneute Importieren eines Meshs mit demselben Dateinamen funktioniert nicht mehr
* &lbrack;Plugin&rbrack; Fenster zum automatischen Speichern wird immer über allem angezeigt
* &lbrack;UI&rbrack; Endlose Schleife, wenn Sie im TDR-Dialog &quot;Escape&quot; drücken
* &lbrack;UI&rbrack; UI zum Zurücksetzen zeigt eine zweite Titelleiste im Fenster &quot;Regal&quot; an

### 3.3.0 (2017.3.0)

*(Freigegeben: 28. September 2017)*

**Hinzugefügt:**

* &lbrack;Export&rbrack; Exportieren von Mesh und Texturen für Adobe Project Felix zulassen
* &lbrack;Export&rbrack; Export in das glTF-Dateiformat zulassen
* &lbrack;Engine&rbrack; Optimieren der Größe von Texturen in VRAM mithilfe der Blockkomprimierung
* &lbrack;Viewport&rbrack; Ziehen und Ablegen eines Meshs oder Projekts im Viewport
* &lbrack;UI&rbrack; Verbesserung der Warnmeldungen über TDR
* &lbrack;UI&rbrack; Das Protokoll sollte nur auf Anfrage angezeigt werden.
* &lbrack;UI&rbrack; Inhalt des Protokollfensters löschen
* &lbrack;UI&rbrack; Warnungen und Fehler in der Statuszeile anzeigen
* &lbrack;UI&rbrack; Registerkarten oben wie in Webbrowsern anzeigen
* &lbrack;UI&rbrack; Verbesserung des &quot;nicht bemalbaren&quot; Kontexts und der Botschaft
* &lbrack;UI&rbrack; Aktion &quot;Als Kopie speichern&quot; im Dateimenü hinzufügen
* &lbrack;Ebene&rbrack; Die Standardeinstellung für die Kachelung auf 1 festlegen
* &lbrack;Regal&rbrack; Verbesserter Verlaufsfilter zur Unterstützung von 10 dynamischen Farben
* &lbrack;Regal&rbrack; Fügen Sie ein Leerzeichen in der Standardabfrage des Mini-Regals hinzu
* &lbrack;Regal&rbrack; Hinzufügen einer Aktion &quot;Im Explorer öffnen&quot; für lokale Ressourcen im Regal
* &lbrack;Regal&rbrack; Vorlage und Shader für Adobe Material Standard hinzufügen (Project Felix)
* &lbrack;Regal&rbrack; Erhöhen der maximalen Kachelung auf 128 in Material-Ebenenschattierungen
* &lbrack;Regal&rbrack; Hinzugefügte Krümmung für Mikrodetails der Maskengenerator
* &lbrack;Plugin&rbrack; Plug-in zum automatischen Speichern mit anpassbarem Zeitintervall hinzufügen
* &lbrack;Skripterstellung&rbrack; Funktion &quot;Als Kopie speichern&quot; hinzufügen

**Fest:**

* &lbrack;UI&rbrack; Layout wird beim ersten Start unterbrochen
* &lbrack;Export&rbrack; Beim Export generierter PSD weist Formatfehler auf
* &lbrack;Export&rbrack; EXR exportiert immer 8-Bit-Höhen-Map
* &lbrack;Export&rbrack; Absturz beim Exportieren beschädigter zusätzlicher Maps
* &lbrack;Import&rbrack; Harte Kanten werden bei niedrigen Poly-Meshs in einigen Fällen nicht beibehalten
* &lbrack;Import&rbrack; Verbesserte Fehlermeldungen beim Importieren von Meshs mit Problemen
* &lbrack;Baker&rbrack; ID-Map-Baking schlägt fehl, wenn &quot;Nach Name abgleichen&quot; aktiviert ist
* &lbrack;Viewport&rbrack; Tangente-Speicherplatz wird nicht mit Bakern synchronisiert
* &blase;Effekt&blase; Das Zurückverschieben einer Ebene stellt die Referenz eines Ankers nicht wieder her
* &blase;Effekt&blase; Problem beim Aktualisieren beim Erstellen einer Verknüpfung zwischen zwei Masken mit Ankern
* &blase;Effekt&blase; Maskenanker über der Maske sollten nicht aufgeführt werden
* &blase;Effekt&blase; &quot;Alpha aus Ankerpunkten extrahieren&quot; funktioniert nicht
* &lbrack;Engine&rbrack; Maske kehrt sich nach dem ersten Pinselstrich um
* &lbrack;Engine&rbrack; Absturz beim Wechseln des Textursatzes zu einem bestimmten Projekt
* &lbrack;Regal&rbrack; Absturz beim Löschen einer Vorgabe, die sich in einem Projekt befindet
* &lbrack;Regal&rbrack; Typo in erweitertem Tri-Planarem Filter
* &lbrack;Regal&rbrack; MG Mask Builder AO Rauschen Scale funktioniert nicht richtig
* &lbrack;Regal&rbrack; Der MG-Maskenbildner verfügt über Parameter für invertierte Krümmungen
* &lbrack;Regal&rbrack; Importierte Alphas erzeugen eine Material-Kugelvorschau anstelle einer flachen.

### 3.2.0 (2017.2.0)

*(Freigegeben: 27. Juli 2017)*

**Hinzugefügt:**

* Ankerpunkte - Ebenen- und Maskenreferenzsystem
* &lbrack;Layers&rbrack; Möglichkeit, Füll- und Malen-Effekte umzubenennen
* &lbrack;Plugin&rbrack; Aktualisiertes Substance Source-Plug-in
* &lbrack;Skripterstellung&rbrack; Zulassen, dass die Auflösung des Textursatzes abgefragt wird
* &lbrack;Skripterstellung&rbrack; Abrufen des Status des Engine &quot;Malen&quot; zulassen
* &lbrack;Performance&rbrack; Verbessertes Laden von Projekten und optimiertes Pinselstempeln

**Fest:**

* &lbrack;Werkzeug&rbrack; Leistungsprobleme beim Anpassen von Material-Parametern
* &lbrack;Engine&rbrack; Verschwindende Pinselstriche bei Änderung der Auflösung (4K>2K)
* &lbrack;3D-Ansicht&rbrack; Tangente-Speicherplatz wird nicht mit Bakern synchronisiert
* &lbrack;Regal&rbrack; Der Regal-Pfad in den Benutzerdokumenten wird nicht automatisch erstellt
* &lbrack;Regal&rbrack; Vorgaben nach einem Update mit früheren Versionen kompatibel machen
* &lbrack;Shader&rbrack; Shader ohne PBR funktioniert nicht mehr
* &lbrack;Baker&rbrack; ID-Map-Baking schlägt fehl, wenn &quot;Nach Name abgleichen&quot; aktiviert ist
* &lbrack;Beispiel&rbrack; Die Namen der Meet Mat-Beispielprojekt-Textursatz sind falsch
* Beim Speichern eines Projekts vor dem Erstellen einer Vorlage werden Schreibberechtigungsfehler zurückgegeben.

### 3.1.0 (2017.1.0)

*(Freigegeben: 20. Juni 2017)*

**Hinzugefügt:**

* &lbrack;Plugin&rbrack; Neues Substance Source-Plug-in (ermöglicht das Herunterladen von Assets im Regal)
* &lbrack;Regal&rbrack; 4 Neue Schriftarten (Japanisch + vereinfachtes Chinesisch, Schreibmaschine, Segment)
* &lbrack;Regal&rbrack; 230 neue Alpha (Mischung aus Mustern, Pinseln und Fingerabdruckscans)
* &lbrack;Regal&rbrack; 50 Neue Prozedurale (Stoffmuster mittelalterlicher und zeitgenössischer Kleidung)
* &lbrack;Regal&rbrack; 2 neue Umgebungs-Map (Mondarrain und Villa Nova Street)
* &lbrack;Regal&rbrack; 9 neue Filter (MatFx Detail Edge Wear, Beschränk, HBAO, etc.)
* &lbrack;Regal&rbrack; Verbessertes Panorama-Umgebungs-Map
* &lbrack;Regal&rbrack; Neue Arnold 5-Exportvorgaben
* &lbrack;Skripterstellung&rbrack; Importieren von Ressourcen in das Regal zulassen

**Bekannte Probleme:**

* &lbrack;Export&rbrack; Die Bearbeitung einer Exportvorgabe ist sehr langsam

## Version 2

### 2.6.2

*(Freigegeben: 20. Oktober 2017)*

**Hinzugefügt:**

* &lbrack;Textursatz&rbrack; Löschen deaktivierter Textursatz zulassen
* &lbrack;Regal&rbrack; Schreiben mehrerer Benutzer in denselben Regal-Ordner zulassen
* &lbrack;Skripterstellung&rbrack; Ordner &quot;Plug-ins&quot; neu laden können
* &lbrack;Skripterstellung&rbrack; Fügen Sie eine erforderliche minimale API-Version in den Plug-in-Metadaten hinzu, um die Kompatibilität zu gewährleisten
* &lbrack;Iray&rbrack; Verbesserungen im Dialogfeld &quot;Bild exportieren&quot;

**Fest:**

* &lbrack;Engine&rbrack; Problem mit verschwundenen Strichen beim Ändern der Auflösung (4K>2K)
* &lbrack;Baker&rbrack; ID-Map-Baking schlägt fehl, wenn &quot;Nach Name abgleichen&quot; aktiviert ist
* &lbrack;Baker&rbrack; Fehlermeldungen sind nicht explizit genug
* &lbrack;3D-Ansicht&rbrack; Tangente-Speicherplatz wird nicht mit Bakern synchronisiert
* &lbrack;Werkzeug&rbrack; Schwarze Artefakte bei Verwendung des Wischfinger-Werkzeugs
* &lbrack;Shader&rbrack; Shader ohne PBR funktioniert nicht mehr
* &lbrack;Shader&rbrack; &quot;pbr-coated&quot; ist gebrochen
* &lbrack;Shader&rbrack; Die Rauheit von &quot;pbr-beschichtetem&quot; Shader hat keine Auswirkungen mehr
* &lbrack;Shader&rbrack; Spec Gloss Shader stimmt nicht mit Iray und SD überein
* &lbrack;Regal&rbrack; Absturz beim Laden von zwei Dateien mit demselben Namen, aber unterschiedlichen Erweiterungen
* &lbrack;Regal&rbrack; Die Vorgabe kann in den Regale nicht mehr bearbeitet werden
* &lbrack;Regal&rbrack; Für im Regal importierte Elemente kann keine benutzerdefinierte Vorschau festgelegt werden
* Aus dem Cache geladene Ressourcen verlieren ihre Nutzung
* Beim Speichern eines Projekts vor dem Erstellen einer Vorlage werden Schreibberechtigungsfehler zurückgegeben.
* Falsches Speichern des Projekts, wenn Dateiname zwei Punkte enthält
* Importieren von Dateien mit mehreren Punkten (.) im Dateinamen führt zu Problemen

### 2.6.1

*(Freigegeben: 12. Mai 2017)*

**Hinzugefügt:**

* &lbrack;TextureSet&rbrack; Mesh-Material nicht zu nichts zuweisen

**Fest:**

* Absturz beim Wechseln von TextureSet nach dem Ersetzen von durch Baking erzeugte Map
* Absturz beim Rückgängigmachen und Wiederholen nach dem Ändern der Füllmethode der Ebene
* Absturz oder Einfrieren bei Verwendung des Effekts &quot;Farbauswahl&quot; mit großem ID-Map
* &lbrack;Export&rbrack; Umbenannte Textursatz werden im Exportfenster nicht alphabetisch sortiert
* &lbrack;TextureSet&rbrack; Beim Zurücksetzen auf den Standardnamen wird keine Eindeutigkeit überprüft.
* &lbrack;TextureSet&rbrack; Umbenannter Textursatz wird nach dem erneuten Öffnen des Projekts deaktiviert
* &lbrack;Regal&rbrack; Fehlender Standardvorlageninhalt
* &lbrack;Regal&rbrack; Nicht quadratische Texturen werden als Quadrat angezeigt
* &lbrack;Shader&rbrack; Sobald ein Textursatz deaktiviert wurde, wird der zugehörige Shader gelöscht.
* &lbrack;Skripterstellung&rbrack; alg.Baking.setTextureSetBakingParameters() funktioniert nicht mehr
* &lbrack;Skripterstellung&rbrack; Tippfehler im Websocket-Tutorial
* &lbrack;Skripterstellung&rbrack; Verschiedene Probleme in AlgWidgets
* &lbrack;Log&rbrack; Fehlerhafte Erkennung des verfügbaren virtuellen Speichers in einigen Fällen

### 2.6.0

*(Freigegeben: 27. April 2017)*

**Hinzugefügt:**

* Neues Beispielprojekt &quot;Meet Mat&quot; hinzufügen
* &lbrack;Plugin&rbrack; Neues Plug-in &quot;Resources Updater&quot;
* &lbrack;TextureSet&rbrack; Umbenennen und Hinzufügen einer Beschreibung zu Textursätzen zulassen
* &lbrack;TextureSet&rbrack; Neuzuweisen von Materialien zulassen
* &lbrack;TextureSet&rbrack; Einstellungsschaltfläche im Textursatz-Listenfenster hinzufügen
* &lbrack;TextureSet&rbrack; &quot;Deaktivierte&quot; Textursatz am Ende der Liste anzeigen
* &lbrack;Substance&rbrack; Verwenden zusätzlicher Maps bei der aktuellen Textursatz-Auflösung, um die Leistung zu verbessern
* &lbrack;Skripterstellung&rbrack; Aktualisieren einer in einem Projekt verwendeten Ressource (Material, Generator usw.) zulassen
* &lbrack;Skripterstellung&rbrack; Hinzufügen einer Möglichkeit zum Hinzufügen/Entfernen eines Regals
* &lbrack;Skripterstellung&rbrack; Abfragen von Informationen aus einer Ressource in Projekten zulassen
* &lbrack;Skripterstellung&rbrack; Liste der verfügbaren Shelfs abrufen
* &lbrack;Skripterstellung&rbrack; AlgWidget-Miniaturansicht verbessern
* &lbrack;Export&rbrack; Deaktivieren/Aktivieren der Bittiefe je nach Dateiformatunterstützung
* &lbrack;Log&rbrack; Plug-in-Namen zum Drucken in der Konsole hinzufügen
* &lbrack;Log&rbrack; Fehler zu ausgeblendeten Textursätzen entfernen
* &quot;Begrüßungsbildschirm&quot; mit neuen Symbolen und Text für Beispiele aktualisieren

**Fest:**

* Absturz beim Aktualisieren eines Meshs in bestimmten Projekten
* &lbrack;Viewport&rbrack; Innenfarbe der Symmetrie-Ebene ist nicht mehr sichtbar
* &lbrack;Viewport&rbrack; Einige Nachbearbeitungseffekte sind aktiviert, wenn die Einzelansicht verwendet wird
* &lbrack;Shaders&rbrack; &quot;over_premult&quot;-Füllmethode funktioniert nicht richtig
* &lbrack;Shaders&rbrack; Warnung zum Alphatest mit dem Standard-Shader
* &lbrack;Regal&rbrack; Falsches Analysieren von Tags aus Substance
* &lbrack;Regal&rbrack; MatFX Rost Verwitterung funktioniert nicht richtig
* &lbrack;Regal&rbrack; HSL Filter ist standardmäßig für falsche Kanäle aktiviert
* &lbrack;Regal&rbrack; Der Scharfzeichner ist standardmäßig auf dem Height-/Normalkanal aktiviert
* &lbrack;Export&rbrack; Vray-Exportvorgaben verwenden keine OpenGL-Normalen-Map
* &lbrack;Werkzeug&rbrack; Ungenauigkeitsprobleme mit dem Klon-/Verwischen-Werkzeug erzeugen Artefakte

### 2.5.3

*(Freigegeben: 15. März 2017)*

**Fest:**

* &lbrack;Baker&rbrack; Absturz beim Baking führ mit bestimmten Meshs

**Bekannte Probleme:**

* &lbrack;Mac&rbrack; Partikeln können in einigen Fällen zu Beschädigungen der Textur führen

### 2.5.2

*(Freigegeben: 14. März 2017)*

**Fest:**

* &lbrack;Werkzeug&rbrack; Wacom-Tablets funktionieren unter Linux nicht
* &lbrack;Werkzeug&rbrack; Schwarze Artefakte bei Verwendung des Wischfinger-Werkzeugs
* &lbrack;Baker&rbrack; Baking schlägt fehl, wenn &quot;Nach Name abgleichen&quot; mit einem Käfig verwendet wird
* &lbrack;Baker&rbrack; Ambient occlusion funktioniert nicht, wenn nur mit Normalen-Map Baking geführt wird
* &lbrack;Regal&rbrack; Generische Filter behandeln Alpha nicht richtig (Kontrast/Luminanz, Hochpass usw.)
* &lbrack;Viewport&rbrack; Leistungsproblem beim Laden eines Projekts mit aktivierten Schatten
* &lbrack;Viewport&rbrack; Ditheringe in der 3D-Ansicht über MacOS
* &lbrack;Viewport&rbrack; Partikel-Vorschauen werden falsch angezeigt, wenn Farbprofil aktiviert ist
* &lbrack;Iray&rbrack; Absturz beim Zurückwechseln des Projekts zu OpenGL, wenn Iray nicht initialisiert werden konnte
* &lbrack;Iray&rbrack; Glanz wird beim Rendern von SpecGloss Shader/mdl ignoriert
* &lbrack;Shader&rbrack; Spec/Gloss Shader stimmt nicht mit Iray und SD überein
* &lbrack;Shader&rbrack; sRGB-Konvertierung anders als bei der linearen in sRGB-LUT-Konvertierung
* &lbrack;Shader&rbrack; Falsches Rendering beim Laden des Projekts mit veralteten Shadern
* &lbrack;Shader&rbrack; &quot;pbr-beschichteter&quot; Shader funktioniert nicht mehr
* &lbrack;Export&rbrack; Einige Kanäle werden weiterhin exportiert, auch wenn sie nicht im Textursatz vorhanden sind
* &lbrack;Layers&rbrack; Der Mischmodus &quot;Normalen-Map inverse detail&quot; funktioniert nicht auf Graustufenkanälen
* &lbrack;UI&rbrack; Problem beim &quot;Farbauswahl window&quot; mit HDPI-Monitor und Anzeigezoom bei 150 %

**Bekannte Probleme:**

* &lbrack;Mac&rbrack; Partikeln können in einigen Fällen zu Beschädigungen der Textur führen

### 2.5.1

*(Freigegeben: 27. Februar 2017)*

**Fest:**

* &lbrack;Mac&rbrack; Wacom-Tablet-Eingang in 3D und 2D-Ansicht defekt
* &lbrack;Baker&rbrack; Die Zuordnung nach Namen funktioniert nicht mehr
* &lbrack;Baker&rbrack; Die Einstellung &quot;Durchschnittliche Normale&quot; funktioniert nicht mehr
* &lbrack;Iray&rbrack; Falsches Rendering mit fehlendem Baking geführt Normalen-Map
* &lbrack;Iray&rbrack; Farbprofil verhalten sich anders als beim OpenGL-Renderer
* &lbrack;Iray&rbrack; Beim Exportieren des Renderings als Bitmap wird das Farbprofil nicht korrigiert.
* &lbrack;Substance&rbrack; Materialfilter funktionieren nicht mehr
* &lbrack;Werkzeug&rbrack; Die Konturdeckkraft wird nicht in Pinselvorgaben gespeichert
* &lbrack;Werkzeug&rbrack; Klon-Pinsel-UV-Ausrichtung funktioniert nicht mehr
* &lbrack;Export&rbrack; Beim Exportieren in Ganzzahl sollte der Versatz-Kanal in 0,5 zentriert sein
* &lbrack;Vorlage&rbrack; Absoluter Pfad wird in Vorlagen gespeichert
* &lbrack;TextureSet&rbrack; Die Textur des Kanals bleibt auch nach dem Entfernen des Kanals bestehen.

**Bekannte Probleme:**

* &lbrack;Linux&rbrack; Wacom-Tablet-Eingaben funktionieren nicht in 3D und 2D-Ansicht
* &lbrack;Mac&rbrack; Partikeln können in einigen Fällen zu Beschädigungen der Textur führen
* &lbrack;Export&rbrack; In sehr seltenen Fällen können auf AMD-GPUs schwarze Rechtecke erscheinen

### 2.5.0

*(Freigegeben: 21. Februar 2017)*

**Hinzugefügt:**

* Unterstützung für AMD Radeon Pro- und AMD FirePro-GPUs
* &lbrack;Werkzeug&rbrack; Unterstützung für Konturdeckkraft hinzufügen
* &lbrack;Werkzeug&rbrack; Fügen Sie einen Modifizierer hinzu, mit dem Sie den letzten Pinselstrich fortsetzen können
* &lbrack;Iray&rbrack; Update zur Unterstützung von Pascal-GPUs
* &lbrack;Viewport&rbrack; Unterstützung für Farbprofil hinzufügen (LUT)
* &lbrack;Substance&rbrack; Neues Framework integrieren (SD6-Engine)
* &lbrack;UI&rbrack; Liste &quot;Zuletzt verwendete Datei&quot; im Menü &quot;Datei&quot; vergrößern
* &lbrack;Import&rbrack; Kategorie aus Stoffen verwenden, um das Präfix im Dialogfeld &quot;Einfuhr&quot; auszufüllen
* &lbrack;Baker&rbrack; Baking von 8K-Texturen zulassen
* &lbrack;Baker&rbrack; Nicht quadratische Auflösungen können Baking geführt werden
* &lbrack;Baker&rbrack; Verbessern Sie den Speicherverbrauch beim Baking führ von hochpolaren Meshs
* &lbrack;Regal&rbrack; Regale (und Projekte) sperren, um gleichzeitige Bearbeitung zu verhindern und Beschädigungen zu vermeiden
* &lbrack;Regal&rbrack; Lesen Sie Kategorie und Schlüsselwörter von Stoffen, um sie für die Filterung zu verwenden
* &lbrack;Regal&rbrack; Ausschließen von Ressourcen vom Ergebnis einer Suchabfrage zulassen
* &lbrack;Regal&rbrack; Verbesserte Berechnung der Miniaturansichten
* &lbrack;Regal&rbrack; Einbetten von Vorgaben in Projekte zulassen
* &lbrack;Regal&rbrack; Schnelles Ein- und Ausblenden der Strukturansicht mit UMSCHALTTASTE
* &lbrack;Regal&rbrack; Speichern von Miniaturansichten zulassen, wenn Assets schreibgeschützt sind (lokaler Cache)
* &lbrack;Regal&rbrack; Neue Inhalte : neue Filter (transformieren, Mirror, Tri-planar usw.)
* &lbrack;Regal&rbrack; Neue Inhalte : neue LUTs-Profile (klassisch und künstlerisch, z. B. Film Noir, Vintage usw.)
* &lbrack;Regal&rbrack; Neue Inhalte : 10 neue Font-Substance zur schnellen Generierung benutzerdefinierter Texte
* &lbrack;Regal&rbrack; Neue Vorlagen : Unity 5 und Unreal Engine 4
* &lbrack;Regal&rbrack; Verbesserter HSL-Filter für mehr Künstlerfreundlichkeit
* &lbrack;Shader&rbrack; Unterstützung für Specular level-Kanal in PBR-Shadern hinzufügen
* &lbrack;Shader&rbrack; Unterstützung für Dithering in Alpha Test Shader hinzufügen
* &lbrack;Shader&rbrack; Unterstützung für die Zuordnung von Parallax-Verdeckungen in PBR-Shadern hinzufügen
* &lbrack;Shader&rbrack; Definieren einer benutzerdefinierten Benutzeroberfläche für Shader-Parameter zulassen
* &lbrack;MatLayering&rbrack; Neuen Maskenkanal für Material-Ebenen-Workflow erstellen
* &lbrack;Skripterstellung&rbrack; Schreiben von Metadaten in ein SP-Projekt zulassen
* &lbrack;Skripterstellung&rbrack; Exportieren mit einer bestimmten Exportvorgabe zulassen
* &lbrack;Skripterstellung&rbrack; Shader-Parameter als JSON abrufen
* &lbrack;Skripterstellung&rbrack; Unterstützung für WebSocket-Verbindungen hinzufügen
* &lbrack;Skripterstellung&rbrack; Shader-Instanzen können geladen werden.
* &lbrack;Skripterstellung&rbrack; Hinzufügen der Möglichkeit, ein neues Projekt zu erstellen
* &lbrack;Skripterstellung&rbrack; Abrufen der URL des in ein Projekt importierten Meshs zulassen
* &lbrack;Skripterstellung&rbrack; Nicht quadratisches Baking zulassen
* &lbrack;Skripterstellung&rbrack; Fehler beim Festlegen von Daten über die Skript-API melden
* &lbrack;Substance&rbrack; Benutzerdaten-Tag zum Angeben von Normalen-Map-Format hinzufügen

**Fest:**

* Absturz bei der Farbauswahl mit Stoffen
* Absturz beim Laden eines Nicht-RGBA32f-Bildes als Umgebungs-Map
* Absturz beim Malen auf AMD-GPUs
* &lbrack;Mesh&rbrack; OBJ Import erkennt Materialien ohne MTL-Datei nicht
* &lbrack;Mesh&rbrack; Die Generierung des Namens des UDIM-Textursatzes kann auf einigen Meshs falsch sein
* &lbrack;UI&rbrack; Schaltfläche &quot;Rückgängig/Wiederholen&quot; in Anzeigeeinstellung &quot;Fokus stehlen&quot; und Mausbildlauf anhalten
* &lbrack;UI&rbrack; Einige Beschriftungen werden in High-DPI falsch beschnitten
* &lbrack;Ebene&rbrack; Der Ersetzungsmodus für den Malen-Effekt hat ein falsches Verhalten auf der Maske.
* &lbrack;Ebene&rbrack; Der subtrahieren-Mischmodus verhält sich mit Alpha nicht korrekt.
* &lbrack;Werkzeug&rbrack; Die Pinselgröße wird in der 2D-Ansicht sehr groß, wenn auf UV-Rahmen gemalt wird
* &lbrack;Werkzeug&rbrack; Einrasten Gerade hat ein ungleichmäßiges Verhalten mit High-DPI.
* &lbrack;Werkzeug&rbrack; Die Auflösung der Schablone ist manchmal falsch
* &lbrack;Baker&rbrack; Die Werte für &quot;Max. Verdeckungsabstand&quot; werden festgeklemmt, wenn &quot;relativ zum Begrenzungsrahmen&quot; &quot;Aus&quot; ist.
* &lbrack;Shader&rbrack; Kanaldefinitionen für Stapel und automatische Parameter stimmen nicht überein
* &lbrack;3D-Ansicht&rbrack; Inkonsistente Anzeige des normalen Kanals abhängig von der Projekteinstellung
* &lbrack;Viewport&rbrack; Einige Normalen-Map haben eingeklemmte Werte, die als Artefakte erscheinen
* &lbrack;Viewport&rbrack; Post-Effect sind standardmäßig immer deaktiviert
* &lbrack;Export&rbrack; Normale Mischeinstellung ist falsch, wenn normaler Kanal fehlt
* &lbrack;Export&rbrack; Falsche Generierung von Texturen in einigen Fällen auf AMD-GPUs
* &lbrack;Export&rbrack; Shader-Parameter werden nicht ordnungsgemäß exportiert, wenn sie sich in einer Gruppe befinden
* &lbrack;Export&rbrack; Beim Bearbeiten einer Exportvorgabe in einem benutzerdefinierten Regal wird ein Protokollfehler ausgegeben
* &lbrack;Regal&rbrack; Die Filterungen in der Strukturansicht stimmen nicht genau mit dem Ordnernamen überein
* &lbrack;Regal&rbrack; Das Umbenennen einer Regal-Vorgabe ist schwer zu lesen
* &lbrack;Regal&rbrack; Im Regal importierte Shader-Ressource bleibt nach dem Neustart nicht erhalten
* &lbrack;Regal&rbrack; Inhalt : Werkzeugvorgabe fehlt
* &lbrack;Regal&rbrack; Inhalt : Tile Generator funktioniert nicht richtig
* &lbrack;Regal&rbrack; Inhalt : Falsche Maske auf Gummireifen-Schmutziges intelligente Material behoben
* &lbrack;Regal&rbrack; Inhalt : Falscher Gruppenname auf dem Material der Ledertasche wurde behoben
* &lbrack;Iray&rbrack; Die Hälfte der Mesh fehlt in Iray
* &lbrack;Linux&rbrack; Absturz beim Ziehen einer Ressource über die 3D-Ansicht
* &lbrack;Mac&rbrack; Die Voreinstellungen werden bei jedem Start in Sierra zurückgesetzt

**Bekannte Probleme:**

* &lbrack;Export&rbrack; In sehr seltenen Fällen können auf AMD-GPUs schwarze Rechtecke erscheinen
* &lbrack;Iray&rbrack; Farbprofil können sich manchmal seltsam verhalten

### 2.4.1

*(Freigegeben: 28. Oktober 2016)*

**Fest:**

* Absturz beim Erstellen eines Projekts mit einer Vorlage
* Absturz beim Schließen des Exportdialogfelds während eines Exports
* &lbrack;Mac&rbrack; Fehler beim Speichern des Projekts (Exportvorgabe kann nicht gespeichert werden)
* &lbrack;Regal&rbrack; Beim Erstellen einer neuen Vorgabe wird sie zweimal angezeigt
* &lbrack;Regal&rbrack; Vorgaben können ohne Administratorrechte nicht im schreibgeschützten Modus geladen werden.

### 2.4.0

*(Freigegeben: 27. Oktober 2016)*

**Hinzugefügt:**

* &lbrack;Regal&rbrack; Neue Benutzeroberfläche zum Durchsuchen von Ressourcen (Strukturansicht, Filter usw.)
* &lbrack;Regal&rbrack; Speichern einer Suche als Vorgabe zulassen
* &lbrack;Regal&rbrack; Erstellen eines neuen Fensters aus einer Vorgabe zulassen
* &lbrack;Regal&rbrack; Neue Benutzeroberfläche für den Import von Ressourcen
* &lbrack;Regal&rbrack; Kopieren Sie kein standardmäßiges allegorisches Regal im Ordner &quot;Dokumente&quot;
* &lbrack;Regal&rbrack; Neue Partikeln-Vorgaben : Stromkreis, elektrische Leitungen, Rokoko, Kleinvenen
* &lbrack;Regal&rbrack; Verbesserte Vorgaben für ältere Partikeln, um einfacher zu verwenden (z. B. &quot;Rain&quot;)
* &lbrack;Regal&rbrack; Neue Informationen zum Kontextmenü der Ressource hinzufügen
* &lbrack;Viewport&rbrack; Verbessern der Leistung beim Laden von Umgebungs-Map
* &lbrack;Viewport&rbrack; Unterstützung für Umgebungs-Map, die nicht die Macht von zwei sind

**Fest:**

* Absturz beim Entfernen einer Maske
* Absturz beim Malen nach dem Speichern einer Vorgabe
* Absturz mit Umgebungsunschärfe bei einigen GPUs
* Absturz beim Zuweisen einer falschen Ressource zum Mini-Regal
* &lbrack;Regal&rbrack; Bereinigen + Speichern - Entfernen von Tags und Metadaten für Ressourcen im Projekt
* &lbrack;Regal&rbrack; Beim Importieren einer Vorgabe werden ihre Ressourcen im Regal angezeigt
* &lbrack;Export&rbrack; Normalen-Map, die aus dem Height-Kanal generiert wird, ist niedrig
* &lbrack;Export&rbrack; Normal vom Mesh ist in der endgültigen Normalen-Map nicht immer vorhanden
* &lbrack;Export&rbrack; Ausdehnung mit Transparenz kann manchmal ohne Transparenz erfolgen
* &lbrack;Skripterstellung&rbrack; &quot;alg.plugin_root_directory&quot; kann einen abgeschnittenen Netzwerkpfad zurückgeben
* &lbrack;TextureSet&rbrack; Sperrschaltfläche ist aktiviert, wenn nicht quadratische Projekte erneut geöffnet werden

### 2.3.1

*(Freigegeben: 07. Oktober 2016)*

**Hinzugefügt:**

* &lbrack;Plugin&rbrack;&lbrack;Photoshop&rbrack; Geben Sie an, welches Material/welcher Stapel/welche Kanäle exportiert werden sollen.
* &lbrack;Skripterstellung&rbrack; Funktionsnamen weisen einige Inkonsistenzen auf.

**Fest:**

* &lbrack;Export&rbrack; Alpha kann in benutzerdefinierten Exportvorgaben verworfen werden
* &lbrack;Export&rbrack; Alpha erhält falsche Gamma-Konvertierung auf sRGB-Kanälen
* &lbrack;Export&rbrack; Nicht quadratische Dokumente werden als quadratische
* &lbrack;Export&rbrack; Es ist nicht möglich, zusätzliche Maps zu exportieren, wenn eine fehlt
* &lbrack;Iray&rbrack; Einige Parameter (z. B. &quot;emissive-Intensität&quot;) haben keine Auswirkungen
* &lbrack;NVIDIA&rbrack; Absturz beim Start mit NVIDIA Quadro K2200/GTX 750/760
* &lbrack;AMD&rbrack; Falscher Farbsatz für Miniaturen und Vorschauen
* &lbrack;AMD&rbrack; Einfrieren und Treiberfehler beim Öffnen neuer Dateien und Dateien
* &lbrack;Log&rbrack; &quot;software-version&quot; fehlt in der Protokolldatei

### 2.3.0

*(Freigegeben: 15. September 2016)*

**Hinzugefügt:**

* &lbrack;Plugin&rbrack; Neues Plug-in &quot;Nach Photoshop exportieren&quot; (vollständiger Ebenenstapel exportieren)
* &lbrack;Export&rbrack; Zulassen, dass die Breite der Auffüllung (in Pixeln oder unendlich) angegeben wird
* &lbrack;Export&rbrack; Festlegen des Hintergrundtyps außerhalb der UVs zulassen
* &lbrack;Regal&rbrack; Neues Material mit Shader-Ebenen zum Überblenden von 10 Materialien
* &lbrack;Regal&rbrack; Neuer Ton-Shader zur Anzeige von Details mit dem Height-/Normalkanal
* &lbrack;Regal&rbrack; Neuer Baking geführt Lichtfilter mit Umgebungseingabe
* &lbrack;Regal&rbrack; Einige Maskengenerator wurden aktualisiert, um nicht quadratische Transformationen hinzuzufügen
* &lbrack;Viewport&rbrack; Composited Normalen-Map (Normal+Height+Baking) zum Solomodus hinzufügen
* &lbrack;Skripterstellung&rbrack; Exportieren zusätzlicher Maps zulassen
* &lbrack;Skripterstellung&rbrack; Abfragen verfügbarer zusätzlicher Maps pro Textursatz zulassen
* &lbrack;Skripterstellung&rbrack; Abrufen des Kanalformats zulassen
* &lbrack;Skripterstellung&rbrack; Fügen Sie der Baking führend Dokumentation Beispiele hinzu
* &lbrack;Skripterstellung&rbrack; Abfragen der Sichtbarkeit einer Ebene zulassen
* &lbrack;Skripterstellung&rbrack; Füllmethode und Deckkraft der Ebene abfragen
* &lbrack;Skripterstellung&rbrack; Exportieren konvertierter Maps (endgültige Normalen-Map, gemischte AO usw.) zulassen
* &lbrack;Substance&rbrack; Benutzerdefinierte Verwendungen lesen und verbinden
* &blbrack;Shortcuts&rbrack; Zusatztaste (SHIFT) hinzufügen, um Solo-Modus rückwärts zu durchlaufen
* &lbrack;Export&rbrack; Standardexportvorgabe wurde aktualisiert, um Alpha zu deaktivieren
* &lbrack;UI&rbrack; Miniaturen werden jetzt nur berechnet, wenn das Engine verfügbar ist
* &lbrack;UI&rbrack; Anzeigen einer Erwähnung bei der Berechnung von Miniaturansichten

**Fest:**

* Absturz zu einigen alten Projekten beim Öffnen
* Absturz mit beschädigtem Textur-Kanal-Cache
* Absturz beim Mischen von mehr als 4 Materialien mit dem Material-Ebenen-Arbeitsablauf
* &lbrack;UI&rbrack; Tastaturbefehle funktionieren nicht, wenn die Symbolleiste ausgeblendet ist
* &lbrack;UI&rbrack; Iray-Werkzeugleiste ist im Ansichtsmenü mit &quot;Unbenannt&quot; beschriftet
* &lbrack;UI&rbrack; Plug-in-Symbolleisten werden im Menü &quot;Ansicht&quot; als &quot;Nicht geneigt&quot; bezeichnet
* &lbrack;Baker&rbrack; Durch Drücken der Eingabetaste beim Bearbeiten einer Baking-Einstellung wird der Baking-Prozess gestartet
* &lbrack;Baker&rbrack; Falsche Bereiche für einige Parameter
* &lbrack;Import&rbrack; Import von OBJ-Meshs aufgrund sehr großer Zahlen nicht möglich
* &lbrack;Import&rbrack; Einige OBJ werden mit zu vielen Unterobjekten importiert
* &lbrack;Export&rbrack; Kanalhintergrund wird beim Export mit Schwarz anstelle der Standardfarbe gefüllt
* &lbrack;Werkzeug&rbrack; Partikeln funktionieren nicht richtig, wenn der FOV-Wert zu niedrig ist
* &lbrack;Werkzeug&rbrack; Die Pinselvorschaufarbe ist bei Masken in untergeordneten Stapeln falsch
* &lbrack;Viewport&rbrack; Wenn der Pinsel in leere Bereiche in der 2D-Ansicht übergeht, wird er gigantisch
* &lbrack;Viewport&rbrack; Leere Pinselvorschau beim Malen mit normalen Texturen
* &lbrack;Skripterstellung&rbrack; Falsche Dokumentation : &quot;ao&quot; anstelle von &quot;ambientocclusion&quot; aufgeführt
* &lbrack;Skripterstellung&rbrack; Der mit subprocess() gestartete Prozess wird beim Schließen von Painter beendet
* &lbrack;Regal&rbrack; Baking geführt Beleuchtungsfilter verwenden falsche AO-Eingabe
* &lbrack;MacOS&rbrack; Entferntes Fire Hydrant-Projekt (inkompatibel)
* Standardprojekt wird beim Laden einer \*.spt-Datei geöffnet (anstelle von \*.spp).

**Bekannte Probleme:**

* &lbrack;Plugin&rbrack; Aufgrund von Photoshop können das Height und der normale Kanal nicht unverändert Kamera bewogen werden.

### 2.2.0

*(Freigegeben: 22. Juli 2016)*

**Hinzugefügt:**

* &lbrack;Regal&rbrack; Verbesserung des Suchsystems und der Suchanfragen
* &lbrack;Regal&rbrack; Hinzufügen eines Suchfelds für Mini-Regals
* &lbrack;Shader&rbrack; Festlegen der Schrittgenauigkeit für Schieberegler
* &lbrack;Shader&rbrack; Hinzufügen einer Schaltfläche &quot;Rückgängig/Wiederholen&quot; für Shader-Parameter
* &lbrack;Shader&rbrack; Das erneute Laden eines Shader sollte seine Parameter nicht zurücksetzen.
* &lbrack;MatLayering&rbrack; Unterstützung für Dynamische Materialüberlagerung und Sub-Stapel hinzufügen
* &lbrack;MatLayering&rbrack; JSON-Datei zum Einrichten der Shader-Einstellungen importieren
* &lbrack;MatLayering&rbrack; Limit für Textur-Sampler entsperren (Wechsel zu Bindless-Texturen)
* &lbrack;Skripterstellung&rbrack; Festlegen der Baker-Einstellungen und Starten der Berechnung zulassen
* &lbrack;Substance&rbrack; &quot;Verwendung&quot; für Ein-/Ausgangsverbindungen zusätzlich zu den Identifizierungen verwenden
* &lbrack;Werkzeug&rbrack; Auswahl des Vorschaukanals im Viewport für das Projektion-Werkzeug zulassen

**Fest:**

* Absturz beim Start, wenn sich die Substanzen im falschen Ordner befinden
* Der Absturz-Bericht funktioniert aufgrund einer falschen Protokolldatei manchmal nicht
* &lbrack;Iray&rbrack; Post-Effekte werden nicht aktualisiert, wenn das Iray angehalten wird
* &lbrack;Iray&rbrack; Autofokus-Tastaturbefehl funktioniert nicht mehr
* &lbrack;Iray&rbrack; Verhalten des Reglers &quot;Blende&quot; ändert sich je nach Elementgröße.
* &lbrack;Layers&rbrack; Der Kanal des ersten Materials ist standardmäßig nicht aktiviert, wenn alle deaktiviert sind
* &lbrack;Shader&rbrack; Es werden keine Fehler gedruckt, wenn ein &quot;automatischer Parameter&quot; falsch ist

**Bekannte Probleme:**

* &lbrack;Mac&rbrack; Grenzwert für Textur-Samples auf 16 gesperrt (GPU-Treiberproblem)

### 2.1.1

*(Freigegeben: 1. Juli 2016)*

**Hinzugefügt:**

* &lbrack;Lizenz&rbrack; Ändern des Speicherorts der Lizenzdatei
* &lbrack;Viewport&rbrack; Hinzufügen eines &quot;B&quot;-Tastaturbefehl, um zwischen weiteren Karten zu wechseln
* &lbrack;Import&rbrack; FBX 2016/2017 ordnungsgemäß importieren
* &lbrack;Werkzeug&rbrack; Entfernen von Häkchen bei Verwendung der schnelle Maske
* &lbrack;Iray&rbrack; Informationen zu den Abmessungen der Szene hinzufügen
* &lbrack;Iray&rbrack; Zulassen, dass die maximale Anzahl von Samples und die Renderzeit erhöht werden
* &lbrack;UI&rbrack; Ergebnis sofort aktualisieren, wenn +/- Taste auf Schiebereglern verwendet wird
* &lbrack;UI&rbrack; Höhere Präzision bei den Graustufen-Reglern
* &lbrack;Export&rbrack; Exportieren Sie keinen Alphakanal für Texturen, die nur RGB sind
* &lbrack;Export&rbrack; Exportvorgabe &quot;Dota 2 aktualisieren&quot;
* &lbrack;Regal&rbrack; Neues Muster &quot;Sechseckfliesen&quot;
* &lbrack;Regal&rbrack; Neues Werkzeug &quot;Verschweißt&quot;
* &lbrack;Regal&rbrack; Die Abschlussfilter wurden aktualisiert, um Richtungssteuerungen bereitzustellen.

**Fest:**

* &lbrack;Export&rbrack; PSD-Dateien mit 8 Bit können nicht exportiert werden
* &lbrack;Export&rbrack; 8K-Export ist bei einigen Hardware-Konfigurationen nicht verfügbar
* &lbrack;Export&rbrack; Das Sketchfab-Fenster ist zugeschnitten
* &lbrack;Export&rbrack; Falsche Rauheit in der Vorgabe für den Export von Spezifikation/Glanz
* &lbrack;UI&rbrack; Die Eingabe in Graustufenreglern funktioniert nicht mehr
* &lbrack;UI&rbrack; Es ist nicht möglich, Filter in Substance-Eingaben zu integrieren (wie Generatoren)
* &lbrack;UI&rbrack; Einige Regler haben ein seltsames Verhalten.
* &lbrack;UI&rbrack; DeltaTime +/- für Partikeln ist zu groß
* &lbrack;Iray&rbrack; Einige Projekte blockieren die Anwendung beim Wechsel zu Iray
* &lbrack;Iray&rbrack; Absturz beim Erkennen von Hardware
* &lbrack;Werkzeug&rbrack; Die Pinselvorschaufarbe ist im Maskenmodus falsch
* &lbrack;Werkzeug&rbrack; Die Werkzeugauswahl kann mit inkompatiblen Materialien verwendet werden
* &lbrack;Werkzeug&rbrack; Projektion-Vorschau wechselt nicht zu Diffuse mit Spec/Gloss-Workflow
* &lbrack;Regal&rbrack; Ändern des Standard-Shader unterbricht Smart Mats/intelligente Masken-Vorschauen
* &lbrack;Regal&rbrack; Einige intelligente Material haben falsche Namen.
* &lbrack;Regal&rbrack; Zusätzliche Alpha-Formen sind beschädigt und werden nicht geladen.
* &lbrack;Viewport&rbrack; Wechseln in den Modus &quot;Zusätzliche Karte&quot; zeigt zuerst &quot;andere&quot; an
* &lbrack;Viewport&rbrack; Viewport wechseln zurück zu &quot;Andere&quot;, wenn keine zusätzliche Map vorhanden ist
* &lbrack;Absturz&rbrack;&lbrack;Linux&rbrack; Absturz-Bericht funktioniert nicht auf Ubuntu (Steam)
* &lbrack;Absturz&rbrack;&lbrack;Linux&rbrack; Web-URL-Links funktionieren nicht auf Ubuntu (Steam)
* &lbrack;Absturz&rbrack;&lbrack;Windows&rbrack; Entfernen Sie &quot;crashwatcher&quot;, wenn Substance Painter nicht mehr ausgeführt wird.
* &lbrack;Absturz&rbrack;&lbrack;Mac&rbrack; Absturz-Berichtssystem funktioniert nicht richtig
* &lbrack;Absturz&rbrack; Das Importieren eines Meshs, während bereits ein Mesh importiert wurde, führt zu einem Absturz
* Textursatz beim Auswählen eines Tastaturbefehl nach einem Neustart auf nichts zurückgesetzt

### 2.1.0

*(Freigegeben: Juni 2016)*

**Hinzugefügt:**

* &lbrack;UDIM&rbrack; Importieren von UDIM-Kacheln aus einem Mesh als Textursatz
* &lbrack;Linux&rbrack; Neue Unterstützung für CentOS 6.6 und Ubuntu 12.4
* &lbrack;Export&rbrack; Hinzufügen einer 8K-Auflösung (experimentell)
* &lbrack;Export&rbrack; Auswahl der Bittiefe während des Exports zulassen
* &lbrack;Baker&rbrack; Baking mehrerer Textursatz gleichzeitig zulassen
* Unterstützung hochauflösender Monitore (hohe DPI-Skalierung)
* &lbrack;Skripterstellung&rbrack; Benutzerdefinierte Auflösung und Innenabstände pro Textur beim Export festlegen
* &lbrack;Viewport&rbrack; Erlaubt das Wechseln zwischen Textursatz durch Klicken auf den Mesh (über Strg+Alt+Klick)
* &lbrack;Viewport&rbrack; Bewegen des Mauszeigers beim Zoomen mit dem Mausrad
* &lbrack;UI&rbrack; Standardhintergrundfarbe und Umgebungs-Map-Anzeige aktualisieren
* &lbrack;UI&rbrack; QuickInfos mit Originalnamen für Benutzerkanäle hinzufügen
* &lbrack;UI&rbrack; Hintergrundfarbe für Kanäle ändern, die nicht umbenannt werden können
* &lbrack;Werkzeug&rbrack; Entfernen von Häkchen bei Verwendung der schnelle Maske
* &lbrack;Shader&rbrack; Erlaubt das Definieren von Gruppen für Shader-Parameter und Materialien/Masken.
* &lbrack;Engine&rbrack; Optimierung der Kleinstprägung
* &lbrack;Schablone&rbrack; W als Tastaturbefehl hinzufügen, um die Maske vorübergehend zu aktivieren bzw. zu deaktivieren
* &lbrack;Regal&rbrack; Kreuzschaltfläche zum Löschen des Suchfelds hinzufügen
* &lbrack;Regal&rbrack; Alpha mit einem Klick laden
* &lbrack;Regal&rbrack; Neue Exportvorgabe : Vray UDIM, Arnold UDIM, Spec/Gloss von Metal/Rough
* &lbrack;Regal&rbrack; Neue Alphas : geometrische Formen, Adern und Zeichen
* Namen und Version in den Eigenschaften der ausführbaren Substance Painter-Datei hinzufügen

**Fest:**

* &lbrack;Substance&rbrack; Es ist nicht möglich, den normalen Kanal und die zusätzliche Karte gleichzeitig zu verwenden
* &lbrack;Iray&rbrack; MDL-Brechung und Absorption-Einstellung funktionieren nicht
* &lbrack;Iray&rbrack; Originalskala der Szene wird nicht beibehalten
* &lbrack;Regal&rbrack; Specular/Glanz-Vorlage verwendet falschen Shader
* &lbrack;Export&rbrack; Bei der Standard-Exportvorgabe werden einige Maps (wie AO) nicht exportiert.
* &lbrack;Viewport&rbrack; Pivot-Punkt wird nicht aktualisiert, wenn Sie außerhalb der UVs in der 2D-Ansicht klicken
* &lbrack;UI&rbrack; Reglerwerte sind abgerundet
* &lbrack;UI&rbrack; Manchmal ist beim Bearbeiten der Reglerwerte der Speicherplatz sehr klein
* &lbrack;Neues Projekt&rbrack; Die Dropdown-Liste für Vorlagen wurde nicht korrekt aktualisiert (von 1.x auf 2.x)
* &lbrack;Skripterstellung&rbrack; &quot;Hover&quot;-Verhalten bei benutzerdefinierten Schaltflächen behoben
* &lbrack;Mac&rbrack; Durch Rückgängigmachen für ein leeres Projekt wird die Kamera gesperrt

**Bekannte Probleme:**

* Absturz-Bericht ist auf Ubuntu nicht verfügbar
* Einige URL-Schaltflächen funktionieren möglicherweise nicht. In unseren FAQs finden Sie eine Problemumgehung

### 2.0.5

*(Freigegeben: 29. April 2016)*

**Hinzugefügt:**

* &lbrack;Regal&rbrack; Hinzugefügte/aktualisierte Nicht-PBR-Vorlage, Shader- und Exportvoreinstellung
* &lbrack;Regal&rbrack; Die UE4-Exportvorgabe wurde aktualisiert und enthält jetzt auch Ambient occlusion

**Fest:**

* Absturz beim Öffnen und Speichern einiger Projekte mit beschädigten Ressourcen
* &lbrack;Viewport&rbrack; Drahtgitter erscheint in der 2D-Ansicht beschädigt
* &lbrack;Regal&rbrack; Verbesserte Performance einiger Studio-Umgebungs-Map
* &lbrack;Regal&rbrack; Einige Studio-Umgebungs-Map sind dupliziert.
* &lbrack;Regal&rbrack; Fehlendes &quot;Baking geführt Beleuchtungs-Material&quot;
* &lbrack;Regal&rbrack; Fehlender Generator für &quot;Graustufen-Konvertierung&quot;

### 2.0.4

*(Freigegeben: 26. April 2016)*

**Hinzugefügt:**

* Verbessern von Mesh-Kollisionen und Optimieren des Drahtgitter-Renderings
* Verbessern der Performance und des Arbeitsspeicher-Managements durch umfangreiche Projekte
* Verbessern der Schiebereglerpräzision und des Schrittmachers
* &lbrack;UI&rbrack; Engine nur bei der Validierung eines Schiebereglers aktualisieren (nicht bei der Eingabe eines Werts)
* &lbrack;UI&rbrack; Iray-Switch auf eine dedizierte Schaltfläche in der Hauptsymbolleiste bewegen (und seinen Tastaturbefehl ändern)
* &lbrack;Werkzeug&rbrack; Einstellung für das Quellspeicherortverhalten des Klonwerkzeugs hinzufügen
* &lbrack;Shader&rbrack; Lesen der Scheitelpunkt-Farben von Meshs in benutzerdefinierten Shadern zulassen
* &lbrack;Skripterstellung&rbrack; Liste der Textursatz, Kanäle und Ebenen abrufen
* &lbrack;Skripterstellung&rbrack; Helfer-Funktionen hinzufügen (URL zum Pfad, Exportpfad aus Projekt abrufen)
* &lbrack;Mac&rbrack; Erkennen der Mac OS-&quot;El Capitan&quot;-Version in der Protokolldatei

**Fest:**

* Absturz nach zweitem Export auf Substance share
* Absturz beim Kopieren einer Ebene zwischen Textursätzen mit Schnelle Maske-Daten.
* Einige Projekte haben einen sehr langen Updater, der viel Speicher beansprucht
* &lbrack;Werkzeug&rbrack; Absturz beim Auswählen einer Partikel-Vorgabe mit dem Klon-/Verwischen-Werkzeug
* &lbrack;Baker&rbrack; Das Laden von FBX dauert bei großen Meshs zu lange
* &lbrack;Viewport&rbrack; Gedehnt Umgebungs-Map auf einigen Computern
* &lbrack;Viewport&rbrack; Falsche Gamma-Konvertierung der Alpha-Zahl des Pinsels
* &lbrack;Export&rbrack; Alpha wird als Transparenz gespeichert und nicht als separater Kanal mit Tiff-Dateien.
* &lbrack;Export&rbrack; Normaler Kanal wird immer als OpenGL exportiert
* &lbrack;Iray&rbrack; Fehlende Schiebereglernamen für Iray-Einstellungen
* &lbrack;Iray&rbrack; Das Rendern erfolgt mit einer falschen Auflösung bei Retina/High DPI.
* &lbrack;Iray&rbrack; Absturz beim Skalieren der Benutzeroberfläche im Iray-Modus
* &lbrack;Iray&rbrack; Hohe Leistungsverlangsamung beim Rendern mit einigen niedrigen Auflösungen
* &lbrack;Iray&rbrack; Pause funktioniert nicht (Iray wird noch im Hintergrund berechnet)
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

* &lbrack;Iray&rbrack; Spezifikations-/Glanzvorlage und Shader aktualisieren, um mit Iray kompatibel zu sein
* &lbrack;Export&rbrack; Screenshots nach ArtStation exportieren
* &lbrack;Skripterstellung&rbrack; Unterstützt die Ausführung aus dem Plug-in-Verzeichnis
* &lbrack;Skripterstellung&rbrack; &quot;Speichern unter&quot; zulassen
* &lbrack;UI&rbrack; Doppelklicken auf einen Schieberegler, um den Wert zu bearbeiten
* Vela-Beispiel auf Substance share verschieben
* Neues Beispielprojekt : Kugelvorschau
* Benutzer vor einem Konflikt mit Shellerweiterungen warnen

**Fest:**

* Installation von Substance Painter 1.x durch Installationsprogramm außer Kraft gesetzt
* &lbrack;UI&rbrack; Das Layout der Kanalliste wurde mit Filtern unterbrochen
* &lbrack;UI&rbrack; Shader-Parameter werden nicht angezeigt
* &lbrack;UI&rbrack; Durch Ändern der Größe des Ebenenfensters wird der Inhalt falsch zugeschnitten
* &lbrack;Werkzeug&rbrack; Der Deckkraftkanal wird nicht immer richtig verwendet
* &lbrack;Werkzeug&rbrack; Verwischen/Klon funktioniert nicht mit Symmetrie
* &lbrack;Werkzeug&rbrack; Die Deckkraft der Pinselvorschau ist bei einigen Kanälen falsch
* &lbrack;Iray&rbrack; Absturz bei der Verwendung von Iray, obwohl es noch nicht erstellt wurde
* &lbrack;Iray&rbrack; Die Rastereinstellungsdaten aus dem Projekt können nicht geladen werden.
* &lbrack;Iray&rbrack; Iray kümmert sich nicht um die Einstellungsänderung, nachdem sie angehalten wurde
* &lbrack;Regal&rbrack; Das Importieren eines Materials in das Regal funktioniert nicht
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
* &lbrack;Werkzeug&rbrack; Neues Verwischen-Werkzeug zum Mischen und Verteilen von Farben
* &lbrack;Werkzeug&rbrack; Neues Klon-Werkzeug zum Kopieren von Teilen einer Textur
* &lbrack;Werkzeug&rbrack; Auswählen von Kanälen für das Verwischen-, Klon- und Radiergummi-Werkzeug zulassen
* &lbrack;Ebene&rbrack; Name des Substance für den Fülleffekt hinzufügen
* &lbrack;Ebene&rbrack; Exportieren der Maske in die Zwischenablage zulassen
* &lbrack;Viewport&rbrack; Zwischen Perspektive und orthografischem Modus wechseln
* &lbrack;Viewport&rbrack; Sichtfeld im Perspektive-Modus steuern
* &lbrack;Viewport&rbrack; Erlaubt das Festlegen der Tiefe des Feldabstands mit STRG + Mittelklick
* &lbrack;Viewport&rbrack; Lassen Sie zu ziehen und Umgebungs-Map in der 3D-Ansicht ablegen.
* &lbrack;Viewport&rbrack; Verbessertes Feedback bei umfangreichen Berechnungen des Engine
* &lbrack;Export&rbrack; Exportieren von Shader-Parametern in eine JSON-Datei zulassen
* &lbrack;UI&rbrack; Benutzeroberfläche mit neuen Symbolen, Farben und Layout aktualisieren
* &lbrack;UI&rbrack; Namen von Elementen zu Mini-Regals hinzufügen
* &lbrack;UI&rbrack; &quot;Kanal-Mapping&quot; standardmäßig reduzieren
* &lbrack;Shader&rbrack; Benutzerdefinierte Farbe für die Parameter der Shader-Textur auswählen
* &lbrack;Regal&rbrack; Frage beim Ziehen und Ablegen von Ressourcen nach dem Speicherort für Dateien
* &lbrack;Regal&rbrack; Neuer Vorschaubereich für Intelligente Material und Generatoren
* &lbrack;Regal&rbrack; Specular Glanz Shader hinzufügen
* &lbrack;Regal&rbrack; Neue Formen für harte Oberflächen
* &lbrack;Regal&rbrack; Neue Alphas Texturen und Formen
* &lbrack;Regal&rbrack; Neue Skin-Texturen
* &lbrack;Regal&rbrack; Neue Scan-basierte Material und Smart-Material
* &lbrack;Regal&rbrack; Neue intelligente Materialien und Spec/Gloss-Unterstützung von alten
* &lbrack;Regal&rbrack; Neue Finish-Filter für die metallic Oberflächensimulation
* &lbrack;Regal&rbrack; Neuer leistungsstarker Maskengenerator &quot;Maskeneditor&quot;
* &lbrack;Regal&rbrack; Alte Materialien überarbeitet und bereinigt
* Neues Beispielprojekt &quot;Vela&quot;

**Fest:**

* &lbrack;Einstellungen&rbrack; Die Drehung der Kamera und die Zoomgeschwindigkeit werden vom Projekt außer Kraft gesetzt.
* &lbrack;Viewport&rbrack; Genauigkeitsproblem bei der standardmäßigen normalen Textur führt zu falschen Reflexionen
* &lbrack;Viewport&rbrack; Vignette ist standardmäßig aktiviert
* &lbrack;Viewport&rbrack; Artefakte werden an den Umgebungs-Map-Rändern angezeigt (Nvidia-GPUs)
* &lbrack;Viewport&rbrack; Miniaturansicht im Modus &quot;Projektion/Schablone&quot; ist sehr lang zum Laden
* &lbrack;Baker&rbrack; Baking geführt Texturen in 16-Bit- statt in 32-Bit-Ganzzahl speichern
* &lbrack;Ebene&rbrack; Veraltete Stoffe werden im Stapel falsch dargestellt
* Standardfarbe und Bit-Tiefe für einige Kanäle sind falsch (z. B. : Specular, Glanz)
* Radierverhalten zum Deaktivieren der Füllmethode im Passthrough-Modus wurde korrigiert

**Bekannte Probleme:**

* Symmetrie funktioniert nicht mit dem Verwischen- und Klon-Werkzeug
* ArtStation-Export fehlt

## Version 1

### 1.7.3

*(Freigegeben: 1. März 2016)*

**Hinzugefügt:**

* &lbrack;Export&rbrack; Hinzufügen einer Option zum Deaktivieren der Auffüllung
* &lbrack;Regal&rbrack; Untergeordnete Elementhierarchie innerhalb eines Regal-Regals unterstützen

**Fest:**

* Absturz beim Speichern über einer zuvor schreibgeschützten Datei
* Absturz beim Öffnen eines zweiten Projekts
* Absturz beim Laden einiger Miniaturansichten (Regal, Ebenen oder QuickInfos)
* Die Deaktivierung von &quot;Konturpositionen auf dem Mesh beibehalten&quot; funktioniert nicht
* &lbrack;Export&rbrack; Die Hochskalierung von Bitmaps erfolgt mit nächstgelegenen Filterungen
* &lbrack;Regal&rbrack; Die Suche nach Ressourcen ist sehr langsam
* &lbrack;Regal&rbrack; Weichzeichnungsfilter sind nicht 16 Bit kompatibel
* &lbrack;Werkzeug&rbrack; Symmetrie funktioniert nicht, wenn Sie eine alte Werkzeugvorgabe laden
* Das Farbdialogfeld für den Specular-Kanal führt keine Farbraumkonvertierung durch

### 1.7.2

*(Freigegeben: 13. Januar 2016)*

**Hinzugefügt:**

* &lbrack;Layers&rbrack; Festlegen der Standardbearbeitung für Füllebenen zulassen

**Fest:**

* &lbrack;Export&rbrack; Sketchfab-Export funktioniert nicht mehr
* &lbrack;Ebene&rbrack; Bilineare Filterung wird auch bei &quot;Füllung&quot; ohne Transformation angewendet
* &lbrack;Werkzeug&rbrack; Schlechte Projektion durch Substance-Effekte mit Bildeingaben im Bewegungsmodus
* &lbrack;Werkzeug&rbrack; Material-Auswahl ist defekt

### 1.7.1

*(Freigegeben: 18. Dezember 2015)*

**Fest:**

* Absturz beim Wechseln des Textursatzes
* Langsame Bewegungen beim Malen

### 1.7.0

*(Freigegeben: 17. Dezember 2015)*

**Hinzugefügt:**

* &lbrack;Performances&rbrack; Berechnen des Inhalts von Ebenen und ihrer Miniaturansichten gleichzeitig
* &lbrack;Export&rbrack; Speichern Sie den Exportpfad als relativ, wenn er sich neben dem Projekt befindet
* &lbrack;Layers&rbrack; Neuer Mischmodus hinzugefügt : Subtrahieren und Hinzufügen/Subtrahieren
* &lbrack;Layers&rbrack; Neue Bilineare Filterungen des Hauptquartiers für Füllebenen
* &lbrack;Shader&rbrack; Legen Sie in den Voreinstellungen einen Standard-Shader für die Miniaturansichtenerstellung fest.
* &lbrack;Shader&rbrack; Geben Sie einen Shader pro Textursatz an
* &lbrack;Shader&rbrack; Texturen aus dem Regal aufnehmen
* &lbrack;Werkzeug&rbrack; Neues Pinselverhalten &quot;Umbrechen&quot; für das Malen
* &lbrack;Werkzeug&rbrack; Verbesserte Filterung und reduziertes Aliasing beim Malen
* &lbrack;Werkzeug&rbrack; Verbesserte Malqualität von Subpixeln
* &lbrack;Werkzeug&rbrack; &quot;Einfache&quot; Anzeige für Pinseleinstellungen entfernt und das Symbol zum Öffnen/Schließen des Rahmens verbessert
* &lbrack;Menü&rbrack; Hinzufügen von Effektsymbolen im Kontextmenü
* Vorlagenerstellung aus Projekten
* &lbrack;Regal&rbrack; Neue Vorlagen : PBR, Dota 2
* &lbrack;Regal&rbrack; Neue Exportvorgabe : Dota 2
* &lbrack;Regal&rbrack; Neue Shader : Dota 2, PBR Car Malen, PBR Coated, PBR Velvet
* &lbrack;Regal&rbrack; Neues Material : Rost und Verschleiß aus Stahl, Stilisierte Beleuchtung
* &lbrack;Regal&rbrack; Neue Filter : Weichzeichnen von gerichtetem, stilisiertem Licht
* &lbrack;Regal&rbrack; Neuer Pinsel : Standardmäßige weiche und Standardfestplatte mit einem neuen Alpha für eine bessere Steuerung der Härte
* &lbrack;Regal&rbrack; Neue Generatoren : 3D-Abstand und -Licht
* &lbrack;Regal&rbrack; Aktualisierte Pinsel mit Projektion und Rückseiten-Ausblendung des Textumbruchs (standardmäßig aktiviert)
* &lbrack;Regal&rbrack; Weißer Rauschen mit Pixelprozessor-Version wurde für eine schnellere Berechnung aktualisiert

**Fest:**

* &lbrack;Begrüßungsbildschirm&rbrack; Link &quot;Tutorials&quot; - an alte Videos senden
* &lbrack;Channels&rbrack; Wenn Sie &quot;Nein&quot; zur Erstellung einer Füllebene mit AO sagen, wird trotzdem die Ebene erstellt.
* &lbrack;Channels&rbrack; Benutzer-X-Kanalnamen werden in der Schnittstelle nicht weitergegeben
* &lbrack;Viewport&rbrack; Der Maskeneintrag ist in der Liste der Solokanäle leer.
* &lbrack;Share&rbrack; Beim Exportieren eines Alpha-Elements in die Freigabe vom SP wird eine unlesbare .image-Datei erstellt.
* &lbrack;Lizenz&rbrack; Aktivierung für Benutzernamen mit Nicht-ASCII-Zeichen beheben
* &lbrack;Shader&rbrack; Dialogfeld &quot;Farbparameter&quot; wird beim Auswählen einer Farbe ausgeblendet
* &lbrack;Regal&rbrack; Miniaturen werden nicht aus dem Speicher entladen, wenn sie nicht verwendet werden
* &lbrack;Regal&rbrack; Filter mit festem Verlauf
* &lbrack;Werkzeug&rbrack; Symmetrie funktioniert nicht mit Schablone/Projektion
* &lbrack;Werkzeug&rbrack; Falscher Name beim Erstellen einer neuen Pinselvorgabe
* Die Option &quot;Kontur beibehalten&quot; bleibt auch beim erneuten Importieren eines Meshs deaktiviert
* TDR (Driver Reset) beim Berechnen von Partikeln mit großen Abmessungen.

### 1.6.1

*(Freigegeben: 9. November 2015)*

**Fest:**

* Absturz beim Öffnen des Projekts, wenn die 2D-Ansicht sichtbar ist
* Absturz beim Erstellen einer neuen Exportvorgabe, wenn das aktuelle Regal nicht vorhanden ist
* &lbrack;Werkzeug&rbrack; Symbol für die Material-Auswahl kann angezeigt bleiben
* &lbrack;Werkzeug&rbrack; Material-Auswahl blendet den Mauszeiger aus, wenn gleichzeitig gemalt wird
* &lbrack;Regal&rbrack; Metadaten werden nach jedem Beenden auf die Festplatte geschrieben

### 1.6.0

*(Freigegeben: 29. Oktober 2015)*

**Hinzugefügt:**

* Offizielle Unterstützung für Windows 10
* &lbrack;Substance&rbrack; Substanzparametergruppen standardmäßig reduzieren
* &lbrack;Substance&rbrack; Neues Framework hinzufügen (Verbesserung der Pixelprozessor-Performance)
* &lbrack;Viewport&rbrack; Erlaubt die Deaktivierung der Anzeige der Symmetrie-Ebene im Symmetrie-Modus.
* &lbrack;Viewport&rbrack; Verbessern des Renderings von Schatten und der Leistung
* &lbrack;Viewport&rbrack; Berechnung von Schatten beim Malen anhalten
* &lbrack;Viewport&rbrack; Verbessern der Drahtgitter-Renderleistung
* &lbrack;Engine&rbrack; Verbesserte VRAM-Speicherverwaltung zur Reduzierung des Speicherplatzbedarfs
* &lbrack;Engine&rbrack; Verbessern der Leistungsaktualisierung auf AMD-GPUs für eine bessere Textur
* &lbrack;Engine&rbrack; Deaktivieren der Einstellung für die Threadoptimierung auf NVIDIA-GPUs für bessere Leistung
* &blase;Effekt&blase; Tag hinzufügen, um eine &quot;aufgefüllte&quot; Bildeingabe anzufordern
* &lbrack;Ebene&rbrack; Präzision des UV-Versatzes/der Skalierung in der Füllung erhöhen
* &lbrack;Ebene&rbrack; Skalierungsregler in der Füllung exponentiell machen
* &lbrack;Ebene&rbrack; Erlauben Sie, Materialien direkt in den Ebenenstapel zu ziehen und abzulegen.
* &lbrack;Ebene&rbrack; Ermöglicht das Ziehen und Ablegen von Filtern direkt in den Ebenenstapel
* &lbrack;Ebene&rbrack; Maskenpinselfarbe an die neu erstellte Maskenfarbe anpassen
* &lbrack;Shader&rbrack; Leg mehrerer Texcoords
* &lbrack;Shader&rbrack; Leg der Gamma-/Tonzuordnungsfunktion, um benutzerdefinierte Funktionen zu ermöglichen
* &lbrack;Baker&rbrack; Ändern der Standardeinstellungen des Bakers &quot;Position&quot; für die Verwendung von TriPlanar
* &lbrack;Werkzeug&rbrack; Benennen Sie &quot;Geometry Decal&quot; in &quot;Polygon Fill&quot; um.
* &lbrack;Regal&rbrack; Generatoren zur Unterstützung von TriPlanar aktualisieren : MG Metallkantenverschleiß, MG Maskenbildner, MG Glasfaser, MG Dirt
* &lbrack;Regal&rbrack; Aktualisieren von Materials mit neuen Einstellungen und Entfernen nicht verwendeter Materials
* &lbrack;Regal&rbrack; 22 neue intelligente Materialien (Kunststoff, Eisen, Stoff, Stahl und mehr)
* &lbrack;Regal&rbrack; Die Filter &quot;Schärfen&quot;, &quot;Weichzeichnen&quot; und &quot;Verformen&quot; mit aufgefüllten Bilddaten aktualisieren, um Nähte zu vermeiden
* &lbrack;Regal&rbrack; Verbessern der Verkrümmungseinstellungen für eine einfachere Verwendung
* &lbrack;Regal&rbrack; 2 neue prozedurale Rauschen: 3D Perlin Rauschen und 3D Worley Rauschen

**Fest:**

* &lbrack;Engine&rbrack; Die VRAM-Betragserkennung für die dedizierte GPU ist auf Mac falsch
* &lbrack;Engine&rbrack; Texturen werden im Viewport dunkler
* &lbrack;Engine&rbrack; Schlechte Leistung beim Malen unter mehreren Ebenen
* &lbrack;Engine&rbrack; Beim Öffnen des Projekts berechnete Ebenen unterscheiden sich von der zwischengespeicherten Version
* &lbrack;Substance&rbrack; Falsche Ergebnisse in 4K auf Mac
* &lbrack;Substance&rbrack; Die Parameter haben die falsche Reihenfolge.
* &lbrack;Shader&rbrack; Toon und verpixelte Shader sind total schwarz
* &lbrack;Shader&rbrack; Parameter verschwinden nach dem Ändern der env-map
* &lbrack;Regal&rbrack; Absturz beim Bereitstellen von PNG-Dateien im Generatorordner
* &lbrack;Regal&rbrack; Miniaturansichten werden mit niedriger Rauheit generiert
* &lbrack;Werkzeug&rbrack; Absturz bei Verwendung einer Bitmap im Pinsel-Alpha unter Windows
* &lbrack;Export&rbrack; Eine zusätzliche Kartenexportvorgabe exportiert jetzt eine RGB-Karte für die Position

### 1.5.7

*(Freigegeben: 24. September 2015)*

**Fest:**

* Absturz-Bericht funktioniert nicht mehr

### 1.5.6

*(Freigegeben: 21. September 2015)*

**Hinzugefügt:**

* &lbrack;Regal&rbrack; Verbessern der Qualität der Miniaturansichten (verwenden Sie 1K-Texturen)

**Fest:**

* &lbrack;Share&rbrack; Anmeldung mit einem anderen Konto nicht möglich
* &lbrack;Regal&rbrack; Miniaturansichten sind auf der Festplatte zu groß
* &lbrack;Regal&rbrack; Intelligente Materialien sind sehr langsam
* &lbrack;Windows&rbrack; Installation des Lizenz-Service beheben
* &lbrack;Channels&rbrack; Transmissive map wird standardmäßig als G8 erstellt

### 1.5.5

*(Freigegeben: 15. September 2015)*

**Hinzugefügt:**

* &lbrack;Regal&rbrack; Exportieren von Assets auf Substance share
* &lbrack;Regal&rbrack; Neue Kugelvorschau für Materialien hinzufügen
* &lbrack;Regal&rbrack; Verwenden Sie die Env-Karte &quot;Glasüberdachter Patio&quot; zum Generieren von Miniaturen
* &lbrack;Regal&rbrack; Auflösung der Miniaturbildgröße auf 512 x 512 Pixel erhöhen
* &lbrack;3D-Ansicht&rbrack; Umgebungsdrehungswert gelegt
* &lbrack;Windows&rbrack; Anwendung signieren

**Fest:**

* &lbrack;Baker&rbrack; Falsche Ergebnisse beim gleichzeitigen Baking von Karten
* &lbrack;3D-Ansicht&rbrack; Die Env-Map wird angezeigt, wenn kein Projekt geöffnet ist
* &lbrack;Layers&rbrack; Maskengenerator funktionieren nicht auf Ebeneninhalten
* &lbrack;Layers&rbrack; Sie können Malen auf ausgeblendeten Ebenen durchführen
* &lbrack;Regal&rbrack; Rauschen mit Dirt_5 und Dirt_6 sind identisch
* &lbrack;Regal&rbrack; Einige Maskengenerator sind verpixelt oder haben eine niedrige Qualität
* &lbrack;Werkzeug&rbrack; Falsche Gizmo-Drehung um bestimmte Winkel.
* &lbrack;Werkzeug&rbrack; Zu viele Kanäle führen dazu, dass die Kanalschaltflächen abgeschnitten werden
* &lbrack;Werkzeug&rbrack; Tastaturbefehl der Maske für Schnelle Maske umkehren funktioniert nicht
* &lbrack;Export&rbrack; Sketchfab: Schaltfläche &quot;Abbrechen&quot; wird nicht korrekt berücksichtigt
* &lbrack;Lizenz&rbrack; Aktivierung fehlgeschlagen, wenn die Lizenz nicht kopiert werden kann
* Der Framerate-Begrenzer funktioniert nicht mehr auf der Benutzeroberfläche

### 1.5.0

*(Freigegeben: 20. August 2015)*

**Hinzugefügt:**

* &lbrack;Shader&rbrack; Zeilennummer in Fehlermeldungen beim Kompilieren von Shader hinzufügen
* &lbrack;Regal&rbrack; Verbessern der Vorschauqualität von Miniaturen
* &lbrack;Regal&rbrack; Miniaturansichten für Intelligenten Materials automatisch erstellen
* &lbrack;Werkzeug&rbrack; Tastaturbefehl zur Einstellung der Härte im Stoff
* &lbrack;Werkzeug&rbrack; Graustufen-Widget für Geometrieaufkleber verwenden, wenn Sie sich über einer Maske befinden
* &lbrack;Werkzeug&rbrack; Tastaturbefehl zum Umkehren der Malen-Farbe beim Malen auf einer Graustufenkarte
* &lbrack;Viewport&rbrack; Anzeige des Drahtgitter und Farbänderung zulassen
* &lbrack;Viewport&rbrack; Hintergrund der Umgebung weichzeichnen
* &blbrack;Steuerung&blbrack; Hinzufügen von Drehung zu Pinselmaus-Kurzbefehlen
* &lbrack;Export&rbrack; Exportieren nach Sketchfab
* &lbrack;Export&rbrack; Erstellen von Exportvorgaben für Renderer
* &lbrack;Export&rbrack; Konvertierte Abbildung hinzufügen - Reflexion, F0 und 1/IOR
* &lbrack;UI&rbrack; Startbildschirm hinzufügen
* &lbrack;UI&rbrack; Standardlayout aktualisieren
* &lbrack;UI&rbrack; Hinzufügen fehlender QuickInfos und Umbenennen einiger Menüeinträge
* &lbrack;Layers&rbrack; Exportieren der aktuell ausgewählten Maske als Bitmap
* &lbrack;Layers&rbrack; Aktion &quot;Maske umkehren&quot; im Kontextmenü hinzufügen

**Fest:**

* &lbrack;Projekt&rbrack; Wenn sich die Pivot-Werte der Meshs in der FBX unterscheiden, werden die Meshs beim Importieren explodiert
* &lbrack;Substance&rbrack; Substance in Projektion-Tools sind in 256\*256 gesperrt
* &lbrack;Layers&rbrack; Absturz bei Verwendung von &quot;Maske löschen&quot;
* &lbrack;Export&rbrack; Falsche Gamma-Konvertierung auf sehr dunklen Texturen
* &lbrack;Export&rbrack; Die Positionszuordnung kann nur in Exportvorgaben als Graustufenzuordnung verwendet werden.
* &lbrack;Werkzeug&rbrack; Die Anfangsfarbe des Geometrie-Aufklebers ist schwarz, wenn er auf einer Maske verwendet wird
* &lbrack;Werkzeug&rbrack; &quot;Drehung - Tastaturbefehl&quot; funktioniert nicht, wenn keine Härte im Alpha-Wert vorhanden ist

### 1.4.2

*(Freigegeben: 15. Juli 2015)*

**Fest:**

* &lbrack;Werkzeug&rbrack; Absturz bei der Verwendung von Geometrieaufklebern mit schnelle Maske
* Beim Aktualisieren des Projekts von 1.4.0 auf 1.4.1 wird der gesamte Computerspeicher belegt.
* Falscher Import des alten Projektformats
* Bei benutzerdefinierten Regalen wird die gesamte Hierarchie analysiert, und Assets werden überall dupliziert.

### 1.4.1

*(Freigegeben: 23. Juni 2015)*

**Hinzugefügt:**

* &lbrack;Viewport&rbrack; Andocken von Fenstern nebeneinander zulassen
* &blase;Effekt&blase; Hinzufügen eines Hintergrunds und eines Lineals für den Ebeneneffekt
* &blase;Effekt&blase; Einen Malen-Effekt hinzufügen, der es ermöglicht, über andere Effekte zu arbeiten

**Fest:**

* &lbrack;Regal&rbrack; Miniaturgenerierung funktioniert nicht, wenn kein Projekt geöffnet ist
* &lbrack;Regal&rbrack; Materialvorgabe-Vorschau kann nicht generiert werden
* &lbrack;Regal&rbrack; Material-Vorschauen werden auf einem Mesh mit invertierten Normalen generiert
* &lbrack;Regal&rbrack; Miniaturen werden aufgrund einer falschen Hash-Funktion immer neu berechnet
* &lbrack;Regal&rbrack; Wenn Sie auf ein Substance-Material klicken, werden keine zusätzlichen Maps verbunden.
* &lbrack;Werkzeug&rbrack; Falscher Wert, der mit der Material-Auswahl aufgenommen wurde
* &lbrack;Werkzeug&rbrack; Farbwähler Viewport auswählen Cursorfarbe
* &lbrack;2D-Ansicht&rbrack; Sehr niedrige Framerate/Performance
* &lbrack;Export&rbrack; Absturz beim Öffnen des Exportfensters mit zu aktuellen Exportvorgaben.
* &lbrack;Export&rbrack; Height-Kanal auf Normalen-Map wird in den falschen Bereich konvertiert
* &lbrack;Mac&rbrack; BaseColor aus Substance-Effekten wird als Linear angezeigt
* &lbrack;Mac&rbrack; Widget für gerade Linien wurde auf der Retina falsch gezeichnet
* Gerade Linien können auch bei einem Loslassen des Tastaturbefehl aktiviert bleiben.
* Gerade Linien Guizmo verschwinden nach dem Drehen des Umgebungs-Map
* Ambient occlusion-Ausgänge von Stoffen werden nicht automatisch an den AO-Kanal angeschlossen
* Problem mit Lizenzkopien unter Windows mit Sonderzeichen im Benutzernamen beheben

### 1.4.0

*(Freigegeben: 10. Juni 2015)*

**Hinzugefügt:**

* &lbrack;Export&rbrack; Zusätzliche Maps in der Liste der verfügbaren Eingabe-Map hinzufügen
* &lbrack;Regal&rbrack; SBSAR-Materialien als Materialvorgaben verwenden
* &lbrack;Regal&rbrack; Verwenden benutzerdefinierter Bibliothekspfade zulassen
* &lbrack;Regal&rbrack; Die Mindestgröße ändern.
* &lbrack;Regal&rbrack; Neue Inhalte : 20 neue intelligente Material
* &lbrack;Regal&rbrack; Neue Inhalte : neuer prozeduraler Stoff (Gewebe, Mesh)
* &lbrack;Regal&rbrack; Aktualisierter Weichzeichnungsfilter
* Zeichnen von geraden Linien mit einer Zusatztaste
* Hinzufügen eines Ambient occlusion-Kanals und Überarbeiten des AO/Normal-Verhaltens im Ebenenstapel
* Lesen der Standardfarbe aus der Bildeingabe, die in den Substance-Benutzerdaten definiert ist
* Exportieren des Protokolls über das Hilfemenü zulassen

**Fest:**

* &lbrack;Baker&rbrack;&lbrack;Mac&rbrack; Absturz mit Normal vom Mesh Baker
* &lbrack;Baker&rbrack; Absturz, wenn die Käfig-Datei keine UVs enthält
* &lbrack;Baker&rbrack; Das Abgleichen nach Namen funktioniert nicht mit aus zBrush exportierten OBJ
* &lbrack;Baker&rbrack; Beim Baking mit einem Käfig wird das Baking überschrieben, wenn mehrere Textursatz und überlappende UVs verwendet werden.
* &lbrack;Baker&rbrack; Bestimmte OBJ führen zu schwarzen Texturen
* &lbrack;Regal&rbrack; Ressourcen können nicht gelesen werden, wenn sie auf schreibgeschützt festgelegt sind
* &lbrack;Regal&rbrack; Asset-Dateien werden in Painter geschrieben, wenn sie im Projekt verwendet wurden.
* &lbrack;Regal&rbrack; Durch erneutes Laden von Stoffen wird auch die Schicht aktualisiert
* &lbrack;Export&rbrack; Tiff exportiert 32-Bit-Bilder, die von Photoshop oder Game-Enginen nicht richtig gelesen werden können
* &lbrack;Export&rbrack; Standardkanalvorgaben werden immer als RGB exportiert
* &lbrack;Material&rbrack; Diffuse-Kanal überschreibt BaseColor-Zuordnung mit Stoffen
* &lbrack;3D-Ansicht&rbrack; Falsche Diffuse mit spezifischen Umgebungskarten
* &lbrack;Werkzeug&rbrack; Pinsel kann nicht in einen bestimmten Winkel gedreht werden
* Viewport erhält den Fokus, wenn der Mauszeiger während der Eingabe in einem Textfeld auf
* Absturz mit zu aktuellen Vorgaben für die aktuelle Version des Regals
* Absturz nach dem Ersetzen von Mesh
* Absturz beim erneuten Laden eines Stoffes mit einer anderen Anzahl von Einsatzstoffen
* FBX von Meshs aus dem Cinema4D-Import mit falschen Material-Namen

### 1.3.5

*(Freigegeben: 29. Mai 2015)*

**Hinzugefügt:**

* &lbrack;Lizenz&rbrack; Aktivierungsproblem, wenn eine bereits vorhandene Lizenzdatei vorhanden ist
* &lbrack;Mac&rbrack; Absturz beim Laden bestimmter FBX
* &lbrack;Mac&rbrack;&lbrack;3D-Ansicht&rbrack; Falsche Spiegelung für integrierte GPU
* &lbrack;3D-Ansicht&rbrack; Schnelle Maske-Schrift ist defekt
* &lbrack;3D-Ansicht&rbrack; Material-Picker macht den Viewport komplett schwarz
* Absturz nach dem Öffnen von Projekten, die in 1.3.3 erstellt wurden
* Die Vorschau des Materials ist leer, wenn Shader mit Alpha verwendet werden
* Malerei funktioniert nicht mehr an bestimmten Meshs
* Die Leistung nimmt mit bestimmten OBJ Meshs stark ab
* Benutzerkanäle werden bei Verwendung von Effekten nicht zugeordnet
* Temporäre Ordner werden beim Start nicht gesäubert

**Fest:**

* Verbesserte Berechnung des Projekts, das extrem lange geladen werden muss
* Ändern Sie das Fenster &quot;GPU-Fehlerbehebung&quot;, um verständlicher zu sein
* &lbrack;Layers&rbrack; Speichern Sie den Status der Verhältnissperre für Füllebenen und stellen Sie sie standardmäßig auf &quot;Ein&quot;
* &lbrack;Baker&rbrack; Bei der Zuordnung nach Namen wird jetzt das Suffix als Trennzeichen verwendet.

### 1.3.4

*(Freigegeben: 27. April 2015)*

**Hinzugefügt:**

* &lbrack;Mac&rbrack; Absturz mit Mac OS X Yosemite (10.10)
* &lbrack;Mac&rbrack; Vollbildmodus kann nicht beendet werden
* &lbrack;Baker&rbrack; Baking der Option &quot;Namensübereinstimmungen&quot; funktioniert nicht
* &lbrack;Baker&rbrack; Mikk-Tangente-Speicherplatz in SP funktioniert nicht mit UE4
* &lbrack;Baker&rbrack; ID-Baker kann die ID-Farben des Materials nicht Baking geführt haben
* &lbrack;2D-Ansicht&rbrack; Drahtgitter wird bei Verwendung des Geometry-Aufklebers nicht angezeigt
* &lbrack;Werkzeug&rbrack; Pinsel-Alphakanal wird bei Materialien als Checker anstelle von Transparenz angezeigt
* &lbrack;Werkzeug&rbrack; Absturz mit geometrischem Aufkleber
* &lbrack;Layers&rbrack; Der Steckplatz des Materials ist bei der Füllebene standardmäßig ausgeblendet
* &lbrack;Export&rbrack; Absturz beim Exportieren mit einer höheren Auflösung als der Textursatz
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
* &lbrack;Regal&rbrack; Neue Umgebungs-Map hinzufügen : Korsika Strand, Studio 05, Tornoco Studio und mehr
* &lbrack;Regal&rbrack; MG-Maskenbildner mit neuen Parametern aktualisieren
* &lbrack;Regal&rbrack; Alte Umgebungs-Map aktualisieren und kalibrieren

**Fest:**

* Absturz beim Öffnen des Exportfensters
* Drag &amp; Drop im UI-Widget ist nicht möglich, wenn abgedockt
* &quot;Nach Updates suchen&quot; funktioniert nicht
* &lbrack;Layers&rbrack; Wählen Sie die Maske nicht aus, wenn Sie bei gedrückter Alt-Taste darauf klicken
* &lbrack;Werkzeug&rbrack; Tri-planar funktioniert nicht mit dem normalen Kanal
* &lbrack;3D-Ansicht&rbrack; Diffuse Beleuchtung von env map ist nicht korrekt
* &lbrack;3D-Ansicht&rbrack; Die Berechnung der Belichtung unterscheidet sich von der in Designer
* &lbrack;3D-Ansicht&rbrack; Schatten sollten auf 100 % metallic Fläche nicht sichtbar sein.
* &lbrack;3D-Ansicht&rbrack; Mesh mit gespiegelten UVs hat gespiegelte Tangente/Binomale
* &lbrack;3D-Ansicht&rbrack; Schatten führen bei bestimmten Meshs zu falschen Ergebnissen
* &lbrack;Baker&rbrack; Ordner &quot;.alg_meta&quot;, der mit Assbin-Dateien erstellt wurde, entfernen
* &lbrack;Baker&rbrack; Absturz beim Baking, wenn Painter ein TextureSet gleichzeitig neu berechnet
* &lbrack;Mac&rbrack; Benutzeroberflächenfehler beim Starten der Anwendung

### 1.3.2

*(Freigegeben: 06. März 2015)*

**Fest:**

* &lbrack;3D-Ansicht&rbrack; Fehler beim erneuten Laden einer mit dem Projekt gespeicherten Env-Map.

### 1.3.1

*(Freigegeben: 05. März 2015)*

**Hinzugefügt:**

* &lbrack;Baker&rbrack; Fügen Sie eine zwischengespeicherte Version von Meshs mit hohem Poly-Anteil hinzu, um die Berechnung zu beschleunigen
* &lbrack;Baker&rbrack; Warnsymbol hinzufügen, wenn kein Mesh mit hoher Poly-Qualität geladen wird
* &lbrack;Baker&rbrack; Wenn kein Mesh mit hoher Poly-Qualität geladen wird, verwenden Sie stattdessen den Projekt-Mesh

**Fest:**

* &lbrack;Baker&rbrack; Drücken der &quot;Eingabe&quot; beim Bearbeiten des Werts eines Schiebereglers, um das Fenster zu schließen
* &lbrack;Baker&rbrack; Das Aktivieren/Deaktivieren eines Bakers löst ebenfalls die Schaltfläche aus.
* &lbrack;Baker&rbrack; Es kann nicht Baking geführt werden, wenn Sie die Schaltfläche &quot;all/none&quot; verwenden.
* &lbrack;Baker&rbrack; Die Sortierung der Baker-Schaltflächen ist nicht in der richtigen Reihenfolge.
* &lbrack;Baker&rbrack; Kontrollkästchen werden ignoriert und alle Baker werden immer verarbeitet.
* &lbrack;Baker&rbrack; Fortschritt der Fortschrittsleiste behoben

### 1.3.0

*(Freigegeben: 04. März 2015)*

**Hinzugefügt:**

* &lbrack;Baker&rbrack;&lbrack;3D-Ansicht&rbrack; Mikkt-Tangente-Raum-Berechnung verwenden, wenn keine Tangenten/Binormale gefunden wurden
* &lbrack;Baker&rbrack; Neue Baker hinzugefügt : Normal, ID, Verdeckung, Krümmung, Thickness, Position
* &blase;Effekte&blase; Der Stapel &quot;Effekt&quot; ist jetzt invertiert und wird von oben nach unten (wie Ebenen) angezeigt.
* &blase;Effekte&blase; Hinzufügen neuer Symbole auf dem Stapel des Effekts
* &blase;Effekte&blase; Fülloptionen im Stapel &quot;Effekt&quot; mit Füllmethode versehen
* &blase;Effekte&blase; Effekte umbenennen (Substance-Effekt = Filter, usw.)
* Hinzufügen einer &quot;gesperrten&quot; Datei während des Speichervorgangs
* &blase;Effekte&blase; Aktion &quot;Füllen&quot; im Stapel &quot;Effekt&quot; hinzufügen
* Neue Ressource hinzugefügt : Intelligente Materialien
* &lbrack;Layers&rbrack; Neuanordnung von Ebeneneffekten zulassen
* &lbrack;Werkzeug&rbrack; Planare Projektion hinzufügen
* &lbrack;3D-Ansicht&rbrack; Unterstützung für Schatten hinzufügen
* &lbrack;3D-Ansicht&rbrack; Möglichkeit, erforderliche OpenGL-Status in benutzerdefinierte Shader umzuwandeln
* &lbrack;3D-Ansicht&rbrack; Unterstützung für Alpha über neue Shader
* &lbrack;3D-Ansicht&rbrack; Shader sind jetzt versioniert und vollständig in einem Projekt gespeichert
* &lbrack;3D-Ansicht&rbrack; Benutzer warnen, wenn der Shader nicht mehr kompiliert wird

**Fest:**

* &lbrack;Layers&rbrack; Ablegen unter einem reduzierten Ordner korrigieren
* &lbrack;Regal&rbrack; Filterung von Inhalten in Mini-Regals korrigieren
* &lbrack;Regal&rbrack; Umbenennen von Kategorien und Neuanordnen von Registerkarten

### 1.2.1

*(Freigegeben: 12. Februar 2015)*

**Hinzugefügt:**

* \*.spp-Dateien können jetzt durch einen Doppelklick im Explorer geöffnet werden
* &lbrack;Export&rbrack; Neues Tag &quot;$project&quot; für Exportvorgaben
* &lbrack;Export&rbrack; Kartenliste (mit Nomenklatur) unter jedem Textursatz hinzufügen
* &lbrack;Export&rbrack; Schaltfläche &quot;Alle/Keine&quot; hinzufügen, um die Textursatz auszuwählen
* &lbrack;Export&rbrack; Leere Karten werden beim Export verworfen

**Fest:**

* &lbrack;Export&rbrack; Unity5-Vorgaben haben invertierte Karten
* &lbrack;Export&rbrack; Durch Hinzufügen eines Schrägstrichs in einem Vorgabename wird ein beschädigter Ordner erstellt.
* &lbrack;Export&rbrack; Height-Kanal, der in 32-Bit-Formate exportiert wird, ist falsch eingespannt
* &lbrack;Export&rbrack; Die Liste der Textursatz wird nicht wie im Projekt sortiert
* &lbrack;Werkzeug&rbrack; Rückseiten-Ausblendung funktioniert nicht mehr
* Speichern funktioniert nicht mit Sonderzeichen im Pfad

### 1.2.0

*(Freigegeben: 28. Januar 2015)*

**Hinzugefügt:**

* Neuer Normalkanal, der das Malen von Normalen-Map-Daten und das Kombinieren der Ergebnisse ermöglicht
* &lbrack;Export&rbrack; Neues Exportfenster mit der Möglichkeit, ein benutzerdefiniertes Packing zu erstellen und benutzerdefinierte Namen festzulegen
* Das Projektdateiformat ist jetzt eine einzelne Datei anstelle von Ordnern
* &lbrack;Export&rbrack; Unterstützung verschiedener Normalformate (DirectX, OpenGL)
* &lbrack;Export&rbrack; Erstellen einer temporären Sperrdatei während des Exports
* &lbrack;Layers&rbrack; Umschalt+Linksklick kann zum Umschalten einer Maske verwendet werden
* &lbrack;Parameter&rbrack; Legt den Farbraum am unteren Rand einer Bildeingabe bei
* &lbrack;Regal&rbrack; Effekt &quot;MG Mask Builder&quot; hat jetzt neue Einstellungen
* &lbrack;3D-Ansicht&rbrack; Ambient occlusion-Map verschließt jetzt den diffusen Beitrag, nicht den Specular

**Fest:**

* Projektion Material/Schablone Vorschau wird im Viewport nicht richtig angezeigt
* &lbrack;3D-Ansicht&rbrack; Tastaturbefehl-QuickInfo wird nicht angezeigt, wenn &quot;S&quot; (Schablone) Tastaturbefehl verwendet wird
* &lbrack;Regal&rbrack; Effekt &quot;MatFx Skin Scale&quot; hat jetzt bessere Leistung bei niedriger Auflösung
* &lbrack;Export&rbrack; Texturen aus dem Export werden beim Festlegen einer größeren Dokumentgröße einfach hochskaliert

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

* &lbrack;Ebene&rbrack; Auswählen der Ebene oben beim Öffnen eines Projekts/Wechseln zwischen Textursätzen
* Verbesserte Geschwindigkeit beim Speichern und Speichern unter mit neuem Komprimierungsalgorithmus
* Anzeige eines Fehlers beim Öffnen eines zu aktuellen Projekts für Painter

**Fest:**

* &lbrack;Werkzeug&rbrack; Geometry Decal produziert Speicherbeschädigungen
* &Klammer;Pinsel&Klammer; Es ist nicht möglich, Schwimmerwerte unter 1 für die Pinselgröße manuell einzugeben
* &lbrack;Ebene&rbrack; Durch das Erstellen eines Farbauswahl-Effekts wird dieser nicht in den Ebenenstapel eingefügt
* &lbrack;Ebene&rbrack; Wenn Sie den Mauszeiger über die Ebenen bewegen, wechselt Painter in die Taskleiste.
* &lbrack;Ebene&rbrack; Das Hinzufügen einer Bitmap als Maske kann zu einem Absturz führen
* GUI für den Solo-Modus mit dem Height-Kanal ist falsch
* &quot;Projekt speichern&quot; kann fehlschlagen und ein Projekt beschädigen
* Absturz beim Öffnen eines Projekts nach dem Laden eines anderen Projekts mit einem veralteten Shader

### 1.1.0

*(Freigegeben: 16. Dezember 2014)*

**Hinzugefügt:**

* &blase;Effekt&blase; Erstellen einer neuen Materialien-ID-Maske
* Neue gepunktete weiße/schwarze Linie für das Pinsel-Gizmo
* Neuer Parameter &quot;Winkelfolge&quot;
* Neuer Parameter &quot;Rückseiten-Ausblendung&quot;
* Neuer Parameter für die Verzögerte Mausbewegung
* &lbrack;Layers&rbrack; Unterstützung für Mehrfachauswahl und -verwaltung
* &lbrack;Layers&rbrack; Kopieren und Einfügen von einem Textursatz in einen anderen
* &lbrack;Export&rbrack; PSD-Format von Adobe Photoshop
* &lbrack;Regal&rbrack; Neues Werkzeug : Fell, Metallstiche und Reißverschluss
* &lbrack;Regal&rbrack; Neuer Pinsel : Schimmel, Bleistift, scharfe Linie und Stich
* &lbrack;Regal&rbrack; Neues Alpha : Gaußsches Rauschen, scharfe Linie, Form, Stift, Spritzen, Stich, Reißverschluss
* Verbesserte Malleistung durch Aktualisierung nur eines Teils der benötigten Texturen

**Fest:**

* &lbrack;Regal&rbrack; Es ist nicht möglich, einen Stoff mit Graf mit gleichen Etiketten zu laden.
* &lbrack;Layers&rbrack; Der Mischmodus &quot;Hindurchwirken&quot; funktioniert nicht mit Masken
* &lbrack;Schablone&rbrack; Skalierung in 2D-Ansicht funktioniert nicht
* Probleme und Absturz auf Mac OS Yosemite

### 1.0.2

*(Freigegeben: 9. November 2014)*

**Hinzugefügt:**

* Verbesserte Performance bei der Vorschau von Materialien mit Substanzen
* Verbesserte Leistung mit der Vorschau des Pinselstrichs beim Aktualisieren des Dokuments
* Verbesserte Leistung im Viewport mit niedrigerer Aktualisierungsrate für nicht funktionierenden Bereich
* &lbrack;Post-Effekte&rbrack; Verbesserte Benutzeroberfläche zum Verwalten von Einstellungen
* &lbrack;Post-Effekte&rbrack; Auf Standardwerte zurücksetzen
* Substance von Effekten und Ebenenoperationen im Kontextmenü
* Unterstützung für die vormultiplizierte Ein-/Ausgabe in Stoffen

**Fest:**

* &lbrack;3D-Ansicht&rbrack; Benutzerdefinierte Shader-Parameter werden durch einen großen Leerraum voneinander getrennt
* &lbrack;Export&rbrack; Fehlende sRGB-Konvertierung für Unity4-Vorgabe
* Möglicher Absturz beim Laden von FBX-Meshs
* Absturz kann beim Laden von einfachen obj-Meshs auftreten
* Die Rechenleiste bleibt beim Laden auf 100 % blockiert.
* Durch das erneute Laden eines Stoffes wird dieser in jede Kategorie verschoben
* DirectX/OpenGL-Switch defekt

### 1.0.1

*(Freigegeben: 27. Oktober 2014)*

**Hinzugefügt:**

* &lbrack;Werkzeug&rbrack; Verbesserte Verwendung von Material-Parametern
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
* &lbrack;Export&rbrack; Fügen Sie vor dem Nachbearbeiten der Diffusion eine Ausdehnung hinzu.
* Befehlszeilenargumente in SP für einfache Vorgänge
* Neue Material und Effekte
* Werkzeugvorschau (separate Echtzeitvorschau von Materialien und Bereich für Konturtests)
* Beim Starten von Painter kein Standarddokument erstellen
* &lbrack;Werkzeug&rbrack; Hinzufügen der Möglichkeit zum manuellen Bearbeiten eines Graustufenwerts
* Verschiedene Verbesserungen für die Schablonen (Einrasten, Reset)
* Partikeln sind jetzt Unterwerkzeuge des Malpinsels, des Radiergummis und der Projektion
* &lbrack;3D-Ansicht&rbrack; Baking geführt AO im Viewport-Rendering verwenden
* Teilen der Steuerelemente für Schablonen zwischen der 2D- und 3D-Ansicht
* Kleine Anpassung der Daumengröße in der Bibliothek
* Suchfelder sind für jedes Fenster spezifisch
* Anpassen der Benutzeroberfläche

**Fest:**

* &lbrack;Substance&rbrack; Schalter funktioniert nicht
* &blbrack;Farbdialog&rbrack; Farbtonverlauf nicht aktualisiert
* Mesh kann nicht aktualisiert werden, wenn der Dateiname identisch ist
* Werkzeug ist in zu kleinen Ansichten nicht sichtbar
* Das Aufkleber-Werkzeug auf dem Retina-Display funktioniert nicht richtig
* &lbrack;Substance&rbrack; Int1 werden als float1 angezeigt
* &lbrack;Substance&rbrack; Grundfarbeingabe/-ausgabe werden nicht erkannt
* &lbrack;Substance&rbrack; Filter können nicht neu geladen werden
* &lbrack;Werkzeug&rbrack; Graustufen-Widget ist immer ausgeblendet

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
* &lbrack; und &rbrack; Tastaturbefehle für die Pinselgröße
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
