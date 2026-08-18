---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/technical-support/technical-issues/gpu-issues/gpu-is-not-recognized.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie Probleme mit der GPU-Erkennung in Substance 3D Painter beheben, um die richtige Hardwarebeschleunigung und -leistung zu ermöglichen.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > GPU Issues > GPU is not recognized
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: GPU wird nicht erkannt
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '79'
ht-degree: 0%

---


# GPU wird nicht erkannt

![](../../../assets/not-recognized-gpu.png){width="500px"}

Einige **NVIDIA Optimus**-Benutzer können Probleme haben, Substance 3D Painter auf der richtigen GPU auszuführen. Eine Problemumgehung besteht darin, die folgenden Schlüssel in der Windows-Registrierung auf 0 festzulegen:

* HKEY\_LOCAL\_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion\Windows\RequireSignedAppInit
* HKEY\_LOCAL\_MACHINE\SOFTWARE\Wow6432Node\Microsoft\Windows NT\CurrentVersion\Windows\RequireSignedAppInit
