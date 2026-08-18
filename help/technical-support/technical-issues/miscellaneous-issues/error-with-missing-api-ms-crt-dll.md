---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/miscellaneous-issues/error-with-missing-api-ms-crt-dll.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie fehlende api-ms-crt DLL-Fehler in Substance 3D Painter für die richtige Unterstützung der Windows-Laufzeitbibliothek beheben.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Miscellaneous Issues > Error with missing api-ms-crt dll
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Fehler mit fehlender api-ms-crt-DLL
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '201'
ht-degree: 0%

---


# Fehler mit fehlender api-ms-crt-DLL

Substance 3D Painter kann nicht gestartet werden, da **api-ms-win-crt-runtime-l1-1-0.dll** auf Ihrem Computer fehlt.\
Dies ist höchstwahrscheinlich darauf zurückzuführen, dass das Update KB2999226, das Teil von **Visual C++ Redistributable** für Visual Studio 2015 ist, nicht installiert werden konnte.

## Wie behebt man das Problem?

### 1 - Stellen Sie sicher, dass Windows auf dem neuesten Stand ist

1. Öffnen Sie das Startmenü
1. Systemsteuerung auswählen
1. Klicken Sie auf **Windows Update**.
1. Klicken Sie auf **Nach Updates suchen**
1. **Installieren** aller verfügbaren Updates.
1. Nach der Installation der Updates **starten Sie Ihren Computer neu**.

Wiederholen Sie nach dem Neustart die obigen Schritte erneut, bis keine Updates mehr verfügbar sind.

### 2 - Visual C++ Redistributable installieren

1. Laden Sie Visual C++ Redistributable herunter:
   1. Für [Windows 64-Bit](http://download.microsoft.com/download/9/3/F/93FCF1E7-E6A4-478B-96E7-D4B285925B00/vc_redist.x64.exe)
   1. Für [Windows 32-Bit](http://download.microsoft.com/download/9/3/F/93FCF1E7-E6A4-478B-96E7-D4B285925B00/vc_redist.x86.exe)
1. Führen Sie **vcredist\_x64.exe** (64 Bit) oder **vcredist\_x86.exe** (32 Bit) aus.
1. Wählen Sie Deinstallieren und folgen Sie den Anweisungen.
1. Ausführbare Datei erneut ausführen
1. &quot;Installieren&quot; auswählen
