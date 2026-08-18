---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/release-notes/old-versions/version-2-5.html"
breadcrumb-title: ''
description: Lesen Sie die Versionshinweise für Substance 3D Painter 2.5, um mehr über neue Funktionen, Verbesserungen und Fehlerbehebungen zu erfahren.
helpx_creative_field: ""
helpx_description: Painter > Release notes > Old versions > Version 2.5
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Version 2.5
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '1699'
ht-degree: 0%

---


# Version 2.5

**Substance Painter 2.5** bietet viele neue Funktionen: von der Unterstützung der Deckkraft in den Pinseleinstellungen (zusätzlich zum Fluss) bis hin zur Möglichkeit, zusätzliche Karten in 8K und vieles mehr zu backen.

Freigabedatum: *21. Februar 2017*

## Wichtigste Funktionen

### Neue Pinseldeckkraft

![](../../assets/brush-combined.gif){width="650px"}

In den **Pinselparametern** beim Malen im Substance Painter gibt es jetzt eine neue Einstellung, die **Deckkraft** ist.\
Die **Deckkraft** steuern die **Gesamtintensität eines Pinselstrichs**, im Gegensatz zur **Fluss**-Einstellung, die die Intensität von **jedem einzelnen Stempel** innerhalb eines Pinselstrichs steuert. Dies bedeutet, dass es jetzt möglich ist, denselben Bereich &quot;**&quot; zu malen und neu zu malen, ohne überlappende Werte zu erstellen.** Setze dazu den Durchfluss auf 100 und den Deckkraftwert auf die gewünschte Intensität. Aufgrund der Funktionsweise der Deckkraft ist es nicht möglich, diese mit dem Stiftdruck zu verknüpfen. Für diese Art von Kontrolle ist der Fluss immer noch die beste Wahl.

Wir haben außerdem einen **neuen Modifizierer** neben diesem neuen Parameter hinzugefügt, der standardmäßig auf dem Schlüssel **&quot;A&quot;** vorhanden ist. Durch Drücken dieser Taste kann **den vorherigen Pinselstrich** fortsetzen, anstatt einen neuen Pinselstrich zu erstellen. Dies bedeutet, dass Sie eine einheitliche Farbe mit der gewünschten Deckkraft malen können, während Sie die Farbe möglicherweise beibehalten, um die Kamera zu bewegen. Ein weiteres Beispiel wäre, mit der Kopie fortzufahren, die Sie mit dem Kopierwerkzeug erstellt haben.

![](../../assets/stroke-opacity-parameter.png)

### Neues Backen bei 8K und nicht quadratischer Auflösung

![](../../assets/baking-250-8k.png)

Der Bäcker wurde verbessert, um Auflösungen von bis zu **8192x8192** (8K plus Anti-Aliasing) zu unterstützen, was bedeutet, dass Sie jetzt mit den zusätzlichen Maps bei 8K im Verhältnis 1:1 exportieren können.\
Wir haben auch Unterstützung für **nicht quadratische** Auflösungen hinzugefügt. Es ist jetzt möglich, beispielsweise eine Textur von **4096x2048** zu backen. Klicken Sie dazu einfach auf das &quot;**Schloss**&quot;-Symbol neben der Dropdown-Liste, um die Auflösung auszuwählen.

### Neue Unterstützung für Farbprofile im Ansichtsfenster

![](../../assets/lut-example.jpg)

Wir haben die Unterstützung von **LUT** (Texturen) hinzugefügt, um das Rendern des **Ansichtsports** im Substance Painter zu steuern. Um ein Profil anzuwenden, aktivieren Sie einfach die Einstellung &quot;**Farbprofil**&quot; im Fenster &quot;**Anzeigeeinstellungen**&quot; und laden Sie die LUT in den dedizierten Steckplatz. Es funktioniert sowohl mit dem **OpenGL**-Viewport (Malen) als auch mit dem **IRay**-Renderer. Einige Beispiele sind standardmäßig von den allgemeinen **Kameravorgaben** bis zu mehr **Künstlerischen Effekten** verfügbar. Weitere Informationen finden Sie auf der entsprechenden Seite der Dokumentation : [Farbprofil](../../features/post-processing/color-profile.md)

### Neue Substance-Engine, kompatibel mit Substance Designer 6

![](../../assets/font-shelf.png)

