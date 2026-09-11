---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/stability-issues/crash-while-baking.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie Substance 3D Painter-Absturz beim Baking beheben können, um zuverlässige Workflows zum Baking von Texturen zu erhalten.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Stability Issues > Crash while baking
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Absturz beim Baking
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---


# Absturz beim Baking

Bei einigen Konfigurationen kann es zu Abstürzen beim Baking von Substance 3D Painter kommen. Auf dieser Seite finden Sie eine Liste der bekannten Probleme und wie sie behoben werden können.

## Absturz mit Baking führend Vorschau

Standardmäßig zeigt Substance 3D Painter im Viewport den Status an, in dem sich das Backen einer Textur befindet. Auf einigen Computern kann diese Funktion zu Instabilitäten führen.

So deaktivieren Sie es:

1. Verwenden Sie **Bearbeiten > Einstellungen**, um die Haupteinstellungen zu öffnen.
1. Scrollt unter **Allgemein** nach unten zum Abschnitt mit dem Namen **Baking-Optionen** .
1. Deaktivieren/deaktivieren Sie die Option **Live-Vorschau-Baking aktivieren** .

## Absturz mit GPU-Raytracing

Bei einigen GPUs mit instabilen Treibern kann das Baking aufgrund der GPU-Raytracing-Funktion zu Abstürzen führen.

So deaktivieren Sie es:

1. Verwenden Sie **Bearbeiten > Einstellungen**, um die Haupteinstellungen zu öffnen.
1. Scrollt unter **Allgemein** nach unten zum Abschnitt mit dem Namen **Baking-Optionen** .
1. Deaktivieren Sie die Option **GPU-Raytracing aktivieren** .

## Absturz mit Ryzen CPUs

Die Anwendung kann während des Bakings auf einer Computerkonfiguration, die mit einer Ryzen-CPU ausgeführt wird, einen Absturz aufweisen. Ein Update des BIOS behebt das Problem in der Regel.

Dies bezieht sich auf Multithreadberechnungen. Viele Motherboard-Konstruktoren haben neue BIOS-Updates veröffentlicht, um dieses Problem zu beheben. Wir empfehlen daher, das Update anzuwenden. Weitere Informationen finden Sie im Handbuch zur Hauptplatine und auf der Website des Konstruktors.

## Inkompatible Assbin-Dateien

Beim Baking werden Mesh mit hohem Poly standardmäßig in **\*.assbin**-Dateien vorverarbeitet, um das Nachbilden zu einem späteren Zeitpunkt zu beschleunigen. In einigen seltenen Fällen können diese Dateien Absturz in der Anwendung verursachen, wenn sie mit einer anderen Version generiert wurden. Einfach löschen sollte das Problem lösen, da sie regeneriert werden.
