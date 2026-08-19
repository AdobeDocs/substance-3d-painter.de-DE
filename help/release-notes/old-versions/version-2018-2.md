---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/release-notes/old-versions/version-2018-2.html"
breadcrumb-title: ''
description: Lesen Sie die Versionshinweise für Substance 3D Painter 2018.2, um mehr über neue Funktionen, Verbesserungen und Fehlerbehebungen zu erfahren.
helpx_creative_field: ""
helpx_description: Painter > Release notes > Old versions > Version 2018.2
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Version 2018.2
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '2346'
ht-degree: 0%

---


# Version 2018.2

**Substance Painter 2018.2** fügt lange erwartete Funktionen hinzu, wie z. B. das Malen mit Untergrundstreuung, die die Texturierung noch einfacher als zuvor machen.

Freigabedatum: *2. August 2018*

## Wichtigste Funktionen

### Streuung unter der Oberfläche

![](../../assets/changelog-sss.jpg)

**Das Streuen von Unterflächen** wird jetzt im **Echtzeit**-Viewport und mit dem **Iray-Renderer** unterstützt.\
Die Volumenstreuung ist ein Mechanismus, der das Licht beim Eindringen in ein Objekt oder eine Oberfläche beeinflusst. Anstatt wie bei metallischen Oberflächen reflektiert zu werden, wird ein Teil des Lichts vom Material absorbiert und dann **in das Material gestreut**. Viele Materialien im echten Leben haben unterirdische Streuung wie Haut oder Wachs.

Unsere Subsurface-Effekt-Implementierung entspricht sehr genau den Echtzeit-Implementierungen anderer Game-Engines sowie anderen Offline-Renderern. So lassen sich ganz einfach streuende Texturen für die Verwendung in anderen Anwendungen erstellen.

![](../../assets/comparison-1.jpg){width="650px"}

Oben sehen Sie ein Beispiel mit dem bekannten Element Digital Emily 2. Vielen Dank an das USC Institute for Creative Technologies und Mitglieder des Wikihuman-Projekts, die es uns ermöglicht haben, unsere Renderings mit den Digital Emily 2-Assets zu demonstrieren.\
(Bitte beachten Sie, dass dieser Vergleich unter ähnlichen, aber nicht exakten Lichtverhältnissen durchgeführt wurde, was visuelle Unterschiede erklären kann.)

Führen Sie die folgenden Schritte aus, um in einem Projekt Untergrundstreuung hinzuzufügen:

1. Wechseln Sie zum Fenster **Anzeigeeinstellungen**, und **aktivieren** Sie die Einstellung **Untergrundstreuung**.
1. Hinzufügen eines **Streuungskanals** im aktuellen Textursatz
1. Verwenden Sie eine Füllebene oder **Malen in Weiß** im neuen Kanal, um **den Unteroberflächeneffekt im Viewport sichtbar zu machen**.

Eine ausführlichere Vorgehensweise finden Sie in der [Dokumentation zur Untergrundstreuung](../../features/subsurface-scattering/subsurface-scattering.md).

>[!NOTE]
>
> Um Subsurface Scattering im Echtzeit-Viewport zu unterstützen, müssen die **Shader** in den Projekten **aktualisiert** sein.\
> Informationen zu benutzerdefinierten Shadern finden Sie in der Dokumentation im **Hilfemenü**. Dort erfahren Sie, welche Änderungen im **Shader-API** vorgenommen wurden.

### Manipulatoren für Füllebenen

![](../../assets/changelog-manipulator.png)

Die Steuerelemente für Füllebenen wurden verbessert, um Manipulatoren mehr Möglichkeiten zu bieten. Es ist jetzt einfacher, Füllvorsprünge präzise zu platzieren und zu steuern.

Bei Verwendung der **UV-Projektion** wird ein Manipulator in der **2D-Ansicht** angezeigt:

* Durch Klicken auf **außerhalb von** wird der Manipulator **gedreht**.
* Durch Klicken auf das **Quadrat** an den **Rändern** wird es **skaliert/skaliert**.
* Durch Klicken auf **innerhalb von** wird der Manipulator **übersetzt**.
* Verwenden Sie **STRG**, um mehrere Ecken in **Symmetrie** zu beeinflussen.
* Verwenden Sie **UMSCHALT** zu **Einschränkung** für eine Transformation (Transformieren, Drehen oder Skalieren).\
  ![](../../assets/manipulator-uv.gif)

