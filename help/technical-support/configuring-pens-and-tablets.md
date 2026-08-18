---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/configuring-pens-and-tablets.html"
breadcrumb-title: ''
description: Hier erfahren Sie, wie Sie in Substance 3D Painter Stifte und Tablets für eine optimale Druckempfindlichkeit und Zeichenerfahrung konfigurieren.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Configuring Pens and Tablets
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Konfigurieren von Stiften und Tablets
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '877'
ht-degree: 0%

---


# Konfigurieren von Stiften und Tablets

Auf dieser Seite finden Sie mehrere Empfehlungen zur Konfiguration eines Grafiktablettstifts unter Windows, um die Kompatibilität mit der Anwendung zu verbessern.

## Was ist Windows Ink?

Windows Ink ist eine Software/ein Dienst, die Stifte wie Stifte oder Stifte von Grafiktabletts verarbeitet. Es bietet verschiedene Anwendungen wie Notizen und Skizzenblock, um mit einem Stift auf dem Computer zu interagieren.

Seit der Version 2019.3 ist die Anwendung für Grafiktabletts darauf angewiesen. Vor dieser Version wurde stattdessen Wintab verwendet (älterer Dienst, der nicht von allen Grafiktablett-Modellen unterstützt wird).

## Aktivieren von Windows Ink in Tablet-Treibereinstellungen

Um sicherzustellen, dass der Stiftdruck richtig erkannt wird, muss Windows Ink in den Treibereinstellungen des Grafiktabletts aktiviert sein.

>[!NOTE]
>
> Windows Ink wird auf virtuellen Computern nicht unterstützt, daher werden Grafiktablett-Ereignisse nicht an die Anwendung weitergeleitet. Der Stiftdruck wird daher in dieser Konfiguration nicht unterstützt.

### Aktivieren von Windows Ink für Wacom-Tablets

1. Öffnen Sie das Menü **Start**.
1. Geben Sie **Wacom Tablet Properties** ein, und klicken Sie auf das erste Suchergebnis.
1. Klicken Sie im Fenster **Wacom Tablet Properties** auf den **Stift** in der Werkzeugliste.\
   ![](../assets/wacom-tool-pen.png)
1. Klicken Sie auf die Schaltfläche mit dem Pluszeichen **&quot;+&quot;**, um ein Anwendungsprofil hinzuzufügen.\
   ![](../assets/wacom-profile-plus.png)
1. Klicken Sie im neuen Fenster auf die Schaltfläche **Durchsuchen**, um die ausführbare Substance 3D Painter-Datei zu suchen.\
   ![](../assets/wacom-profile-browse.png)
1. Klicken Sie auf **OK**, um das Profil zu validieren und zu erstellen.\
   ![](../assets/wacom-profile-sp.png)
1. Klicken Sie auf die Registerkarte **Zuordnung**.\
   ![](../assets/wacom-tab-mapping.png)
1. Vergewissern Sie sich links unten im Fenster, dass **Windows Ink verwenden** aktiviert ist.\
   ![](../assets/wacom-use-windows-ink.png)

>[!NOTE]
>
> Starten Sie nach dem Aktivieren von Windows Ink die Anwendung neu, um sicherzustellen, dass die Änderungen ordnungsgemäß berücksichtigt werden.

### Aktivieren von Windows Ink für Huion-Tablets

1. Öffnen Sie das Menü **Start**.
1. Geben Sie **Huion Tablet** ein, und klicken Sie auf das erste Suchergebnis.
1. Klicken Sie im Fenster **Huion Tablet** auf **Digital Pen** .\
   ![](../assets/huion-pen-settings.png)
1. Vergewissern Sie sich links unten im Fenster, dass **Windows Ink aktivieren** aktiviert ist.\
   ![](../assets/huion-pen-winink.png)

## So greifen Sie auf Windows Ink-Einstellungen zu

Auf die Windows Ink-Einstellungen können Sie in den allgemeinen Windows-Einstellungen zugreifen:

1. Öffnen Sie das Menü **Start**.
1. Klicken Sie auf das Symbol **Einstellungen**.\
   ![](../assets/setting-menu-start.png)
1. Klicken Sie im Fenster Einstellungen auf **Geräte** .\
   ![](../assets/settings-device.png)
1. Klicken Sie im Fenster **Geräte** auf **Stift &amp; Windows Ink** (nur verfügbar, wenn ein Grafiktablett angeschlossen ist).\
   ![](../assets/setting-pen-windows-ink.png)

## Empfohlene Windows Ink-Einstellungen

Im Folgenden finden Sie die Windows Ink-Einstellungen und die empfohlene Konfiguration für jede dieser Einstellungen.

>[!NOTE]
>
> Auch nach der Befolgung dieses Leitfadens sind einige Grafiken im Zusammenhang mit Windows Ink weiterhin sichtbar. Leider bietet Microsoft unter Windows keine Einstellungen zur Deaktivierung an.
> 
> Die restlichen Grafiken sind:
> 
> * **Kreis** beim Rechtsklick.
> * **QuickInfo** unter der Maus beim Drücken eines Tastenmodifikators (Strg, Alt oder Umschalt).

### Zeichenstift-Einstellungen

![](../assets/ink-settings-main.png)

