---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/release-notes/version-8-3.html"
breadcrumb-title: ''
description: Lesen Sie die Versionshinweise für Substance 3D Painter 8.3, um mehr über neue Funktionen, Verbesserungen und Fehlerbehebungen zu erfahren.
helpx_creative_field: ""
helpx_description: Painter > Release notes > Version 8.3
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Version 8.3
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '2607'
ht-degree: 0%

---


# Version 8.3

Mit **Substance 3D Painter 8.3** wird ein brandneuer Backmodus eingeführt. USD-Dateien werden importiert und die Physische Größe im UV-Projektion-Modus wird unterstützt.

Freigabedatum: *10. Januar 2023*

## Hauptmerkmal

### Neuer Backmodus

![](../assets/banner-baking_1.jpg)

Das alte Backfenster wurde durch einen speziellen Modus mit mehreren neuen Funktionen ersetzt, insbesondere mit Darstellungsmöglichkeiten wie der Anzeige des Käfigs und Anpassungsfehlern.

* **Zugriff auf Modi und Wechsel zwischen Modi**\
  Backen ist jetzt ein neuer und separater Modus zusätzlich zu den bereits vorhandenen Mal- und Rendermodi der Anwendung. Um in den Backmodus zu wechseln, verwenden Sie einfach das kleine Croissant-Symbol in der kontextabhängigen Symbolleiste. Das Umschalten zwischen den Modi kann auch anders erfolgen: über das Menü &quot;Modus&quot; oder die Tastaturbefehle. Um zu einem anderen Modus zurückzukehren, verwenden Sie einfach das dedizierte Symbol des Modus (außerdem kann die Schaltfläche **Gitterzuordnungen backen** in den [Einstellungen für Textursätze](../interface/texture-set/texture-set-settings.md) weiterhin verwendet werden, um in den neuen Modus zu gelangen).

  ![](../assets/baking-mode-switch-menu.png)

  ![](../assets/baking-mode-switch-icon.png)

* **Neue Modusschnittstelle**\
  Das traditionelle Backfenster wurde in einen Modus mit speziellen Docks umgewandelt, insbesondere:

  * **Die Textursatzliste** kann verwendet werden, um zu definieren, welche Teile des Projekts gebacken werden.
  * **Mesh Map Bakers** ermöglicht die Auswahl zwischen den allgemeinen Backeinstellungen und den Backeinstellungen. Hier können Sie auch angeben, welcher Bäckerprozess gestartet wird.
  * **Mesh Map Settings**&quot; befindet sich dort, wo sich alle Baker- und allgemeinen Einstellungen befinden, und kann, abhängig von der Auswahl aus den beiden vorherigen Fenstern, geändert werden.
  * **Das Sicherungsprotokoll** gruppiert verschiedene Informationen zum Sicherungsprozess, insbesondere Fehlermeldungen, neu.
  * **Visualisierung wird gebacken**: Dieses Bedienfeld befindet sich im Viewport und steuert verschiedene Optionen für die Anzeige der Polygonnetze mit niedriger und hoher Poly-Zahl.

  ![](../assets/baking-mode-overview.jpg){width="500px"}

* **Starten und Abbrechen des Backvorgangs direkt im Ansichtsport**\
  Die Schaltfläche zum Starten oder Abbrechen des Backvorgangs befindet sich jetzt unten im Ansichtsfenster. Ein kleiner Pfeil kann auch verwendet werden, um den Backmodus anzugeben: basierend auf der Listenauswahl &quot;Textursatz&quot; oder mithilfe des aktuell aktiven Textursatzes.

  ![](../assets/baking-button.png)

  ![](../assets/baking-button-cancel.png)

* **Anzeigen eines hochpolaren Gitters im Viewport**\
  Wenn Sie ein High-Poly-Gitter in den Backeinstellungen angeben, wird es jetzt auch im Viewport geladen (sofern die dedizierte Visualisierungseinstellung nicht deaktiviert ist). Auf diese Weise kann überprüft werden, ob die Geometrie des Polygonnetzes mit der Geometrie des Polygonnetzes mit der Geometrie des Polygonnetzes mit der Geometrie des Polygonnetzes übereinstimmt.

  ![](../assets/low-vs-high.jpg){width="400px"}