Wir haben die Unterstützung für **Substance Designer 6** hinzugefügt. Das bedeutet, dass mit **SD6** erstellte Ressourcen geöffnet und in **Substance Painter 2.5** verwendet werden können!\
Ein gutes Beispiel ist die Möglichkeit, den **neuen Textknoten** von SD6 zu verwenden und in eine Substanz zu integrieren. Auf diese Weise ist es möglich, **dynamischen Text** zu erstellen und direkt zu malen, ohne die Anwendung verlassen zu müssen. **Wir haben standardmäßig 10 Schriftarten** mit jeweils einem anderen Stil zur Abdeckung der häufigsten Verwendung eingeschlossen. Sie finden sie im Abschnitt &quot;**prozedurale**&quot; der **Ablage**.

![](../../assets/text-sp250-optim.gif){width="400px"}

### Neuer Inhalt im Regal

![](../../assets/new-filters.jpg)

Neben einigen Korrekturen und Verbesserungen am neuen Regal haben wir auch einige **neue Filter** hinzugefügt, um das Malen und die Texturierung zu verbessern. Außerdem **wurde das Verhalten des bereits vorhandenen Filters** verbessert (z. B. der &quot;**HSL**&quot;). Außerdem haben wir beim Erstellen von **neuen Projekten** neue **Vorlagen** hinzugefügt (z. B. **Unity 5** und **Unreal Engine 4**).

### Neue Skriptverbesserungen mit Unterstützung für benutzerdefinierte Shader-Benutzeroberfläche

![](../../assets/ui-shader.jpg)

Mit dieser Version haben wir einen Weg zu **Skript und Kontrolle** der **Shader-Parameter** hinzugefügt. Wir haben auch die Unterstützung für die Verwendung einer **benutzerdefinierten Benutzeroberfläche** anstelle der Standardbenutzeroberfläche hinzugefügt, wodurch viele neue Möglichkeiten eröffnet werden, z. B. **animierter Shader**.\
Weitere Informationen finden Sie in der Skriptdokumentation, die im Hilfemenü der Anwendung verfügbar ist.

## Tutorial

Die neuen Hauptfunktionen sind in unserem neuesten Twitch-Stream beschrieben:

## Versionshinweise

### 2.5.3

(Release 15. März 2017)

**Fest:**

* [Baker] Absturz beim Backen mit bestimmten Netzen

**Bekanntes Problem :**

* [Mac] Partikel können in einigen Fällen Texturbeschädigungen verursachen

### 2.5.2

(Release 14. März 2017)

**Fest:**

* [Tool] Wacom-Tablet funktionieren unter Linux nicht
* [Werkzeug] Schwarze Artefakte bei Verwendung des Verwischen-Werkzeugs
* [Bäcker] Backen schlägt fehl, wenn &quot;Nach Name abgleichen&quot; mit einem Käfig verwendet wird
* [Bäcker] Umgebungs-Verdeckung funktioniert nur bei Backen mit Normalmap nicht
* [Shelf] Generische Filter behandeln Alpha nicht ordnungsgemäß (Kontrast/Luminanz, Hochpass usw.)
* [Viewport] Leistungsproblem beim Laden eines Projekts mit aktivierten Schatten
* [Viewport] Dithering-Problem in der 3D-Ansicht auf MacOS
* [Viewport] Partikelvorschauen werden bei aktiviertem Farbprofil falsch angezeigt
* [Iray] Absturz beim Zurückwechseln des Projekts zu OpenGL, wenn Iray nicht initialisiert werden konnte
* [IRay] Beim Rendern von SpecGloss shader/mdl wird die Glossiness ignoriert.
* [Shader] Spec/Gloss Shader stimmt nicht mit Iray und SD überein
* [Shader] sRGB-Konvertierung unterscheidet sich von der linearen in die sRGB-LUT-Konvertierung
* [Shader] Falsches Rendering beim Laden eines Projekts mit veralteten Shadern
* [Shader] &quot;pbr-coated&quot; Shader funktioniert nicht mehr
* [Exportieren] Einige Kanäle werden weiterhin exportiert, auch wenn sie nicht im Textursatz vorhanden sind
* [Ebenen] Der Mischmodus &quot;Inverse Details der normalen Karte&quot; funktioniert nicht auf Graustufenkanälen
* [UI] Problem beim &quot;Farbauswahlfenster&quot; mit HDPI-Monitor und Anzeigezoom bei 150 %

**Bekanntes Problem :**

* [Mac] Partikel können in einigen Fällen Texturbeschädigungen verursachen

### 2.5.1

(Release 27. Februar 2017)

**Fest:**

