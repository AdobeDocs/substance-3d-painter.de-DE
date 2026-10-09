---
breadcrumb-title: ""
description: Lesen Sie die Versionshinweise für Substance 3D Painter 9.0, um mehr über neue Funktionen, Verbesserungen und Fehlerbehebungen zu erfahren.
title: Version 9.0
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '1447'
ht-degree: 0%
---

# Version 9.0

Mit <b>Substance 3D Painter 9.0</b> wird eine neue Möglichkeit zum Malen von Strichen mit einem erneut bearbeitbaren Pfad im 3D-Viewport sowie aktualisiertem Standardinhalt eingeführt.

Freigabedatum: *20. Juni 2023*

## Wichtigste Funktionen

### Neues Malen entlang des Pfades im 3D-Viewport

![Nahaufnahme eines Lederschuhs, oben ein Pfad mit der Helfer-Benutzeroberfläche](../assets/v90_banner_path.jpg)

Das Werkzeug <b>Malen entlang Pfad</b> ist eine neue Möglichkeit zum Malen von Strichen im 3D-Viewport. Wie in anderen Anwendungen können Sie Bézier-basierte Kurven erstellen, die durch Punkte auf der Oberfläche Ihres 3D-Objekts gesteuert werden, um Muster zu zeichnen. In Kombination mit Substance-Materialien eröffnet dieses neue Tool viele neue Möglichkeiten.

* <b>Neues Tool zum Erstellen von Malen-Strichen, die von einem Pfad mit Punkten gesteuert werden</b>\
  In der Werkzeugleiste des Werkzeugs befindet sich ein neues Symbol, das dem Pfad-Werkzeug gewidmet ist. Mit diesem neuen Werkzeug können Sie Kurven auf der Oberfläche des 3D-Modells zeichnen, um Malen-Striche zu erstellen. Diese Konturen können immer erneut bearbeitet werden. Wenn das Mesh aktiv ist, klicke einfach auf die Punktoberfläche, um einen Punkt hinzuzufügen. Klicken Sie auf einen vorhandenen Punkt und drücken Sie die Löschtaste, um ihn zu entfernen.

  ![Screenshot der Symbolleistenoberfläche mit den drei Arten von Pfadwerkzeugen.](../assets/v90_path_toolbar.png)

  ![GIF, das das Hinzufügen und Entfernen von Punkten auf einem Pfad anzeigt](../assets/v90_path_add_remove_points.gif)
* <b>Ziehen und Verschieben von Punkten auf der Oberfläche des Meshs</b>\
  Um die Form eines Pfades zu bearbeiten, klicken und ziehen Sie einfach einen Punkt, um ihn entlang der Oberfläche des 3D-Moduls zu verschieben.

  ![Gif zeigt, wie Punkte verschoben werden](../assets/v90_path_move_points.gif)
* <b>Pfad schließen, um nahtlose Muster zu erstellen</b>\
  Der Pfad kann auch geschlossen werden, um Schleifen zu erstellen. Dies kann nützlich sein, um sich wiederholende Muster um bestimmte Bereiche herum zu erstellen, z. B.

  ![Gif zeigt einen geöffneten oder geschlossenen Pfad an](../assets/v90_path_open_close.gif)

  ![GIF, das einen geschlossenen Pfad zum Zeichnen von Nieten auf einer mechanischen Oberfläche zeigt](../assets/v90_path_closed_loop_demo.gif)
* <b>Pfade (und ihre Eigenschaften) mit dem Pfadbedienfeld erneut bearbeiten</b>\
  Wenn das Pfadwerkzeug ausgewählt ist, werden die in der aktuellen Malebene erstellten Pfade im speziellen Pfadbedienfeld oben im 3D-Viewport aufgelistet. In diesem Bereich können Sie Pfade in

  ![Gif zeigt das Pfadfenster in Aktion an](../assets/v90_path_panel_demo.gif)

  ![Gid zeigt Pfadeigenschaften an, die geändert werden](../assets/v90_path_edit_properties.gif)
