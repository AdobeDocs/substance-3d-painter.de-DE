---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/release-notes/old-versions/version-7-3.html"
breadcrumb-title: ''
description: Lesen Sie die Versionshinweise für Substance 3D Painter 7.3, um mehr über neue Funktionen, Verbesserungen und Fehlerbehebungen zu erfahren.
helpx_creative_field: ""
helpx_description: Painter > Release notes > Old versions > Version 7.3
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Version 7.3
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '1822'
ht-degree: 0%

---


# Version 7.3

**Substance 3D Painter 7.3** bietet neue Möglichkeiten für die Texturierung von Meshs mit den neuen Warp- und Zylinder-Projektionen für Füllebenen.

Freigabedatum: *13. Oktober 2021*

## Wichtigste Funktionen

### Neue Verkrümmungs-Projektion

![](../../assets/proj-warp.jpg)

In dieser Version wird die neue 3D-Verkrümmungs-Projektion für Füllebenen und Fülleffekte eingeführt. Diese Projektion erlaubt es, eine Textur oder ein Bild mithilfe eines Deformations-Rasters und steuerbarer Punkte zu verzerren.

* **Schnelle Einrichtung per Drag &amp; Drop** Wählen Sie ein Material, ein Alpha, eine Textur oder ein prozedurale aus der Elementbibliothek, ziehen Sie es und legen Sie es auf den gewünschten Teil des Meshs ab (Tastaturbefehl **ALT** erforderlich für Materialien). Wenn das Element kein Material ist, wird ein Popup mit der Frage angezeigt, welchem Kanal es zugewiesen werden soll.\
  Sobald die Ebene erstellt wurde, wird die neue *Verkrümmungs-Projektion* automatisch ausgewählt. Die Ebene verfügt über standardmäßige Steuerelemente für den 3D-Projektion-Modus, aber auch über den neuen Parameter *Projektion Tiefe*, mit dem die Tiefe der Verkrümmungs-Projektion (dargestellt durch grüne Pfeile als visuelle Warteschlange) festgelegt werden kann.\
  Sie können diesen Projektion-Modus auch manuell für jede Füllebene oder jeden Effekt auswählen, ohne ein Element per Drag &amp; Drop in den Viewport ziehen zu müssen.

  ![](../../assets/drop-viewport-warp.gif)

* **Automatische Platzierung mit dem Oberflächenwerkzeug** Wenn die neue Verkrümmungsebene erstellt wird, wird das Oberflächenwerkzeug automatisch ausgewählt. Auf diese Weise können Sie das Bild so verschieben, dass es immer auf der Oberfläche Ihres Meshs bleibt. Sie können jedoch jederzeit zu einem der anderen Manipulatoren wechseln und dessen Übersetzung (Tastaturbefehl **W**), Drehung (Tastaturbefehl **E**) oder Skalierung (Tastaturbefehl **R**) anpassen. Um zum Oberflächenwerkzeug zurückzukehren, verwenden Sie Tastaturbefehl **UMSCHALT + W**. Wenn Sie in den Modus *Scheitelpunkt bearbeiten* wechseln, ist das Oberflächenwerkzeug auch die Standardauswahl und einrasten die Bewegung des Scheitelpunkts auf die Oberfläche Ihres Meshs bei. Sie können jedoch das Oberflächenwerkzeug vorübergehend und schnell überschreiben, indem Sie **STRG** beibehalten. Dadurch können Sie den ausgewählten Punkt in eine beliebige Richtung verschieben, nicht nur auf der Oberfläche.

* **Einfach bearbeitbarer Verkrümmungs-Raster** Nachdem die globale Platzierung des Bildes abgeschlossen ist, ist es auch möglich, den Verkrümmungs-Raster selbst zu bearbeiten, um eine höhere Präzision und Flexibilität zu erzielen. Um in den Raster-Bearbeitungsmodus zu wechseln, können Sie entweder das neu hinzugefügte Verkrümmungsmenü oder den Tastaturbefehl **UMSCHALT + V** verwenden. Auf diese Weise können Sie bestehende Scheitelpunkt des Rasters bearbeiten.\
  Sie können den Raster insgesamt gleichmäßig unterteilen, aber beachten Sie, dass die Scheitelpunkt, die Sie vorher verschoben haben, auf ihre ursprüngliche Position zurückgesetzt werden. Die Unterteilung von Rastern kann über das neue Menü mit den Verkrümmungsoptionen vorgenommen werden.\
  Alternativ ist es möglich, individuell platzierte Splits hinzuzufügen, die nur bei Bedarf mehr Details ermöglichen würden. Um Teilungen hinzuzufügen, wähle eine der drei Optionen im Menü &quot;Verkrümmen&quot; aus: &quot;Kreuzen&quot;, &quot;Horizontal&quot; oder &quot;Vertikal&quot;. Wenn du einen Clip auswählst und den Cursor über die Projektion &quot;Verformen&quot; bewegst und auf eine beliebige Stelle darin klickst, wird ein neuer Teil hinzugefügt. Dies ändert nichts an der Position der vorhandenen Punkte.

  ![](../../assets/warp-split.gif)