* [Mac] Wacom-Tablet-Eingang in 3D- und 2D-Ansicht defekt
* [Bäcker] Die Zuordnung nach Namen funktioniert nicht mehr
* [Bäcker] Die Einstellung &quot;Durchschnittliche Normale&quot; funktioniert nicht mehr
* [Iray] Falsches Rendering mit fehlender gebackenen Normalmap
* [Iray] Farbprofile verhalten sich anders als beim OpenGL-Renderer
* [Iran] Exportieren von Rendering als Bitmap beinhaltet keine Farbprofilkorrektur
* [Substance] Materialfilter funktionieren nicht mehr
* [Werkzeug] Die Konturdeckkraft wird nicht in den Pinselvorgaben gespeichert
* [Tool] Kopierpinsel-UV-Ausrichtung funktioniert nicht mehr
* [Versatz] Beim Exportieren als Ganzzahl sollte der Exportkanal in 0,5 zentriert sein.
* [Vorlage] Absoluter Pfad wird in Vorlagen gespeichert.
* [TextureSet] Die Kanaltextur bleibt nach dem Entfernen des Kanals bestehen.

**Bekanntes Problem :**

* [Linux] Die Eingabe von Wacom-Tablets funktioniert nicht in der 3D- und 2D-Ansicht
* [Mac] Partikel können in einigen Fällen Texturbeschädigungen verursachen
* [Exportieren] In sehr seltenen Fällen können auf AMD-GPUs schwarze Rechtecke erscheinen

### 2.5.0

(Release 21. Februar 2017)

**Hinzugefügt:**

* Unterstützung für AMD Radeon Pro- und AMD FirePro-GPUs
* [Werkzeug] Unterstützung für Konturdeckkraft hinzufügen
* [Werkzeug] Fügen Sie einen Modifizierer hinzu, mit dem Sie den letzten Pinselstrich fortsetzen können
* [Iray] Update zur Unterstützung von Pascal-GPUs
* [Viewport] Hinzufügen von Unterstützung für Farbprofile (LUT)
* [Substance] Integration eines neuen Frameworks (SD6-Engine)
* [UI] Liste der &quot;zuletzt verwendeten Dateien&quot; im Menü &quot;Datei&quot; vergrößern
* [Importieren] Verwenden Sie die Kategorie aus Stoffen, um das Präfix im Dialogfeld &quot;Importieren&quot; auszufüllen.
* [Bäcker] Backen von 8K-Texturen zulassen
* [Bäcker] Nicht quadratische Auflösungen backen
* [Bäcker] Verbessern Sie den Speicherverbrauch beim Backen von schweren High-Poly-Netzen
* [Shelf] Sperren Sie Regale (und Projekte), um die gleichzeitige Bearbeitung zu verhindern und Beschädigungen zu vermeiden
* [Shelf] Lesen Sie Kategorie und Schlüsselwörter von Stoffen, um sie für die Filterung zu verwenden
* [Shelf] Ausschließen von Ressourcen aus dem Ergebnis einer Suchabfrage zulassen
* [Shelf] Verbesserte Berechnung der Miniaturansichten
* [Shelf] Einbetten von Vorgaben in Projekte zulassen
* [Shelf] Schnelles Reduzieren/Erweitern der Strukturansicht mit UMSCHALT
* [Shelf] Speichern von Miniaturansichten, wenn Assets schreibgeschützt sind (lokaler Cache)
* [Shelf] Neuer Inhalt : neue Filter (Transformieren, Spiegeln, triplanar usw.)
* [Shelf] Neuer Inhalt : neue LUTs-Profile (klassisch und künstlerisch, z. B. Film Noir, Vintage usw.)
* [Shelf] Neuer Inhalt : 10 neue Font-Substance zur schnellen Generierung benutzerdefinierter Texte
* [Shelf] Neue Vorlagen : Unity 5 und Unreal Engine 4
* [Shelf] Verbesserter HSL-Filter, um künstlerfreundlicher zu sein
* [Shader] Unterstützung für Specular level-Kanal in PBR-Shadern hinzufügen
* [Shader] Unterstützung für Dithering in Alpha Test Shader hinzufügen
* [Shader] Unterstützung für Parallax Verdeckung Mapping in PBR Shadern hinzufügen
* [Shader] Definieren einer benutzerdefinierten Benutzeroberfläche für Shader-Parameter zulassen
* [MatteLayering] Erstellen eines neuen Maskenkanals für den Workflow der Materialschichtung
* [Skripterstellung] Metadaten in einem SP-Projekt schreiben dürfen
* [Scripting] Export mit einer bestimmten Exportvorgabe zulassen
* [Scripting] Ermöglicht das Abrufen von Shader-Parametern als JSON.
* [Scripting] Unterstützung für WebSocket-Verbindungen hinzufügen
* [Scripting] Fügen Sie die Möglichkeit hinzu, Shader-Instanzen zu laden
* [Scripting] Fügen Sie die Möglichkeit hinzu, ein neues Projekt zu erstellen
* [Scripting] Ermöglicht das Abrufen der URL des in ein Projekt importierten Gitters.
* [Skripterstellung] Nicht quadratisches Backen zulassen
* [Scripting] Berichtsfehler beim Festlegen von Daten über die Scripting-API
* [Substance] Benutzerdaten-Tag hinzufügen, um Normalen-Map-Format anzugeben

