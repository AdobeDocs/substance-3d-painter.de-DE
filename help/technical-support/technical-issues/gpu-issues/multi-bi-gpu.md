---
breadcrumb-title: ""
description: Erfahren Sie, wie Sie Substance 3D Painter für Systeme mit mehreren GPUs und zwei GPUs konfigurieren, um die Rendering-Leistung zu optimieren.
title: MultiBi-GPU
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
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
