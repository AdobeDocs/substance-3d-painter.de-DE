---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/technical-support/technical-issues/stability-issues/windows-blue-screens.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie Bluescreen-Fehler unter Windows vermeiden, wenn Sie Substance 3D Painter für einen stabilen Systembetrieb verwenden.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Stability Issues > Windows Blue Screens
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Bluescreens in Windows
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '526'
ht-degree: 0%

---


# Bluescreens in Windows

Unter Windows [Blue Screens of Death (BSOD)](https://en.wikipedia.org/wiki/Blue_screen_of_death) stehen normalerweise im Zusammenhang mit Treibern oder Hardwarefehlern. Substance 3D Painter selbst ist nicht für diese BSODs verantwortlich, kann aber ein Problem mit dem Computer selbst beleuchten, da die Anwendung sehr intensiv ist. Im Fall von Substance 3D Painter kann ein BSOD aufgrund der folgenden Probleme verursacht werden.

## Instabile GPU-Treiber

Substance 3D Painter ist bei der Durchführung der verschiedenen Berechnungen stark auf die GPU angewiesen. GPU-Treiber können manchmal instabil sein oder eine Regression aufweisen. Wir empfehlen, die GPU auf dem neuesten Stand zu halten, um die neuesten Korrekturen und Leistungsverbesserungen zu erhalten. Siehe: [GPU hat veraltete Treiber](../gpu-issues/gpu-has-outdated-drivers.md).

### Instabile Windows-Installation

Windows selbst kann nach einigen Updates instabil sein. Verwenden Sie die Diagnosetools von Windows, um potenzielle Fehler im System zu erkennen.

Es wird empfohlen, das **Bereitstellungs-Image-Servicing und -Management** (DISM) und das **Systemdatei-Überprüfungsprogramm** (SFC) auszuführen. DISM ist nützlich, um die Ersatzdateien wiederherzustellen, die von SFC benötigt werden, um beschädigte oder fehlende Systemdateien zu reparieren.

**DISM** wird ausgeführt:

1. Öffnen Sie das **Startmenü**
1. Suchen nach **Eingabeaufforderung**
1. **Klicken Sie mit der rechten Maustaste** auf das Ergebnis und wählen Sie &quot;**Als Administrator ausführen** &quot;
1. Geben Sie den folgenden Befehl ein :  **DISM /Online /Cleanup-Image /RestoreHealth**
1. **Eingabe** drücken

**SFC** wird ausgeführt:

1. Öffnen Sie das **Startmenü**
1. Suchen nach **Eingabeaufforderung**
1. **Klicken Sie mit der rechten Maustaste** auf das Ergebnis und wählen Sie &quot;**Als Administrator ausführen** &quot;
1. Geben Sie den folgenden Befehl ein :  **sfc /scannow**
1. **Eingabe** drücken

Starten Sie den Computer nach beiden Befehlen neu, um Updates zu installieren.

Weitere Informationen zu diesem Thema unter:  [Verwenden Sie das Systemdatei-Überprüfungsprogramm, um fehlende oder beschädigte Systemdateien zu reparieren](https://support.microsoft.com/en-us/help/929833/use-the-system-file-checker-tool-to-repair-missing-or-corrupted-system)

### Mangel an Festplattenspeicher

Seit der Einführung von [Spare Virtual Textures](../../../features/sparse-virtual-textures.md) in Substance 3D Painter verwendet die Anwendung jetzt den Datenträger, um Texturen während der Arbeit zwischenzuspeichern. Wenn auf dem System nicht mehr genügend Speicherplatz zur Verfügung steht, kann dies zu Instabilitäten führen.

Es gibt zwei einfache Lösungen für dieses Problem:

* Geben Sie Speicherplatz auf der Festplatte frei, um mehr Platz für das Cache-System zu schaffen.
* Verschieben Sie das Cache-Verzeichnis auf ein anderes Laufwerk mit mehr Speicherplatz. Dieser Speicherort kann über die Haupteinstellungen der Anwendung geändert werden. Weitere Informationen finden Sie in der [-Einstellung &quot;Temporäre Dateien&quot; &#x200B;](https://docs.substance3d.com/display/SPDOC/General) .

### Defektes Laufwerk (HDD oder SSD)

Wie bereits erwähnt, ist das Cache-System stark von der Festplatte abhängig. Wenn das Laufwerk defekt ist, kann dies dazu führen, dass das System beim Schreiben oder Lesen von Daten instabil wird.

Um festzustellen, ob ein Datenträger fehlerhaft ist, können Sie CHKDSK unter Windows ausführen:

1. Öffnen Sie das Menü **Stern**.
1. Wählen Sie **Computer/Dieser PC** aus.
1. **Klicken Sie mit der rechten Maustaste auf** auf der Festplatte und wählen Sie **Eigenschaften.**
1. Wechseln Sie zur Registerkarte **Extras**.
1. Klicken Sie unter **Fehlerüberprüfung** auf **Jetzt überprüfen** .

### Speicherdefekt

Fehlerhafter Arbeitsspeicher (RAM) kann zu Systeminstabilitäten führen, wenn ein Programm nicht sicher in den Arbeitsspeicher lesen oder schreiben kann. Zum Überprüfen der Speicherintegrität wird empfohlen, **MemTest** auszuführen.

Weitere Informationen zum Installieren und Verwenden von MemTest finden Sie in [diesem Handbuch](https://www.memtest86.com/technical.htm).
