---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/technical-support/technical-issues/gpu-issues/crash-when-working-with-overclocked-gpu.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie Substance 3D Painter-Abstürze beim Arbeiten mit übertakteten GPUs für eine stabile Anwendungsleistung beheben können.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > GPU Issues > Crash when working with overclocked GPU
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Absturz beim Arbeiten mit übertakteter GPU
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---


# Absturz beim Arbeiten mit übertakteter GPU

Übertaktete GPUs können oft instabiler sein, da sie auf Frequenzen basieren, die ursprünglich nicht vom GPU-Konstruktor entworfen wurden. Wenn Ihre GPU übertaktet ist und Sie Stabilitätsprobleme haben, empfehlen wir, für eine Weile zu den werkseitigen Standardfrequenzen zurückzukehren.

## Nvidia GPU

Auf NVIDIA-GPUs ist es ab den Treibern 355.82 möglich, das GPU-Übertakten vorübergehend zu deaktivieren, indem ein Debugmodus in den Treibereinstellungen aktiviert wird. Auf diese Weise können Probleme im Zusammenhang mit den Grafikkarten überprüft und festgestellt werden.

So aktivieren Sie den Debugmodus:

1. Öffnen Sie die **Nvidia-Systemsteuerung** (klicken Sie mit der rechten Maustaste auf Ihren Desktop).
1. Klicken Sie auf das Menü **Hilfe**.
1. Klicken Sie auf **Debugmodus**.

>[!NOTE]
>
> Der Debugmodus ist möglicherweise nicht verfügbar, wenn die GPU eine Referenzkarte ist. Sie ist nur verfügbar, wenn die GPU auf nicht standardmäßigen Uhren oder mit einem geänderten BIOS ausgeführt wird. In diesem Fall empfehlen wir, die Übertaktung manuell zu deaktivieren.
