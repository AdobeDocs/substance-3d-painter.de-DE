---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/release-notes/old-versions/version-2018-1.html"
breadcrumb-title: ''
description: Lesen Sie die Versionshinweise für Substance 3D Painter 2018.1, um mehr über neue Funktionen, Verbesserungen und Fehlerbehebungen zu erfahren.
helpx_creative_field: ""
helpx_description: Painter > Release notes > Old versions > Version 2018.1
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Version 2018.1
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '2400'
ht-degree: 0%

---


# Version 2018.1

Mit **Substance Painter 2018.1** wird eine brandneue Benutzeroberfläche mit vielen verbesserten Verhaltensweisen eingeführt. Auch die Leistungen wurden in vielen Bereichen verbessert.

Freigabedatum: *15. März 2018*

## Wichtigste Funktionen

### Neue Benutzeroberfläche und Verhaltensweisen

![](../../assets/2018-03-15-16-34-59-greenshot.jpg){width="650px"}

Mit Substance Painter 2018.1 wird eine **vollständige Überarbeitung der Benutzeroberfläche** eingeführt, die von Farb- und Symbolen bis hin zu Widgetverhalten reicht.

* Die **neue Schnittstelle** konzentriert sich auf ein brandneues Design, das das Lesen erleichtert und die Navigation erleichtert.\
  Wir überarbeiteten alle unsere Icons, um sie deutlicher zu machen. Wir haben auch unser Farbschema überarbeitet, das jetzt einheitlicher sein sollte.\
  ![](../../assets/flat-design.png)
* Wir haben viele Widgets, insbesondere unsere **Regler**, verbessert, um **benutzerfreundlicher** zu sein, mit einem **Tablet-Stift**.\
  Sie können auf die Leiste klicken, um den Schieberegler zu verschieben, oder das Wertfeld verwenden, um die Zahlen präziser zu bearbeiten.\
  ![](../../assets/sliders.gif) ![](../../assets/grayscale-slider.gif)
* Wir verfügen über eine **neue Symbolleiste**, mit der **Docks** im Handumdrehen geöffnet werden können.\
  Wenn Sie auf eine der Schaltflächen in der Symbolleiste klicken, wird das Dock neben der Schaltfläche angezeigt und schwebt über dem Rest der Benutzeroberfläche. Wenn Sie erneut auf die Schaltfläche klicken, wird sie geschlossen.\
  Wenn sich das Dock von seiner Schaltfläche entfernt, wird es zu einem normalen schwebenden Fenster, das in der Benutzeroberfläche angedockt werden kann. Wenn sie geschlossen wird, ist die Schaltfläche wieder in der Dock-Symbolleiste verfügbar.\
  Dieses neue Docksystem funktioniert einfacher mit dem Vollbildmodus. Es ist nicht mehr erforderlich, dass jedes Dock immer in der Benutzeroberfläche vorhanden ist.\
  ![](../../assets/ui-dock-collapse-recall-optim.gif)
* Docks verwenden jetzt unser neues **Registerkarten-Layout**, das Elemente in Abschnitten organisiert, während gleichzeitig ein schneller Bildlauf in ihm möglich ist.\
  Dieses Registerkartenlayout erlaubt **große Fenster** und kann **alle Informationen** gleichzeitig anzeigen, im Gegensatz zu normalen Registerkartensystemen, die Informationen ausblenden.\
  ![](../../assets/tab-layout.gif) ![](../../assets/tab-layout-display.gif) ![](../../assets/full-window.png)
* Es ist jetzt ein **Schnellmenü** vorhanden, das **Werkzeugeigenschaften** direkt im Viewport **verfügbar macht.**\
  Klicken Sie zum Öffnen des Schnellmenüs einfach mit der rechten Maustaste auf den Viewport **.** Um das Schnellmenü **zu schließen**, klicken Sie **erneut in den Viewport**.\
  Das Menü wird nur geschlossen, wenn Sie in den Viewport klicken, sodass Ressourcen per Drag &amp; Drop aus dem Regal direkt in das Schnellmenü gezogen werden können.\
  ![](../../assets/quick-menu-optim.gif)
