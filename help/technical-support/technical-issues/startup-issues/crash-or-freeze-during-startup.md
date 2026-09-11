---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/startup-issues/crash-or-freeze-during-startup.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie Absturz und Abstürze während des Starts von Substance 3D Painter für einen stabilen Anwendungsstart beheben.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Startup Issues > Crash or freeze during startup
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Absturz oder Einfrieren beim Starten
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '618'
ht-degree: 0%

---


# Absturz oder Einfrieren beim Starten

Auf dieser Seite finden Sie eine Liste bekannter Probleme und deren Lösungen im Zusammenhang mit dem nicht ordnungsgemäßen Starten der Anwendung.

## Softwarekonflikte

Auf der folgenden Seite finden Sie eine Liste aller Software-Produkte, die Konflikte verursachen können: [Softwarekonflikte](software-conflicts.md).

## Auf falscher GPU ausführen

Wenn die Anwendung nicht auf der rechten GPU startet, kann dies zu Stabilitätsproblemen führen. Weitere Informationen finden Sie auf dieser Seite: [Painter startet nicht auf der rechten GPU](../gpu-issues/painter-doesn-t-start-on-the-right-gpu.md).

## Veraltete GPU-Treiber

Die Verwendung alter GPU-Treiber kann zu Einfrieren und/oder Abstürzen führen. Wir empfehlen, die neuesten GPU-Treiber zu verwenden, sobald sie verfügbar sind. Siehe: [GPU hat veraltete Treiber](../gpu-issues/gpu-has-outdated-drivers.md).

## Weißer Bildschirm und nicht reagiert

Wenn die Anwendung beim Start unter Windows sofort einfriert (was zu einem weißen Bildschirm führt), kann dies verschiedene Gründe haben:

* Eine externe Anwendung verursacht einen Konflikt. Informationen zu Softwarekonflikten finden Sie unter [Softwarekonflikte](software-conflicts.md).
* Einige Fenster der Anwendung wurden auf einem anderen Monitor geöffnet. Durch Wiederherstellen des Standardlayouts der Benutzeroberfläche kann die Anwendung normal gestartet werden:
  1. Öffnen Sie den Registrierungseditor (**regedit** aus dem Startmenü).
  1. Navigieren Sie zu den Anwendungsvoreinstellungen (siehe: [Speicherort von Voreinstellungen und Anwendungsdaten](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/application-preferences-location-147095594.html))
  1. Erweitern Sie den Schlüssel **Adobe Substance 3D Painter**
  1. Wählen Sie den Schlüssel **Hauptfenster 2018** aus, und löschen Sie ihn.
  1. Starten Sie die Anwendung neu

## Absturz aufgrund eines falschen Systempfads/Pythonpfads

Die Anwendung überprüft den Systempfad, um Python-Module und Umgebungseinstellungen zu laden. Wenn das System nicht ordnungsgemäß eingerichtet wurde, kann dies beim Start zu einem Absturz führen.

Unter Windows:

1. Öffnen Sie das Menü **Start**.
1. Suchen Sie nach dem **System (Systemsteuerung)** und wählen Sie es aus.
1. Klicken Sie auf **Erweiterte Systemeinstellungen**.
1. Klicken Sie auf **Umgebungsvariablen**.
1. Suchen Sie unter **Systemvariablen** die Variable **PATH**.

Anschließend können Sie die Variable bearbeiten, um ihren Inhalt zu überprüfen. Wenn die Variable beispielsweise folgende Zeichen enthält, führt sie zu einem Absturz

```
ï–›éŒ à €è¸€ì‡ì‡ç¿¹
```


## Updates für Windows 10

Ein Update von Windows 10 kann manchmal zu Instabilitäten führen. Verwenden Sie die Diagnosetools von Windows, um potenzielle Fehler im System zu erkennen.

Es wird empfohlen, das **Bereitstellungs-Image-Servicing und -Management** (DISM) und das **Systemdatei-Überprüfungsprogramm** (SFC) auszuführen. DISM ist nützlich, um die Ersatzdateien wiederherzustellen, die von SFC benötigt werden, um beschädigte oder fehlende Systemdateien zu reparieren.

**DISM** wird ausgeführt:

1. Öffnen Sie das Startmenü
1. Nach Eingabeaufforderung suchen
1. Klicken Sie mit der rechten Maustaste auf das Ergebnis und wählen Sie &quot;Als Administrator ausführen&quot;
1. Geben Sie den folgenden Befehl ein :  **DISM /Online /Cleanup-Image /RestoreHealth**
1. Eingabetaste drücken

**SFC** wird ausgeführt:

1. Öffnen Sie das Startmenü
1. Nach Eingabeaufforderung suchen
1. Klicken Sie mit der rechten Maustaste auf das Ergebnis und wählen Sie &quot;Als Administrator ausführen&quot;
1. Geben Sie den folgenden Befehl ein :  **sfc /scannow**
1. Eingabetaste drücken

Starten Sie den Computer nach beiden Befehlen neu, um Updates zu installieren.

Weitere Informationen zu diesem Thema:  [Verwenden Sie das Systemdatei-Überprüfungstool, um fehlende oder beschädigte Systemdateien zu reparieren](https://support.microsoft.com/en-us/help/929833/use-the-system-file-checker-tool-to-repair-missing-or-corrupted-system).

## Absturz beim Starten älterer Versionen

Unter Windows wird Version 2018 (4.x) oder eine ältere Version möglicherweise nicht gestartet, da eine der DLL-Dateien, die mit dem Installationsordner bereitgestellt wird, für das Betriebssystem zu alt ist. Dieser Absturz kann behoben werden, indem die Datei manuell durch eine neuere Version ersetzt wird.

Gehen Sie folgendermaßen vor:

1. Navigieren Sie zum Installationsordner des Substance Painters.
1. Benennen Sie die Datei <b>libeay32.dll</b> in <b>backup\_libeay32.dll</b> um.
1. Laden Sie die folgende Datei herunter: [aktualisiert\_library32.zip](https://helpx.adobe.com/content/dam/help/en/substance-3d/documentation/spdoc/files/182266673/225968681/1/1644000679697/updated-libeay32.zip).
1. Extrahieren Sie die DLL-Datei aus der ZIP-Datei in den Installationsordner (neben der Datei &quot;Substance Painter.exe&quot;).
1. Starten Sie die Anwendung.
