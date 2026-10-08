---
breadcrumb-title: ""
description: Lesen Sie die Versionshinweise für Substance 3D Painter 2017.3 , um mehr über neue Funktionen, Verbesserungen und Fehlerbehebungen zu erfahren.
title: Version 2017.3
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '1588'
ht-degree: 0%
---

# Version 2017.3

**Substance Painter 2017.3** konzentriert sich auf neue erweiterte Exportvoreinstellungen mit Unterstützung von **Adobe Project Felix** und dem offenen Format **glTF**. Diese neue Version konzentriert sich auch auf das Benutzererlebnis, indem die Benutzeroberfläche verbessert und ein automatisch gespeichertes Plug-in hinzugefügt wird.

Freigabedatum: *28. September 2017*

## Wichtigste Funktionen

### Adobe Standard Material-Exportvorgabe

![](../../assets/adobe-dimension-meetmat.jpg)

Einer der neuen Exporter, die in dieser Version enthalten sind, ist die Unterstützung des Adobe Standard Materials, das mit Adobe Dimension (früher Adobe Project Felix) verwendet werden kann. Sie können den Szene-Mesh und seine Texturen exportieren, um sie mit einem Klick in Project Felix zu importieren. Um darauf zuzugreifen, wählen Sie einfach &quot;**Adobe Standard Material**&quot; im Fenster &quot;Texturen exportieren&quot; aus. Weitere Informationen finden Sie unter: [http://www.adobe.com/products/dimension.html](https://www.adobe.com/products/dimension.html)

Sie können auch unseren Blogpost darüber lesen: <https://www.allegorithmic.com/blog/new-dimension-substance-ecosystem>

### glTF 2.0-Exportvorgabe

![](../../assets/gltf-export.jpg)

Wir haben außerdem Unterstützung für das Dateiformat **glTF** mit dem Export des Meshs **Szene** und der Texturen **PBR** (metallic/Rauheit) hinzugefügt. Um darauf zuzugreifen, wählen Sie im Fenster &quot;Exporteinstellungen&quot; einfach &quot;**glTF PBR Metal Rauheit**&quot; aus. **glTF** ist ein Open-Source-Dateiformat, das von der Gruppe Khronos geleitet wird. Sie können Ihre glTF-Datei in **Windows 10** anzeigen oder einfach einen WebGL-Viewer wie [**Babylon**](http://sandbox.babylonjs.com/) verwenden.

Weitere Informationen finden Sie unter: <https://github.com/KhronosGroup/glTF>

### Plug-in für automatische Speicherung

![](../../assets/autosave-details.png)

In dieser Version wurde auch ein neues Plug-In hinzugefügt, mit dem **Sicherungen** des derzeit geöffneten Projekts erstellt werden können. Es wird eine Sicherungsdatei auf der Seite des derzeit geöffneten Projekts erstellt.\
Aus diesem Grund haben wir auch den Eintrag &quot;**Als Kopie speichern**&quot; im Menü &quot;Datei&quot; hinzugefügt. Das **automatische Speichern** kann gestoppt werden, indem das Plug-In selbst deaktiviert wird. Auf die **Einstellungen** kann über den Konfigurationsbereich **** zugegriffen werden. Wenn die Warnungszeitverzögerung erreicht ist, wird eine **Fortschrittsleiste** unter der Schaltfläche in der Hauptsymbolleiste angezeigt, die es ermöglicht, bei Bedarf einige Minuten lang zu schnüffeln (praktisch, wenn Sie vor der Sicherung etwas fertigstellen möchten).

Wenn eine Sicherung erstellt wird, das Projekt aber nicht gespeichert wurde (auch Untilted genannt), wird die Sicherung im Ordner **Documents/Allegorithmic/Substance Painter/autosave** gespeichert. Andernfalls befindet sich die Sicherung neben dem Projekt selbst (es sei denn, der Pfad wird vom Konfigurationsbereich überschrieben).

### Verbesserter Verlaufsfilter

![](../../assets/gradient-rust.jpg)

Der **Verlaufsfilter** wurde vollständig überarbeitet. Die Funktion ähnelt der des **Verlaufsumsetzung**-Knotens, der in **Substance Designer** verfügbar ist. Es unterstützt jetzt bis zu **10 verschiedene Farben**, mit der Möglichkeit, **anzugeben, wo sich die Farbe innerhalb** des Farbverlaufs ****befindet, und damit viele neue Türen zu öffnen. Dadurch können weitere **erweiterte Farbmuster**, aber auch **Relaishöhenzuordnungen**erstellt und **neue Formen**erstellt werden.

Der Hauptregler (Farbmenge) legt die Anzahl der Gesamtfarben fest, die zum Erstellen des Verlaufs verwendet werden. Die Schaltfläche direkt unten definiert den Farbüberblendmodus (sRGB oder Linear). Dies ist wichtig, wenn Sie eine ordnungsgemäße Überblendung zwischen Farben haben möchten. Wenn Sie beispielsweise ein reines Rot und ein reines Grün mischen, erhalten Sie dazwischen ein schönes Gelb. Dies ist nicht der Fall, wenn die Schaltfläche deaktiviert ist (stattdessen wird dunkelbraun angezeigt). Wenn Sie das Height oder andere Graustufenkanäle neu zuordnen, sollte diese Schaltfläche deaktiviert sein, um eine Gamma-Konvertierung zu vermeiden.

Mit der Schaltfläche oben kann das Filterergebnis durch den Verlauf selbst ersetzt werden, um den Verlauf in der 2D-Ansicht darzustellen.

![](../../assets/gradient-height-demo.jpg)

### Verbesserungen der Benutzeroberfläche und des Verhaltens

![](../../assets/tabs-top.png)

In dieser Version befinden sich die **Registerkarten** der verschiedenen Docks der Anwendung jetzt **oben anstatt unten** in ihren jeweiligen Fenstern. Diese Auswahl wurde getroffen, um die Lesbarkeit der Benutzeroberfläche zu verbessern, aber auch, um mit anderen Anwendungen konsistenter zu sein. Nach dieser Änderung folgt die Einführung des **kleinen Kreuzes** neben dem Registerkartentitel, um es **einfach zu schließen**. Es ist auch möglich, **mit der rechten Maustaste** auf die Registerkarte zu klicken, um ein **Kontextmenü** aufzurufen (mit dem Sie das Fenster schließen oder abdocken können). Ein Tastaturbefehl zum Abdocken des Fensters besteht darin, die Registerkarte einfach aus dem Fensterbereich heraus zu ziehen und abzulegen.

Es ist jetzt auch möglich, **Projekte** zu öffnen, indem Sie sie einfach **per Drag &amp; Drop aus dem Explorer in den Viewport** ziehen. Dies funktioniert auch mit **Mesh**-Dateien: Durch Ziehen und Ablegen einer Meshdatei in einen **leeren Viewport** wird das **neue Projektfenster** geöffnet. Wenn Sie dies jedoch in einem **bereits geöffneten Projekt** tun, wird das **Projektkonfigurationsdialogfeld** geöffnet, sodass ein Mesh schnell **aktualisiert werden kann**.

**Hinweis** : Wenn Sie Probleme mit dem Ziehen und Ablegen haben, stellen Sie sicher, dass Sie [unsere FAQ zum Thema](../../technical-support/technical-issues/miscellaneous-issues/impossible-to-drag-and-drop-files-into-the-shelf.md) überprüfen.

### Geschwindigkeitssteigerungen

Diese Version von Substance Painter bietet außerdem eine neue, deutliche Leistungsverbesserung für die Verwaltung des GPU-Speichers (VRam). Einheitliche Farben (z. B. Füllebenen) werden jetzt in kleinere Texturen komprimiert, wodurch ihre Übertragung zwischen dem Hauptspeicher und dem GPU-Speicher beschleunigt wird, aber auch ihr Speicherbedarf und ihre Berechnung reduziert werden. Dies sollte besonders beim Öffnen großer Projekte und beim Erreichen der Grenzen des GPU-Speichers sichtbar sein.

## Versionshinweise

### 2017.3.3

(Release 01. Dezember 2017)

**Fest:**

* [Steam] Popup zur Versionsprüfung sollte beim Start nicht sichtbar sein
* [Exportieren] Beim Öffnen von PSD-Dateien in Photoshop CS6 sind die Gruppen gesperrt

### 2017.3.2

(Release 20. November 2017)

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

### 2017.3.1

(Release 26. Oktober 2017)

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

### 2017.3

(Release 28. September 2017)

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
