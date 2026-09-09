---
helpx_url: 'https://helpx.adobe.com/substance-3d-painter/painting/tool-list/path.html'
breadcrumb-title: ''
description: Mit dem Pfadwerkzeug in Substance 3D Painter können Sie Pfade erstellen und bearbeiten, um die Textur präzise zu zeichnen und Konturen zu platzieren.
helpx_creative_field: ''
helpx_description: Painting > Path tools list > Path tool
helpx_experience_level: ''
helpx_learn_topic: ''
helpx_tags: ''
title: Pfad-Werkzeug - Übersicht
user-guide-description: ''
user-guide-title: ''
source-git-commit: 6fcf10add7086a0e2a070ee6046c0a261ef1ae34
workflow-type: tm+mt
source-wordcount: '1666'
ht-degree: 0%

---


# Pfad-Werkzeug - Übersicht

![Bild, das das auf einem Schuh verwendete Pfadwerkzeug zeigt](../../assets/v90_banner_path.jpg)

Mit den **Pfadwerkzeugen** können Sie eine Kurve mit Punkten auf der Oberfläche Ihres Meshs definieren. Nachdem die Kurve erstellt wurde, können Sie mit den verschiedenen Pfadwerkzeugen verschiedene Effekte entlang der Kurve erstellen.

## Erstellen eines Pfads

Pfade können auf Malebenen und Malen-Effekten erstellt werden. Es gibt zwei Möglichkeiten, auf das Pfad-Werkzeug zuzugreifen:

* **Über die Schnittstelle**: auf der linken Seite zur Werkzeugleiste navigieren und auf das dritte Symbol oben klicken.
* **Über einen Tastatur-Tastaturbefehl**: Standardmäßig ist dem Werkzeug keine zugewiesen. Dies kann im Einstellungsmenü durch Bearbeiten des Tastaturbefehl &quot;Malen entlang Pfad auswählen&quot; geändert werden.

Sobald das Werkzeug ausgewählt ist, können Sie Punkte platzieren, indem Sie auf die Oberfläche des 3D-Modells innerhalb des 3D-Viewports klicken. Zum Erstellen eines Pfads werden mindestens zwei Punkte (oder Scheitelpunkt) benötigt.

![Gif zeigt die Auswahl des Pfadwerkzeugs und die Erstellung von Punkten an](../../assets/path_create_points.gif)

Das Pfadwerkzeug verfügt über verschiedene Modi, die den anderen in der Anwendung verfügbaren Malen-Tools ähneln können:

* Malen entlang Pfad: Zeichnen Sie einen normalen Pinselstrich entlang eines definierten Pfads.
* [Bandpfad](ribbon-tool.md): Zeichnet ein sich wiederholendes oder gedehnt Bild entlang eines Pfades.
* [Ausgefüllter Pfad](filled-path.md): Füllt das Innere eines Pfades mit einer einheitliche Farbe.
* entlang Pfad radieren: Zeichnen Sie einen Strich, der Informationen entlang eines definierten Pfads löscht/entfernt.
* Verwischen entlang des Pfades: Zeichnen Sie einen Strich, der Informationen entlang eines definierten Pfads verwischt/verwischt.

![Screenshot der Werkzeugleiste mit den verschiedenen Pfadwerkzeugmodi](../../assets/PathTools.png)

Hier ist z. B. das Pfadwerkzeug im Modus &quot;**Verwischen**&quot;, das andere Malinformationen beeinflusst:

![GIF, das ein Pfadwerkzeug im Verwischmodus anzeigt](../../assets/v90_path_smudge.gif)

>[!NOTE]
>
> Die **Pfadwerkzeuge** funktionieren nur im 3D-Raum auf der Oberfläche der Geometrie. Das Erstellen eines Pfads im UV-Raum oder als Projektion im Bildschirmraum wird derzeit nicht unterstützt.

### Bearbeiten eines Pfads