Bei Verwendung der **Dreiplanaren Projektion** erscheint ein Manipulator in der **3D-Ansicht** :

* Der gepunktete Würfel stellt die globale Projektion dar
* Verwenden Sie die Tastenkombination **W**, **E** oder **R**, um zwischen dem Modus **Übersetzen**, **Drehen** und **Skalieren** zu wechseln.
* Verwenden Sie den Tastaturbefehl **T**, um für den Manipulator zwischen der lokalen und der globalen Ausrichtung zu wechseln.
* Verwenden Sie **SHIFT**, um **die Transformation zu beschränken**.
* Die triplanare Kubikprojektion kann auch in den erweiterten Füllebeneneigenschaften geändert werden:\
  ![](../../assets/fill-properties-triplanar.png)\
  ![](../../assets/manipulator-3d-optim.gif)

Die kontextbezogene Symbolleiste am oberen Rand des Ansichtsfensters wird sich ebenfalls abhängig vom aktuellen Projektionsmodus anpassen und zusätzliche Werkzeuge und Steuerelemente bereitstellen:

![](../../assets/contextual-toolbar-manipulator.png)

Weitere Informationen finden Sie in der Dokumentation zur [Füllebene](../../painting/fill-projections/fill-projections.md).

### Nicht quadratische und nicht bearbeitungsfertige Unterstützung für Schablonen- und Projektionswerkzeug

![](../../assets/non-square-stencil.jpg)

Der Schablonenparameter und das Projektionswerkzeug wurden verbessert, um nicht quadratische Auflösungen und nicht bearbeitungsfreies Verhalten zu unterstützen.\
Der Standardparameter ist jetzt standardmäßig auf &quot;Nicht bestellen&quot; festgelegt. Dieser Parameter kann in den Werkzeugeigenschaften geändert werden:

![](../../assets/tilling-parameter-stencil.png)

Der Bearbeitungsmodus kann wie folgt eingestellt werden:

* **Keine Unterteilung** (Standard)
* **Horizontale Unterteilung**
* **Vertikale Kachelung**
* **H- und V-Kachelung** (altes Verhalten)

Dieser neue Parameter kann in einer Werkzeug- oder Pinselvorgabe gespeichert werden, was die Freigabe mit benutzerdefinierten Inhalten erleichtert.

>[!NOTE]
>
> * Das Projektionsverhältnis wird sich auch bei Substance-Dateien anpassen, die nicht quadratische Auflösungen ausgeben. Das Verhältnis wird direkt vom Ausgabeknoten aus berechnet.
> * Wenn mehrere Kanäle unterschiedliche Verhältnisse aufweisen, wird mit dem Projektionswerkzeug das erste gefundene Verhältnis auf alle anderen Kanäle angewendet.

### Import und Verwaltung von Kameras

![](../../assets/camera-import.png)

Es ist jetzt möglich, **benutzerdefinierte Kameras** in Substance Painter neben dem Gitterimport zu importieren.\
Kameras können im **3D-Ansichtsport** **ausgewählt werden, um sie zu durchsuchen** und **zum Rendern in Irak zu verwenden**.

Weitere Informationen finden Sie in der [Dokumentation zur Kameraverwaltung](../../interface/viewport/camera-management.md).

So **importieren Sie Kameras** in ein Projekt:

1. Exportieren des Gitters für das Projekt mit Kameras in derselben Datei (mit einem unterstützten Format wie FBX, Alembic oder glTF)
1. Wählen Sie die &quot;Kameraimport&quot;-Einstellungen im [neuen Projektfenster](../../getting-started/project-creation.md) (oder [Projektkonfiguration](../../interface/project-configuration.md)) aus.\
   ![](../../assets/new-project-cameras.png)
1. Wechseln Sie mit der Dropdown-Liste im Ansichtsfenster oder mithilfe der Einstellungen in [Anzeigeeinstellungen](../../interface/display-settings/camera-settings.md) zur gewünschten Kamera.\
   ![](../../assets/cmaera-select-viewport.png)

Die Kameraeinstellungen im Fenster Anzeigeeinstellungen wurden erweitert, um die Eigenschaften der Kamera zu steuern.\
Es ist möglich, **zwischen Kameras zu wechseln**. Weitere Informationen finden Sie in den Eigenschaften **ratio** und **lock**, um eine Änderung zu vermeiden. Mit einer Wiederherstellungsschaltfläche kann die Kamera auf ihre ursprünglichen Werte zurückgesetzt werden.

