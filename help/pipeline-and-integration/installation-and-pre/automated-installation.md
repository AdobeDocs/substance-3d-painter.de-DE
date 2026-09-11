---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/pipeline-and-integration/installation-and-preferences/automated-installation.html"
breadcrumb-title: ''
description: Hier erfahren Sie, wie Sie die Installation von Substance 3D Painter für Arbeitsabläufe zur Unternehmensbereitstellung und Pipelineintegration automatisieren.
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Installation and preferences > Automated installation
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Automatisierte Installation
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '129'
ht-degree: 0%

---


# Automatisierte Installation

Bei Verwendung des eigenständigen Substance 3D-Installationsprogramms ist es möglich, die Anwendung zur einfacheren Bereitstellung im Hintergrund zu installieren.

Wir verwenden **InnoSetup** zum Generieren des Installationsprogramms. Der gesamte Parametersatz, der mit dem Installationsprogramm verwendet werden kann, ist hier [verfügbar](http://www.jrsoftware.org/ishelp/index.php?topic=setupcmdline).

## Installation im Hintergrund über die Befehlszeile

Das Flag, das zum Ausführen einer unbeaufsichtigten Installation verwendet werden soll, ist **/SILENT**. Das Flag **/NCRC** kann auch verwendet werden, um die CRC (Überprüfung) des Pakets zu überspringen, um den Prozess zu beschleunigen.

Beispiel:

```
SubstancePainter_Installer.exe /NCRC /SILENT /DIR="C:InstallationFolder"
```


>[!NOTE]
>
> Der Installationspfad muss einen einzelnen umgekehrten Schrägstrich verwenden, um Ordner zu trennen, andernfalls erkennt das Installationsprogramm den Pfad nicht.
