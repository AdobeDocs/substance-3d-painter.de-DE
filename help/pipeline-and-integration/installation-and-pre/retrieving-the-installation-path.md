---
breadcrumb-title: ""
description: Erfahren Sie, wie Sie den Installationspfad für Substance 3D Painter für Skripterstellung und Pipelineintegration abrufen.
title: Ermitteln des Installationspfads
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 6%
---

# Ermitteln des Installationspfads

Auf dieser Seite werden Informationen darüber neu gruppiert, wie der Installationspfad der Anwendung je nach Version und Plattform abgerufen werden kann.

## Windows

### Creative Cloud Desktop

1. Öffnen Sie den Windows-Registrierungseditor (**regedit**).
1. Navigieren Sie zum Registrierungsschlüssel: ** HKEY\_LOCAL\_MACHINE\Software\Microsoft\Windows\CurrentVersion\App Pfade\**
1. Öffnen Sie den Unterschlüssel &quot;**Adobe Substance 3D Painter.exe**&quot;.
1. Der Wert des Schlüssels enthält den Pfad zur ausführbaren Anwendungsdatei, in der er installiert ist

>[!NOTE]
>
> Dieser Registrierungsschlüssel ist nur seit Version 7.2 verfügbar.\
>  Bei älteren Versionen kann der Installationspfad aus den Dateizuordnungen in **HKEY\_CURRENT\_USER\Software\Microsoft\Windows\CurrentVersion\ Explorer\FileExts** abgerufen werden.

### Substance 3D Standalone

1. Öffnen Sie den Windows-Registrierungseditor (**regedit**).
1. Navigieren Sie zum Registrierungsschlüssel: **HKEY\_LOCAL\_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Uninstall**
1. Suchen Sie den Unterschlüssel, der mit der AppID Ihrer Anwendungsversion übereinstimmt (siehe Tabelle unten).
1. Der Wert des Schlüssels enthält den Pfad zum Speicherort der Anwendungsinstallation

| Version | AppId |
| --- | --- |
| **Version 1.x** | `{410F5B6E-A29C-4F43-9DE3-44A1357D6AF5}` |
| **Version 2.x** | `{f42b7a996fa1d13a1d0a2e33eea2c0800bb5d1b8}` |
| **3.x (2017.x) bis 7.1** | `{33C3E9E2-0675-4196-9019-28AB9C5E9BB0}` |
| **7.2 oder neuer** | `{2a8bbb68-725b-477c-9194-60efc5ece348}` |

### dämpfen

Die Anwendung wird im Unterordner **steamapps/common/** des Steam-Installationsordners installiert.

## Mac

Unter Mac wird die Anwendung wie folgt installiert:

| Version | Pfad |
| --- | --- |
| **7.2 oder neuer** | **/Applications/Adobe Substance 3D Painter.app** |
| **Veraltet** | **/Applications/Substance Painter.app** |

## Linux

Unter Linux wird das rpm-Paket unter folgendem Pfad installiert:

| Version | Pfad |
| --- | --- |
| **7.2 oder neuer** | **/opt/Adobe/Adobe\_Substance\_3D\_Painter** |
| **Veraltet** | **/opt/Allegorithmic/Substance\_Painter** |
