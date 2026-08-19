---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/pipeline-and-integration/installation-and-preferences/preferences-and-application-data-location.html"
breadcrumb-title: ''
description: Informieren Sie sich über die Speicherorte von Voreinstellungen und Anwendungsdaten für Substance 3D Painter zum Verwalten von Einstellungen und Benutzerdaten.
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Installation and preferences > Preferences and application data location
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Speicherort von Voreinstellungen und Anwendungsdaten
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 4%

---


# Speicherort von Voreinstellungen und Anwendungsdaten

Auf dieser Seite werden Informationen zum Speicherort der Anwendungsvoreinstellungen für die jeweilige Version und Plattform neu gruppiert.\
Es kann nützlich sein, zu wissen, wo Voreinstellungen gespeichert sind, falls Sie **benutzerdefinierte Shelfs** hinzufügen möchten (für Studioinstallationen) oder diese Voreinstellungen entfernen möchten, um eine **Neuinstallation** der Anwendung durchzuführen.

## Voreinstellungen

Dieser Pfad enthält die Einstellungen der Anwendung (gespeicherte Verknüpfungen, Shelf-/Asset-Pfade, Schnittstellenlayout usw.).

<table data-preserve-html="true"><colgroup> <col/> <col/> <col/> </colgroup><tbody><tr><th>System</th><th>Version</th><th>Pfad</th></tr><tr><td rowspan="2"><p><strong>Windows</strong></p><p>(Registrierung)</p></td><td><strong>7.2</strong> oder höher</td><td>HKEY_CURRENT_USER\Software\Adobe\Adobe Substance 3D Painter</td></tr><tr><td>Alte Version</td><td>HKEY_CURRENT_USER\Software\Allegorithmic\Substance Painter</td></tr><tr><td rowspan="2"><p><strong>Mac</strong></p><p>(Bibliothek)</p></td><td><strong>7.2</strong> oder höher</td><td>/Users/[Benutzername]/Library/Preferences/com.adobe.Adobe Substance 3D Painter.plist</td></tr><tr><td>Alte Version</td><td>/Users/[Benutzername]/Library/Preferences/com.substance3d.Substance Painter.plist</td></tr><tr><td rowspan="2"><strong>Linux</strong></td><td><strong>7.2</strong> oder höher</td><td>/home/[Benutzername]/.config/Adobe/Adobe Substance 3D Painter.conf</td></tr><tr><td>Alte Version</td><td>/home/[Benutzername]/.config/Allegorithmic/Substance Painter.conf</td></tr></tbody></table>

## Anwendungsdaten

Dieser Pfad enthält die zusätzlichen Anwendungsdaten (Miniaturansichten der Elemente, Protokolldatei usw.).

<table data-preserve-html="true"><colgroup> <col/> <col/> <col/> <col/> </colgroup><tbody><tr><th>Plattform</th><th>Version</th><th colspan="2">Pfad</th></tr><tr><td rowspan="4"><strong>Windows</strong></td><td rowspan="2"><strong>7.2</strong> oder höher</td><td colspan="1">App-Daten (lokal)</td><td colspan="1">C:\Users\[Benutzername]\AppData\Local\Adobe\Adobe Substance 3D Painter</td></tr><tr><td colspan="1">App-Daten (Roaming)</td><td colspan="1">C:\Users\[Benutzername]\AppData\Roaming\Adobe\Adobe Substance 3D Painter</td></tr><tr><td rowspan="2">Alte Version</td><td colspan="1">App-Daten (lokal)</td><td colspan="1">C:\Users\[Benutzername]\AppData\Local\Allegorithmic\Substance Painter</td></tr><tr><td colspan="1">App-Daten (Roaming)</td><td colspan="1">C:\Users\[Benutzername]\AppData\Roaming\Allegorithmic\Substance Painter</td></tr><tr><td rowspan="2"><strong>Mac</strong></td><td colspan="1"><strong>7.2</strong> oder höher</td><td colspan="2">/Users/[Benutzername]/Library/Application Support/Adobe/Adobe Substance 3D Painter</td></tr><tr><td colspan="1">Alte Version</td><td colspan="2">/Users/[Benutzername]/Library/Application Support/Allegorithmic/Substance Painter</td></tr><tr><td rowspan="2"><strong>Linux</strong></td><td colspan="1"><strong>7.2</strong> oder höher</td><td colspan="2">/home/[Benutzername]/.local/share/Adobe/Adobe Substance 3D Painter</td></tr><tr><td>Alte Version</td><td colspan="2">/home/[Benutzername]/.local/share/Allegorithmic/Substance Painter</td></tr></tbody></table>

>[!NOTE]
>
> Einige der Verzeichnisse in den oben genannten Pfaden sind möglicherweise standardmäßig ausgeblendet. Geben Sie den Pfad manuell im Datei-Explorer ein oder zeigen Sie ausgeblendete Dateien an, um sie anzuzeigen.