* <b>Kompatibel mit anderen Malen-Funktionen wie Symmetrie, Geometriemaske, Dynamische Pinselstriche usw.</b>\
  Viele Einstellungen von normalen Malen-Konturen können mit dem Pfadwerkzeug verwendet werden:

  * Durch Aktivieren der Symmetrie können Sie einen Pfad mehrmals zeichnen, während Sie nur einen Pfad verwalten.
  * Pfade auf einer Ebene mit aktivierter Geometriemaske können unter verborgener Geometrie Malen werden.

  ![Gif zeigt einen Pfad, der mithilfe der Eigenschaft &quot;Symmetrie&quot; zweimal ertränkt wird](../assets/v90_path_symmetry.gif)
* <b>Malen mit anderen Tools wie Radiergummi oder Smudge</b>\
  Das Pfadwerkzeug ist auch mit dem Radiergummi- und dem Verwischen-Werkzeug kompatibel, sodass fortschrittlichere Möglichkeiten zum Malen und Kombinieren von Strichen mit der einfachen und erneut bearbeitbaren Möglichkeit zum Bearbeiten von Pfadpunkten verfügbar sind.

  ![Gid zeigt einen Pfad an, der verschoben wird, und aktualisiert den Verwischungseffekt](../assets/v90_path_smudge.gif)

* <b>Speichern und Wiederverwenden von Pfadeigenschaften mit Vorgaben</b>\
  Wenn Sie das Pfadwerkzeug verwenden, können Sie die Pinseleigenschaften auch als Vorgaben speichern. Auf diese Weise können Sie Werkzeugvorgaben speichern, die automatisch zum Pfadwerkzeug wechseln, wenn sie im Fenster &quot;Elemente&quot; ausgewählt werden.

>[!NOTE]
>
> Weitere Informationen finden Sie in der [dedizierten Dokumentation](../painting/tool-list/path.md).

### Neue Inhalte zum Malen entlang des Pfades

![Bild, das eine Kapuze mit einem anderen Typ von Pinselstrichen zeigt, die darauf verwendet werden.](../assets/v90_banner_content_path.jpg)

In dieser Version wurden einige neue Werkzeugvorgaben hinzugefügt, um die neue Funktion &quot;Malen entlang Pfad&quot; zu nutzen:

* Pipe Rack Sci-Fi
* Zusammenziehen
* Nahtstelle
* Topstiching
* Schweißmetall
* Reißverschlussband

![Abbildung des Fensters &quot;Elemente&quot; mit den neuen Werkzeugvorgaben](../assets/v90_path_presets_list.png)

![Bild, das ein Beispiel für die neue Schweißvorgabe zeigt](../assets/v90_path_welding_demo.jpg)

### Verbesserte Dynamische Pinselstriche für das Malen entlang des Pfades

![Bild mit einem Pfadstrich, der wie ein Pfeil aussieht, mit einer runden Form als Anfang und einem Pfeilkopf als Ende.](../assets/v90_banner_dyn_strokes.jpg)

Bei dieser Gelegenheit haben wir mit dem neuen Pfadwerkzeug dem dynamischen Kontursystem neue Eigenschaften hinzugefügt. Diese neuen Eigenschaften ermöglichen neue Arten von Strichen, die vorher nicht möglich waren, wie den Pfeil auf dem Bild, über dem ein anderes visuelles Anfangs- und Endbild zu sehen ist.

* <b>Neue Start-/Mittel-/Endeigenschaft</b>\
  Es kann eine neue Eigenschaft definiert werden, die für den Substance-Graf angegeben wird, ob ein Stempel innerhalb einer Kontur der erste, letzte oder ein Stempel in der Mitte ist. So können Start- und Endpunkte erstellt werden, die z. B. zum Erstellen von Reißverschlüssen sehr nützlich sein können. (<b>Hinweis</b>: Der Endstatus ist nur mit dem Pfadwerkzeug verfügbar.)
