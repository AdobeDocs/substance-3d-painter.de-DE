---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/stability-issues/crash-while-baking.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie Substance 3D Painter-Abstürze während des Backens für zuverlässige Workflows zum Backen von Texturen beheben können.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Stability Issues > Crash while baking
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Absturz beim Backen
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---


# Absturz beim Backen

Substance 3D Painter kann bei einigen Konfigurationen während des Backprozesses abstürzen. Auf dieser Seite finden Sie eine Liste der bekannten Probleme und wie sie behoben werden können.

## Absturz mit Backvorschau

Standardmäßig zeigt Substance 3D Painter im Viewport den Status an, in dem sich das Backen einer Textur befindet. Auf einigen Computern kann diese Funktion zu Instabilitäten führen.

So deaktivieren Sie es:

1. Verwenden Sie **Bearbeiten > Einstellungen**, um die Haupteinstellungen zu öffnen.
1. Scrollt unter **Allgemein** nach unten zum Abschnitt mit dem Namen **Backing-Optionen** .
1. Deaktivieren/deaktivieren Sie die Option **Aktivieren Sie den Live-Vorschau-Backvorgang** .

## Absturz mit GPU-Raytracing

Bei einigen GPUs mit instabilen Treibern kann der Backvorgang aufgrund der GPU-Raytracing-Funktion zu Abstürzen führen.

So deaktivieren Sie es:

1. Verwenden Sie **Bearbeiten > Einstellungen**, um die Haupteinstellungen zu öffnen.
1. Scrollt unter **Allgemein** nach unten zum Abschnitt mit dem Namen **Backing-Optionen** .
1. Deaktivieren Sie die Option **GPU-Raytracing aktivieren** .

## Absturz mit Ryzen-CPUs

Die Anwendung stürzt möglicherweise während des Backprozesses auf einer Computerkonfiguration ab, die mit einer Ryzen-CPU ausgeführt wird. Ein Update des BIOS behebt das Problem in der Regel.

Dies bezieht sich auf Multithreadberechnungen. Viele Motherboard-Konstruktoren haben neue BIOS-Updates veröffentlicht, um dieses Problem zu beheben. Wir empfehlen daher, das Update anzuwenden. Weitere Informationen finden Sie im Handbuch zur Hauptplatine und auf der Website des Konstruktors.

## Inkompatible Assbin-Dateien

Beim Backen werden hochgepolte Gitter standardmäßig in **\*.assbin**-Dateien vorverarbeitet, um das Backen später zu beschleunigen. In seltenen Fällen können diese Dateien die Anwendung abstürzen lassen, wenn sie mit einer anderen Version generiert wurden. Einfach löschen sollte das Problem lösen, da sie regeneriert werden.