* Oben befindet sich jetzt eine neue **Kontextsymbolleiste** für den Viewport.\
  Diese Symbolleiste ändert ihre Parameter in Abhängigkeit vom aktuell verwendeten Werkzeug. Auf diese Weise können Sie schnell auf grundlegende Werkzeugfunktionen zugreifen (z. B. die Pinselgröße).\
  ![](../../assets/contextual-toolbar_1.png)
* Es ist jetzt möglich, **Effekte** mithilfe von **Ziehen und Ablegen** im **Ebenenstapel** neu anzuordnen.\
  ![](../../assets/re-order-effects.gif)
* Während die Tastaturbefehle &quot;**C**&quot; und &quot;**B**&quot; es Ihnen ermöglichen, die **Kanal** und **Gebackenen Texturen** schnell in den **Viewport** zu visualisieren, ist es jetzt möglich, die **einheitliche Dropdown-Liste** zu verwenden, um die Viewport-Anzeige zu ändern.\
  In der **oberen rechten Ecke** des **Ansichtsports** befindet sich jetzt eine Dropdownliste mit **allen Kanälen und Meshmaps** (zuvor Zusätzliche Karten). Diese vereinheitlichte Dropdown-Liste ist auch im Dock **Anzeigeeinstellungen** verfügbar.\
  ![](../../assets/dropdown-viewport.gif)
* Die **Anzeigeeinstellungen** und **Anzeigeeinstellungen** wurden **zusammengeführt** zu einem einzigen Dock.\
  **Die Einstellungen für Umgebung**, **Kamera** und **Viewport** sind jetzt **gruppiert**, während die **Shader**-Parameter **verschoben** in ein **dediziertes Dock** wurden.\
  Die Anzeigeeinstellungen nutzen jetzt das neue **Registerkarten-Layout**, um schnell durch das Fenster zu navigieren.\
  ![](../../assets/display-shader-settings.png)

### Ziehen und Ablegen von Materialien und Smart-Materialien in den Viewport

![](../../assets/drag-drop-material-resize.gif){width="650px"}

Sie können jetzt **Materials und Intelligenten Materials von** direkt in den Viewport ziehen und ablegen **&#x200B;**.\
Durch diese neue Aktion wird **gleichzeitig die Geometrie** des **Ziel-Textursatzes** hervorgehoben. Mit dieser Aktion werden die neuen Ebenen am oberen Rand des Ebenenstapels des Textursatzes erstellt.

### Verbessertes Verhalten von Tablet-Stiften

![](../../assets/tablet-pen-events.png)

In dieser Version haben wir die Art und Weise verbessert, wie wir Grafiktablett-Stift-Bewegungen und Eingaben verarbeiten, insbesondere wenn Substance Painter unter einer großen Belastung ist.\
Wir verlieren die Eingänge nicht mehr, während wir aufeinander folgende Berechnungen durchführen. Dies sollte in allen Situationen präzise Pinselstriche ermöglichen.

### Verbesserte Innenabstände der Naht

![](../../assets/seam-3.png)

Wir haben die Art und Weise überarbeitet, wie wir Auffüllungen außerhalb der UV-Inseln generieren. Anstatt das aktuelle Pixel auf eine bestimmte Distanz zu erweitern, suchen wir nun nach dem benachbarten Pixel auf der anderen Seite der UV-Naht und interpolieren die beiden Werte.\
Dies führt zu einem viel besseren Endergebnis und reduziert die Sichtbarkeit der Teilung zwischen UV-Inseln, auch wenn die Textelverhältnisse nicht übereinstimmen.

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../assets/seam-2.png){width="200px"}

</td>
<td style="border: 0;" valign="top">

![](../../assets/seam-1.png){width="200px"}

</td>
</tr>
</table>

Dieser neue Abstand wird automatisch nach jedem Pinselstrich, jeder Änderung der Auflösung oder jeder Änderung der Ebene generiert.

### Verbesserte Leistung

![](../../assets/painting-viewport-optim.gif){width="650px"}

Wir haben auch die Leistung in dieser Version auf mehreren Ebenen verbessert:

* Das Öffnen und Speichern von Projekten sollte etwas schneller als zuvor erfolgen.\
  Wir haben die Codierung/Decodierung unserer **Maldaten** überarbeitet. Dies betrifft insbesondere Projekte mit vielen Malen-Informationen (Pinselstriche).
* Wir unterstützen jetzt viele **Unterobjekte** mit Meshs.\
  Es ist nicht mehr zwingend erforderlich, einen Mesh zu einem Stück zusammenzufügen, bevor er in Substance Painter geladen wird. Die Leistung sollte auch bei **8000 Unterobjekten** in einem Projekt gut bleiben.
* Wir haben die Art und Weise geändert, in der **Viewport** **aktualisiert** wurde, um die Belastung der GPU beim Malen zu reduzieren.\
  Das bedeutet, dass wir nicht mehr das gesamte Bild aktualisieren, sondern eine kleine Region, in der Sie gerade arbeiten.\
  Sie können den Unterschied bei weniger leistungsstarken GPUs oder bei Verwendung einer hohen Sample-Anzahl in Ihrem Shader feststellen.
* Das System **Regal** ist jetzt **schneller, um** Ressourcen beim Starten der Anwendung zu erkennen.\
  Substance-Materialien mit eingebetteten Bitmaps sind **doppelt so schnell** zu erkennen (wenn sie als nicht-solid gekocht werden). **Vorgaben** sollten ebenfalls Verbesserungen sehen.

### Baker für die globale Szene

![](../../assets/position-baker.jpg)

Wir haben jetzt eine neue Einstellung, die es ermöglicht, eine Positionskarte pro Textursatz Baking führen, die die Größe der gesamten Szene berücksichtigt.\
Mit diesem neuen Verhalten können Sie triplanare Projektionen in Maskengeneratoren verwenden, die über die gesamte Szene übereinstimmen, anstatt wie zuvor Nähte zu erstellen. Dies ist bei Projekten mit vielen Textursätzen (wie UDIM-basierten Projekten) wirklich nützlich.

Ändern Sie in den Positionsparametereinstellungen den Baker &quot;**Normalisierungsskala**&quot; von &quot;**Pro Material**&quot; in &quot;**Volle Szene**&quot;, um dieses neue Verhalten zu aktivieren.

![](../../assets/position-baker-example.png)

### Neuer Inhalt

![](../../assets/3d-noises.png)

Wir haben in dieser Version auch einige neue Inhalte hinzugefügt:

* Neue **3D-Rauschen.**\
  Direkt aus Substance Designer importiert, wurden dem Standard-Regal 4 neue 3D- und völlig nahtlose Rauschen hinzugefügt.\
  Diese neuen Rauschen nutzen die Positionskarte des Projekts, um ein Ergebnis ohne Nähte zu generieren.
* **Nicht quadratische** Rauschen\
  Die Basisversionen wurden auf die neueste Rauschen von Substance Designer aktualisiert.\
  Dies bedeutet, dass die Funktion für nicht quadratische Erweiterungen jetzt in den Rauschen-Parametern verfügbar ist.
* Neuer Maskengenerator **3D Linear gradient.** Mit diesem neuen Maskengenerator können Sie einen linearen Verlauf in jede beliebige Richtung im 3D-Raum erstellen.\
  Die Richtung kann mit zwei 3D-Positionen definiert werden, die direkt auf der Positionskarte ausgewählt werden können.\
  Beispiel :

1. &#x200B;
   1. Erstellen Sie den Maskengenerator **3D Linear gradient** in einer Ihrer Ebenen.
   1. Wechseln Sie die Viewport-Anzeige zu &quot;**Position**&quot; (über die Viewport-Dropdownliste oder mithilfe der Taste &quot;**B**&quot;).
   1. Klicken Sie auf den Parameter &quot;**3D-Positionsstart**&quot;, um das Popup **Farbwähler** zu öffnen.
   1. **Wählen Sie eine Farbe** für das Gitter **im Viewport aus**
   1. Wiederholen Sie den Vorgang für den zweiten Parameter &quot;**3D Position End**&quot;.

      ![](../../assets/3d-gradient.jpg)

