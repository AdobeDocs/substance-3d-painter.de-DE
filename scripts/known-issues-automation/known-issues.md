---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/release-notes/know-issues.html"
breadcrumb-title: ''
description: Informieren Sie sich über bekannte Probleme bei Substance 3D Painter , um über die aktuellen Einschränkungen und Problemumgehungen in der neuesten Version auf dem Laufenden zu bleiben.
helpx_creative_field: ""
helpx_description: Substance 3D Painter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Bekannte Probleme
user-guide-description: ''
user-guide-title: ''
source-git-commit: 99ba6e8d891dab9cebbf6035a6850bab331e7472
workflow-type: tm+mt
source-wordcount: '905'
ht-degree: 0%

---


# Bekannte Probleme

Auf dieser Seite werden alle aktiven bekannten Probleme in Version 12.1.0 von Substance 3D Painter aufgeführt:

* `[Engine]` Fehler bei Verwendung von Smart-Materialien, wenn der Textursatz keine Kachel 1001 aufweist
* `[Engine]` Malen mit dem Kopierwerkzeug in normalen Kanalverschiebungsfarben falsch
* `[Engine]` Geometriemaske zeigt Artefakte an UV-Rändern mit instanzierten Ebenen
* `[Engine]` UV-Auffüllung &quot;3D Space Neighbor&quot;-Modus funktioniert nicht gut bei dünnen Dreiecken
* Das Ergebnis des `[Engine]`-Ankerpunkts wird nicht zwischen einer Maske und einem Farbkanal gerendert.

* `[Baking]` Falsche AO bei einfachen Würfeln
* `[Baking]` Die Interpretation des Namensuffixes stimmt nicht überein.
* `[Baking]` UV-Nähte werden nach dem erneuten Importieren von Mes nicht angezeigt
* `[Baking]` Rasterähnliche Artefakte mit einigen Einstellungen

* `[Substance]` Mehrere Rechtschreibfehler in Ressourcen
* `[Substance]` Bedingung für leere Leerraumunterbrechungen für Sichtbarkeit
* Das Laden von `[Substance]`-Vorgaben für einige Materialien dauert zu lange
* `[Substance]` Ressource mit gemischten Verwendungen kann nicht importiert werden.

* `[Color Management]` Inkompatible Bindungen mit Generator werden nicht in der Maske verwendet
* `[Color Management]` Filterausgabe wird nicht ordnungsgemäß berücksichtigt.
* `[Color Management]` HDR-Farbraumkonvertierungen mit ACE unter Linux erzeugen eingeklemmte Farben

* `[Shelf]` Ressourcen erhalten die falsche Verwendung, wenn sie in einen Ordner mit einem bestimmten Namen platziert werden
* `[Shelf]` `[Substance]` Benutzerdaten werden für die Generierung von Miniaturansichten in der Ablage nicht berücksichtigt

* `[Shader]` Parameter &quot;camera_vp_matrix_inverse&quot; wird nicht erkannt.
* `[Shader]` Benutzer0-Kanal kann mit einem bestimmten Shader immer nicht als sRGB gelesen werden.

* `[Scripting]` `[Javascript]` Tippfehler &quot;deaktiviert&quot; beim Festlegen des Dithering-Parameters in Exportfunktionen
* `[Scripting]` `[Python]` Verschiedene Tippfehler im Modul substance_painter.project

* Das in der Grundfarbenansicht gespeicherte Projekt &quot;`[Single Channel View]`&quot; sieht nach dem Painter-Versionsupdate dunkler aus
* Das in der Grundfarbenansicht gespeicherte Projekt &quot;`[Single Channel View]`&quot; sieht nach dem Painter-Versionsupdate dunkler aus

