---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/pipeline-and-integration/configuration/remote-desktop.html"
breadcrumb-title: ''
description: Hier erfahren Sie, wie Sie Substance 3D Painter für den Remote-Desktopzugriff konfigurieren, um Remote-Workflows und die Zusammenarbeit zu ermöglichen.
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Configuration > Remote Desktop
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Remotedesktop
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---


# Remotedesktop

Auf dieser Seite werden Lösungen und Alternativen beschrieben, mit denen Substance 3D Painter über Remote Desktop (RDP) unter Windows ausgeführt werden kann.

Standardmäßig wird RDP unter Windows in einem OpenGL-Kontext ausgeführt, der nicht vorhanden oder zu niedrig ist, wodurch die Anwendung nicht ordnungsgemäß funktionieren oder abstürzen kann. Substance 3D Painter erfordert einen OpenGL 3.3-Kontext. Im Folgenden finden Sie Lösungen, um das Problem zu beheben, aber es gibt keine Garantien, dass sie funktionieren, da das ursprüngliche Problem von Windows und einigen GPU-Treibern abhängt.

>[!NOTE]
>
> Nvidia Quadro-GPUs können die Anwendung standardmäßig im RDP-Modus ausführen, während Nvidia GeForce-GPUs nur einen OpenGL 1.4-Kontext bereitstellen (was für Substance 3D Painter zu niedrig ist). Es ist möglich, eine ausführbare Datei zu installieren, um dies zu beheben, siehe: <https://developer.nvidia.com/designworks>

## Windows-Richtlinienkonfiguration

Unter Windows 10 muss möglicherweise die **Gruppenrichtlinie** geändert werden, damit die GPU im RDP-Modus ausgeführt werden kann.

Gehen Sie folgendermaßen vor:

1. Drücken Sie **Win + R**, um das Ausführungsfenster zu öffnen.
1. Geben Sie &quot;**gpedit.msc** &quot; ein, und geben Sie dann Folgendes ein:
1. Navigieren Sie zu **Richtlinie des lokalen Computers\Computerkonfiguration\Verwaltungsvorlagen\Windows-Komponenten\Remotedesktopdienste\Remotedesktop-Sitzungshost\Remotesitzungsumgebung**.
1. Aktivieren Sie die Option **Standardgrafikadapter für alle Remotedesktopdienste-Sitzungen verwenden** .

## Windows TSCON-Befehl

Wenn die vorherige Richtlinienänderung nicht funktioniert, können Sie versuchen, die Befehlszeile **tscon** zu verwenden. Dieser Befehl trennt den Remote-Computer und verbindet einen neuen mit der physischen Hardware (Maus, Tastatur usw.). Wenn Sie dann die Anwendung einfach ausführen und eine Remote-Verbindung wiederherstellen, sollte es möglich sein, mit der Anwendung auf der GPU zu arbeiten.

1. Drücken Sie die Taste **Windows+R**, um das Fenster **execute** zu öffnen.
1. Geben Sie **cmd** ein und drücken Sie die **Eingabetaste** .
1. Geben Sie in der Befehlszeile Folgendes ein:  **tscon 1 /dest:console**
1. Eingabetaste drücken
1. Geben Sie in der Befehlszeile den folgenden Befehl ein:  **Starten Sie &quot;Path/To/Substance/Painter/Folder/Substance 3D Painter.exe&quot;** (stellen Sie sicher, dass der Pfad dem Computer entspricht).
1. Eingabetaste drücken

Warten Sie nach diesen Schritten einige Sekunden, bis die Anwendung gestartet wird, und stellen Sie dann die Verbindung zur Sitzung wieder her.

Falls dieses Verfahren nicht funktioniert, müssen Sie die Windows-Befehlszeile möglicherweise im Administratormodus ausführen.

## Alternativen

Wenn vorherige Vorschläge immer noch nicht funktionieren, empfehlen wir alternative Lösungen wie VNC oder Teamviewer zu verwenden, die die GPU über Remote-Verbindungen unterstützen.