* Neue Vorlage **Lens-studio** (Einrasten Chat 3D-App).\
  Wir haben eine neue Vorlage, mit der Sie ganz einfach Projekte erstellen können, die auf die von Einrasten erstellte Lens-Studio-Anwendung abzielen.\
  Eine spezielle Shader- und Exportvorgabe ist ebenfalls verfügbar. Weitere Informationen zu Lens Studio finden Sie unter : <https://lensstudio.snapchat.com/>
* **Intelligenten Materials** und **Intelligente Masken** wurden mit der neuesten Version unserer Maskengenerator aktualisiert.\
  Unsere Smart-Vorgaben unterstützen jetzt alle die Funktion **micro details** , die mit **Ankerpunkten** verwendet werden kann.

### Neues Beispielprojekt

![](../../assets/seamless-paint-material-optim.gif){width="650px"}

Es gibt jetzt ein neues Beispielprojekt mit dem Namen &quot;**TilingMaterial**&quot;, das Sie über die Menüaktion &quot;**Datei > Beispiel öffnen**&quot; öffnen können.\
Dieses Projekt verwendet einen einfachen ebenen Mesh mit überlappenden UVs, der das nahtlose **Malen von** Materialien und Pinselstrichen zum **Erstellen von Kachelung-Materialien** ermöglicht.

![](../../assets/seamless-paint-optim.gif){width="400px"}

## Tutorial

