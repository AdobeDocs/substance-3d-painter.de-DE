---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/stability-issues/crash-during-export.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie Substance 3D Painter-Absturz während Exportvorgängen beheben können, um zuverlässige Workflows für den Export von Texturen zu erhalten.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Stability Issues > Crash during export
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Absturz beim Exportieren
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '318'
ht-degree: 0%

---


# Absturz beim Exportieren

In bestimmten Fällen kann es beim Export zu einem Absturz von Substance 3D Painter kommen, insbesondere bei sehr hoher Auflösung (wie 4K oder 8K). Im Folgenden finden Sie eine Liste der häufigsten Quellen für dieses Problem.

## TDR (Timeout Detection and Recovery)

Die Zeitüberschreitungserkennung und -wiederherstellung (Timeout Detection and Recovery, TDR) ist ein Sicherheitsmechanismus von Microsoft Windows, um zu verhindern, dass eine GPU das System mit einer nie endenden Berechnung blockiert. Dieser Mechanismus ist leider standardmäßig zu restriktiv für Substance 3D Painter.

Weitere Informationen finden Sie unter: [GPU-Treiber-Absturz mit langen Berechnungen (TDR-Absturz)](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/gpu-drivers-crash-with-long-computations-128745489.html).

## Wenig virtueller Speicher

Beim Exportieren kann viel RAM (Computer-Speicher) verbraucht werden. In diesem Fall versucht das System, auf den virtuellen Speicher zurückzugreifen, wenn dem System der RAM-Speicher ausgeht. Bei dem virtuellen Speicher handelt es sich in der Regel um zusätzlichen Speicher, der auf Festplatten gespeichert ist. Wenn der virtuelle Speicher zu klein ist, tritt bei Substance 3D Painter ein Absturz auf, da der gesamte Speicher erschöpft ist.

Weitere Informationen finden Sie unter: [Absturz mit wenig virtuellem Arbeitsspeicher](crash-with-low-virtual-memory.md).

## Mangel an Festplattenspeicher

Seit der Einführung der Dünn besetzte virtuelle Texturen (SVT) kann Substance 3D Painter auf der Festplatte etwas Cache-Speicher ausgeben, um die Leistung zu verbessern. Wenn nicht genügend freier Speicherplatz auf der Festplatte vorhanden ist, kann dies zu einem Absturz führen, da die Anwendung den Cache nicht übertragen und schreiben konnte.

Der Cache-Speicherort kann aus dem Standardsystemordner für temporäre Dateien verschoben werden. Weitere Informationen finden Sie unter: [Dünn besetzte virtuelle Texturen](../../../features/sparse-virtual-textures.md).

## Übertaktete GPU-Frequenz

Übertaktete GPUs können oft instabiler sein, da sie auf Frequenzen basieren, die ursprünglich nicht vom GPU-Konstruktor entworfen wurden. Es kann hilfreich sein, das Übertakten für eine Weile zu deaktivieren.

Weitere Informationen finden Sie unter: [Absturz beim Arbeiten mit übertakteter GPU](../gpu-issues/crash-when-working-with-overclocked-gpu.md).
