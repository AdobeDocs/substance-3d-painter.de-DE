---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/painting/tool-list/path.html"
breadcrumb-title: ''
description: Mit dem Pfadwerkzeug in Substance 3D Painter können Sie Pfade für ein präzises Strukturmalen und die Platzierung von Konturen erstellen und bearbeiten.
helpx_creative_field: ""
helpx_description: Painting > Path tools list > Path tool
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Pfad-Werkzeug - Übersicht
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '1699'
ht-degree: 0%

---


# Pfad-Werkzeug - Übersicht

![Bild, das das auf einem Schuh verwendete Pfadwerkzeug zeigt](../../assets/v90_banner_path.jpg)

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

<b>Audio</b>

Passe Audio an oder füge Audio zu deinem Projekt hinzu.


* Passen Sie die Quellvideolautstärke an, wenn sie Audio enthält.
* Externe Audiodateien hinzufügen, entfernen oder ersetzen
* Passen Sie die externe Lautstärke der Audiodatei an.

</td>
<td style="border: 0;" valign="top">

![](../../assets/image_180.png)

</td>
</tr>
</table>

Mit den <b>Pfadwerkzeugen</b> können Sie eine Kurve mit Punkten auf der Oberfläche des Gitters definieren. Nachdem die Kurve erstellt wurde, können Sie mit den verschiedenen Pfadwerkzeugen verschiedene Effekte entlang der Kurve erstellen.

## Erstellen eines Pfads

Pfade können auf Malebenen und Maleffekten erstellt werden. Es gibt zwei Möglichkeiten, auf das Pfad-Werkzeug zuzugreifen:

* <b>Über die Schnittstelle</b>: auf der linken Seite zur Werkzeugleiste navigieren und auf das dritte Symbol oben klicken.
* <b>Über einen Tastaturbefehl</b>: Standardmäßig ist dem Werkzeug keine zugewiesen. Dies kann im Menü &quot;Einstellungen&quot; geändert werden, indem Sie den Tastaturbefehl &quot;entlang des Pfades malen auswählen&quot; bearbeiten.

Sobald das Werkzeug ausgewählt ist, können Punkte platziert werden, indem Sie auf die Oberfläche des 3D-Modells im 3D-Viewport klicken. Mindestens zwei Punkte (oder Scheitelpunkte) sind erforderlich, um einen Pfad zu erstellen.

![Gif zeigt die Auswahl des Pfadwerkzeugs und die Erstellung von Punkten an](../../assets/path_create_points.gif)

Das Pfadwerkzeug verfügt über verschiedene Modi, die den anderen in der Anwendung verfügbaren Malwerkzeugen ähneln können:

* Malen entlang Pfad: Zeichnen Sie einen normalen Pinselstrich entlang eines definierten Pfads.
* [Bandpfad](ribbon-tool.md): Zeichnet ein wiederholtes oder gestrecktes Bild entlang eines Pfades.
* [Ausgefüllter Pfad](filled-path.md): Füllen Sie das Innere eines Pfades mit einer einheitlichen Farbe.
* entlang Pfad radieren: Zeichnen Sie einen Strich, der Informationen entlang eines definierten Pfads löscht/entfernt.
* Verwischen entlang des Pfades: Zeichnen Sie einen Strich, der Informationen entlang eines definierten Pfads verwischt/verwischt.

![Screenshot der Werkzeugleiste mit den verschiedenen Pfadwerkzeugmodi](../../assets/PathTools.png)

Hier ist z. B. das Pfadwerkzeug im Modus &quot;<b>Verwischen</b>&quot;, das andere Malinformationen beeinflusst:

![GIF, das ein Pfadwerkzeug im Verwischmodus anzeigt](../../assets/v90_path_smudge.gif)

>[!NOTE]
>
> Die <b>Pfadwerkzeuge</b> funktionieren nur im 3D-Raum auf der Oberfläche der Geometrie. Das Erstellen eines Pfads im UV-Raum oder als Bildschirmraumprojektion wird derzeit nicht unterstützt.

### Bearbeiten eines Pfads

Pfadpunkte (oder Scheitelpunkte) haften automatisch an der Oberfläche des Gitters. Sie können jederzeit verschoben und angepasst werden. Sie können einem vorhandenen Pfad neue Scheitelpunkte hinzufügen, indem Sie an einer beliebigen Stelle entlang der Linie klicken. 

