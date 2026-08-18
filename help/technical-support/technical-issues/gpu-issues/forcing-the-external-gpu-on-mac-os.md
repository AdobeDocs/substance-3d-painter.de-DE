---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/gpu-issues/forcing-the-external-gpu-on-mac-os.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie erzwingen können, dass Substance 3D Painter eine externe GPU für macOS verwendet, um die Rendering-Leistung zu verbessern.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > GPU Issues > Forcing the external GPU on Mac OS
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Erzwingen der externen GPU unter Mac OS
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '149'
ht-degree: 0%

---


# Erzwingen der externen GPU unter Mac OS

Unter Mac OS Mojave ist es möglich, die Verwendung der externen GPU pro Anwendung anzugeben. Wenn diese Einstellung aktiviert ist, können sich die Leistung und Stabilität von Substance 3D Painter verbessern.

Weitere Informationen finden Sie in der [Apple-Dokumentation](https://support.apple.com/en-us/HT208544).

So aktivieren Sie es:

1. Schließen Sie Substance 3D Painter, wenn es bereits ausgeführt wird.
1. Wählen Sie Substance 3D Painter im Finder aus. Sie finden es im Ordner &quot;**Anwendungen**&quot;**.**
1. Drücken Sie **Befehl-I** oder klicken Sie mit der rechten Maustaste auf die Anwendung **Substance 3D Painter** und wählen Sie **Informationen abrufen**.
1. Aktivieren Sie im neuen Fenster die Einstellung **Externe GPU bevorzugen**.
1. Starten Sie Substance 3D Painter neu.

>[!NOTE]
>
> Diese Einstellung ist nicht sichtbar, wenn keine eGPU angeschlossen ist oder die aktuelle Version von MacOS zu alt ist.