* **Käfiggitter im Viewport mit verpassten Bereichen als Fehler anzeigen**\
  Das Gitter des Käfigs kann auch im Darstellungsfenster angezeigt werden. Wenn keine dedizierte Gitterdatei verwendet wird, wird stattdessen ein impliziter Käfig angezeigt, der auf den Parameter &quot;Max. Frontalentfernung&quot; reagiert. Wenn Sie die Käfiggröße anpassen, wird jeder Teil des hochgepolten Gitters, der sich außerhalb des Käfigs befindet, standardmäßig rot angezeigt, sodass Sie leicht einen Teil des Gitters finden können, der beim Backen verloren geht.

  ![](../assets/cage-distance.gif)

* **Gitter beim Laden und Backen durchsuchen**\
  Das Laden von Gittern und das Backen friert die Anwendung nicht mehr ein, sodass es möglich ist, während dieser Vorgänge mit dem Viewport zu interagieren. Dies kann nützlich sein, um den Backvorgang zu untersuchen, Probleme frühzeitig zu erkennen und den Backvorgang abzubrechen, um am Ende Zeit zu sparen. In ähnlicher Weise wird jetzt zuerst der sichtbarste Textursatz im Viewport eingebrannt, der dabei hilft, die Ergebnisse in bestimmten Bereichen im Voraus zu überprüfen.

  ![](../assets/interaction-while-baking.gif)

* **Neutrales Material und Viewport-Einstellungen**\
  Um sich auf die Backergebnisse zu konzentrieren und gegebenenfalls nach Problemen zu suchen, zeigt der Backmodus keine gemalten Texturen an, sondern verwendet stattdessen ein neutrales Material. Die Einstellungen für dieses neutrale Material können im Visualisierungsbedienfeld für das Backen im Viewport angepasst werden.

  ![](../assets/neutral-material-demo.gif)

* **Harte Kanten mit fehlenden UV-Nähten anzeigen**\
  Beim Backen entstehen unter anderem Artefakte durch harte Kanten, die keine UV-Nähte aufweisen. Das kann zu sichtbaren Linien führen und die Smoothness der Schattierung unterbrechen. Zu diesem Zweck wurden Visualisierungseinstellungen hinzugefügt, um sie sowohl in der 3D- als auch in der 2D-Ansicht hervorzuheben, da sie sonst leicht zu übersehen sind.

  ![](../assets/hard-edge-missing-seams.png){width="450px"}

  ![](../assets/hard-edge-missing-seams-2d.jpg){width="300px"}

* **Parameter synchronisieren und nicht synchronisieren**\
  Mit der neuen Synchronisierungsaktion können Sie angeben, welcher Teil der Backing-Einstellungen über Textursätze hinweg synchronisiert wird. Andernfalls wäre es mühsam, Einstellungen mehrfach auf identische Weise zu konfigurieren. Manchmal ist es nützlich, über Textursätze mit dedizierten Einstellungen zu verfügen und diese nicht zu synchronisieren. Wenn Sie z. B. die allgemeinen Einstellungen getrennt halten, können Sie jetzt eine maximale Frontalentfernung, Auflösung und/oder eine Liste von Netzen mit hohem Poly verwenden, die sich je nach Textursatz unterscheiden würden.

  ![](../assets/sync-icon-1.png){width="400px"}

  ![](../assets/sync-ao-settings.png){width="400px"}

* **Übereinstimmung mit der Namensüberprüfung**\
  Die Registerkarte &quot;**Zuordnung nach Name**&quot; im **Sicherungsprotokoll** kann bei der Suche nach Fehlern im Zuordnungsvorgang helfen, bevor das Sichern beginnt. Dadurch werden Gitter, die nicht übereinstimmen, leichter erkannt. Übereinstimmende Gitter werden gruppiert, andere werden isoliert und rot dargestellt.

  ![](../assets/matching-by-name-log.png){width="450px"}

>[!NOTE]
>
> Es gibt viele weitere neue Einstellungen in diesem neuen Modus. Weitere Informationen finden Sie auf der [Seite zur dedizierten Dokumentation](../baking/baking.md).

### Neuer Import und Export von USD-Dateien

![](../assets/banner-usd.jpg)