* Durch Drücken von <b>Escape </b> oder <b>Enter </b> wird die Pfadausgabe beendet.
* Wenn Sie auf eine leere Oberfläche des Gitters klicken, wird ein neuer Pfad erstellt.
* Wenn Sie mit der Maus auf einen vorhandenen Pfad klicken, wird er ausgewählt, sodass Sie den Pfad fortsetzen oder bearbeiten können. Pfade können auch über das Bedienfeld &quot;<b>Pfade</b>&quot; neu ausgewählt werden (siehe unten).

![Gif zeigt das Hinzufügen neuer Punkte und das Verschieben vorhandener Punkte auf einem Pfad an](../../assets/path_edit_move_points.gif)

Einige Eigenschaften sind für einen Pfad als Ganzes spezifisch. Dies ist der Fall bei Optionen, die im Fenster <b>Eigenschaften </b> gefunden werden. Wie bei einer normalen Kontur (siehe [Paint-Tool-Dokumentation](paint-brush.md)) können die folgenden Eigenschaften für einen Pfad definiert werden:

* <b>Pinsel</b>
* <b>Alpha</b>
* <b>Material</b>

Der Abschnitt <b>Pinsel </b> enthält zusätzliche Optionen, die nur mit dem Pfadwerkzeug verfügbar sind:

| <b>Einstellung</b> | <b>Beschreibung</b> |
| --- | --- |
| <b>Tiefe der Projektion</b> | Legt fest, wie nah der Pfad an der Gitteroberfläche sein muss, damit die Pinselstempel angezeigt werden. Um dieses visuelle Feedback direkt im Viewport anzuzeigen, können Sie <b>Normale</b> in den <b>Pfad-Anzeigeeinstellungen </b> aktivieren (siehe unten). |
| <b>Achse nach oben</b> | Die Achse, an der die Pinselstempel ausgerichtet werden, wenn <b>Pfad folgen</b> deaktiviert ist.   In einem bestimmten Kontext ist es sinnvoller, alle Stempel entlang einer globalen Achse/Richtung und nicht entlang des Pfades auszurichten. Zum Beispiel mit Nieten auf einer metallischen Oberfläche. |

Andere Eigenschaften werden für Punkte (Scheitelpunkte) auf dem Pfad definiert, z. B. der Druck. Um einen bestimmten Punkt zu bearbeiten, klicken Sie einfach darauf (oder verwenden Sie die rechteckige Auswahl). Verwenden Sie dann die kontextbezogene Symbolleiste, um die ausgewählten Punktwerte zu bearbeiten.

![Gif zeigt die Druckausgabe pro Scheitelpunkt an](../../assets/path_point_pressure_example.gif)

### Steuern von Tangenten

Manchmal ist ein glatter Pfad nicht ideal, weil er nicht der Oberfläche des 3D-Modells am besten entspricht oder weil er nicht zu einem bestimmten Look passt. Um diese Probleme zu lösen, ist es möglich, die Tangenten eines bestimmten Scheitelpunktes zu ändern. Die Tangenten sind die Richtungen eines Punktes, die steuern, wie der Pfad gebeugt wird.

Um zwischen glatten oder linearen/unterbrochenen Tangenten zu wechseln, doppelklicken Sie einfach auf einen Scheitelpunkt (oder verwenden Sie die entsprechende Schaltfläche in der kontextbezogenen Symbolleiste):

![Gid zeigt, wie Tangenten auf einem Pfad gesteuert werden](../../assets/path_break_tangents.gif)

Um die Ausrichtung der Tangenten genauer zu steuern, verwenden Sie die Schaltfläche Benutzerdefinierte Tangenten in der kontextbezogenen Symbolleiste, um sie manuell zu überschreiben:

![Gid zeigt, wie Tangenten auf einem Pfad gesteuert werden](../../assets/path_control_tangents.gif)

Verwenden Sie die Tastenkombination <b>ALT</b>, um die Tangenten beim Bewegen zu unterbrechen, wenn der Punkt noch nicht bewegt wurde.

Verwenden Sie den Tastaturbefehl <b>STRG</b>, um beide Tangenten gleichzeitig zu skalieren.

>[!NOTE]
>
> Die Tangentensteuerungen werden entlang der Ebene definiert, die mit der Normalen des angegebenen Punkts im Pfad ausgerichtet ist. Das bedeutet, dass sich Tangenten nicht in bestimmte Richtungen biegen können.

### Kontextsymbolleiste

![Screenshot der kontextbezogenen Symbolleiste im Pfadmodus](../../assets/path_contextual_toolbar_overview.png)

Die <b>kontextbezogene Symbolleiste</b>, wenn das <b>Pfad</b>-Tool ausgewählt ist, stellt mehrere Einstellungen bereit, mit denen der aktuell ausgewählte Pfad gesteuert werden kann:

| <b>Parameter</b> | <b>Beschreibung</b> |
| --- | --- |
| <b>Viewport-Schnittstelle ein-/ausblenden</b>  <div><img alt="Pfadwerkzeug - Symbol ausblenden" class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_table_row-1k12728-column-xc227lz_image" src="../../assets/path_contextual_toolbar_showhide.png"/></div> | Wenn diese Option aktiviert ist, werden die Überlagerungen von Pfaden und Scheitelpunkten im Viewport angezeigt. |
| <b>Anzeigeeinstellungen</b>  <div><img alt="Symbol für die Pfadanzeigeeinstellungen" class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_table_row-uj427cc-column-xc227lz_image" src="../../assets/path_contextual_toolbar_display.png"/></div> | Steuern Sie das Aussehen des visuellen Pfadfeedback im Viewport:<ul data-preserve-html="true"> <li data-preserve-html="true"><b>Handle-Größe</b>: steuert, wie groß die Punkte des Pfades aussehen.</li> <li data-preserve-html="true"><b>Pfadbreite</b>: die Thickness der Pfadlinie steuern.<br/> </li> <li data-preserve-html="true"><b>Pfadfarbe</b>: die Farbe der Pfadlinie steuern.<br/> </li> <li data-preserve-html="true"><b>Nicht ausgewählte Pfadfarbe</b>: die Farbe der nicht aktiven Pfade steuern.<br/> </li> <li data-preserve-html="true"><b>Normale</b>: Wenn aktiviert, zeigen Sie die Projektionsrichtung an jedem Punkt eines Pfades an.<br/> </li> <li data-preserve-html="true"><b>Tangenten</b>: Wenn aktiviert, zeigen Sie die Kurvenrichtung der Kontrollpunkte des Pfads an.<br/> </li> <li data-preserve-html="true"><b>Pfadrichtung</b>: Wenn diese Option aktiviert ist, zeigen Sie einen kleinen Pfeil am Ende des Pfades an, um die Malrichtung anzugeben. Das ist nützlich, um zu erfahren, wie Stempel innerhalb des Strichs ausgerichtet werden.</li> </ul>  <div><img alt="Screenshot des Einstellungsfensters für die Pfadanzeige" class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_table_row-uj427cc-column-vo327hy_image" src="../../assets/path_contextual_toolbar_display_settings.png"/></div> |
| <b>Pfadrichtung umkehren</b>  <div><img alt="Symbol der umgekehrten Pfadrichtung" class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_table_row-5xb27rp-column-xc227lz_image" src="../../assets/path_contextual_toolbar_direction.png"/></div> | Spiegeln Sie die Richtung des aktuellen Pfads. Die Richtung definiert die allgemeine Ausrichtung, die zum Malen der Stempel innerhalb des Strichs verwendet wird. Durch Umkehren des Pfads kannst du das gezeichnete Muster neu ausrichten. |
| <b>Ecke/Glättung ein/aus</b>  <div><img alt="Symbol für überflüssige Ecke des Umschalters" class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_table_row-8wd27al-column-xc227lz_image" src="../../assets/path_contextual_toolbar_smoothcorner.png"/></div> | Unterbrechen oder richten Sie die Tangente der aktuell ausgewählten Scheitelpunkte aus, sodass Sie zwischen einer glatten oder linearen Kurve wechseln können.  <div><img alt="Screenshot eines Pfades mit einem glatten und einem linearen Pfad " class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_table_row-8wd27al-column-vo327hy_image" src="../../assets/path_smooth_corner_demo.png"/></div>  **Hinweis:** Der Wechsel zwischen Eck- und Übergangsparameter kann auch durch Doppelklicken auf einen Punkt direkt auf dem Pfad erfolgen. |
| <b>Benutzerdefinierte Tangenten</b>  <div><img alt="Pfadwerkzeug-Symbol für benutzerdefinierte Tangenten" class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_table_row-r302zw8-column-xc227lz_image" src="../../assets/path_icon_custom_tangents.png"/></div> | Wenn diese Option aktiviert ist, können Sie die Tangenten eines bestimmten Punkts auf dem Pfad manuell steuern.  <div><img alt="Bild mit benutzerdefinierten Pfadtangenten" class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_table_row-r302zw8-column-vo327hy_image" src="../../assets/paht_cutom_tangents_demo.png"/></div> |
| <b>Pfad öffnen/schließen</b>  <div><img alt="Symbol für geöffneten Pfad zum Schließen" class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_table_row-7ve27oq-column-xc227lz_image" src="../../assets/path_contextual_toolbar_close.png"/></div> | Öffnen oder schließen Sie den aktuellen Pfad. Um einen Pfad zu schließen, muss zuerst einer der beiden Endpunkte des aktuellen Pfads ausgewählt werden.  <div><img alt="GIF-Datei, die einen geöffneten und dann geschlossenen Pfad zeigt" class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_table_row-7ve27oq-column-vo327hy_image" src="../../assets/v90_path_open_close.gif"/></div> |
| <b>Scheitelpunkt löschen</b>  <div><img alt="Symbol zum Löschen des Pfadscheitelpunkts" class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_table_row-v0f273z-column-xc227lz_image" src="../../assets/path_contextual_toolbar_delete.png"/></div> | Entfernen Sie die aktuell ausgewählten Scheitelpunkte auf einem Pfad. |
| <b>Symmetrie</b>  <div><img alt="Symbol des Symmetrie-Merkmals" class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_table_row-hkg27qa-column-xc227lz_image" src="../../assets/path_contextual_toolbar_symmetry.png"/></div> | Aktivieren oder deaktivieren Sie die Symmetrie für den aktuellen Pfad. Weitere Informationen finden Sie in der [Symmetrie-Dokumentation](../symmetry/symmetry.md).  <div><img alt="GIF, das einen symmetrisch gezeichneten Pfad zeigt" class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_table_row-hkg27qa-column-vo327hy_image" src="../../assets/v90_path_symmetry.gif"/></div> |
| <b>Ausgeschlossene Geometrie ausblenden/ignorieren</b>  <div><img alt="Symbol der Geometriemaske zum Ausschließen des KE" class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_table_row-52h27be-column-xc227lz_image" src="../../assets/path_contextual_toolbar_exclude.png"/></div> | Wenn diese Option aktiviert ist, lassen Sie den aktuellen Pfad durch die verborgene Geometrie malen. Weitere Informationen finden Sie in der [Dokumentation zu Geometriemasken](../../interface/layer-stack/geometry-mask.md). |

