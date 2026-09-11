---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/pipeline-and-integration/resource-management/preferences-and-content-migration.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie Voreinstellungen und Inhalte in Substance 3D Painter migrieren, wenn Sie ein Upgrade oder einen Wechsel auf ein neues System durchführen.
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Resource management > Preferences and content migration
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Voreinstellungen und Inhaltsmigration
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '484'
ht-degree: 1%

---


# Voreinstellungen und Inhaltsmigration

Auf dieser Seite wird beschrieben, wie Daten aus den Voreinstellungen und Regalen/Assets migriert werden, um sie in den neuen Versionen zu verwenden.

Nach der Veröffentlichung von Version 7.2 wurden die Voreinstellungen und der Speicherort des Regals geändert, um sie in den verschiedenen Versionen der Anwendung (eigenständige Substance 3D-, Steam- und Creative Cloud-Desktop-Version) gemeinsam zu nutzen. Diese Änderung bedeutet, dass vorherige Voreinstellungen und benutzerdefinierte Ressourcen **jetzt standardmäßig ignoriert** werden (**, aber nicht verloren**). Da das **Regal** in **Elemente** umbenannt wurde, umfasst die Migration einige der unten beschriebenen Schritte.

## Migrieren von Regal- und Asset-Ressourcen

Der Ressourcenspeicherort des Standardbenutzers hat sich geändert, was bedeutet, dass jeder Inhalt, der in den Ordner &quot;Dokumente&quot; verschoben wurde, jetzt von neuen Versionen der Anwendung ignoriert wird. Um diesen Inhalt wiederherzustellen, verschieben Sie die Dateien einfach von einem Speicherort an einen anderen.

### Wo finde ich Inhalte?

Der Pfad zum Regal oder zu den Elementen befindet sich an folgenden Speicherorten:

<table data-preserve-html="true" style="width: 100.0%;"><colgroup> <col style="width: 15.0%;"/> <col style="width: 15.0%;"/> <col style="width: 70.0%;"/> </colgroup><tbody><tr><th>Plattform</th><th>Version</th><th>Pfad</th></tr><tr><td rowspan="2"><strong>Windows</strong></td><td><strong>7.2</strong> oder höher</td><td colspan="1">C:\Users\username\Documents\Adobe\Adobe Substance 3D Painter</td></tr><tr><td colspan="1">Alte Version</td><td colspan="1">C:\Users\username\Documents\Allegorithmic\Substance Painter</td></tr><tr><td rowspan="2"><strong>Mac</strong></td><td colspan="1"><strong>7.2</strong> oder höher</td><td colspan="1">/Users/Benutzername/Documents/Adobe/Adobe Substance 3D Painter</td></tr><tr><td colspan="1">Alte Version</td><td colspan="1">/Users/Benutzername/Documents/Allegorithmic/Substance Painter</td></tr><tr><td rowspan="2"><strong>Linux</strong></td><td colspan="1"><strong>7.2</strong> oder höher</td><td colspan="1">/home/username/Documents/Adobe/Adobe Substance 3D Painter</td></tr><tr><td>Alte Version</td><td colspan="1">/home/username/Documents/Allegorithmic/Substance Painter</td></tr></tbody></table>

### Migrieren von Regal-Inhalten

Bei den alten Regalen handelt es sich nur um Dateien auf der Festplatte. Bei der Migration geht es also nur darum, diese Dateien an der richtigen Stelle zu platzieren.

1. Schließen der Anwendung
1. Navigieren Sie zum alten Regal-Ordner
1. Kopieren oder Ausschneiden der Unterordner (Alphas, Prozedurale, Materialien usw.)
1. Navigieren Sie zum neuen Assets-Ordner
1. Fügen Sie die Unterordner ein, die Sie zuvor in den Ordner &quot;Assets&quot; kopiert haben. Überschreiben Sie sie, wenn Sie dazu aufgefordert werden.

Starten Sie die Anwendung neu, und der Inhalt sollte jetzt im Fenster &quot;Elemente&quot; angezeigt werden.

>[!NOTE]
>
> Achten Sie darauf, die Unterordner und nicht nur den übergeordneten Ordner der Ressourcen zu kopieren. Der übergeordnete Ordner wurde von &quot;**Regal**&quot; in &quot;**Elemente**&quot; umbenannt. Wenn Sie also nur den übergeordneten Ordner kopieren, werden die Ressourcen für die Anwendung nicht sichtbar.

### Regal-Presets migrieren

Regal-Vorgaben werden in einer Konfigurationsdatei gespeichert. So migrieren Sie diese Vorgaben:

1. Schließen der Anwendung
1. Navigieren Sie zum alten Regal-Ordner
1. Kopieren oder schneiden Sie die Datei Regal.ini
1. Navigieren Sie zum neuen Assets-Ordner
1. Einfügen der Datei und Überschreiben der vorhandenen Datei

Starten Sie die Anwendung neu. Die gespeicherten Suchvorgänge sollten nun im entsprechenden Abschnitt oder im Fenster &quot;Elemente&quot; angezeigt werden.

## Migration der Voreinstellungen

Es wird empfohlen, die Anwendungseinstellungen manuell über die Benutzeroberfläche anzupassen. Dies ist der sicherste Weg, um Informationen ohne Kompatibilitätsprobleme zu migrieren.

Andernfalls sehen Sie sich die folgende Seite an, um zu erfahren, wo sich die Voreinstellungen jetzt befinden: [Speicherort von Voreinstellungen und Anwendungsdaten](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/application-preferences-location-147095594.html).