Pfadpunkte (oder Scheitelpunkt) haften automatisch an der Oberfläche des Meshs. Sie können jederzeit verschoben und angepasst werden. Sie können einem bestehenden Pfad neue Scheitelpunkt hinzufügen, indem Sie an einer beliebigen Stelle entlang der Linie klicken.

* Durch Drücken von **Escape** oder **Enter** wird die Pfadausgabe beendet.
* Wenn Sie auf eine leere Fläche des Meshs klicken, wird ein neuer Pfad erstellt.
* Wenn Sie mit der Maus auf einen vorhandenen Pfad klicken, wird er ausgewählt, sodass Sie den Pfad fortsetzen oder bearbeiten können. Pfade können auch über das Bedienfeld &quot;**Pfade**&quot; neu ausgewählt werden (siehe unten).

![Gif zeigt das Hinzufügen neuer Punkte und das Verschieben vorhandener Punkte auf einem Pfad an](../../assets/path_edit_move_points.gif)

Einige Eigenschaften sind für einen Pfad als Ganzes spezifisch. Dies ist der Fall bei Optionen, die im Fenster **Eigenschaften** gefunden wurden. Wie bei einer normalen Kontur (siehe [Malen-Tool-Dokumentation](paint-brush.md)) können die folgenden Eigenschaften für einen Pfad definiert werden:

* **Pinsel**
* **Alpha**
* **Material**

Der Abschnitt **brush** enthält zusätzliche Optionen, die nur mit dem Pfadwerkzeug verfügbar sind:

| **Einstellung** | **Beschreibung** |
| --- | --- |
| **Projektion Tiefe** | Legt fest, wie nah der Pfad an der Pinseloberfläche sein muss, damit die Mesh-Stempel angezeigt werden. Um dieses visuelle Feedback direkt im Viewport anzuzeigen, können Sie **Normale** in den **Pfad-Anzeigeeinstellungen** aktivieren (siehe unten). |
| **Achse nach oben** | Die Achse, die zum Ausrichten von Pinselstempeln verwendet wird, wenn **Pfad folgen** deaktiviert ist.   In einem bestimmten Kontext ist es sinnvoller, alle Stempel an einer globalen Achse/Richtung auszurichten und nicht an einem Pfad. Zum Beispiel mit Nieten auf einer metallic Fläche. |

Andere Eigenschaften werden für Punkte (Scheitelpunkt) auf dem Pfad definiert, z. B. der Druckwert. Um einen bestimmten Punkt zu bearbeiten, klicken Sie einfach darauf (oder verwenden Sie die rechteckige Auswahl). Verwenden Sie dann die kontextbezogene Symbolleiste, um die ausgewählten Punktwerte zu bearbeiten.

![Gif zeigt die Druckausgabe pro Scheitelpunkt an](../../assets/path_point_pressure_example.gif)

### Steuern von Tangenten

Manchmal ist ein glatter Pfad nicht ideal, weil er nicht der Oberfläche des 3D-Modells am besten entspricht oder weil er nicht zu einem bestimmten Look passt. Um diese Probleme zu lösen, ist es möglich, die Tangenten eines bestimmten Scheitelpunkts zu ändern. Die Tangenten sind die Richtungen eines Punktes, die steuern, wie der Pfad gebeugt wird.

Um zwischen glatten oder linearen/fehlerhaften Tangenten zu wechseln, doppelklicken Sie einfach auf einen Scheitelpunkt (oder verwenden Sie die entsprechende Schaltfläche in der Kontextsymbolleiste):

![Gid zeigt, wie Tangenten auf einem Pfad gesteuert werden](../../assets/path_break_tangents.gif)

Um die Ausrichtung der Tangenten genauer zu steuern, überschreiben Sie sie mithilfe der Schaltfläche Benutzerdefinierte Tangenten in der kontextbezogenen Symbolleiste manuell:

![Gid zeigt, wie Tangenten auf einem Pfad gesteuert werden](../../assets/path_control_tangents.gif)

