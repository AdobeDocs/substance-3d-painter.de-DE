---
breadcrumb-title: ""
description: Lesen Sie die Versionshinweise für Substance 3D Painter 2018.2, um mehr über neue Funktionen, Verbesserungen und Fehlerbehebungen zu erfahren.
title: Version 2018.2
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '2346'
ht-degree: 0%
---

# Version 2018.2

**Substance Painter 2018.2** fügt lange erwartete Funktionen hinzu, wie z. B. das Malen von Volumenstreuungen, die das Texturieren noch einfacher machen als zuvor.

Freigabedatum: *2. August 2018*

## Wichtigste Funktionen

### Streuung unter der Oberfläche

![](../../assets/changelog-sss.jpg)

**Volumenstreuung** wird jetzt im **Echtzeit**-Viewport und mit dem **Iray-Renderer** unterstützt.\
Volumenstreuung ist ein Lichtmechanismus, der beim Eindringen in ein Objekt oder eine Fläche entsteht. Anstatt wie bei metallic Flächen reflektiert zu werden, wird ein Teil des Lichts vom Material absorbiert und dann **in das Innere gestreut**. Viele Materialien im echten Leben haben Volumenstreuung wie Haut oder Wachs.

Unsere Subsurface-Effekt-Implementierung entspricht sehr genau den Echtzeit-Implementierungen anderer Game-Engine sowie anderen Offline-Renderern. So lassen sich ganz einfach streuende Texturen für die Verwendung in anderen Anwendungen erstellen.

![](../../assets/comparison-1.jpg){width="650px"}

Oben sehen Sie ein Beispiel mit dem bekannten Element Digital Emily 2. Vielen Dank an das USC Institute for Creative Technologies und Mitglieder des Wikihuman-Projekts, die es uns ermöglicht haben, unsere Renderings mit den Digital Emily 2-Assets zu demonstrieren.\
(Bitte beachten Sie, dass dieser Vergleich unter ähnlichen, aber nicht exakten Lichtverhältnissen durchgeführt wurde, was visuelle Unterschiede erklären kann.)

Um einem Projekt eine Volumenstreuung hinzuzufügen, gehen Sie wie folgt vor:

1. Wechseln Sie zum Fenster **Anzeigeeinstellungen**, und **aktivieren** Sie die Einstellung **Volumenstreuung**.
1. Hinzufügen eines Kanals &quot;**Streuung**&quot; im aktuellen Textursatz
1. Verwenden Sie eine Füllebene oder **Malen in Weiß** im neuen Kanal, um **den Unteroberflächeneffekt im Viewport freizulegen**.

Eine ausführlichere Vorgehensweise finden Sie in der [Volumenstreuung-Dokumentation](../../features/subsurface-scattering/subsurface-scattering.md).

>[!NOTE]
>
> Um die Volumenstreuung im Echtzeit-Viewport zu unterstützen, müssen die **Shader** in den Projekten **aktualisiert** sein.\
> Informationen zu benutzerdefinierten Shadern finden Sie in der Dokumentation im **Hilfemenü**. Dort erfahren Sie, welche Änderungen im **Shader-API** vorgenommen wurden.

### Manipulator für Füllebenen

![](../../assets/changelog-manipulator.png)

Die Steuerelemente für Füllebenen wurden verbessert, um Manipulatoren zu bieten. Es ist jetzt einfacher, die Projektionen der Füllung präzise zu platzieren und zu steuern.

Bei Verwendung der **UV-Projektion** wird ein Manipulator in der **2D-Ansicht** angezeigt:

* Durch Klicken auf **außerhalb von** wird der Manipulator **gedreht**.
* Durch Klicken auf das **Quadrat** an den **Rändern** wird es **skaliert/skaliert**.
* Durch Klicken auf **in** wird der Manipulator **Kamera bewogen**.
* Verwenden Sie **STRG**, um mehrere Eckpunkte in **Symmetrie** zu beeinflussen.
* Verwenden Sie **UMSCHALT** bis **Einschränkung** für eine Transformation (Kamera beweg, Drehung oder Skalierung).\
  ![](../../assets/manipulator-uv.gif)

Bei Verwendung der **Tri-Planaren Projektion** wird ein Manipulator in der **3D-Ansicht** angezeigt:

* Der gepunktete Würfel repräsentiert die globale Projektion
* Verwenden Sie den **W**, **E** oder **R**-Tastatur-Tastaturbefehl, um zwischen den Modi **Kamera beweg**, **Drehen** und **Skalieren** zu wechseln.
* Verwenden Sie den **T**-Tastatur-Tastaturbefehl, um für den Manipulator zwischen &quot;Lokal&quot; und &quot;Welt&quot; zu wechseln.
* Verwenden Sie **SHIFT**, um **die Transformation zu beschränken**.
* Die Tri-Planare Cube-Projektion kann auch in den erweiterten Füllebene-Eigenschaften geändert werden:\
  ![](../../assets/fill-properties-triplanar.png)\
  ![](../../assets/manipulator-3d-optim.gif)

Die kontextbezogene Symbolleiste am oberen Rand des Viewports wird sich auch je nach aktuellem Projektion-Modus anpassen und bietet zusätzliche Tools und Steuerelemente:

![](../../assets/contextual-toolbar-manipulator.png)

Weitere Informationen finden Sie in der Dokumentation zur [Füllebene](../../painting/fill-projections/fill-projections.md).

### Nicht quadratische und nicht bearbeitungsfertige Unterstützung für Schablone und Projektion

![](../../assets/non-square-stencil.jpg)

Der Parameter &quot;Schablone&quot; und das Werkzeug &quot;Projektion&quot; wurden verbessert und unterstützen nun auch nicht quadratische Auflösungen und Verhalten ohne Bodenbearbeitung.\
Der Standardparameter ist jetzt standardmäßig auf &quot;Nicht bestellen&quot; festgelegt. Dieser Parameter kann in den Werkzeugeigenschaften geändert werden:

![](../../assets/tilling-parameter-stencil.png)

Der Bearbeitungsmodus kann wie folgt eingestellt werden:

* **Keine Kachelung** (Standard)
* **Horizontale Kachelung**
* **Vertikale Kachelung**
* **H- und V-Kachelung** (altes Verhalten)

Dieser neue Parameter kann in einem Tool oder in einer Pinselvorgabe gespeichert werden, sodass es einfach ist, ihn mit benutzerdefiniertem Inhalt zu teilen.

>[!NOTE]
>
> * Das Projektion-Verhältnis wird sich auch bei Substance-Dateien anpassen, die nicht quadratische Auflösungen ausgeben. Das Verhältnis wird direkt vom Ausgabeknoten aus berechnet.
> * Wenn mehrere Kanäle unterschiedliche Verhältnisse aufweisen, wird das erste gefundene Verhältnis mit dem Projektion-Werkzeug auf alle anderen Kanäle angewendet.

### Import und Verwaltung von Kameras

![](../../assets/camera-import.png)

Es ist jetzt möglich, **benutzerdefinierte Kameras** in Substance Painter neben dem Mesh-Import zu importieren.\
Kameras können **ausgewählt werden, um sie im** 3D-Viewport **zu durchsuchen** und **zum Rendern in Iray** zu verwenden.

Weitere Informationen finden Sie in der [Dokumentation zur Kamera-Verwaltung](../../interface/viewport/camera-management.md).

So **importieren Sie Kameras** in ein Projekt:

1. Mesh für das Projekt mit Kameras in derselben Datei exportieren (mit einem unterstützten Format wie FBX, Alembic oder glTF)
1. Wählen Sie die Einstellungen für &quot;Kameras importieren&quot; im [neuen Projektfenster](../../getting-started/project-creation.md) (oder [Projektkonfiguration](../../interface/project-configuration.md)).\
   ![](../../assets/new-project-cameras.png)
1. Wechseln Sie mit der Dropdown-Liste im Viewport oder mithilfe der Kameras in [Anzeigeeinstellungen](../../interface/display-settings/camera-settings.md) zur gewünschten Version.\
   ![](../../assets/cmaera-select-viewport.png)

Die Kamera-Einstellungen im Fenster Anzeigeeinstellungen wurden erweitert, um die Eigenschaften der Kamera zu steuern.\
Es ist möglich, **zwischen Kameras zu wechseln**. Weitere Informationen finden Sie unter **Verhältnis** und **Sperre** der Eigenschaften, um eine Änderung zu vermeiden. Mit einer Wiederherstellungsschaltfläche kann die Kamera auf ihre ursprünglichen Werte zurückgesetzt werden.

![](../../assets/camera-properties-2.png)