Der Substance Academy wurde ein neuer Tutorial-Kurs hinzugefügt, der unsere neue Benutzeroberfläche behandelt: [Erste Schritte mit Substance Painter 2018](https://academy.allegorithmic.com/courses/a97b433a5997fd800b5ed300d783cc41/youtube-e-zpEL0Wcqg)

## Versionshinweise

### 2018.1.3

(Release 28. Juni 2018)

**Hinzugefügt:**

* Zusammenfassung: Hotfix
* [Voreinstellungen] Vorschlag zum Speichern des Projekts beim Neustart von Painter

**Fest:**

* [Plug-In] Substance Source &quot;Suchen&quot; funktioniert nicht
* [Smart Materials] Das Importieren von Smart-Materialien führt in einigen Fällen zu einem Absturz
* [Smart Materials] Das Löschen von Smart Materials führt in einigen Fällen zu einem Absturz
* [Speichern] Das Speichern führt in seltenen Fällen zu einem Absturz
* [Shelf] Umkehren funktioniert nicht auf Zellen 2 und Zellen 3
* [Shelf] Typo in einigen Alphas
* [Shelf] Einige Substance-Materialien lassen sich nicht richtig rendern

**Bekannte Probleme:**

* Einfrieren der Berechnung auf AMD VEGA-GPUs

### 2018.1.2

(veröffentlicht am 6. Juni 2018)

**Hinzugefügt:**

* Zusammenfassung: Verbesserte Geschwindigkeit beim Baking, verbessertes Speichersystem, aktualisierte Schieberegler, aktualisierte Plug-in-API, Übersetzung ins Chinesische, verbesserter Abstand jetzt optional
* [Bäcker] Leistungssteigerung mit neuer Bäcker-Version
* Erzwungene Anzeige von Dialogfeldern mit inkompatibler GPU
* [Speichern] Neue Funktion für kompakte Projekte bereitstellen (vollständiger/kompakter Speichermodus)
* [Speichern] Benutzer informieren, wenn Fehler beim Speichern auftritt
* [Clean] Nächste Speicherung im Voll-/Kompaktmodus
* [Schieberegler] Verbesserung der Präzision der Farb-/Graustufenbalken und Schieberegler
* [Schieberegler] Hinzufügen der Pfeilsteuerungen nach oben/unten
* [Schieberegler] Dieselbe Erkennungszone für Farb- und Graustufenbalkenschieberegler
* [Plugin] Automatische Speicherung immer im inkrementellen Modus
* [Plug-In] Option zum Wechseln von Plug-Ins zu einem neuen Schnittstellenstil
* [Sprache] Chinesische Übersetzung hinzufügen
* [Auffüllung] Option zum Wechseln zwischen UV- und 3D-Raum-Nachbarauffüllung pro Textursatz in den Textursatzeinstellungen
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

### 2018.1.1

(veröffentlicht am 3. April 2018)

**Fest:**

* [Tablet] Problem beim Ändern der Standardinteraktionsoptionen
* [Baker] Absturz mit Assimp-Bibliothek
* [Baker] Leistungsrückgang mit A.O.-Map
* [Iray] Die Verzerrung des Objektivs wird nicht auf den Alphakanal angewendet
* [Treiber] Aktualisierung der Mindestanforderungen für Treiber
* [3Dview] Normale, die nicht korrekt auf UDIM-Netzen ohne Normaleninformationen generiert wurden
* [Intel] Absturz mit Substance Painter 2018.1.0
* [Intel]&#x200B;[Viewport] Problem mit der Auffüllung (schwarze Artefakte)

**Bekannte Probleme:**

* Einfrieren der Berechnung auf AMD VEGA-GPUs

### 2018.1

(veröffentlicht am 15. März 2018)

**Hinzugefügt:**

* Neuer allgemeiner Stil (Symbole, Farbe, Verhalten)
* Neues Standardlayout
* [Tablet] Benutzererfahrung beim Malen verbessert
* [Hauptmenü] Sortieren Sie native Elemente zuerst in Ansichten und Symbolleisten
* [Hauptmenü] Schnellmaskierungsaktionen im Ansichtsfenster verschieben
* [Hauptmenü] Verschieben von Rechtsklick-Aktionen in den Ansichtsfenster-Abschnitt
* [Hauptmenü] Menü &quot;Ansicht&quot; in &quot;Fenster&quot; umbenennen
* [Schnellmenü] Neue Werkzeugeigenschaften durch Rechtsklick im Ansichtsfenster
* [Dock-Widget] Neue Dock-Symbolleiste zum schnellen Reduzieren/Zurückrufen
* [Anzeigeeinstellungen] Fenster &quot;Kamera- und Anzeigeeinstellungen&quot; wurde zusammengeführt
* [Ebenenstapel] Kontextmenü (rechte Maustaste)
* [Ebenenstapel] Ziehen und Ablegen, um beliebige Effekte innerhalb derselben Ebene zu verschieben
* [Symbolleiste] Neuorganisation der Symbolleiste und neue kontextbezogene Symbolleiste
* [Werkzeugleiste] Klonwerkzeug in zwei separate Werkzeuge teilen
* [Werkzeugeigenschaften] Hellerer Graustufenwert im Hintergrund in der Vorschau
* [Eigenschaften von Tools] Organisation in Registerkarten (Füllung und Werkzeuge)
* [Tool] Malergebnis entspricht der Schablone
* [Viewport] Neuer Cursor für Füllebene
* [Viewport] Einfachere Navigation und besseres Malen (höhere Framerate)
* [Viewport] Kombinationsfeld für Material-/Kanal-/Kartenauswahl im Viewport
* [Viewport] Flackern beim Drehen reduzieren (Schatten aktiviert)
* [Shelf] Zeigt Materialien standardmäßig beim Öffnen von Painter an
* [Shelf] Ladezeitverbesserung von Substance-Texturen und -Materialien (2- bis 6-mal schneller)
* [Shelf] Neuorganisieren von Materialordnern, um die Struktur der Substance Source anzupassen
* [Shelf] Ziehen Sie Materialien per Drag &amp; Drop direkt auf das Gitter im Viewport
* [Shelf] Neue 3D-Geräusche (Perlin, Perlin Fraktal, Simplex und Worley)
* [Shelf] Neuer 3D Linear gradient-Maskengenerator unter Verwendung der Gitterposition
* [Shelf] Basisgeräusche zur Unterstützung der quadratische Ausbreitung aktualisiert
* [Shelf] Neue Vorlage und Exportvorgabe für Lens Studio (Snap-Anwendung) hinzugefügt
* [Shelf] Smart-Materialien und Smart-Masken wurden aktualisiert, um die neueste Version des Masken-Editors zu verwenden (Mikrodetails)
* [Shelf] Neues Beispielprojekt &quot;TilingMaterial&quot; zur Erstellung nahtloser Kachelmaterialien
* [Shelf] Neue Pinselvorgaben (Kalligrafie, Nass, Schraffur usw.)
* [Schieberegler] Neue Schieberegler und Stil und Verhalten von Graustufen-/Farbbalken
* [Bäcker] Verwenden des vollständigen Begrenzungsrahmens der Szene, um die Positionskarte zu berechnen
* [Shader] Entfernen des Height Force-Parameters aus den Standard-Shader-Parametern
* [Engine] Substance-Engine aktualisiert
* [Engine] Keine oder weniger Diskontinuitäten zwischen UV-Blöcken (neue Nahtauffüllung)
* [Plug-ins] Importieren Sie schneller aus Substance Source heruntergeladene Materialien
* [Plug-ins] Alle Plug-ins aktualisieren, um dem neuen Gesamtstil zu entsprechen
* [Voreinstellungen] Automatische Vorschau der Hintergrundfarbänderungen
* [Clean] Geringeres Risiko für Projektbeschädigung
* [Öffnen] Verbesserung der Projektzeit wird geöffnet
* [Neues Projekt] Neues Projekt - Verbesserung der Aktualisierungszeit des Gitters
* [Speichern] Speichern der Zeitverbesserung für das Projekt
* [Protokoll] Im Protokoll angegebener Lizenztyp
* [TextureSet] Umbenennen der Schaltfläche &quot;Texturen backen&quot; in &quot;Gitterzuordnungen backen&quot;
* &quot;Zusätzliche Karten&quot; in &quot;Gitterkarten&quot; umbenennen

**Fest:**

* [Viewport] Fehlerhafte Bewegungen mit Gittern, die viele Unterobjekte enthalten
* [Werkzeugeigenschaften] Kanal deaktiviert, wenn ein Bild per Drag &amp; Drop in den Materialschlitz gezogen wird
* [Werkzeugeigenschaften] Pinselvorschau wird mit Verwisch- und Kopierwerkzeugen beschädigt
* [Textursatz] Die Reihenfolge der Kanäle ist bei Verwendung von Vorlagen falsch
* [Shelf] Fehlendes Symbol für Graustufen-Konvertierungsgenerator
* [Shelf] Alpha-Zahl für Signaturkreise ist defekt (fehlende Schrift)
* Falsche Erkennung integrierter GPUs beim Start
* [Absturz] Ziehen und Ablegen einer importierten Ressource mit dem Namen #
* [Engine] VRAM-Erkennungsproblem auf integrierter GPU
* [Engine] Mehrere Abstürze im Substance Engine Linker behoben
* [Engine] Quadratische Artefakte bei Änderung der Auflösung
* [Post Effects] Die Größe der Benutzeroberfläche ist langsam, wenn Post-Effekte aktiviert sind
* [Bäcker] Die Szeneneinheit wird bei den Werten für die Strahlentfernung nicht korrekt eingehalten.
* [Bäcker] AO aus Mesh Occluder-Entfernung wird unabhängig vom Eingangswert auf 1 geklemmt
* [Bäcker] Bei der Namensübereinstimmung werden einige Gitter mit bestimmten Namen ignoriert.
* [Bäcker] Die Einstellung &quot;Farbe aus Gitter - Polygruppe&quot; und &quot;Teilgitter-ID&quot; gibt immer ein schwarzes Bild zurück.
* [Bäcker] ID-Backen schlägt mit binären FBX-Netzen aus Blender fehl
* [Shader] Rauschen in der 2D-Ansicht mit dota-2 und nicht-pbr-spec-gloss
* [Linux] Beim Backen wird nur ein CPU-Thread verwendet
* [MacOS] Absturz mit Pinselcursor, der sich über den Viewport bewegt

**Bekannte Probleme:**

* Einfrieren der Berechnung auf AMD VEGA-GPUs
* Verzerrungsnachbearbeitung wird beim Export in Iray nicht berücksichtigt (Alphakanal)