* **Automatische Anpassung der Ausrichtung des Scheitelpunkts** Standardmäßig werden die Tangenten der einzelnen Scheitelpunkt an die Oberfläche des Meshs angepasst, was bedeutet, dass sie immer korrekt in Bezug auf den Mesh ausgerichtet sind, unabhängig davon, wo sie gezogen werden. Diese Option für die automatische Tangente kann über eine neue Schaltfläche in der kontextabhängigen Symbolleiste deaktiviert werden. In diesem Fall bleibt die Ausrichtung jederzeit unverändert.

  ![](../../assets/warp-tangent-adjustment.gif)

Weitere Informationen zu den Einstellungen und Eigenschaften der Verkrümmungsdokumentation finden Sie auf der [dedizierten Dokumentationsseite](../../painting/fill-projections/warp-projection.md) der Projektion &quot;Verkrümmen&quot;.

### Neue Zylinder-Projektion

![](../../assets/cylinder-proj.jpg)

Mit dieser Version wird eine Methode zur zylindrischen Projektion für Füllebenen und Fülleffekte hinzugefügt. Mit der neuen Projektion können Sie ein Bild oder eine Textur um Objekte wie Spalten, Säulen oder mehr organische Formen wie die Arme einer Figur anpassen.

* **Ein Bild um einen Mesh legen**\
  Sie können ein Bild ganz einfach um eine zylindrische Fläche legen, indem Sie eine Füllebene oder einen Fülleffekt verwenden und *Zylindrische Projektion* in der Dropdown-Liste &quot;Projektion&quot; auswählen. Wenn das Bild nicht außerhalb des Projektion-Gizmos wiederholt werden muss, müssen Sie *Keine* für *Bildumbruch* und *Auf Form zugeschnitten* in *Form zuschneiden* auswählen, um sicherzustellen, dass das UV nicht außerhalb der zulässigen Grenzen liegt. Dann müssen Sie nur den Manipulator verwenden, um die Projektion an die gewünschte Position anzupassen.

* **Winkel der Projektion anpassen**\
  Sobald dein Bild an Ort und Stelle ist, ist eine neue Winkeleinstellung verfügbar. Diese Einstellung kann verwendet werden, um einzustellen, ob das Bild vollständig um die zylindrische Form projiziert oder auf einen bestimmten Winkel beschränkt wird. Es schneidet das Bild nicht zu, sondern reduziert seine Breite.

  ![](../../assets/cylindrical-angle.gif)

Weitere Informationen finden Sie auf der [Seite der dedizierten Dokumentation](../../painting/fill-projections/cylindrical-projection.md).

### Verbesserter Farbwähler

![](../../assets/colorpicker-banner.jpg)

Diese Version bietet verschiedene Verbesserungen der Lebensqualität beim Farbwähler.

* **Neues Fensterlayout**\
  Das verbesserte Farbwählerfenster wurde überarbeitet, um ein vertikales Layout zu ermöglichen, das dem der neuesten Version von Sampler ähnelt. Es ist in drei Abschnitte unterteilt - das Hauptfarbfeld, das die aktuelle und letzte Auswahl enthält, das Hexadezimalfeld, die Pipette und den Farbtonregler. den Abschnitt mit den manuellen RGB-/HSV-Reglern; und die Farbfelder.\
  ![](../../assets/colorpicker.jpg)

* **Neue 0-255 RGB-Werte**\
  Neben den bestehenden Möglichkeiten zur Eingabe von Farbwerten ermöglicht der verbesserte Farbwähler auch das Arbeiten mit 0-255 RGB-Werten. Diese Option ist verfügbar, wenn im Dropdownmenü des Schiebereglerabschnitts die Option *Fließkommawert* deaktiviert ist.

  ![](../../assets/colorpicker-floatingpoints.jpg)