### Pfadebedienfeld

![Pfadbereich](../../assets/path_panel_visibility.png)

>[!NOTE]
>
> Das Bedienfeld ist ausgeblendet, wenn das aktuelle Werkzeug nicht das Pfadwerkzeug ist oder wenn eine Füllebene/ein Ordner ausgewählt ist.

Im Viewport befindet sich das Bedienfeld &quot;<b>Pfade</b>&quot;, in dem alle Pfade der aktuell ausgewählten Malebene/des Effekts aufgeführt sind. Pfade lassen sich einfach auswählen und verwalten.

Mit diesem Bedienfeld können Sie:

* Doppelklicken Sie auf einen Pfad, um &quot;<b>umzubenennen</b>&quot;.
* <b>Löschen</b> Sie einen Pfad, indem Sie ihn auswählen und dann die Löschtaste drücken.
* <b>Kopieren</b>/<b>Einfügen</b>/<b>Duplizieren</b> Sie einen Pfad mit den dedizierten Tastaturbefehlen.
* <b>Einblenden</b> oder <b>Ausblenden</b> eines Pfads mit dem Augensymbol (das steuert, ob der Pfad auf die Texturierung angewendet wird).

Der Einfachheit halber können Sie auch mit der rechten Maustaste auf einen Pfad klicken, um das Kontextmenü mit den gleichen Aktionen zu öffnen:

![Rechtsklick-Menü im Bedienfeld &quot;Pfad&quot;](../../assets/path_panel_rightclick_menu_copy_properties.png)

Im Kontextmenü können Sie auch Aktionen öffnen, um die Eigenschaften oder die Position eines Pfads auf einen anderen Pfad zu kopieren. Auf diese Weise können Features problemlos über verschiedene Pfade hinweg freigegeben oder synchronisiert werden:

![Gif zeigt, wie Pfadeigenschaften kopiert und eingefügt werden](../../assets/path_copy_paste_properties.gif)

![Gif zeigt, wie Pfadpositionen kopiert und eingefügt werden](../../assets/path_copy_paste_vertices.gif)

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

Wie andere Werkzeuge können auch Voreinstellungen erstellt werden, um die Pinseleinstellungen/-konfigurationen schnell wiederherzustellen. Klicken Sie dazu einfach mit der rechten Maustaste in das Fenster <b>Eigenschaften</b> und wählen Sie <b>Werkzeugvorgabe erstellen.</b> Diese neu erstellte Vorgabe wechselt automatisch zum Pfadwerkzeug, wenn sie im Fenster <b>Elemente</b> ausgewählt wird.