Der Rahmen der Kamera (und sein Tor) wird ebenfalls berücksichtigt, sodass es möglich ist, über einen ganz bestimmten Blickwinkel zu betrachten und zu Malen. Der Rahmen und das Gate werden über dem 3D-Viewport angezeigt, und seine Deckkraft kann in den **Viewport-Einstellungen** im Fenster [Anzeigeeinstellungen](../../interface/display-settings/camera-settings.md) gesteuert werden:

![](../../assets/camera-gate.png)

### Verbesserungen am Verhalten von Ebenenstapeln

* **Ziehen Sie Materialien und Intelligente Materialien per Drag &amp; Drop auf den ID-Map :**\
  Das Ziehen und Ablegen von Inhalten aus dem Regal in den Viewport wurde verbessert. Durch Drücken von **STRG** beim Ziehen und Ablegen eines Materials können Sie jetzt die ID-Farbe auswählen, die als Maske verwendet wird.\
  Eine schwarze Maske mit dem Effekt &quot;Farbauswahl&quot; wird zur neuen Ebene hinzugefügt, die im Ebenenstapel erstellt wurde. Wenn dasselbe Material per Drag-and-Drop auf eine andere ID-Farbe platziert wird, wird die bereits vorhandene Ebene aktualisiert und die ID-Farben werden kombiniert.\
  ![](../../assets/id-drop.gif)
* **Scroll per Drag &amp; Drop von Ebenenstapeln:**\
  Beim Ziehen von Ebenen um den Ebenenstapel wird nun ein kleines Fenster angezeigt.\
  Wenn eine Ressource oder eine Ebene in die Nähe der Ränder des Ebenenstapel-Fensters gezogen wird, wird automatisch ein Bildlauf für den Inhalt durchgeführt.\
  ![](../../assets/layer-drag.gif)

### glTF- und Alembic-Mesh importieren

![](../../assets/logo-mesh-import.png)

Neue Dateiformate werden jetzt für das Importieren von Meshs und das Erstellen neuer Projekte unterstützt:

* **glTF** : Dieses Format war bereits beim Exportieren von Texturen verfügbar und kann jetzt während des Imports verwendet werden. Wenn eine glTF-Datei Texturen enthält, werden diese importiert und im Ebenenstapel abgelegt (für den Workflow &quot;metallic/Rauheit&quot;).
* **Alembic** : Dieses Format ist in der VFX-/Animationsbranche weit verbreitet, um Mesh zu übertragen.

>[!NOTE]
>
> Substance Painter bietet keine Möglichkeit, zu steuern, welcher Rahmen der Animation gerade importiert werden soll.\
> Dies bedeutet, dass beim Exportieren einer Alembic-Datei der Rahmen der Referenz für das Malen auf dem Asset bereits festgelegt sein muss.

### Verbesserungen an der Substance-Integration

![](../../assets/integration.png)

Die Substance-Integration in Substance Painter wurde mit lange erwarteten Anfragen verbessert:

* <b>Sichtbar, wenn:</b>\
  Das &quot;Visible if&quot; ist eine großartige Funktion des Substance-Dateiformats, das es ermöglicht, Parameter auf Basis von Bedingungen auszublenden.\
  Diese Funktion bietet eine klarere Liste von Parametern und Kontexteinstellungen, sodass Material und Filter insgesamt einfacher zu verwenden sind.\
  Weitere Informationen finden Sie in der Dokumentation zu [Substance Designern](https://experienceleague.adobe.com/en/docs/substance-3d-designer/home).\
  ![](../../assets/visible-if.gif)
* **Substance-Vorgaben** Substance-Vorgaben sind eine einfache Möglichkeit, erweiterte Anpassungen und Variationen von Materialien bereitzustellen. Viele Material auf [Substance Source](https://source.allegorithmic.com) verfügen über Vorgaben. Probieren Sie es aus!\
  Wenn eine Substance-Datei eine oder mehrere Vorgaben enthält, ist ein neues Dropdown-Menü in der Parameterliste verfügbar. Wählen Sie die Vorgabe aus, die zum Aktualisieren der Parameter angewendet werden soll.\
  ![](../../assets/presets.png)
* **Substance-Attribute**\
  Substance-Attribute werden jetzt in der Benutzeroberfläche angezeigt, sodass Informationen zu einer bestimmten Datei leichter abgerufen werden können.\
  Attribute können an zwei verschiedenen Orten angezeigt werden: über den Parametern im Eigenschaftenfenster oder durch Klicken mit der rechten Maustaste auf ein Element im Regal.\
  ![](../../assets/attributes.png) ![](../../assets/attributes-shelf.png)

### Neues Beispielprojekt &quot;Jade Toad&quot;

![](../../assets/toad-samle.jpg)

Ein neues Beispielprojekt mit dem Namen &quot;**JadeToad**&quot; ist jetzt im Substance Painter enthalten. Für dieses Beispielprojekt ist der Effekt **Volumenstreuung** standardmäßig aktiviert.\
Verwenden Sie zum Suchen des Projekts die Datei **Datei** > **Beispiel öffnen...**-Menüeintrag.

## Versionshinweise

### 2018.2.3

(Release 25. September 2018)

****Fest:****

* [2D-Ansicht] Bei der Erstellung eines neuen Projekts ist die 2D-Ansicht mit einigen Meshs beschädigt.
* [Absturz] Der Wechsel von der UV-Projektion zur dreimal planaren Projektion führt zu einem Absturz
* [RayCollider] Mehrere Absturz durch &quot;RayCollider&quot;
* [Werkzeug] Beim Wechseln von Ebenen gehen die geänderten Pinseleigenschaften verloren
* Pinseleinstellungen werden beim Wechsel zum Radierer zurückgesetzt

**Bekannte Probleme:**

* Einfrieren der Berechnung auf AMD VEGA-GPUs
* Problem mit Huion-Tablets mit Tastaturbefehlen unter Windows

### 2018.2.2

(Release 11. September 2018)

**Hinzugefügt:**

* Zusammenfassung: Hotfix mit Inhaltsaktualisierung, neuen Skriptfunktionen und der Möglichkeit, die automatische Aktualisierung zu deaktivieren
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

### 2018.2.1

(veröffentlicht am 3. August 2018)

**Fest:**

* Fehlende Shader-Parameter für die Volumenstreuung beim Aktualisieren von Projekten

**Bekannte Probleme:**

* Einfrieren der Berechnung auf AMD VEGA-GPUs
* Problem mit Huion-Tablets mit Tastaturbefehlen unter Windows

### 2018.2

(Release 2. August 2018)

**Hinzugefügt:**

* Zusammenfassung: Sommerversion, Volumenstreuung-Unterstützung, Verbesserungen bei Projektion und Füllung, Import und Auswahl von Kameras, Alembic/glTF-Unterstützung, Drag-and-Drop auf dem ID-Map, verbesserte Unterstützung für Substance-Formate und neue Inhalte
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
* [Kameras][UI][Neues Projekt][Projektkonfiguration] &quot;Kameras importieren&quot; ist standardmäßig aktiviert.
* [Kameras][Tastaturbefehle] Fügen Sie die Tastaturbefehle &quot;&lt;&quot; und &quot;>&quot; hinzu, um zwischen den Kameras zu wechseln.
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
* [UI][Neues Projekt][Projektkonfiguration] Ersetzen Sie &quot;Mesh&quot; durch &quot;Datei&quot;.
* [UI][Substance] Anzeigen von Substance-Attributen in der Benutzeroberfläche
* [Tastaturbefehle] &quot;F4&quot; wechselt zwischen 2D- und 3D-Ansicht
* [Tastaturbefehle] Neue Tastaturbefehle für die Schablone &quot;N&quot; zum Umschalten und die schnelle Maske &quot;U&quot; zum Umschalten
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
* [API] Rufen Sie das `onNewProjectCreated`-Skript-API-Ereignis auf, selbst wenn Sie mit einer Vorlage erstellen.
* [Shader] Kompilierter Shader wird nicht aus dem Cache geladen, wenn die Shader-Datei nicht kompiliert wird
* [Regal] Exportieren der HDR-Datei aus dem Regal gibt eine Datei mit festgeklemmten Werten aus
* [Exportieren] EXR exportieren Klammern RGB Farbwerte zwischen 0-1
* [Inhalt] Prozedurale Rauschen &quot;3D Perlin Rauschen Fractal&quot; ist verpixelt

**Bekannte Probleme:**

* Einfrieren der Berechnung auf AMD VEGA-GPUs
* Problem mit Huion-Tablets mit Tastaturbefehlen unter Windows