* **Farbfelder speichern**\
  Farbfelder können jetzt in Painter gespeichert werden! Sobald die gewünschte Farbe ausgewählt ist, können Sie im Farbfeldbereich des Farbwählers auf das Pluszeichen klicken. Die Farbe wird sitzungs- und projektübergreifend gespeichert. Ein Farbfeld kann gelöscht werden, indem Sie mit der rechten Maustaste darauf klicken, oder alternativ können Sie alle Farbfelder gleichzeitig über das Dropdown-Menü in diesem Abschnitt löschen. Die Anzahl der Farbfelder, die gespeichert werden können, ist nicht begrenzt.

  ![](../../assets/colorpicker-swatches.gif)
* **Das Farbauswahlfenster bleibt geöffnet**\
  Das Farbwählerfenster kann jetzt verschoben und an einer beliebigen Stelle platziert werden, auch auf einem anderen Bildschirm. Es bleibt geöffnet, solange kein Kontextschalter vorhanden ist. Das bedeutet, dass Sie das Farbwählerfenster für einen einfacheren Zugriff geöffnet lassen können, wenn Sie beim Malen von Texturen zwischen den Malebenen wechseln.

  ![](../../assets/picker-persistent.gif)

* **Pipette für mehr Barrierefreiheit**\
  Die Pipette für den Farbwähler befindet sich direkt neben dem Farbfeld. Sie können sie aber auch im Farbwähler finden. Die leichter zugängliche Pipette behält alle vorherigen Funktionen bei - Sie können immer noch klicken und die Maustaste gedrückt halten, um eine Farbe an einer beliebigen Stelle auf Ihrem Bildschirm auszuwählen. Diese gelegt Pipette befindet sich neben allen Farbfeldern in Painter, nicht nur in den Ebenenkanälen.

  ![](../../assets/eyedropper-5.jpg)

Weitere Informationen finden Sie auf der [Seite der dedizierten Dokumentation](../../interface/color-picker.md).

### Weitere Funktionen und Verbesserungen

* **Verbesserungen beim Ziehen und Ablegen von Elementen**\
  Mit der Einführung der Verkrümmung wurde die Aufkleberfunktion, mit der Elemente aus der Bibliothek in den Viewport gezogen und abgelegt werden können, während die ALT-Taste beibehalten wird, überarbeitet. Wenn ein Aufkleber auf diese Weise erstellt wird, verwendet er nicht mehr die Planare Projektion, sondern die Verkrümmen-Projektion. Die automatische Auswahl der Projektion &quot;Verformen&quot; sollte die Geschwindigkeit und Effizienz der Aufkleberanpassungen auf dem Mesh verbessern.\
  Darüber hinaus ist es jetzt möglich, nicht nur Materialien, sondern bildartige Elemente in den Viewport zu ziehen und dort abzulegen. Bei der Auswahl eines Alpha-Elements, einer Textur oder eines prozeduralen Elements ist die Verwendung des ALT-Modifizierers nicht erforderlich. Das Bild kann auf den Mesh abgelegt werden. In diesem Menü kannst du auswählen, ob das Bild in einer Maske oder in einem der Ebenenkanäle verwendet werden soll.

  ![](../../assets/improved-decal.gif)

* **Verbesserung des Plug-ins zum automatischen Speichern**\
  Das automatische Speichern wird nicht mehr bei längeren oder umfangreicheren Vorgängen wie dem Neuladen, Baking oder Exportieren von Meshs ausgelöst.

* **Leistungsverbesserungen**\
  Es wurden einige Wartungsarbeiten und Optimierungen für die Schieberbearbeitung und die Malleistung durchgeführt.

* **Neue Funktionen in der Python-API**\
  Die Python-API hatte einige kürzlich hinzugefügte Funktionen, die es ermöglichen, Mesh neu zu laden, Ressourcen zu aktualisieren sowie die Auflösung von UV-Kacheln über Skripte festzulegen und abzufragen.

* **Substance Engine-Update 8.3.0**\
  Neben einigen Korrekturen und allgemeinen Verbesserungen berücksichtigt dieses Substance Engine-Update jetzt neue Graf. Es ist auch möglich, die .sbsar-Datei-Version zu überprüfen, was die Nutzung und das Herunterladen der entsprechenden Substance 3D Assets-Versionen verbessern sollte.

* **Substance 3D Assets wird vom CC-Desktop empfangen**\
  Es ist jetzt möglich, über die CC-Desktop-Applikation auf Substance 3D Assets wie Materials, Atlanten und Aufkleber zuzugreifen. Außerdem können sie direkt an die Painter Library gesendet werden.

## Versionshinweise

### 7.3.0

*(veröffentlicht am 13. August 2021)*\
Zusammenfassung: **Hauptversion. Es enthält eine neue 3D-Verkrümmungsfunktion, eine neue zylindrische Projektion, Projektionen am Farbwähler, neue Funktionen in der Python-API und Fehlerbehebungen**