Verwenden Sie den **ALT**-Tastatur-Tastaturbefehl, um die Tangenten während des Bewegens zu unterbrechen, wenn der Punkt noch nicht erreicht wurde.

Verwenden Sie den Tastaturbefehl **STRG**, um beide Tangenten gleichzeitig zu skalieren.

>[!NOTE]
>
> Die Steuerelemente für die Tangente werden entlang des Plans definiert, der mit der Normalen des angegebenen Punkts im Pfad ausgerichtet ist. Das bedeutet, dass sich die Tangenten nicht in bestimmte Richtungen biegen können.

### Kontextsymbolleiste

![Screenshot der kontextbezogenen Symbolleiste im Pfadmodus](../../assets/path_contextual_toolbar_overview.png)

Die **kontextbezogene Symbolleiste**, wenn das **Pfad**-Tool ausgewählt ist, stellt mehrere Einstellungen bereit, mit denen der aktuell ausgewählte Pfad gesteuert werden kann:

<table>
  <tr>
    <th><strong>Parameter</strong></th>
    <th><strong>Beschreibung</strong></th>
  </tr>
  <tr>
    <td><strong>Viewport-Oberfläche ein-/ausblenden</strong><br><img src="../../assets/path_contextual_toolbar_showhide.png" alt="Pfadwerkzeug - Symbol ausblenden"/></td>
    <td>Wenn diese Option aktiviert ist, werden die Überlagerungen von Pfaden und Scheitelpunkten im Viewport angezeigt.</td>
  </tr>
  <tr>
    <td><strong>Anzeigeeinstellungen</strong><br><img src="../../assets/path_contextual_toolbar_display.png" alt="Symbol für die Pfadanzeigeeinstellungen"/></td>
    <td>Steuern Sie das Aussehen des visuellen Pfadfeedback im Viewport:<br><ul><li><strong>Handle-Größe</strong>: steuert, wie groß die Punkte des Pfades aussehen.</li><li><strong>Pfadbreite</strong>: steuert die Thickness der Pfadlinie.<br></li><li><strong>Pfadfarbe</strong>: steuert die Farbe der Pfadlinie.<br></li><li><strong>Nicht ausgewählte Pfadfarbe</strong>: steuert die Farbe der nicht aktiven Pfade.<br></li><li><strong>Normale</strong>: Wenn aktiviert, zeigen Sie die Richtung der Projektion an jedem Punkt eines Pfades an.<br></li><li><strong>Tangenten</strong>: Wenn aktiviert, zeigen Sie die Kurvenrichtung der Kontrollpunkte des Pfades an.<br></li><li><strong>Pfadrichtung</strong>: Wenn diese Option aktiviert ist, zeigen Sie einen kleinen Pfeil am Ende des Pfades an, um die Malrichtung anzugeben. Das ist nützlich, um zu erfahren, wie Stempel innerhalb des Strichs ausgerichtet werden.</li></ul><br><img src="../../assets/path_contextual_toolbar_display_settings.png" alt="Screenshot des Einstellungsfensters für die Pfadanzeige"/></td>
  </tr>
  <tr>
    <td><strong>Pfadrichtung umkehren</strong><br><img src="../../assets/path_contextual_toolbar_direction.png" alt="Symbol der umgekehrten Pfadrichtung"/></td>
    <td>Spiegeln Sie die Richtung des aktuellen Pfads. Die Richtung definiert die allgemeine Ausrichtung zum Malen der Stempel innerhalb der Kontur. Durch Umkehren des Pfads kannst du das gezeichnete Muster neu ausrichten.</td>
  </tr>
  <tr>
    <td><strong>Ecke/Glättung umschalten</strong><br><img src="../../assets/path_contextual_toolbar_smoothcorner.png" alt="Symbol für überflüssige Ecke des Umschalters"/></td>
    <td>Brechen Sie die Tangente der aktuell ausgewählten Scheitelpunkt auf oder richten Sie sie aus, sodass Sie zwischen einer glatten oder geraden Kurve wechseln können.<br><img src="../../assets/path_smooth_corner_demo.png" alt="Screenshot eines Pfades mit einem glatten und einem linearen Pfad "/><br><strong>Hinweis:</strong> Sie können auch zwischen dem Eckverhalten und dem Glättungsverhalten wechseln, indem Sie auf einen Punkt direkt auf dem Pfad doppelklicken.</td>
  </tr>
  <tr>
    <td><strong>Benutzerdefinierte Tangenten</strong><br><img src="../../assets/path_icon_custom_tangents.png" alt="Pfadwerkzeug-Symbol für benutzerdefinierte Tangenten"/></td>
    <td>Wenn aktiviert, können Sie die Tangenten eines bestimmten Punktes auf dem Pfad manuell steuern.<br><img src="../../assets/paht_cutom_tangents_demo.png" alt="Abbildung mit Tangenten für benutzerdefinierte Pfade"/></td>
  </tr>
  <tr>
    <td><strong>Pfad öffnen/schließen</strong><br><img src="../../assets/path_contextual_toolbar_close.png" alt="Symbol für geöffneten Pfad zum Schließen"/></td>
    <td>Öffnen oder schließen Sie den aktuellen Pfad. Um einen Pfad zu schließen, muss zuerst einer der beiden Endpunkte des aktuellen Pfads ausgewählt werden.<br><img src="../../assets/v90_path_open_close.gif" alt="GIF-Datei, die einen geöffneten und dann geschlossenen Pfad zeigt"/></td>
  </tr>
  <tr>
    <td><strong>Eckpunkt löschen</strong><br><img src="../../assets/path_contextual_toolbar_delete.png" alt="Symbol zum Löschen des Scheitelpunkts "Pfad""/></td>
    <td>Entfernt die aktuell markierten Scheitelpunkt eines Pfades.</td>
  </tr>
  <tr>
    <td><strong>Symmetrie</strong><br><img src="../../assets/path_contextual_toolbar_symmetry.png" alt="Funktion "Symbol der Symmetrie""/></td>
    <td>Aktivieren oder deaktivieren Sie die Symmetrie für den aktuellen Pfad. Weitere Informationen finden Sie in der <a href="../symmetry/symmetry.md">Symmetrie-Dokumentation</a>.<br><img src="../../assets/v90_path_symmetry.gif" alt="GIF, das einen in Symmetrie gezeichneten Pfad zeigt"/></td>
  </tr>
  <tr>
    <td><strong>Ausgeschlossene Geometrie ausblenden/ignorieren</strong><br><img src="../../assets/path_contextual_toolbar_exclude.png" alt="Symbol der Geometriemaske zum Ausschließen des KE"/></td>
    <td>Wenn diese Option aktiviert ist, wird der aktuelle Pfad durch die verborgene Malen geführt. Weitere Informationen finden Sie in der <a href="../../interface/layer-stack/geometry-mask.md">Dokumentation zu Geometriemasken</a>.</td>
  </tr>
