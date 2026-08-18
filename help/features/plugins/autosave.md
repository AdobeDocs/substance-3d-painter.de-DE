---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/features/plugins/autosave.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie das Plug-in "Automatisch speichern" in Substance 3D Painter verwenden, um Ihre Projekte automatisch in regelmäßigen Abständen zu speichern.
helpx_creative_field: ""
helpx_description: Painter > Features > Plugins > Autosave
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Automatisches Speichern
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '375'
ht-degree: 0%

---


# Automatisches Speichern

![](../../assets/autosave-details.png){width="500px"}

Mit den Plug-ins zum automatischen Speichern können **Sicherungen** des derzeit geöffneten Projekts erstellen. Es wird eine Datei auf der Seite erstellt, während das aktuelle Projekt unverändert bleibt.

Die Sicherungsdateien befinden sich an drei möglichen Speicherorten:

* Wenn das aktuelle Projekt gespeichert wurde, werden die Sicherungen daneben angezeigt.
* Wenn das Projekt noch nie gespeichert wurde (ohne Titel), befinden sich die Sicherungen im Ordner &quot;Dokumente&quot; des Benutzers, der automatisch gespeichert wird. ( **Dokumente/Allegorithmic/Substance 3D Painter/autosave** )
* Wenn die Außerkraftsetzungseinstellung aktiviert wurde, befinden sich die Sicherungen in dem Pfad, der in den Einstellungen angegeben ist.

*In der Schnittstelle ist eine Schaltfläche zum automatischen Speichern verfügbar, um das automatische Speichern zu verzögern.*

## Wie löst das automatische Speichern aus?

Das automatische Speichern basiert auf einem internen Zeitgeber, sobald der Zeitgeber über dem automatischen Speichervorgang ist.\
Die Schlummertaste aktiviert sich, wenn sich der Timer dem Ende nähert, sodass das automatische Speichern um einige Zeit verzögert werden kann.

Alle zeitbasierten Werte können über das Einstellungsfenster geändert werden.

## Wie deaktiviere ich das automatische Speichern?

Wenn es aus irgendeinem Grund notwendig ist, den automatischen Speichervorgang zu deaktivieren, kann dies über das Plug-in-Menü erfolgen. Klicken Sie dazu auf das Menü **Plug-ins** > **Automatisches Speichern** > **Deaktivieren**.

## Konfigurieren der automatischen Speicherung

Um das automatische Speicherverhalten zu konfigurieren, klicken Sie auf das Menü **Plug-Ins** > **Automatisches Speichern** > **Konfigurieren**.

* **Automatisches Speicherintervall in Minuten** : Geben Sie an, wie lange zwischen jedem automatischen Speichern gewartet werden soll.
* **Anzahl automatisch gespeicherter Dateien** : die Anzahl der Backup-Dateien, die maximal für ein bestimmtes Projekt erstellt wurden.
* **Intervall in Minuten zum Snooze**: wie lange die automatische Speicherung verzögert wird, wenn auf die Schaltfläche zum Speichern geklickt wird.
* **Warnungszeit vor dem Speichern in Sekunden** : wie lange, bevor die Schaltfläche zum automatischen Speichern aktiviert ist und die Fortschrittsleiste vor dem Auslöser für das automatische Speichern angezeigt wird.

>[!NOTE]
>
> Der Zeitgeber für das automatische Speichern wird angehalten, wenn:
> 
> * Der Motor berechnet
> * Texturen werden exportiert
> * Das Konfigurationsfenster ist geöffnet
> * Das Projekt wird derzeit gespeichert.

Am unteren Rand des Fensters können Sie den Standardspeicherort der Sicherungsdateien überschreiben.\
Wenn die Einstellung &quot;**Immer im folgenden Verzeichnis speichern** &quot; aktiviert ist, befindet sich die gesamte Sicherungsdatei im angegebenen Ordner (Standardpfad ist der Ordner &quot;Dokumente&quot; des Benutzers).