* <b>Neue Eigenschaft &quot;Größe&quot; und &quot;Abstand&quot;</b>\
  Mit der Property &quot;size&quot; und &quot;Abstand&quot; kannst du die Ausgabe eines Substance-Grafen auf Basis des aktuellen Stempelstatus anpassen.
* <b>Neue Konturlängeneigenschaften</b>\
  Der Abstand entlang des Pfades und der maximale Abstand eines Pfades ermöglichen eine bessere Kontrolle, wenn sich einige Effekte wiederholen, anstatt direkt einen normalisierten Wert bereitzustellen.\
  Es ist möglich, sowohl einen Wachstumshub, als auch einen Strich mit einem sich wiederholenden Muster auf der Grundlage der gezeichneten Entfernung (und nicht der Gesamtzahl der gezeichneten Stempel) zu erstellen.

![Gif zeigt einen Pfad mit einer dynamischen Kontur an](../assets/v90_path_dyn_stroke_wave_demo.gif)

>[!NOTE]
>
> Weitere Informationen finden Sie in der [dedizierten Dokumentation](../painting/dynamic-strokes/creating-custom-dynamic-strokes.md).

### Aktualisierte Standard-Material

![Eine Liste von Kugeln, die nebeneinander angezeigt werden und die verschiedenen neuen Material zeigen](../assets/v90_banner_materials.jpg)