</table>

### Pfadebedienfeld

![Pfadbereich](../../assets/path_panel_visibility.png)

>[!NOTE]
>
> Das Bedienfeld ist ausgeblendet, wenn das aktuelle Werkzeug nicht das Pfadwerkzeug ist oder wenn eine Füllebene/ein Ordner ausgewählt ist.

Im Viewport befindet sich das Bedienfeld &quot;**Pfade**&quot;, in dem alle Pfade der aktuell ausgewählten Malebene/des Effekts aufgelistet sind. Pfade lassen sich einfach auswählen und verwalten.

Mit diesem Bedienfeld können Sie:

* Doppelklicken Sie auf einen Pfad, um &quot;**umzubenennen**&quot;.
* **Löschen** Sie einen Pfad, indem Sie ihn auswählen und dann die Löschtaste drücken.
* **Kopieren**/**Einfügen**/**Duplizieren** Sie einen Pfad mit den dedizierten Tastaturbefehlen.
* **Einblenden** oder **Ausblenden** eines Pfads mit dem Augensymbol (das steuert, ob der Pfad auf die Texturierung angewendet wird).

Der Einfachheit halber können Sie auch mit der rechten Maustaste auf einen Pfad klicken, um das Kontextmenü mit den gleichen Aktionen zu öffnen:

![Rechtsklick-Menü im Bedienfeld &quot;Pfad&quot;](../../assets/path_panel_rightclick_menu_copy_properties.png)

Im Kontextmenü können Sie auch Aktionen öffnen, um die Eigenschaften oder die Position eines Pfads auf einen anderen Pfad zu kopieren. Auf diese Weise können Features problemlos über verschiedene Pfade hinweg freigegeben oder synchronisiert werden:

![Gif zeigt, wie Pfadeigenschaften kopiert und eingefügt werden](../../assets/path_copy_paste_properties.gif)![Gif zeigt, wie Pfadpositionen kopiert und eingefügt werden](../../assets/path_copy_paste_vertices.gif)

>[!NOTE]
>
> Kopieren und Einfügen von Eigenschaften funktioniert nur, wenn Pfade auf demselben Malwerkzeug basieren. Beispielsweise ist es nicht möglich, Eigenschaften zwischen einem Pfad mit Verwisch-Einstellungen und einem anderen Pfad mit Pinseleinstellungen zu teilen.

## Werkzeugvorgaben

![Ein Screenshot des Abschnitts &quot;Vorgaben&quot; des Eigenschaftenfensters, wenn ein Pfadwerkzeug ausgewählt ist](../../assets/path_presets.png){width="400px"}

Wenn ein Pfadwerkzeug ausgewählt ist, steht oben im Bedienfeld &quot;Eigenschaften&quot; der Bereich &quot;Vorgaben&quot; zur Verfügung. Hier können Sie schnell auf Vorgaben für die verschiedenen Pfadwerkzeuge zugreifen.

### Bevorzugte Pfadvorgaben

Die Option &quot;Favoriten&quot; im Bereich &quot;Vorgaben&quot; enthält nur Vorgaben, die Sie für einen noch schnelleren Zugriff als Favoriten festgelegt haben. Um Favoriten hinzuzufügen, wählen Sie Favoriten und dann &quot;Kompatible Vorgaben in Elementen anzeigen&quot;, um eine vollständige Liste der verfügbaren Pfadvorgaben anzuzeigen.

Um eine Vorgabe als Favorit festzulegen, klicken Sie im Bedienfeld Elemente oder im Bereich Vorgaben des Bedienfelds Eigenschaften mit der rechten Maustaste auf die Vorgabe und wählen Sie dann &quot;Zu Favoriten hinzufügen&quot; aus.

Sie können Vorgaben auch aus der Favoritenliste entfernen. Mache einen Rechtsklick bzw. Ctrl-Klick auf eine Vorgabe, und wähle &quot;Aus Favoriten entfernen&quot;.

![Ein Screenshot des Abschnitts &quot;Vorgaben&quot; des Eigenschaftenfensters, wenn ein Pfadwerkzeug ausgewählt ist. Die Option &quot;Favoriten&quot; ist ausgewählt, und die Schaltfläche &quot;Kompatible Vorgaben in Elementen anzeigen&quot; ist hervorgehoben.](../../assets/ShowCompatiblePresets.png){width="400px"}

### Erstellen von Pfadvorgaben

Wie andere Werkzeuge können auch Voreinstellungen erstellt werden, um die Pinseleinstellungen/-konfigurationen schnell wiederherzustellen. Klicken Sie dazu einfach mit der rechten Maustaste in das Fenster **Eigenschaften** und wählen Sie **Werkzeugvorgabe erstellen.** Diese neu erstellte Vorgabe wechselt automatisch zum Pfadwerkzeug, wenn sie im Fenster **Elemente** ausgewählt wird.