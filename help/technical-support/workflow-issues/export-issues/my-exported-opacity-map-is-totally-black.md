---
breadcrumb-title: ""
description: Erfahre, wie du in Substance 3D Painter die Deckkraft einer exportierten Karte komplett schwarz anzeigst, um sie transparent zu exportieren.
title: Meine exportierte Deckkraftkarte ist komplett schwarz
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '117'
ht-degree: 0%
---

# Meine exportierte Deckkraftkarte ist komplett schwarz

Wenn Sie ein neues Projekt erstellen, kommt die Standardfarbe vom Shader und nicht von den Texturen. Wenn Sie also alle Teile exportieren, die Sie nicht Malen haben, werden sie schwarz sein und einen Alpha-Wert von 0 haben (da für diese Teile keine Daten vorhanden sind).

Der einfachste Weg, dies zu beheben, ist, eine Füllebene am unteren Rand Ihres Ebenenstapels zu platzieren: Es füllt alle UVs mit einer Standardfarbe, die mit der Standardfarbe des Shader identisch ist.
