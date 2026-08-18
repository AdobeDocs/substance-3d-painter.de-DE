---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/gpu-issues/running-on-integrated-gpu.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie Substance 3D Painter so konfigurieren, dass dedizierte GPU statt integrierter Grafiken für eine bessere Leistung verwendet werden.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > GPU Issues > Running on integrated GPU
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Ausführung auf integrierter GPU
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 0%

---


# Ausführung auf integrierter GPU

![](../../../assets/integrated-gpu.png){width="500px"}

Es kann vorkommen, dass einige Computer standardmäßig auf einen integrierten Chipsatz und nicht auf eine dedizierte GPU eingestellt sind.\
Da die Leistung des integrierten Chipsatzes sehr niedrig ist, empfehlen wir stattdessen die Verwendung einer dedizierten GPU. Ein Popup-Fenster wird angezeigt, in dem Sie darüber gewarnt werden.

Bei einer NVIDIA-GPU hängt der Wechsel zur NVIDIA-GPU von den Anwendungsprofilen ab. Wenn eine Anwendung nicht über ein solches Profil verfügt, können Sie die Grafikkarte manuell zuweisen:

1. Klicken Sie mit der rechten Maustaste auf den Desktop und wählen Sie NVIDIA-Systemsteuerung **oder** Navigieren Sie zur Systemsteuerung und suchen Sie nach NVIDIA-Systemsteuerung.
1. Gehen Sie unter **3D-Einstellungen** zu **3D-Einstellungen verwalten**
1. Fügen Sie auf der Registerkarte **Programmeinstellungen** ein neues Profil für **Substance 3D Painter** hinzu.
1. Ändern Sie die Einstellung des bevorzugten Grafikprozessors auf NVIDIA-Hochleistungsprozessor.