Mit dieser neuen Version wird die Unterstützung des Dateiformats [Universal Scene Description (USD)](https://graphics.pixar.com/usd/release/intro.html) hinzugefügt. Es ist jetzt möglich, ein Painter-Projekt zu starten, bei dem Gitter und Texturen im USD-Format exportiert werden. Dies ermöglicht einen konsistenteren Workflow über Anwendungen hinweg.

* **Importieren einer USD-Datei mit Varianten, Skinning und in einem bestimmten Frame**\
  Ein USD-Dateiformat kann verwendet werden, wenn ein Projekt erstellt oder ein Gitter innerhalb eines Projekts erneut importiert wird. USD-Dateien können häufig komplexe Szenen sein, daher ist auch ein Selektor &quot;scope&quot; und &quot;variant&quot; verfügbar, um nur einen Teil der Datei zu importieren.

  ![](../assets/usd-import-settings.png){width="400px"}

  ![](../assets/usd-scope-variants.png){width="400px"}

* **USD als neue Datei exportieren oder mit dem im Projekt verwendeten ursprünglichen USD verknüpft**\
  Wenn Ihre Texturierung fertig ist, können Sie das Fenster **Datei > Texturen exportieren** verwenden, um Ihre USD-Datei zusammen mit Ihren Texturdateien zu exportieren. Aktivieren Sie dazu einfach die Einstellung **USD-Asset exportieren**. Dadurch werden mehrere USD-Dateien generiert, die anschließend einfach in eine Pipeline integriert werden können. Wenn Sie eine Nicht-USD-Datei oder eine USD-Datei ohne UVs verwendet haben, wird dadurch eine neue USD-Geometriedatei zusätzlich zu Texturmaps und USD-Materialdatei exportiert.\
  Darüber hinaus ist es auch möglich, die Projektgeometrie mit **Datei > Mesh exportieren** als USD-Datei zu exportieren.

  ![](../assets/usd-export-textures.png)

  ![](../assets/usd-export-mesh.png){width="400px"}

### Verbesserte Unterstützung der Physische Größe im UV-Modus

![](../assets/banner-physicalsize-1.jpg)

Die Unterstützung von Substance-Materialien mit eingebetteten Physische Größen wurde auf UV-basierte Projektionen erweitert.

* **Physische Größe im UV-Modus**\
  Es ist jetzt möglich, den Skalierungsmodus auf &quot;Physische Größe&quot; festzulegen, anstatt Füllebenen und Fülleffekte mit &quot;UV-Projektion&quot; einzukacheln. Die Größe der UV-Strahlung wird automatisch auf der Grundlage der mittleren Größe der Dreiecke aus der UV-Strahlung berechnet.

  ![](../assets/physicalsize-uvmode.png){width="400px"}

* **Automatisch zur Physische Größe wechseln** Es wurde eine neue Projekteinstellung hinzugefügt, um die Skalierungseinstellung beim Erstellen eines Materials (z. B. beim Ziehen und Ablegen einer Ressource für das Elementfenster) automatisch auf Physische Größe festzulegen. Auf diese Weise können Sie die konsistente Größe in einem Projekt verwenden, ohne die Einstellungen jedes Mal manuell wechseln zu müssen, wenn eine neue Füllebene erstellt wird. Um sie in einem bestehenden Projekt zu aktivieren, gehen Sie zu **Bearbeiten > Projektkonfiguration** und aktivieren Sie **Skalierung der Füllebene auf Physische Größe umschalten, wenn Materialien zugewiesen werden**. Diese Einstellung kann auch beim Erstellen eines neuen Projekts aktiviert werden.

  ![](../assets/physicalsize-settings.png)

## Informationen zur Plattformunterstützung

Mit dieser Version haben wir die mindestens unterstützte Version von Painter auf Steam auf Ubuntu 20.04 erhöht.

## Tutorials

In unserem neuesten Tutorial erfahren Sie mehr über den neuen Backmodus:

## Versionshinweise

*(Freigegeben: 10. Januar 2023)*\
Zusammenfassung: **Hauptversion mit neuem Backmodus, neuem Import und Export von USD-Dateien und Physische Größe-Unterstützung für UV-Projektion**

**Hinzugefügt:**

* [Backmodus] Neuer Backmodus, der dem Backvorgang gewidmet ist
* [Backmodus] Kurzbefehl zum Wechseln in den Backmodus auf F8 festlegen
* [Backmodus] Hinzufügen der Schaltfläche &quot;Backen beginnen&quot; und &quot;Backen abbrechen&quot; im Viewport
* [Backmodus] Backauswahl in der Liste &quot;Textursatz&quot; hinzufügen
* [Backmodus] Neues Fenster &quot;Gitterzuordnungs-Bäcker&quot; hinzufügen, um Bäcker auszuwählen
* [Backing-Modus] Neues Fenster &quot;Gitterzuordnungs-Einstellungen&quot; hinzufügen, um Backing-Einstellungen zu bearbeiten
* [Backing Mode] Neues Backing Log-Fenster hinzufügen, um Backing-Prozess zu verfolgen
* [Backing Mode] Backing-Parameter hinzufügen und Aktionen im Verlaufsfenster rückgängig machen
* [Backing-Modus] Hinzufügen von Breadcrumbs in den Mesh-Map-Einstellungen
* [Backmodus] Hinzufügen von Mesh Maps-Miniaturansichten im Fenster &quot;Gitter-Map-Bäcker&quot;
* [Backmodus] Menü &quot;Visualisierungseinstellungen reduzierbar&quot; im 3D-Viewport hinzufügen
* [Backmodus] Fügen Sie eine Visualisierungseinstellung hinzu, um das High-Poly-Gitter ein- oder auszublenden
* [Backmodus] Visualisierungseinstellung hinzufügen, um das Gitter und das Drahtgitter des Käfigs ein- bzw. auszublenden
* [Backmodus] Fügen Sie eine Visualisierungseinstellung hinzu, um das Gitter mit der niedrigen Poly-Intensität ein- oder auszublenden.
* [Backmodus] Hinzufügen einer Visualisierungseinstellung, um harte Kanten ohne UV-Nähte als Fehler anzuzeigen
* [Backing Mode] Informieren Sie im Viewport über Gitter- und Backing-Fehler, wenn das Backing-Protokoll nicht sichtbar ist
* [Backmodus] Aktion hinzufügen, um die Backeinstellungen für alle Textursätze zu synchronisieren

  Im Fenster &quot;Gitter-Map-Bäcker&quot; kann jeder Bäcker (sowie die allgemeinen Einstellungen) über Textursätze hinweg synchronisiert werden, indem Sie auf das Verknüpfungssymbol neben seinem Namen klicken. Durch diese Aktion wird ein Fenster geöffnet, in dem Sie auswählen können, welche Textursätze dieselben Parameter verwenden sollen.
* [Backmodus] Hinzufügen von Aktionen zum Kopieren und Einfügen von Backereinstellungen

  Im Fenster &quot;Gitterzuordnungs-Bäcker&quot; stehen Aktionen zum Kopieren und Übergehen der einzelnen Bäckereinstellungen über Textursätze entweder über das spezielle Menü oben im Fenster oder das Kontextmenü mit der rechten Maustaste zur Verfügung.
* [Backing Mode] Schaltfläche Hinzufügen im Backing Log, um von Fehler zu den richtigen Einstellungen zu springen

  Wenn ein Bäcker ausfällt oder ein Gitter nicht ordnungsgemäß geladen wird, wird im Backprotokoll eine Fehlermeldung angezeigt. Mit einer Schaltfläche neben der Meldung können Sie das Fenster Gitterzuordnungs-Bäcker und Gitterzuordnungs-Einstellungen ändern, um die zugehörigen Einstellungen anzuzeigen. Dies hilft dabei, die Ursache eines Problems einfacher zu isolieren, um es beheben zu können.
* [Backmodus] Hinzufügen von Menüs zum Verwalten von Textursätzen und Bäcker-Auswahlen

  Sowohl in der &quot;Texture Set-Liste&quot; und &quot;Mesh Map Bakers&quot; Fenster wurden ein kleines Action-Menü hinzugefügt, um zu kopieren, invertieren Auswahlen.
* [Backmodus] Baker-Auswahlliste nach Textursatz teilen
* [Backmodus] Teilen allgemeiner Einstellungen pro Textursatz
* [Backmodus] Laden von High-Poly- und Käfigmaschen ohne Einfrieren der Schnittstelle
* [Backmodus] Verwenden Sie die Viewport-Fortschrittsleiste, um die Gitterbelastung anzuzeigen
* [Backing-Modus] Hinzufügen des Netzladestatus im Backing-Protokoll
* [Backmodus] Umkehren des Gitters im Viewport während des Backens zulassen
* [Backmodus] Backreihenfolge basierend auf der aktuellen Gittersichtweite des Ports festlegen
* [Backmodus] Anzeige des impliziten Backkäfigs im Viewport

  Wenn Sie keine benutzerdefinierte Gitterdatei für den Käfig verwenden, wird ein automatisches Gitter für den Käfig generiert und im Viewport angezeigt. Die Größe basiert auf dem Parameter &quot;Max. Frontalentfernung&quot; der üblichen Backeinstellungen. Das Gitter des Käfigs wird verwendet, um anzuzeigen, wie weit die Anpassung zwischen dem niedrigen und dem hohen Poly gehen wird.
* [Backing-Modus] Übereinstimmende Liste von Gitternamen für &quot;Übereinstimmender Name&quot; im Backing-Protokoll anzeigen
* [Backmodus] Verwenden Sie neutrales Material, um das 3D-Modell im Viewport anzuzeigen.
* [Backing-Modus] Deaktivieren der Engine-Berechnung im Backing-Modus
* [Backmodus] Beim Beenden der App während des Backens wird eine Warnung angezeigt
* [Bäcker] Aktualisieren der Beschriftungen für Anti-Aliasing-Einstellungen

  Die Einstellungswerte für das Anti-Aliasing wurden in &quot;Supersampling&quot; umbenannt und mit einer expliziten Multiplikatornummer versehen, um das Verhalten zu verdeutlichen.
* [Bakers] Aktualisieren Sie Bakers auf Version 2.5.7.
* [USD] Importieren und Exportieren von Universal Scene Description (USD)-Dateien
* [USD] Hinzufügen von USD-Optionen zum Fenster &quot;Neues Projekt&quot;, wenn Sie eine USD-Datei auswählen
* [USD] Neues Auswahlfenster für Umfang und Varianten hinzufügen

  Wenn Sie eine USD-Datei importieren, können Sie durch Klicken auf die Schaltfläche &quot;Ändern&quot; im Fenster &quot;Neues Projekt&quot; oder &quot;Projektkonfiguration&quot; auswählen, welcher Teil und welche Varianten einer USD-Datei importiert werden sollen.
* [USD] Option &quot;Unterteilungsebenen hinzufügen&quot;

  Wenn Sie ein neues Projekt mit einer USD-Gitterdatei erstellen, die Unterteilungen enthält, können Sie die Ebene der Unterteilungen mithilfe eines Schiebereglers auswählen. Das Projekt wird mit dem unterteilten Gitter erstellt. Die Ebene kann über die Projektkonfiguration geändert werden.
* [USD] Importieren von in USD gehäuften Netzen in einem bestimmten Frame

  Wenn Sie ein neues Projekt mit einer USD-Gitterdatei erstellen, die Animationen enthält, können Sie den Frame mit einem Schieberegler auswählen, der die eingebettete Timeline-Sequenz widerspiegelt. Der Frame kann über die Projektkonfiguration geändert werden.
* [USD][Exportieren] Fügen Sie eine Option zum Exportieren von USD-Dateien hinzu.

  Das neue Kontrollkästchen &quot;USD exportieren&quot; wurde dem Fenster &quot;Texturen exportieren&quot; hinzugefügt. Wenn diese Option aktiviert ist, können Sie USD-Dateien sowie Texturmaps aus beliebigen Vorlagen exportieren.
* [USD][Exportieren] Fügen Sie dem Gitterexport das USD-Dateiformat hinzu.
* [USD] Benennen Sie die vorhandene Exportvoreinstellung &quot;USD PBR Metal Roughness&quot; um, um ein expliziteres Format zu erhalten

  Die USD-Exportvorlage, die zuvor als &quot;USD PBR Metal Roughness&quot; bekannt war, ist weiterhin über &quot;Texturen exportieren&quot; > &quot;Ausgabevorlage&quot; > &quot;USDz&quot; (Apple AR) verfügbar.
* [Automatisch entpacken] Ausrichtung für Packing sperren hinzufügen

  Neue Option für Einstellungen zum automatischen Ausgliedern, mit der die Ausrichtung vorhandener UV-Inseln beibehalten werden kann, wenn die Funktion &quot;Packing&quot; verwendet wird. Der Zugriff darauf erfolgt über &quot;Neues Projekt&quot; > &quot;Optionen zum automatischen Ausgliedern&quot; > &quot;Ausrichtung der UV-Insel&quot;.
* [Physische Größe] Fügen Sie eine Einstellung hinzu, um die Physische Größe automatisch in Fülleffekt/Ebene zu verwenden.

  Es wurde eine neue Option hinzugefügt, mit der bei Verwendung eines Materials mit eingebetteter Physische Größe automatisch zur Physische Größe-Skala gewechselt werden kann. Sie kann pro Projekt über &quot;Neues Projekt&quot; oder über &quot;Bearbeiten&quot; > &quot;Projektkonfiguration&quot; > &quot;Physische Größe&quot; > &quot;Beim Zuweisen von Materialien Füllebenenskalierung auf Physische Größe umschalten&quot; aktiviert werden.
* [Physische Größe] Physische Größe für UV-Projektion verfügbar machen

  Physische Größe-Skalierung ist jetzt für UV-Projektionen verfügbar - sie ermöglicht die automatische Größenänderung für ein Material basierend auf der Physische Größe eines Gitters. Sie kann über &quot;Skalieren > Physische Größe&quot; in der Füllebene oder im Effekteigenschaftsfenster ausgewählt werden.
* [Scripting][Python] Abfrage der Anwendungsversion zulassen
* [Scripting][JavaScript] Update-API für neue Backing-Parameter
* [Scripting][Python] Backmodul: Backparameter bearbeiten
* [Scripting][Python] Backmodul: Backen starten/abbrechen
* [Scripting][Python] Backmodul: Methode der selektierten Krümmung
* [Scripting][Python] Backmodul: Auswahl an Bäckereien/UV-Fliesen
* [Scripting][Python] Backmodul: Bäckereinstellungen für alle Textursätze synchronisieren
* [SVT] Aktivieren der Unterstützung für wenig Hardware auf AMD-GPUs

  Hardwarebeschleunigung für das System &quot;Spare Virtual Textures&quot; kann jetzt mit AMD-GPUs aktiviert werden. Diese Einstellung wird in den allgemeinen Voreinstellungen automatisch aktiviert.
* [Projektion] Umbenennen zylindrischer Projektionsparameter

  Der Parameter &quot;Cylinder Cap Culling&quot; wurde in &quot;Backface Culling&quot; umbenannt, um seine Aktion besser darzustellen. Die zugehörige QuickInfo wurde entsprechend angepasst.
* [Project] Speichern Sie die Anwendungsversion im Projekt und rufen Sie sie über Skripterstellung ab.

  Seit Version 8.2 wird die Version der Anwendung beim Speichern in der spp-Datei gespeichert.\
  Diese Versionsnummer kann mit der Funktion last\_saved\_substance\_painter\_version() im Projektmodul der Python-API abgerufen werden.\
  Für Projekte, die vor 8.2 erstellt wurden, ist der zurückgegebene Wert null.
* [Import] Verbessern der allgemeinen Importzeit von 3D-Modellen

  Wir haben die allgemeine Importzeit von Meshes verbessert. So wird beispielsweise die Wartezeit beim Beladen von hochpolaren Maschen zum Backen verkürzt. Diese Optimierung gilt insbesondere für das Laden von OBJ-Dateien.

**Fest:**

* [Absturz] Ändern von Kanälen bei Filtern mit bestimmtem Stapel
* [Mac][M1] Absturz beim Erstellen einer Füllebene und Verlassen des Ebenenstapels

  Dieses Problem kann durch Aktualisieren auf Mac OS 13 (Ventura) behoben werden.
* [Scripting][Python] Absturz bei Verwendung von ui.add\_dock\_widget() mit falschem Typ
* [Backen] Unvollständige Fehlermeldung im Protokoll, wenn ein Backen fehlschlägt
* [Backen] Speicher wird nach Abschluss des Backens nicht freigegeben
* [Engine] Texturcache wird nicht aktualisiert, wenn die Effektsichtbarkeit geändert wird
* [Export] 2DView exportiert zufällig einheitliche Karte
* [Projekt] Speicherzuordnungsfehler beim Speichern eines Projekts mit großem Gitter
* [Viewport] TAA verursacht beim Malen in einigen Fällen Artefakte

**Bekannte Probleme:**

* [Farbmanagement] HDR-Farbraumkonvertierungen mit ACE unter Linux erzeugen festgeklemmte Farben
* [Ebenenstapel] Eingabequelle nicht pro Ebene gespeichert
* [Exportieren] 2D-Ansicht exportiert zufällig einheitliche Karte