**Fest:**

* Absturz beim Aufnehmen von Farbe mit Substanzen
* Absturz beim Laden eines Nicht-RGBA32f-Bildes als Umgebungszuordnung
* Absturz beim Malen auf AMD-GPUs
* [Mesh] Der OBJ-Import erkennt Materialien ohne MTL-Datei nicht.
* [Mesh] Die Generierung des Satznamens für UDIM-Texturen kann in einigen Meshes falsch sein
* [UI] Schaltfläche &quot;Rückgängig/Wiederholen&quot; in Anzeigeeinstellung &quot;Fokus stehlen&quot; und Mausbildlauf anhalten
* [UI] Einige Beschriftungen werden in High-DPI falsch beschnitten
* [Ebene] Der Modus &quot;Ersetzen&quot; für den Maleffekt hat ein falsches Verhalten auf der Maske
* [Ebene] Ungültiges Verhalten des Mischmodus &quot;Subtrahieren&quot; mit Alpha
* [Tool] Die Pinselgröße wird in der 2D-Ansicht beim Malen auf UV-Rahmen enorm
* [Tool] Geraden, die ausgerichtet sind, verhalten sich ungleichmäßig mit High-DPI.
* [Werkzeug] Die Auflösung der Schablone ist manchmal falsch
* [Bäcker] Die Werte für &quot;Max. Okklusionsentfernung&quot; werden geklemmt, wenn &quot;relativ zum Begrenzungsrahmen&quot; &quot;Aus&quot; ist.
* [Shader] Die Kanaldefinitionen für Stapel und automatische Parameter stimmen nicht überein
* [3D-Ansicht] Inkonsistente Anzeige des normalen Kanals abhängig von der Projekteinstellung
* [Viewport] Einige Normalmaps haben festgeklemmte Werte, die als Artefakte angezeigt werden
* [Viewport] Nacheffekte sind standardmäßig immer deaktiviert
* [Export] Die normale Mischeinstellung ist falsch, wenn der normale Kanal fehlt
* [Exportieren] Falsche Texturgenerierung in einigen Fällen auf AMD-GPUs
* [Export] Shader-Parameter werden nicht ordnungsgemäß exportiert, wenn sie sich in einer Gruppe befinden
* [Export] Bearbeiten einer Exportvorgabe in einer benutzerdefinierten Ablage gibt einen Protokollfehler aus
* [Shelf] Die Strukturansichtsfilterung stimmt nicht genau mit dem Ordnernamen überein
* [Shelf] Das Umbenennen einer Shelf-Vorgabe ist schwer zu lesen
* [Shelf] Die im Shelf importierte Shader-Ressource bleibt nach dem Neustart nicht erhalten
* [Shelf] Inhalt : Die Vorgabe für das Schweißwerkzeug fehlt
* [Shelf] Inhalt : Tile Generator funktioniert nicht richtig
* [Shelf] Inhalt : Falsche Maske auf Gummireifen korrigiert Schmutziges Smart-Material
* [Shelf] Inhalt : Falscher Gruppenname auf Material der Ledertasche wurde behoben
* [Iray] Die Hälfte der Maschen fehlt in Iray
* [Linux] Absturz beim Ziehen einer Ressource über die 3D-Ansicht
* [Mac] Voreinstellungen werden bei jedem Start in Sierra zurückgesetzt

**Bekanntes Problem :**

* [Exportieren] In sehr seltenen Fällen können auf AMD-GPUs schwarze Rechtecke erscheinen
* [Iray] Farbprofile können sich manchmal ungerade verhalten.