![](../../assets/camera-properties-2.png)

Der Kamerarahmen (und sein Tor) wird ebenfalls berücksichtigt, sodass es möglich ist, über einen ganz bestimmten Blickwinkel zu sehen und zu malen. Der Rahmen und das Gate werden über dem 3D-Viewport angezeigt, und seine Deckkraft kann in den **Viewport-Einstellungen** im Fenster [Anzeigeeinstellungen](../../interface/display-settings/camera-settings.md) gesteuert werden:

![](../../assets/camera-gate.png)

### Verbesserungen des Ebenenstapelverhaltens

* **Ziehen Sie Materialien und Smart-Materialien per Drag &amp; Drop auf die ID-Map :**\
  Das Ziehen und Ablegen von Inhalten aus dem Regal in den Viewport wurde verbessert. Durch Drücken von **STRG** beim Ziehen und Ablegen eines Materials können Sie jetzt die ID-Farbe auswählen, die als Maske verwendet wird.\
  Eine schwarze Maske mit einem Farbauswahleffekt wird zu der neuen Ebene hinzugefügt, die im Ebenenstapel erstellt wurde. Wenn dasselbe Material per Drag-and-Drop auf eine andere ID-Farbe platziert wird, wird die bereits vorhandene Ebene aktualisiert und die ID-Farben werden kombiniert.\
  ![](../../assets/id-drop.gif)
* **Bildlauf durch Ziehen und Ablegen des Ebenenstapels:**\
  Wenn Sie Ebenen um den Ebenenstapel ziehen, wird ein kleines Fenster angezeigt.\
  Wenn eine Ressource oder eine Ebene an den Rändern des Ebenenstapelfensters gezogen wird, wird automatisch ein Bildlauf für den Inhalt durchgeführt.\
  ![](../../assets/layer-drag.gif)

### glTF- und Alembic-Netzimport

![](../../assets/logo-mesh-import.png)

Neue Dateiformate werden jetzt für den Import von Gittern und das Erstellen neuer Projekte unterstützt:

* **glTF** : Dieses Format war bereits beim Exportieren von Texturen verfügbar und kann jetzt während des Imports verwendet werden. Wenn eine glTF-Datei Texturen enthält, werden diese importiert und in den Ebenenstapel eingefügt (für den Metall-/Raueit-Workflow).
* **Alembic** : Dieses Format ist in der VFX-/Animationsbranche weit verbreitet, um Meshes zu übertragen.

>[!NOTE]
>
> Substance Painter bietet keine Möglichkeit, zu steuern, welcher Animationsframe derzeit importiert werden soll.\
> Dies bedeutet, dass beim Exportieren einer Alembic-Datei der Referenzrahmen, der zum Malen auf dem Asset verwendet werden soll, bereits festgelegt sein muss.

### Verbesserungen an der Substance-Integration

![](../../assets/integration.png)

Die Substance-Integration in Substance Painter wurde mit lange erwarteten Anfragen verbessert:

