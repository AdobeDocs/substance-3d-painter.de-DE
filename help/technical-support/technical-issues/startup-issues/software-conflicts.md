---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/technical-support/technical-issues/startup-issues/software-conflicts.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie Softwarekonflikte beheben, die verhindern, dass Substance 3D Painter auf Ihrem System ordnungsgemäß gestartet wird.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Startup Issues > Software conflicts
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Softwarekonflikte
user-guide-description: ''
user-guide-title: ''
source-git-commit: 22871eab2f25d09bd82f1292d8b3e5f8c4f1c2cf
workflow-type: tm+mt
source-wordcount: '681'
ht-degree: 0%

---


# Softwarekonflikte

Auf dieser Seite finden Sie eine Liste bekannter Probleme mit anderer Software, bei denen Substance 3D Painter möglicherweise nicht mehr ordnungsgemäß ausgeführt wird oder Absturz bei der Ausführung auftreten.

| *Potenzielle Konfliktquelle* | *Problem* |
| --- | --- |
| **Virenschutz/Spyware-Schutz** | Antiviren- oder Anti-Spyware-Software kann einige der folgenden Probleme verursachen:<ul data-preserve-html="true"> <li data-preserve-html="true"><b> Falsch positiv</b>: Painter wird fälschlicherweise als Virus oder Malware gekennzeichnet.</li> <li data-preserve-html="true"><b> blockierte Dateien </b>: Painter kann keine Dateien lesen oder schreiben (Exportieren, Erstellen von Vorgaben usw.).</li> <li data-preserve-html="true"><b> Dateilöschung </b>: Painter kann nicht gestartet werden oder normal arbeiten, da erforderliche Dateien entfernt wurden.</li> </ul>In diesem Fall empfehlen wir, das Antivirenprogramm vorübergehend zu deaktivieren, um festzustellen, ob es hilfreich ist, oder um manuell Ausnahmen für Painter hinzuzufügen. |
| **AMD CrossFire &amp; NVIDIA SLI** | Mehrere GPU-Konfigurationen werden von Painter nicht unterstützt, was zu Abstürzen führt. Wir empfehlen, diese Funktion zu deaktivieren. |
| <b> Autodesk-Assistent </b> | Die Autodesk Assistant-Anwendung kann Konflikte verursachen und die Anwendung beim Start oder beim Öffnen einer Projektdatei in einen Absturz bringen. Aktualisieren Sie die Autodesk-Anwendung, um das Problem zu beheben. |
| <b> Alienware/Dell Computer</b> | Weitere Informationen finden Sie auf dieser Seite: [Absturz beim Öffnen oder Speichern einer Datei](../stability-issues/crash-when-opening-or-saving-a-file.md). |
| **APFS von Paragon Software** | Diese Software kann einen Speicherort in der Windows Path-Umgebungsvariable registrieren, an dem die Anwendung beim Start Absturz werden kann. Die Deinstallation der Software ist möglicherweise nicht ausreichend, und die Umgebungsvariable muss möglicherweise manuell entfernt werden. Beispiel für problematische Position:  `C:Program Files (x86)Paragon SoftwareAPFS for Windowsï–›éŒ à €è¸€ì‡ì‡ç¿¹` |
| **Avecto** | Wenn eine ältere Version von Avecto ausgeführt wird, kann dies zu Verzögerungen und Abstürzen führen. Stellen Sie sicher, dass Sie auf die neueste Version aktualisieren. |
| **Asus GPU Tweak** | Diese Software kann Probleme beim Kompilieren von Shadern in Substance 3D Painter verursachen oder sogar den Start der Shader-Kompilierung verhindern. Wenn dieses Problem auftritt, empfehlen wir, die Software zu deinstallieren, um zu sehen, ob sie das Problem behebt. |
| **Asus RAMCache** | Diese Software kann verhindern, dass Substance 3D Painter ordnungsgemäß gestartet wird, oder sie kann während der Ausführung instabil werden. Wir empfehlen, Asus RAMCache zu deaktivieren oder zu installieren, wenn Stabilitätsprobleme auftreten. |
| **Asus Sonic Suite** | Auf Computern mit einer ASUS-Hauptplatine kann <b>Asus Sonic Suite</b> standardmäßig installiert werden. Durch Deinstallieren dieser Software können einige Anzeige-/Schnittstellenprobleme in Substance 3D Painter behoben werden. |
| **Cloud-Sicherungssoftware** **(** OneDrive,**GDrive,** **Dropbox,** **Filestream, etc)** | Die Cloud-Backup-Software kann beim Speichern eines Projekts die Ursache für eine Vielzahl von Abstürzen sein. In diesem Fall empfiehlt es sich, an der Projektdatei zu arbeiten und sie in einem nicht synchronisierten Ordner zu speichern, und die Projektdateien stattdessen nach dem Ende der Änderungen wieder auf das Cloud-Laufwerk zu kopieren. |
| **Chitubox** | Diese Software kann beim Öffnen eines Dateidialogs (wie beim Öffnen oder Speichern eines Projekts) einen Konflikt verursachen und einen Absturz in der Anwendung verursachen. Sie können die Einstellung <b>Miniaturvorschau des Desktopmodells aktivieren</b> in den Chitubox-Einstellungen deaktivieren, um dieses Problem zu vermeiden. |
| **Duet-Anzeige** | Von <b>Duet Display</b> sind Probleme mit GPU-Treibern bekannt, die sich auf das Verhalten von Substance 3D Painter auswirken können. Es wird empfohlen, es zu deinstallieren. |
| **Google Chrome** | Google Chrome kann bei der Ausführung zusammen mit Substance 3D Painter einige Absturz verursachen. Um die Stabilität von Substance 3D Painter zu verbessern, wird empfohlen, dass Sie Google Chrome und die GPU-Treiber aktualisieren. Wenn weiterhin Absturz auftreten, deaktivieren Sie die Hardwarebeschleunigung in Google Chrome (wodurch Chrome die GPU nicht mehr verwendet). |
| **Nahimic-Audiosoftware** | <b>Nahimic</b> kann die Painter einfrieren oder einen Absturz erstellen. Das Anhalten kann helfen, und das Aktualisieren kann ebenfalls Probleme vermeiden. Nahimic betreibt auch Hintergrunddienste, die die Anwendung stören können und möglicherweise beendet oder deaktiviert werden müssen. |
| **OpenShot-Videosoftware** | <b>Die Openshot-Videosoftware</b> kann einen Konflikt mit Substance 3D Painter mit der Vorschau des Regals verursachen. Das Problem sollte durch Aktualisieren von OpenShot behoben werden. |
| **Pyinstaller** | Diese Anwendung kann eine falsche Umgebungseinrichtung erzeugen, die beim Start zu einem Fehler führt. Weitere Informationen finden Sie unter [Die Anwendung konnte aufgrund von Qt](application-failed-to-start-because-of-qt.md) nicht gestartet werden. |
| **Rptr / Plays.tv** | <b>Rptr</b> (oder <b>[Plays.tv](http://plays.tv/) </b>) ist standardmäßig mit einigen GPU-Treibern installiert. Diese Software kann Instabilitäten verursachen und die Anwendung Absturz. Es wird empfohlen, die Anwendung zu deinstallieren. |
| **RGBFusion** | Diese Software kann zu Konflikten mit Grafik-Tablet-Treibern führen, das Beenden des Prozesses kann das Problem vorübergehend beheben oder RGBFusion deinstallieren, um eine dauerhafte Lösung zu erhalten. |
