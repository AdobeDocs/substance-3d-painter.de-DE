---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/startup-issues/application-failed-to-start-because-of-qt.html"
breadcrumb-title: ''
description: Hier erfahren Sie, wie Sie Startfehler von Substance 3D Painter beheben, die durch Probleme mit dem Qt-Framework beim ordnungsgemäßen Start der Anwendung verursacht wurden.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Startup Issues > Application failed to start because of Qt
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Anwendung konnte aufgrund von Qt nicht gestartet werden
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '130'
ht-degree: 0%

---


# Anwendung konnte aufgrund von Qt nicht gestartet werden

Beim Starten der Anwendung wird möglicherweise die folgende Fehlermeldung angezeigt:

&#x200B;>> 

Diese Anwendung konnte nicht gestartet werden, da kein Qt-Plattform-Plug-in initialisiert werden konnte. Das Problem kann durch eine Neuinstallation der Anwendung behoben werden.

Verfügbare Plattformen sind: minimal, offscreen, webgl, windows.

Dieser Fehler kann auftreten, weil eine andere softwaredefinierte Umgebungsvariable mit der Anwendung in Konflikt steht.

Stellen Sie sicher, dass Sie die folgenden Variablen aus der aktuellen Umgebung entfernen, bevor Sie die Anwendung starten:

```
QT_PLUGIN_PATH 

QML2_IMPORT_PATH
```


>[!NOTE]
>
> Diese Variablen können auch von einem Python-Kontext geerbt werden, z. B. mit **pyinstaller**. Stellen Sie sicher, dass Sie sie aus dem Kontext entfernen, in dem die Anwendung gestartet wird.