* <b>Sichtbar, wenn:</b>\
  Das &quot;Visible if&quot; ist eine großartige Funktion des Substance-Dateiformats, das es ermöglicht, Parameter auf Basis von Bedingungen auszublenden.\
  Diese Funktion bietet eine klarere Liste von Parametern und Kontexteinstellungen, sodass Materialien und Filter insgesamt einfacher zu verwenden sind.\
  Weitere Informationen finden Sie in der Dokumentation zu [Substance Designern](https://experienceleague.adobe.com/en/docs/substance-3d-designer/home).\
  ![](../../assets/visible-if.gif)
* **Substance-Vorgaben** Substance-Vorgaben sind eine einfache Möglichkeit, erweiterte Anpassungen und Variationen von Materialien bereitzustellen. Viele Materialien auf [Substance Source](https://source.allegorithmic.com) verfügen über Vorgaben. Probieren Sie es aus!\
  Wenn eine Substance-Datei eine oder mehrere Vorgaben enthält, ist ein neues Dropdown-Menü in der Parameterliste verfügbar. Wählen Sie die Vorgabe aus, die zum Aktualisieren der Parameter angewendet werden soll.\
  ![](../../assets/presets.png)
* **Substance-Attribute**\
  Substance-Attribute werden jetzt in der Benutzeroberfläche angezeigt, sodass Informationen zu einer bestimmten Datei leichter abgerufen werden können.\
  Attribute können an zwei verschiedenen Orten angezeigt werden: über den Parametern im Eigenschaftenfenster oder durch Klicken mit der rechten Maustaste auf ein Element in der Ablage.\
  ![](../../assets/attributes.png) ![](../../assets/attributes-shelf.png)

### Neues Beispielprojekt &quot;Jade Toad&quot;

![](../../assets/toad-samle.jpg)

Ein neues Beispielprojekt mit dem Namen &quot;**JadeToad**&quot; ist jetzt im Substance Painter enthalten. Für dieses Beispielprojekt ist der Effekt **Unterflächenscattering** standardmäßig aktiviert.\
Verwenden Sie zum Suchen des Projekts die Datei **Datei** > **Beispiel öffnen...**-Menüeintrag.

## Versionshinweise

### 2018.2.3

(Release 25. September 2018)

**&#x200B;**&#x200B;Fest:**&#x200B;**

* [2D-Ansicht] Die 2D-Ansicht wird bei der Erstellung eines neuen Projekts mit einigen Gittern unterbrochen.
* [Absturz] Das Umschalten von der UV-Projektion- auf die dreiplanare Projektion führt zu einem Absturz
* [RayCollider] Mehrere Abstürze durch &quot;RayCollider&quot;
* [Werkzeug] Beim Wechseln von Ebenen gehen die geänderten Pinseleigenschaften verloren
* Pinseleinstellungen werden beim Wechsel zum Radierer zurückgesetzt

**Bekannte Probleme:**

* Einfrieren der Berechnung auf AMD VEGA-GPUs
* Problem mit Huion-Tablets mit Tastaturbefehlen unter Windows

### 2018.2.2

(Release 11. September 2018)

**Hinzugefügt:**

* Zusammenfassung: Hotfix mit Inhaltsaktualisierung, neuen Skriptfunktionen und der Möglichkeit, die automatische Aktualisierung zu deaktivieren
* [Inhalt]&#x200B;[Regal] Hinzufügen einer Skin-Regalvorgabe
* [Inhalt]&#x200B;[Regal] Konvertierung von 19 Hautnormalen in Materialien zur Untergrundstreuung
* [Scripting] Erstellen einer Projektvorlage aus einem geöffneten Projekt
* [Scripting] Abrufen/Festlegen von Exporteinstellungen eines geöffneten Projekts
* [Updates] Deaktivieren des Popups &quot;Automatische Aktualisierung&quot; in den Einstellungen und der Umgebungsvariablen
* [Updates] Anzeige erst in der nächsten Version des veralteten Wartungs-Popup

**Fest:**

* [Kamera] Falscher Zoom durch Wechsel von orthografischer zur Perspektive
* [Anzeige] Einige Maps werden linear anstelle von sRGB angezeigt
* [Viewports] Der Gitterfokus verhält sich nicht ordnungsgemäß.
* [2D-Ansicht] Projekt mit kaputter Kamera enthält verschwindende UVs-Schalen
* [SSS]&#x200B;[QuickInfo] QuickInfos für die unterirdische Streuung werden im Protokoll angezeigt
* Einige Projekte können nicht in 2018.2 geöffnet werden und die Fehlermeldung kann kein Null-Substance-Paket speichern
* [Maske] Die Farbe des Malwerkzeugs kann in einigen Fällen beim Arbeiten in einer Maske hängen bleiben
* [Material] Karten werden in bestimmten Situationen nicht angezeigt
* [Proj]&#x200B;[Tools] Manipulator aktiv mit einem Generator
* [Substance] Fehlende Substance-Parametergruppen
* [Skripterstellung] Falscher Software-Name in der Dokumentation
* [UDIMs] Keine Informationen im Protokoll über UVs-Schalen auf mehreren UVs-Kacheln

**Bekannte Probleme:**

* Einfrieren der Berechnung auf AMD VEGA-GPUs
* Problem mit Huion-Tablets mit Tastaturbefehlen unter Windows

### 2018.2.1

(veröffentlicht am 3. August 2018)

**Fest:**

* Fehlende Parameter für die Teilflächen-Streuungs-Shader beim Aktualisieren von Projekten

**Bekannte Probleme:**

* Einfrieren der Berechnung auf AMD VEGA-GPUs
* Problem mit Huion-Tablets mit Tastaturbefehlen unter Windows

### 2018.2

(Release 2. August 2018)

**Hinzugefügt:**

* Zusammenfassung: Sommerversion, Streuung auf Untergrund Unterstützung, Verbesserungen bei Projektion und Füllung, Kameraimport und -auswahl, Alembic-/glTF-Unterstützung, Drag-and-Drop-Funktionen für ID-Maps, verbesserte Unterstützung für Substance-Formate und neue Inhalte
* [SSS]&#x200B;[Viewport]&#x200B;[Iray] Generische Untergrundstreuung
* [SSS] Synchronisierungsparameter für MDL und Untergrundstreuung
* [SSS] Es wurde ein neuer Graustufenkanal mit dem Namen &quot;Streuung&quot; hinzugefügt.
* [SSS]&#x200B;[Schattierungseinstellungen] Streuungstyp-Parameter für Volumenstreuung (Haut oder transluzent)
* [SSS]&#x200B;[Schattierungseinstellungen] Streuungsmaßstabsparameter für Untergrundstreuung
* [SSS]&#x200B;[Schattierungseinstellungen] Streuender Farbparameter für Untergrundstreuung
* [SSS]&#x200B;[Anzeigeeinstellungen] Streuung Abtastanzahl für Untergrundstreuung
* [Shader]&#x200B;[Iray] Integrieren Sie die unterirdische Streuungs-MDL für Iray
* [Shader] Shader-Update über den Ressourcen-Updater
* [Shader] API und Dokumentation für Änderungsprotokoll aktualisieren
* [Werkzeugeigenschaften]&#x200B;[Proj] Neue Parameter für die triplanare Projektion
* [Viewport]&#x200B;[Proj] Steuern Sie die Eigenschaften der Füllebene in der 3D-Ansicht direkt mit Manipulatoren (triplanare Projektion).
* [Shortcuts]&#x200B;[Proj] Neue Shortcuts Q, W, E, R, T für triplanare Projektionsmanipulatoren
* [Viewport]&#x200B;[Proj] Steuern Sie die Eigenschaften der Füllebene in der 2D-Ansicht direkt mit den Manipulatoren (UV-Projektion).
* [Shortcuts]&#x200B;[Proj] Neuer Shortcut Q für UV-Projektion-Manipulatoren
* [Contextual Toolbar]&#x200B;[Proj] Steuern von triplanaren Projektionsmanipulatoren
* [Kontextsymbolleiste]&#x200B;[Proj] Manipulatoren für die UV-Projektion steuern
* [Werkzeugeigenschaften] Deaktivieren der Texturkachelung mit Projektions- und Schablonenwerkzeug
* [Schablone] Verwenden von nicht quadratischen Bildern mit dem Projektionswerkzeug/der Schablone
* [Schablone] Steuerung des Kachelmodus im Eigenschaftenfenster zulassen
* [Schablone] Der Zoom ist nicht auf einer nicht gekachelten Schablone zentriert
* [Kameras] Importieren von Kameras aus Maya, Max, Blender, Modo, DAE
* [Kameras]&#x200B;[Viewport] Wählen und steuern Sie die importierten Kameras im Viewport
* [Kameras]&#x200B;[Iray] Auswählen und Steuern von importierten Kameras in Iray
* [Kameras]&#x200B;[UI]&#x200B;[Neues Projekt]&#x200B;[Projektkonfiguration] &quot;Kameras importieren&quot; ist standardmäßig aktiviert.
* [Kameras]&#x200B;[Tastaturbefehle] Fügen Sie die Tastaturbefehle &quot;&lt;&quot; und &quot;>&quot; hinzu, um zwischen den Kameras zu wechseln.
* [Kameras]&#x200B;[Viewport] Frame im Viewport hinzufügen
* [Kameras]&#x200B;[Viewport-Einstellungen] Steuerung der Frame-Deckkraft
* [Kameras]&#x200B;[Kameraeinstellungen] Maximale Brennweite bei 500 mm
* [Kameras]&#x200B;[Kameraeinstellungen] Belichtungsverhältnis
* [Kameras]&#x200B;[Kameraeinstellungen] Fügen Sie eine Sperroption hinzu
* [Kameras]&#x200B;[Kameraeinstellungen] Hinzufügen einer Wiederherstellungsoption
* [Kameras]&#x200B;[Kameraeinstellungen] Attribut für den Fokusabstand hinzufügen
* [glTF] Import einer glTF-Datei
* [glTF] Umgebungskarte für die Verdeckung importieren
* [Alembic] Importieren Sie Alembic 1-Rahmen mit statischer Geometrie
* [Shelf] Ziehen Sie Materialien per Drag &amp; Drop direkt auf das Gitter, indem Sie ID-Zuordnungen mit einem Modifizierer (STRG/Befehlstaste) verwenden.
* [Ebenenstapel] Automatische Erstellung von ID-Masken durch Ziehen und Ablegen von Materialien auf einem Gitter mit ID-Maps
* [Ebenenstapel] Automatischer Bildlauf von Ebenen per Drag &amp; Drop über den Ebenenstapel
* [UI]&#x200B;[Werkzeugeigenschaften] Zeigt die Vorgabe des Substance an.
* [UI]&#x200B;[Hilfemenü] Verbesserung des Hilfemenüs
* [UI]&#x200B;[Neues Projekt]&#x200B;[Projektkonfiguration] Reorganisation des Fensters
* [UI]&#x200B;[Neues Projekt]&#x200B;[Projektkonfiguration] Ersetzen Sie &quot;Mesh&quot; durch &quot;File&quot;.
* [UI]&#x200B;[Substance] Anzeigen von Substance-Attributen in der Benutzeroberfläche
* [Tastaturbefehle] &quot;F4&quot; wechselt zwischen 2D- und 3D-Ansicht
* [Tastaturbefehle] Neue Tastaturbefehle für Umschaltschablone &quot;N&quot; und Schnellmaske &quot;U&quot;
* [Substance-Integration] Berücksichtigung von &quot;visible if&quot;-Anweisungen in den Substance-Parametern
* [Viewport] Schatten müssen nach dem Verschieben der Kamera nicht berechnet werden.
* [Inhalt] Aktualisieren von MeetMat mit importierten Kameras
* [Inhalt] Muster mit aktivierter Volumenstreuung hinzufügen - JadeToad
* [Inhalt] Neue PBR-Projektvorlage mit aktivierter Untergrundstreuung hinzufügen
* [Inhalt] Exportvorgaben wurden aktualisiert, um einen neuen Streuungskanal hinzuzufügen
* [Content]&#x200B;[Shelf] Zusätzliche Untergrund-Streuunterstützung für: pbr-metal-rau, pbr-metal-rau-alpha-test, pbr-coated, pbr-spec-gloss
* [Content]&#x200B;[Shelf] Hinzugefügter Streuungskanal zu 5 intelligenten Materialien (Marmor und Skins)
* [Inhalt]&#x200B;[Regal] 1 neues Jadematerial
* [Inhalt]&#x200B;[Regal] 1 neues Wachsmaterial

**Fest:**

* [CMD] Verschiedene Ergebnisse über dieselbe Befehlszeile mit unterschiedlichen Versionen
* [TDR] Wenn TdrLevel eingerichtet ist, sind keine Fehler im Protokoll vorhanden.
* [Baker] Umgebungskarte der Verdeckung wird gespiegelt
* [ID Map] Absturz beim Kommissionieren außerhalb des Bereichs 0-1
* [Iray] Absturz beim Wechseln der Textursätze und Zurückkehren zum Malmodus
* [Viewport] Synchronisieren von Ablagebereichen zwischen Viewports für Drag &amp; Drop
* [Engine] Moire-Artefakt beim Kacheln von Füllebenen oder Malen eines kleinen Pinsels
* [Lizenz] Prüfung auf fehlerhafte Softwareversion des Lizenzdiensts
* [Lizenz] Überarbeiten Sie die Art und Weise, wie wir die Authentifizierung verarbeiten
* [API] Rufen Sie das `onNewProjectCreated`-Skript-API-Ereignis auf, selbst wenn Sie mit einer Vorlage erstellen.
* [Shader] Kompilierter Shader wird nicht aus dem Cache geladen, wenn die Shader-Datei nicht kompiliert wird
* [Shelf] Beim Exportieren der HDR-Datei aus dem Shelf wird eine Datei mit eingespannten Werten ausgegeben
* [Exportieren] EXR-Exportklammern RGB Farbwerte zwischen 0-1
* [Inhalt] Verfahrensrauschen &quot;3D Perlin Noise Fractal&quot; ist verpixelt

**Bekannte Probleme:**

* Einfrieren der Berechnung auf AMD VEGA-GPUs
* Problem mit Huion-Tablets mit Tastaturbefehlen unter Windows