**Hinzugefügt:**

* [Projektion]&#x200B;[Verkrümmen] Gelegt 3D-Verkrümmung als neue Projektion
* [Projektion]&#x200B;[Verformen] Erlauben Sie den Aufklebermodus für Alphas, Texturen und Prozedurale mit Drag &amp; Drop im Viewport
* [Projektion]&#x200B;[Verkrümmen] Verwenden Sie die Verkrümmungs-Projektion mit dem Decal-Tastaturbefehl (ALT).
* [Projektion]&#x200B;[Verkrümmen]&#x200B;[Symbolleiste] Transformieren Verkrümmung als Ganzes oder pro Scheitelpunkt
* [Projektion]&#x200B;[Verkrümmen]&#x200B;[Symbolleiste] Fügen Sie Raster-Punkte mit den Optionen &quot;Geteilte Verkrümmung&quot; quer, horizontal oder vertikal hinzu
* [Projektion]&#x200B;[Verkrümmen]&#x200B;[Symbolleiste] Dediziertes Menü für Zurücksetzen-Aktionen
* [Projektion]&#x200B;[Verkrümmen]&#x200B;[Symbolleiste] Option zum automatischen Anpassen der Tangenten beim Verschieben von Punkten
* [Projektion]&#x200B;[Verkrümmen]&#x200B;[Symbolleiste] Spezielles Menü für die Raster-Edition (Größe, Zurücksetzen, Farbe und Griffgröße)
* [Projektion]&#x200B;[Verformen] Neuer Tastatur-Tastaturbefehl zum Schalten des Warp-Editionsmodus für ganze Scheitelpunkt (UMSCHALT+V)
* [Projektion]&#x200B;[Verformen] Klicken + Strg ermöglicht den Wechsel zwischen Flächenwerkzeug und anderen Werkzeugen.
* [Projektion]&#x200B;[Zylindrisch] Gelegt Projektion
* [Projektion]&#x200B;[Symbolleiste] Gruppeneinstellungen für Manipulator (Größe, Raster, Winkelschritte)
* [Farbwähler] Neue Benutzeroberfläche für Farbwähler
* [Farbwähler] Verwenden von sRGB-Werten in Farbwähler-Widgets
* [Farbwähler] Farbfelder speichern und löschen
* [Farbwähler] Pipette, die über Farbkanäle und normale Slots zugänglich ist
* [Farbwähler] Dynamische Farbe zwischen 0 und 255 Werten bearbeiten
* [Farbwähler] Gemeinsamer HSV-/RGB-Status in der App
* [Farbwähler] Das Fenster &quot;Farbwähler&quot; ist halbpersistent.
* [Farbwähler] Durch Drücken von Esc wird das Farbwählerfenster geschlossen.
* Leistungsverbesserung für UI-Interaktion und beim Malen
* [Engine] Update auf die neue Substance-Engine-Version (8.3.0)
* [Scripting]&#x200B;[Python] Ermöglicht das erneute Laden des Meshs des aktuellen Projekts.
* [Scripting]&#x200B;[Python] Aktualisieren von Ressourcen in Projekten zulassen
* [Scripting]&#x200B;[Python] Festlegen und Abfragen der Auflösung von UV-Kacheln zulassen
* [Interoperabilität] Nicht verfügbar für Steam- und Substance-Editionen
* [Interoperabilität] Empfangen mehrerer Ressourcen von Bridge

**Fest:**

* Der Farbwähler zeigt nicht die richtige Farbe an
* [Baking] Liste der Textursatz ist nicht korrekt angeordnet
* [FBX Import] 3ds Max-Gruppen-Pivot-Transformationen werden nicht berücksichtigt
* [Substance Engine] Absturz beim Importieren von beschädigtem SBSAR
* [MacOS] Projektkonfigurationsoption in verschiedenen Sprachen ist nicht vorhanden.
* Automatische Speicherung kann Painter während langer Prozesse einfrieren

**Bekannte Probleme:**

* [Projektion]&#x200B;[Verformen] Die Option &quot;Teilen&quot; bleibt nach dem Teilen ausgewählt.
* [Projektion]&#x200B;[Verkrümmen] Spiegeln funktioniert nicht, wenn die Transformation auf Welt-Raum festgelegt ist
* [Projektion]&#x200B;[Verformen] Artefaktlinien zwischen Patches in seltenen Fällen
* [Projektion]&#x200B;[UV] Der Drehpunkt wird beim Spiegeln der Projektion zurückgesetzt.
* [Mac M1] Smart-Materialien werden nicht korrekt angezeigt
* [M1]&#x200B;[Regression] Materialschichtung funktioniert nicht
