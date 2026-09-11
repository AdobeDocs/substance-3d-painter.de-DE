---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/gpu-issues/painter-doesn-t-start-on-the-right-gpu.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie Substance 3D Painter so konfigurieren, dass es auf der richtigen GPU startet, um eine optimale Leistung und Kompatibilität zu erzielen.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > GPU Issues > Painter doesnt start on the right GPU
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Painter startet nicht auf der rechten GPU
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '624'
ht-degree: 0%

---


# Painter startet nicht auf der rechten GPU

Unter Windows verwendet die Anwendung beim Start möglicherweise nicht die richtige GPU, was zu Leistungs- und Stabilitätsproblemen führen kann. Im Folgenden finden Sie eine Liste der häufigsten Probleme und deren Lösungen, um sicherzustellen, dass die Software mit der richtigen GPU funktioniert.

Um zu erfahren, welche GPU verwendet wird, können Sie die [Protokolldatei](../../exporting-the-log-file.md) überprüfen.

## Windows

### Konfiguration der Monitorkabel

Unter Windows hängt die einer Anwendung zugewiesene GPU vom Monitor ab, auf dem die Anwendung ausgeführt wird. Dies liegt daran, dass die Monitorkabel direkt mit dem Ausgang der GPU selbst verbunden sind. Die Anwendung kann daher auf der falschen GPU starten, wenn der Monitor, auf dem sie gestartet wird, mit der Grafikausgabe der Hauptplatine verknüpft ist, anstatt mit der Grafikkarte selbst. In diesem Fall verwendet Windows wahrscheinlich die integrierte GPU anstelle der dedizierten GPU.

<b>So lösen Sie dieses Problem</b>: Korrigieren Sie einfach die Kabelkonfiguration, indem Sie das Netzkabel des Monitors, der mit der Hauptplatine verbunden ist, abziehen und es stattdessen mit den GPU-Ausgängen verknüpfen.

### Falsche GPU-Treiberinstallation

Wenn die GPU-Treiber nicht ordnungsgemäß installiert sind, kann die Anwendung die dedizierte GPU nicht erreichen und muss stattdessen auf die integrierte GPU zurückgreifen.

<b>So lösen Sie dieses Problem</b>: Deinstallieren Sie die aktuellen GPU-Treiber, führen Sie eine Bereinigung durch und installieren Sie die GPU-Treiber nach einem Neustart des Computers neu.

### Profileinstellung für Nvidia-GPU-Treiber

Auf einigen Computern, z. B. Laptops, kann die Anwendung standardmäßig auf der integrierten GPU anstatt auf der dedizierten Nvidia-GPU ausgeführt werden. Bei einer NVIDIA-GPU hängt der Wechsel zur rechten GPU von den Anwendungsprofilen ab. Wenn eine Anwendung nicht über ein solches Profil verfügt, können Sie es manuell zuweisen.

<b>So lösen Sie dieses Problem</b>:

1. Klicken Sie mit der rechten Maustaste auf den Desktop und wählen Sie NVIDIA-Systemsteuerung <b>oder </b> Navigieren Sie zur Systemsteuerung und suchen Sie nach NVIDIA-Systemsteuerung.
1. Wechseln Sie unter <b>3D-Einstellungen</b> zu <b>3D-Einstellungen verwalten</b>
1. Fügen Sie auf der Registerkarte <b>Programmeinstellungen</b> ein neues Profil für <b>Substance 3D Painter</b> hinzu.
1. Ändern Sie die Einstellung des bevorzugten Grafikprozessors auf NVIDIA-Hochleistungsprozessor.

### Windows-Leistungseinstellung

Windows hat möglicherweise die falsche GPU-Einstellung für die Anwendung festgelegt, da die Standardeinstellungen für Leistung und Stromverbrauch festgelegt sind.

<b>So lösen Sie dieses Problem: </b> Führen Sie die folgenden Schritte aus, um die Standard-GPU-Konfiguration zu überschreiben.

1. Öffnen Sie die Anzeigeeinstellungen, indem Sie mit der rechten Maustaste auf Ihren Desktop klicken:

   ![](../../../assets/settings-33.png)
1. Navigieren Sie zum unteren Rand des Fensters auf der Startseite und klicken Sie auf &quot;Grafikeinstellungen&quot; :

   ![](../../../assets/graphics-settings.png)
1. Klicke auf die Schaltfläche &quot;Durchsuchen&quot;, und navigiere zur ausführbaren Datei von Substance 3D Painter :

   ![](../../../assets/browse-16.png)
1. Nachdem die Anwendung hinzugefügt wurde, klicken Sie auf die Schaltfläche &quot;Optionen&quot; :

   ![](../../../assets/options-19.png)
1. Wählen Sie die Einstellung &quot;High performance&quot; und klicken Sie auf &quot;Save&quot;

   ![](../../../assets/specs.png)

## Linux

### Deaktivieren Sie &quot;Bevorzugte nicht standardmäßige GPU&quot;.

Stellen Sie beim Ausführen von Painter von einem Desktop-Tastaturbefehl oder beim Ausführen über Steam sicher, dass die Einstellung <b>PrefersNonDefaultGPU</b> in der Datei <b>\*.desktop</b> auf <b>false</b> festgelegt ist.

Diese Einstellung kann irreführend sein und dazu führen, dass die integrierte GPU anstelle der diskreten und leistungsfähigeren verwendet/erzwungen wird. Weitere Informationen [finden Sie in dieser Diskussion ](https://github.com/ValveSoftware/steam-for-linux/issues/9940).

### Erzwingen einer bestimmten GPU mithilfe der Umgebungsvariable DRI\_PRIME

Standardmäßig verwendet Painter die erste von der Vulkan-Grafik-API aufgeführte GPU, diese GPU könnte jedoch falsch sein (es könnte sich um die zuerst aufgeführte integrierte GPU handeln), was zu schlechten Leistungen führt. Die Umgebungsvariable DRI\_PRIME kann verwendet werden, um die gewünschte GPU zu erzwingen. Weitere Informationen [finden Sie in der Dokumentation des Arch-Wikis ](https://wiki.archlinux.org/title/PRIME#For_open_source_drivers%E2%80%94PRIME). Sie können auch auf die [Mesa-Dokumentation](https://docs.mesa3d.org/envvars.html#envvar-DRI_PRIME) verweisen.