In dieser Version haben wir uns entschlossen, einige Korrekturen in unserer Bibliothek vorzunehmen. Daher haben wir unsere Standard-Basismaterial geändert, um sie für alle nutzbarer zu machen. Diese Material wurden von demselben Team erstellt, das Inhalte auf [Substance 3D Assets](https://substance3d.adobe.com/assets) bereitstellt.

>[!NOTE]
>
> Der Inhalt, der entfernt wurde, ist auf [Substance 3D Community Assets](https://substance3d.adobe.com/community-assets?q=painter23update&u=painter23update) verfügbar.

## Tutorials

Das neue Pfad-Werkzeug ist in diesem Tutorial beschrieben:

## Versionshinweise

### 9.0.0

Freigabedatum: <b>2023/06/20</b>\
Zusammenfassung: <b>Hauptversion mit Malen entlang des Pfades, die 3D-Kurven, neue Basismaterialien und das Bereinigen älterer Materialien und neue Vorgaben für 3D-Kurven ermöglicht</b>

<b>Hinzugefügt:</b>

* [Pfad] Neues Malen entlang Pfad-Werkzeug hinzufügen
* [Pfad] Fügen Sie einen leeren Tastaturbefehl für das Pfadwerkzeug hinzu.
* [Pfad] Hinzufügen neuer Punkte zu einem vorhandenen Pfad zulassen
* [Pfad] Tastaturbefehl hinzufügen, um die aktuelle Pfaderstellung zu beenden
* [Pfad] Bearbeiten der Pinseleigenschaften für Pfade zulassen
* [Pfad] Automatische Anpassung der Tangenten beim Platzieren eines Punkts
* [Pfad] Tangenten beim Verschieben eines Punkts neu berechnen
* [Pfad] Einrasten neu erstellter Punkte an der Oberfläche eines Meshs
* [Pfad] Bearbeiten des Drucks pro Scheitelpunkt zulassen
* [Pfad] Anpassen des Drucks des neu erstellten Punkts von benachbarten Punkten
* [Pfad] Umwandeln von Punkten in Übergangspunkte/Eckpunkte zulassen (Tangente umbrechen)
* [Pfad] Sofort einen neu hinzugefügten Punkt verschieben
* [Pfad] Punkte aus vorhandenem Pfad entfernen
* [Pfad] Umkehren der Richtung eines Pfads zulassen
* [Pfad] Wählen Sie einen Pfad im Viewport aus.
* [Pfad] Auswählen von Pfadpunkten mit dem Auswahlrechteck zulassen
* [Pfad] Einführung von STRG+A-Tastaturbefehlen zum Auswählen aller Punkte eines Pfads
* [Pfad] Schließen des Pfads zulassen
* [Pfad] Geben Sie die Achse &quot;Pfad nach oben&quot; in den Eigenschaften an.
* [Path] Hinzufügen eines Scheitelpunkt-Steuerungsmenüs zur kontextabhängigen Symbolleiste
* [Pfad] Einführung in die Malen-/Lösch-/Verwischen-Modi im Pfadwerkzeug
* [Pfad] Erstellen von visuellem Feedback für Pfade im Viewport
* [Pfad] Hinzufügen eines visuellen Indikators für die Pfadrichtung
* [Path] Hinzufügen der Thickness zu den Anzeigeeinstellungen des Pfads
* [Path] Pfade ausblenden - Benutzeroberfläche
* [Pfad] Bedienfeld &quot;Pfad hinzufügen&quot; zur Liste der Pfade der aktuell ausgewählten Ebene
* [Pfad] Fügen Sie visuelles Feedback hinzu, wenn Sie den Mauszeiger über einen Pfad im Pfadbedienfeld bewegen
* [Pfad] Pfadbedienfeld anzeigen, wenn das Pfadwerkzeug ausgewählt ist
* [Pfad] Umbenennen, Löschen, Kopieren, Ausschneiden und Duplizieren von Pfaden im Bedienfeld &quot;Pfad&quot; zulassen
* [Pfad] Meldung anzeigen, wenn versucht wird, im 2D-Viewport mit dem Pfad-Werkzeug zu interagieren
* [Library] Integrieren neuer Inhalte (Pfad-Tools und -Basismaterial)
* [Dynamische Pinselstriche] Eigenschaft &quot;Abstand&quot; für Dynamische Pinselstriche hinzufügen
* [Dynamische Pinselstriche] Hinzufügen von Größen- und Abstand-Eigenschaften zu Dynamischen Pinselstrichen
* [Dynamische Pinselstriche] Hinzufügen der Eigenschaft &quot;Anfang&quot;, &quot;Mitte&quot; und &quot;Ende&quot; für Dynamische Pinselstriche
* [Python]&#x200B;[USD] Gelegt Projektkonfigurationsparameter für das USD
* [Python]&#x200B;[USD] Gelegt Projekterstellungsparameter für das USD
* [Exportieren]&#x200B;[USD] Fügen Sie Projektpfadinformationen innerhalb der exportierten USD hinzu
* [GLTF] Aktualisieren von Texturen in der Bibliothek beim erneuten Laden einer GLTF-Datei
* [Shader] Reduzieren von Artefakten in der Naht für UV-Inseln mit unterschiedlicher Ausrichtung
* [Engine] Update auf Substance Engine Version 9.0

<b>Fest:</b>

* [Importieren] Einige GLB mit Texturen erhalten keine Texturen in Painter
* [AMD] Artefakte an Rändern für alle 3D-Projektion-Flächen
* [Engine] Texturen brechen beim Umschalten der Ebenensichtbarkeit ab
* [Engine] Texturen sind an einigen Stellen leer, wenn der Mischmodus geändert wird
* [Engine] Textur/Projektion ist in einigen Fällen leerer Verkrümmungsmodus
* [Iray] Iteration wird beim Speichern des Renderings auf 0 zurückgesetzt
* [Log] USD Fehlermeldung beim Ausführen von Datei > Neu

<b>Bekannte Probleme:</b>

* [Farbmanagement] HDR. Farbraumkonvertierungen mit ACE unter Linux erzeugen festgeklemmte Farben
* [Ebenenstapel] Eingabequelle nicht pro Ebene gespeichert
