---
title: Version 12.1
description: Versionshinweise zu Version 12.1
helpx_description: Substance 3D Painter
source-git-commit: 50df3a58ec4719d302999421774a1c67ce3e0ef1
workflow-type: tm+mt
source-wordcount: '1717'
ht-degree: 0%

---


# Version 12.1

<b>Substance 3D Painter 12.1</b> bietet einen verbesserten Backarbeitsablauf mit automatischem Falzen und Neigungskorrekturmalen, Unterstützung für die OpenPBR-Materialdefinition und einen neuen Hartoberflächenmodus für automatisches UV-Entpacken.

Freigabedatum: <b>22. Juni 2026</b>

>[!NOTE]
>
> Diese Version erhöht die mindestens unterstützte macOS-Version auf 13.0 (Ventura). Weitere Informationen finden Sie auf unserer Seite mit den Systemanforderungen für [&#128279;](../getting-started/system-requirements.md).

## Wichtigste Funktionen

### Verbesserter Backarbeitsablauf mit Skew-Painting

![](../assets/v12/v12_banner_skew.jpg)

Der Backarbeitsablauf wurde überarbeitet und unterstützt jetzt kontinuierliches Backen, On-Mesh-Skew-Korrekturmalen, Kantenschutz und eine neu gestaltete Mesh-Map-Liste.

* <b>Automatisches Ausblenden</b>

  Eine Gittermaske kann fortlaufend umgebrochen werden, wenn die Backparameter angepasst werden, sodass nach jeder Änderung kein manuelles Auslösen eines Backens erforderlich ist. Die automatische Wiederherstellung wird pro Karte aktiviert bzw. deaktiviert und gilt jeweils für eine einzelne Karte. Dies ist besonders praktisch für den Skew-Painting-Arbeitsablauf, aber auch beim Anpassen der allgemeinen Backeinstellungen.

  ![](../assets/v12/v12_auto_rebake.png)

* <b>Malen mit Neigungskorrektur</b>

  Wenn der Käfig auf den Modus <b>Entfernungsbasiert</b> eingestellt ist, können Neigungskorrekturen direkt auf das Gitter mit geringer Poly-Polung gemalt werden, um die Projektionsrichtung während des Backens zu steuern. Die Pinsel-, Radierer- und Polygonfüllwerkzeuge sind mit einer kompakten Graustufenwertauswahl, Symmetrie und den üblichen Pinselsteuerelementen (<b>Strg + Rechtsklick</b> zum Ändern der Pinselgröße, <b>X</b> zum Umkehren des gemalten Werts) verfügbar. Aktionen zum Zeichnen mit Verzerrungen können rückgängig gemacht werden.

  ![](../assets/v12/v12_skew_fix_rebake.gif)

* <b>Kantenschutz</b>

  Beim Malen der Neigungskorrektur behält eine neue Kantenschutzoption die hohe Weichheit bei, die auf harte Kanten projiziert wird. Das Ergebnis wird von den Parametern <b>Edge Distance</b> und <b>Edge Contrast</b> gesteuert.

  ![](../assets/v12/v12_skew_edge_distance.gif)

* <b>Neu gestaltete Netzzuordnungsliste </b>

  Die Gittermapliste bietet Steuerelemente für die einzelnen Maps: Umschalten einer Karte als Ansichtsport <b>Vorschau</b>, <b>Schnellbacken</b> einer einzelnen Karte, Umschalten der zugehörigen <b>automatischen Wiederherstellung</b> und <b>Synchronisieren</b> der Einstellungen in den Textursätzen (verfügbar, wenn das Projekt mehrere Textursätze enthält). Jedes Steuerelement verfügt beim Bewegen des Mauszeigers über eine QuickInfo.

  ![](../assets/v12/v12_quick_bake.png)

* <b>Vereinfachte Backschaltfläche</b>

  Die Viewport-Backschaltfläche wurde durch eine einzelne <b>Backen</b>-Schaltfläche ersetzt, die die Anzahl der zu backenden Maps anzeigt (Textursätze x UV-Kacheln x ausgewählte Mesh-Maps).

  ![](../assets/v12/v12_bake_button.png)

>[!NOTE]
>
> Weitere Informationen zum Backen finden Sie auf der [Seite der dedizierten Dokumentation](../baking/baking.md).

### Unterstützung für OpenPBR

![](../assets/v12/v12_banner_openpbr.jpg)

Das Modell der OpenPBR-Schattierung wird jetzt in Painter unterstützt und als Standard-Arbeitsablauf verwendet, der eine standardisierte Materialdefinition bereitstellt, die anwendungsübergreifend ausgeführt werden kann.

* <b>Neuer OpenPBR-Shader und Standardarbeitsablauf</b>

  Ein Shader, der die OpenPBR 1.1-Spezifikation implementiert, ist verfügbar und wird standardmäßig verwendet. Ein neues Projekt, das ohne Vorlage erstellt wurde, verwendet den OpenPBR-Shader, und der erste Eintrag des neuen Projektfensters ist jetzt mit <b>OpenPBR</b> anstelle von <b>ASM</b> gekennzeichnet. Neue Projektvorlagen für OpenPBR sind enthalten, und die Beispielprojekte wurden aktualisiert, um sie zu verwenden.

  ![](../assets/v12/v12_openpbr_shader_icon.jpg)

* <b>Beim Import aus der Projektvorlage ausgewählter Shader</b>

  Beim Importieren einer USD- oder GLTF-Datei wird der Shader jetzt aus der Projektvorlage festgelegt und nicht aus dem Dateiinhalt erraten. Eine Meldung wird im Protokoll angezeigt, wenn ein Material und eine Vorlage Arbeitsabläufe verwenden, die nicht übereinstimmen.

  ![](../assets/v12/v12_openpbr_template.png)

* <b>OpenPBR-Benennungskonvention beim Export</b>

  Das Fenster <b>Texturen exportieren</b> verfügt über ein neues Dropdown-Menü, in dem Sie die Benennungskonvention auswählen können. Standardmäßig wird OpenPBR verwendet, wenn mindestens ein Shader im Projekt es verwendet, und das ausgewählte Schema wird in der Liste der Maps jedes Textursatzes widergespiegelt.

  ![](../assets/v12/v12_openpbr_export.png)

* <b>USD- und MDL-Support</b>

  OpenPBR-Materialien werden über das USD-Format unterstützt. Außerdem wurde eine neue MDL hinzugefügt, um das Rendern von OpenPBR-Materialien in Irak zu ermöglichen und eine genauere Materialdarstellung zu ermöglichen.

>[!NOTE]
>
> Benutzerdefinierte Shader müssen möglicherweise aktualisiert werden. Der Shader-API wurde geändert, um OpenPBR zu unterstützen. Weitere Informationen finden Sie im Änderungsprotokoll im Hilfemenü der Anwendung.

### Neues automatisches Ausgliedern der harten Oberfläche

![](../assets/v12/v12_banner_uvs.jpg)

Ein neuer Modus für automatisches Ausgliedern, der auf Elemente mit harten Oberflächen zugeschnitten ist, wurde hinzugefügt.

* <b>Modus für das Freilegen von harten Oberflächen</b>

  Eine Option <b>Harte Oberfläche</b> ist in den Einstellungen für das automatische Ausgliedern verfügbar. Es minimiert die UV-Verzerrung und erzeugt orthografisch ausgerichtete UV-Layouts, wodurch es besser für mechanische und harte Oberflächenmaschen geeignet ist.

  ![](../assets/v12/v12_unwrap_mode.jpg)

>[!NOTE]
>
> Weitere Informationen zum automatischen Entpacken finden Sie auf der [Seite für die dedizierte Dokumentation](../features/automatic-uv-unwrapping.md).

### Sonstiges

![](../assets/v12/v12_banner_misc.jpg)

In dieser Version wurden zusätzliche Funktionen und Verbesserungen hinzugefügt:

* <b>Mehrere Kanäle gleichzeitig hinzufügen oder entfernen</b>

  Nach der Einführung von OpenPBR können Sie in einem neuen Fenster, auf das über die <b>Kanaleinstellungen</b> zugegriffen werden kann, mehrere Textursätze gleichzeitig auswählen. Dies ist praktisch, wenn Sie die vom OpenPBR-Workflow verwendete große Kanalliste einrichten möchten.

  * Das neue Fenster ist über die Schaltfläche <b>Kanäle hinzufügen oder entfernen</b> in den Einstellungen für den Textursatz verfügbar.

    ![](../assets/v12/v12_channel_add_remove_button.png)

  * Das Fenster gibt einen Überblick über alle Kanäle, die in Painter verwendet werden können.

    ![](../assets/v12/v12_channel_window_small.jpg)

  * Mit der Schaltfläche <b>Auf alle Textursatz anwenden</b> kann die Kanalkonfiguration aller Textursatz gleichzeitig bearbeitet werden.

    ![](../assets/v12/v12_channel_apply_all.png)

* <b>Alle Instanzen der Textursätze reduzieren</b>

  Eine neue Option <b>Alle Instanzen reduzieren</b> ist für instanzierte Ebenen und Gruppen verfügbar. Es erzeugt ein abgeflachtes Ergebnis über jeden Textursatz, in dem die Instanz angezeigt wird, und geht den gesamten Instanzbaum nach unten. Dies wird als ein einziger Schritt rückgängig gemacht.

  ![](../assets/v12/v12_flatten_instances.png)

* <b>Einheitlicher Rückgängig-Verlauf</b>

  Backen und Malen haben jetzt denselben Verlauf zum Rückgängigmachen. Das Umschalten zwischen dem Baking- und dem Malen-Modus wird als Schritt zum Rückgängigmachen aufgezeichnet. Aktionen können daher nur in dem Modus rückgängig gemacht werden, in dem sie ausgeführt wurden.

## Tutorials

Sehen Sie sich unser neuestes Tutorial auf YouTube an:

[![](../assets/v12/v12_youtube_tutorial.jpg)](https://www.youtube.com/watch?v=WwyElRpiQgY)

## Versionshinweise

### 12.1.3

Freigabedatum: **2026/08/25**

Zusammenfassung: **Nebenversion**

**Hinzugefügt:**

* Aktualisieren der Substance-Engine auf Version 9.4.6v

**Fest:**

* [Graustufenwähler] Die Auswahl bleibt nach dem Ändern des Tools geöffnet
* [Verkrümmungssicherung] Verkrümmungskorrekturunterbrechungen beim Malen und Rückgängigmachen
* [Projektionstool] Die Viewport-Interaktion wird vom Projektionstool blockiert
* [Dynamische Kontur] Fehlende dynamische Konturparameter in den Pinseleigenschaften
* Export in ein Netzwerk funktioniert nicht mehr

### 12.1.2

Freigabedatum: **2026/08/03**

Zusammenfassung: **Nebenversion**

**Fest:**

* \[Absturz\] Einige Substance können beim Rendern zu einem Absturz führen
* \[Absturz\] Importieren des Gitters im Backmodus
* \[Absturz\] Fehler beim Initialisieren der Grafikanzeige kann zu einem Absturz führen.
* \[Absturz\] Exportieren von Texturen kann in einigen Fällen abstürzen, während das Protokoll aktualisiert wird
* \[Absturz\] Absturz im Backing-Modus in einigen Fällen beim Laden/Aktualisieren der Umgebungszuordnung
* \[Backen\] Das erneute Starten des Backens nach dem Ändern einer hohen Poly-Datei kann zu einem Einfrieren führen
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
* [Absturz] Das erneute Laden mehrerer Meshes kann zu einem Absturz führen
* [Absturz] Das Löschen eines Kanals im Maskenansichtsmodus führt zu einem Absturz
* [Absturz] Einige Substance können beim Rendern zu einem Absturz führen
* [Neigung malen] Das ausgewählte Werkzeug in der Neigung bleibt nach dem Wechsel in den Malmodus ausgewählt
* [Allgemeine Einstellungen sichern] Einstellungen für die Käfigentfernung aktualisieren die Drahtgitter- und Shader-Visualisierung für Käfige nicht
* [Engine] UV-Auffüllmodus &quot;3D Space Neighbor&quot; funktioniert nicht gut bei dünnen Dreiecken
* Das Ergebnis des [Engine]-Ankerpunkts wird nicht zwischen einer Maske und einem Farbkanal gerendert

### 12.1.0

Freigabedatum: <b>2026/06/23</b>

Zusammenfassung: <b>Dieses Update ist eine Hauptversion. Es enthält Verbesserungen an Bakern mit dem Standardzustand &quot;Neues Baking&quot;, der Zeichnungs-Skew-Map, dem automatischen Reake, einer neuen Option für den automatischen entpack von UV für Mesh und OpenPBR mit fester Oberfläche. Weitere Informationen finden Sie in den vollständigen Versionshinweisen.</b>

<b>Hinzugefügt</b>:

* [Baking Neigen] Malwerkzeuge Neigen
* [Skew Baking] Hinzufügen von Skew Preview Shader und Skew Direction Vektorgrafiken beim Malen von Skew Map
* [Skew-Backing] Option &quot;Kantenschutz hinzufügen&quot;
* [Backen mit Neigung] Automatische Wiederherstellung
* [Skew Backing] Benutzeroberfläche der Gitterzuordnungs-Liste überarbeiten
* [Skew Baking] Gitterzuordnung teilen/Allgemeine Backeinstellungen + Allgemeine Einstellungen aus Gitterzuordnungsliste verschieben (nur Grundfarbe oder Maske)
* [Skew Backing] Symbolleistenschaltflächen für Ansichtsfenster ändern
* [Schrägbacken] Symmetrie-Schalter für Pinsel in der oberen Symbolleiste anzeigen
* [Skew Backing] Umbenennungsoptionen im Menü &quot;Listensynchronisation&quot; der Gitterzuordnung
* [Skew Backing] Dialogfelder &quot;Synchronisation aktualisieren&quot; und &quot;Überwachter Status&quot;
* [Backen mit Neigung] Erstellen einer Graustufen-Farbwählervariante
* [Skew Backing] Symbol für Aktualisierungsbackmodus
* [Automatisch entpacken] Option &quot;Harte Oberfläche integrieren&quot;
* [OpenPBR] Unterstützung für OpenPBR 1.1 hinzufügen
* [OpenPBR] OpenPBR zum Standard-Workflow und -Shader machen
* [OpenPBR] Importieren von OpenPBR-Materialien und -Texturen über USD
* [OpenPBR] Exportieren von OpenPBR-Materialien und -Texturen über USD
* [OpenPBR] Fenster &quot;Export Textures&quot; aktualisieren, um die OpenPBR-Benennungskonvention anzuzeigen
* [OpenPBR] Hinzufügen von Dokumentationen zu Änderungen an der Support-OpenPBR
* [OpenPBR]&#x200B;[Iray] Fügen Sie eine neue MDL hinzu, um OpenPBR 1.1 in Iray zu unterstützen
* Mehrere geringfügige Verbesserungen bei den USD-Exporten
* [UI] Fügen Sie eine Warnung im Viewport hinzu, wenn Sie versuchen, auf einem anderen Textursatz zu malen
* [Reduzieren] Reduzieren aller instanzierten Ebenen über Textursätze hinweg zulassen
* [Einstellungen für Textursatz] Mehrere Kanäle gleichzeitig über ein neues Fenster auswählen
* [Verlauf] &quot;Wert&quot; aktualisieren Eintragsformulierung rückgängig machen, um den Parameternamen wiederzugeben
* [Ebenenstapel] Fülleffekte in Masken standardmäßig auf Weiß einstellen (1.0)
* [Substance] Neue &quot;mesh_hard_edges_triangle&quot;-Engine-Zuordnungseingabe hinzufügen
* [Substance] Neue Eingabe für die Engine &quot;mesh_hard_edges&quot; hinzufügen
* [Shader] Verhindern, dass Shader-Instanzen dieselben Namen haben
* [Shader] Verwenden Sie den Shader aus der Projektvorlage beim Importieren einer USD- oder GLTF-Datei.
* Adobe Color Engine auf Version 7.0 aktualisieren
* Aktualisieren der MacOSX-Mindestversion auf 13.0 (Ventura)
* [Inhalt] Neue Projektvorlagen für OpenPBR
* [Inhalt] Aktualisieren von Beispielprojekten, um den neuen OpenPBR Shader zu verwenden
* [Python] Erweitern Sie die Geometrie-Masken-API, um Einschluss- und Ausschlussmodi wie in der Benutzeroberfläche zu ermöglichen.

<b>Fest</b>:

* [Absturz]&#x200B;[Einstellungen für Gitterzuordnungen] Anwenden von Einstellungen auf andere Textursätze
* [Absturz] Wenn die Krümmung von der Karte ohne den Weltraum normal gebacken wird
* [Absturz]&#x200B;[Backen] Backen mit aktiviertem benutzerdefiniertem Käfig, aber ohne Dateiauswahl stürzt ab
* [Absturz] Abbrechen des AO-Backens
* [Auto-Cage] Unendliche Belastung, wenn der hohe Poly-Dateipfad ungültig ist
* [Linux]&#x200B;[Windows] Der Farbwähler kann manchmal ganz schwarz sein oder nicht angezeigt werden.
* [Polygon-Füllwerkzeug] Das Werkzeug funktioniert nicht mit Nicht-PBR
* &lbrack;[Malen] Löschen des Kanals für die Grundfarbe löscht keine zuvor gemalte Farbe
* [USD] Shader-Instanzen werden nicht alle korrekt erkannt.
* [Substance] Es wird nur die erste Verwendung eines Eingabe-/Ausgabeknotens berücksichtigt
* [Shader] Umgebungsbelichtung wird zweimal mit Textur-Sets unter Verwendung verschiedener Mischmethoden angewendet.
* [Engine] Normale Texturen mit leerem blauen Kanal (schwarz) können zu falschen Angleichungsergebnissen führen
* [GLTF Import] Alpha-Überblendung ist für jeden Textursatz aktiviert
* [GLTF-Export] Die Alpha-Füllmethode ist beim Export immer aktiviert
* [Export] Doppelseitige Geometrie ist beim Importieren einer GLTF-Datei immer deaktiviert
* [Javascript] Das Ändern von Shader-Einstellungen trägt nicht zum Rückgängigmachen des Verlaufs bei
* [Samples] Die Volumenstreuung ist in den Anzeigeeinstellungen für die Meet Mat nicht aktiviert.
