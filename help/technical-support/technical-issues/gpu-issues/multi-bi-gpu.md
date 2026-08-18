---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/gpu-issues/multi-bi-gpu.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie Substance 3D Painter für Systeme mit mehreren GPUs und zwei GPUs konfigurieren, um die Rendering-Leistung zu optimieren.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > GPU Issues > MultiBi-GPU
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: MultiBi-GPU
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '93'
ht-degree: 0%

---


# Multi/Bi-GPU

Einige GPU-Konfigurationen und/oder GPU-Modelle sind mit Substance 3D Painter nicht kompatibel und führen zu Instabilitäten und Abstürzen. Im Folgenden finden Sie eine Liste der inkompatiblen Konfigurationen:

| ***Konfiguration*** | ***Lösung*** |
| --- | --- |
| **Nvidia SLI / AMD Crossfire** (Grafikkartenbrücken) | Deaktivieren Sie SLI oder Crossfire in den Einstellungen des GPU-Treibers. |
| **Bi-GPU** (zwei GPU-Chipsätze auf einer Grafikkarte) | Deaktivieren Sie die Verwendung der beiden GPU-Chipsätze in den Treibereinstellungen auf nur einen. |