* `[gltf]` Dateien, die über Babylon Exporter exportiert wurden, können nicht geöffnet werden.
* `[Displacement]` Störung beim Malen
* `[Polygon Fill Tool]` Falsche Auswahl mit Symmetrie
* `[2D view]` Striche werden beim Malen manchmal nicht angezeigt
* `[Console]` Symbole, die mit dem Tastaturbefehl verknüpft sind, können nicht geschrieben werden.
* `[LOG]` Fehlermeldung ist falsch, wenn der Export fehlschlägt
* `[3D View]` Schablone funktioniert nicht bei duplizierten Objekten
* `[Resource updater]` Verschiedene Ressourcen im Regal mit demselben Namen werden als eine Ressource gelesen.
* `[Sample]` Fehlerhafte Kamera im Vorschaubeispiel
* `[Instancing]` `[Projection]` Beim Auswählen einer Instanz in einem planaren Projekt wird ein anderes planares Projekt in einem anderen Textursatz ausgewählt.
* `[Slider]` Numerische Eingaben werden deaktiviert, wenn der Cursor das Fenster verlässt
* `[Anchor point]` Fehlerhafte Verweise beim Kopieren und Einfügen von Maskeninhalten
* `[Mesh export]` Neue Textursatznamen werden nicht berücksichtigt
* `[Anchor Points]` Falsche Farbe bei Verwendung im Generator
* `[Bakers]` ID Map Baker berücksichtigt kein physisches Material vom Typ 3ds Max 2021
* `[UV Tiles]` Keine Fehlermeldung beim Überlappen von UV-Leerzeichen mit einem bestimmten Gitter
* `[GLTF]` `[Crash]` Das Erstellen eines Projekts mit einer komprimierten GLTF-Datei führt zu einem Absturz
* `[UV Tile sequence]` Positionszuordnungen werden nicht korrekt importiert
* `[UVTiles]` Height-Kombinationsmaske wird nicht mit UV-Kachelmaske aktualisiert
* `[Import]` Die OBJ-Datei mit &quot;nan&quot;-Werten kann nicht importiert werden.
* `[Export]` GLTF-Exporte in der falschen Größe
* Der Name &quot;`[Texture Set]`&quot; kann leer sein.
* `[Layer stack]` In Maske kopieren, in den Materialmodus wechseln
* `[UI]` Tippfehler in den Einstellungen der Pinselerstellung
* `[Texture Set Settings]` Falscher Name der Shader-Instanz nach einer Umbenennung
* `[Blending]` Farbe und Sättigungsmischmodus ändern auch die Helligkeit.
* `[Librairies]` Breite der gespeicherten Suchen und Filter nach Pfadfenstern, die bei Änderung nicht gespeichert wurden
* `[Geometry mask]` Problem beim erneuten Importieren des Gitters und der instanzierten Ebene
* `[Color management]` Farbraum nicht gefunden, wenn Kachel 1001 fehlt
* `[Export mesh]` Versatz wurde nicht mit eingerichteten bestimmten UV-Kacheln exportiert
* `[RedHat]` Probleme mit der Farbauswahl
* `[Regression]` `[UI]` Das Kontextmenü ist auf dem HD-Bildschirm zu klein.
* `[Resources]` Importierte Netzzuordnungen werden bei der automatischen Aktualisierung ignoriert.
* `[User Channels]` Vorschau des Farbmischraums ist falsch
* Die Geometrieauswahl &quot;`[Mask]`&quot; ist nach dem Wechsel in den Aktivierungsmodus noch aktiv.
* `[Sonoma]` Symbole werden nicht in Menüs angezeigt
* `[Path]` Height-Überblendung vieler Pfade kann Artefakte verursachen
* `[USD]` Falsche Benutzerzuweisung in einigen Fällen
* `[Polygon Fill]` Das Ändern des Farbraums der Grundfarbe aktualisiert die Farbauswahl nicht
* `[Paint Skew]` Das ausgewählte Werkzeug in der Pinselneigung bleibt nach dem Wechsel in den Malmodus ausgewählt
* `[Color Picker]` Picker bleibt nach dem Ändern des Tools geöffnet
* `[UV Padding]` Artefakte beim Hochskalieren der Textur von 4k auf 8k beim Export
* `[Baking Common Settings]` Einstellungen für &quot;Käfigentfernung&quot; aktualisieren die Darstellung von Käfig-Drahtgitter und Shader nicht
* `[Send to Photoshop]`: Fehler beim Exportieren der Ebenenmaske.
* `[Skew Baking]` Pausen der Neigungskorrektur beim Malen und Rückgängigmachen
* `[Projection Tool]` Viewport-Interaktion wird vom Projektionswerkzeug blockiert
* Nicht quadratische Ressourcen werden bei Verwendung in den Steckplätzen des Pinselkanals gestreckt
* Substanz konnte nicht decodiert werden
* Nicht perfekt überlagerte UVs können Artefakte erzeugen
* Ungültige Mesh-Normale mit einigen fbx
* Ansicht wird nicht aktualisiert, wenn der Kanal geändert wird, der von einer Ebene betroffen ist
* Projekte mit einem Textursatz werden im Grundfarbsolomodus erneut geöffnet
* Die Benutzeroberfläche der Kanalschaltfläche in den Material-/Maleigenschaften kann unterbrochen werden.
* Die Reihenfolge der Kanäle in den Eigenschaften kann unterbrochen werden.
* Konturen in L16F und RBG16F können Artefakte anzeigen
* Das Verhalten der Schaltfläche &quot;Wiederherstellen&quot; interagiert nicht mit dem Sperrschlüssel in den Kameraeinstellungen
* Beim Exportieren in Photoshop wird die Auswahl von Geometriemasken ignoriert.
* Die Steigung des Weichzeichners und des Verkrümmungsfilters hängen von der eingestellten Strukturauflösung ab.
* Karten ohne Namen werden außerhalb des Exportordners erstellt
* Schablone wird nicht aktualisiert, wenn die Pinselvorgabe geändert wird
* Problem mit der Transparenz auf PSD von Dateien
* Pinselparameter, die von der kontextabhängigen Symbolleiste geändert werden, werden im Verlauf nicht angezeigt
* Exportvorgaben können nicht umbenannt oder gelöscht werden, wenn Sie sie in dieser Sitzung bereits gelöscht und neu erstellt haben
* Kanalzuordnung funktioniert in einigen Fällen nicht für die Vorschau des Projektionswerkzeugs
* Das Öffnen und Speichern einiger Projekte kann länger als gewöhnlich dauern

## Stabilität

* `[Crash]` Das Klicken auf die Textursatzliste nach fehlgeschlagener Projekterstellung führt zu einem Absturz
* `[Crash]` Kritischer Fehlerabsturz, wenn dasselbe Projekt zweimal geöffnet ist
* `[Crash]` Wählen Sie &quot;Mesh exportieren&quot; aus, wenn das Mesh nicht geladen werden konnte
* `[Crash]` Klicken auf &quot;Malen beginnen&quot;, nachdem versucht wurde, ein altes Projekt zu öffnen
* `[Crash]` Das Erstellen sehr langer Texte in der Multifunktionsleiste kann abstürzen
* `[Crash]` Zurück zum Malmodus, nachdem das Gerät beim Backen verloren hat
* `[Crash]` Beenden Sie Painter nach dem Abbrechen des Kartenexports
* `[Crash]` Exportieren des Gitters mit einigen speziellen Symbolen im Kameranamen
* `[Crash]` Das Löschen eines Kanals im Maskenansichtsmodus führt zu einem Absturz
* `[Crash]` Einige Substance können beim Rendern zu einem Absturz führen
* `[Crash]` Wiederholen des Gitters im Backmodus
* `[Crash]` Das erneute Laden mehrerer Meshes kann zu einem Absturz führen
