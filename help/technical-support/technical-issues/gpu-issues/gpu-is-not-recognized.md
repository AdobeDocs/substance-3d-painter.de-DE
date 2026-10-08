---
breadcrumb-title: ""
description: Erfahren Sie, wie Sie Probleme mit der GPU-Erkennung in Substance 3D Painter beheben, um die richtige Hardwarebeschleunigung und -leistung zu ermöglichen.
title: GPU wird nicht erkannt
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '79'
ht-degree: 0%
---

# GPU wird nicht erkannt

![](../../../assets/not-recognized-gpu.png){width="500px"}

Einige **NVIDIA Optimus**-Benutzer können Probleme haben, Substance 3D Painter auf der richtigen GPU auszuführen. Eine Problemumgehung besteht darin, die folgenden Schlüssel in der Windows-Registrierung auf 0 festzulegen:

* HKEY\_LOCAL\_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion\Windows\RequireSignedAppInit
* HKEY\_LOCAL\_MACHINE\SOFTWARE\Wow6432Node\Microsoft\Windows NT\CurrentVersion\Windows\RequireSignedAppInit