| ***Einstellung*** | ***Beschreibung*** |
| --- | --- |
| **Wählen Sie die Hand aus, mit der geschrieben werden soll** | Empfohlen:  **Rechte Hand** Diese Einstellungen steuern, wie die Stiftausrichtung erkannt wird. Wenn Sie diese Einstellung auf &quot;Linke Hand&quot; festlegen, kann es beim Anpassen von Parametern zum Einfrieren der Benutzeroberfläche kommen. |
| **Visuelle Effekte anzeigen** | Empfohlen:  **Deaktiviert** Diese Einstellungen steuern visuelle Effekte, die während verschiedener Zeichenstift-Interaktionen angezeigt werden. Wenn du die Option deaktivierst, kannst du den Effekt &quot;Kreis und Lücke schließen&quot; ausblenden, wenn du klickst: <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../assets/windows-pen-ripple-circle.jpg"/></div> |
| **Zeiger anzeigen** | Empfohlen:  **Deaktiviert** |
| **Verwenden des Stifts als Maus in einigen Desktop-Anwendungen** | Empfohlen:  **Aktiviert** Mit diesen Einstellungen kann der Grafiktablettstift normale Mauseingaben senden. Wenn diese Einstellung deaktiviert ist, kann dies zu Interaktionsproblemen mit UI-Parametern führen. |

### Handschrifteneinstellungen

![](../assets/ink-settings-handwriting.png)

| ***Einstellung*** | ***Beschreibung*** |
| --- | --- |
| **Schriftgröße beim direkten Schreiben in das Textfeld** | Empfohlen:  **Mittel (Standard)** |
| **Schriftart bei Verwendung von Handschrift** | Empfohlen:  **Segoe-Benutzeroberfläche (Standard)** |
| **Wenn ich mit dem Stift auf ein Textfeld tippe, geben Sie den Text manuell ein** | Empfohlen:  **Nur im Tablet-Modus** Diese Einstellungen steuern, wie und wann das Eingabefenster für Handschrifttext angezeigt wird. Wenn diese Option nicht auf &quot;Nur im Tablet-Modus&quot; eingestellt ist, wird das Fenster jedes Mal angezeigt, wenn ein Textfeld in der Benutzeroberfläche ausgewählt wird. Zum Beispiel, wenn Sie einen bestimmten Wert in einen Schieberegler eingeben. |
| **Verwenden des Stifts als Maus in einigen Desktop-Anwendungen** | Empfohlen:  **Aktiviert** Mit diesen Einstellungen kann der Grafiktablettstift normale Mauseingaben senden. Wenn diese Einstellung deaktiviert ist, kann dies zu Interaktionsproblemen mit UI-Parametern führen. |
| **Mit der Fingerspitze in das Handschriftenfeld schreiben** | Empfohlen:  **Deaktiviert** |

### Einstellungen für Zeichenstift-Tastaturbefehle

![](../assets/ink-settings-pen.png)

| ***Einstellung*** | ***Beschreibung*** |
| --- | --- |
| **Einmal klicken** | Empfohlen:  **Nichts** |
| **Doppelklicken auf** | Empfohlen:  **Nichts** |
| **Drücken und Halten (wird nur bei einigen Stiften unterstützt)** | Empfohlen:  **Nichts** |
| **Apps das Überschreiben der Verknüpfungsschaltfläche erlauben (Verhalten)** | Empfohlen:  **Aktiviert** |
| **Wenn verfügbar, Arbeitsbereich &quot;Tinte&quot; anzeigen, nachdem ich meinen Stift aus dem Speicher entfernt habe** | Empfohlen:  **Deaktiviert** |

## So greifen Sie auf Zeichenstift- und Touch-Einstellungen zu

Auf die Einstellungen für Stift und Touch kann über die Systemsteuerung zugegriffen werden:

1. Öffnen Sie das Menü **Start**.
1. Geben Sie **Systemsteuerung** ein, und klicken Sie auf das erste Suchergebnis.
1. Wechseln Sie im Anzeigemodus der Systemsteuerung **&#x200B;**&#x200B;zum **kleinen Symbol** .\
   ![](../assets/control-panel-display-mode.png)
1. Klicken Sie auf **Zeichenstift- und Touch**-Einstellungen.\
   ![](../assets/control-panel-pen-touch-settings.png)

## Empfohlene Stift- und Touch-Einstellungen

Die folgenden Einstellungen werden empfohlen, um das Malverhalten und die Kamerabewegung zu verbessern.

Um auf die Einstellungen zuzugreifen, klicken Sie im Fenster auf eine der **Aktionen zum Öffnen** und dann auf die Schaltfläche **Einstellungen**.

![](../assets/control-panel-settings.png)

| ***Einstellung*** | ***Beschreibung*** |
| --- | --- |
| **Einfaches Tippen** | Keine Parameter. |
| **Doppeltippen** | Empfohlen:  **Standardwerte.** |
| **Drücken und halten** | Empfohlen:  **Deaktivieren Sie die Einstellung &quot;Drücken und Halten für Rechtsklick aktivieren&quot;** Wenn Sie diese Einstellung deaktivieren, können Sie jedes Element normal ziehen, ohne den Windows-Ziehkreis zu aktivieren: <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r3-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../assets/windows-pen-drag-circle.jpg"/></div> |
| **Verwenden Sie die Schaltfläche &quot;Öffnen&quot; als Äquivalent mit der rechten Maustaste** | Empfohlen:  **Aktiviert** |
| **Verwenden Sie die Oberseite des Stifts, um die Druckfarbe zu löschen (sofern verfügbar)** | Empfohlen:  **Aktiviert** |
