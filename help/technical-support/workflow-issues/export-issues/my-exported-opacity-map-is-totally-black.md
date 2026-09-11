---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/technical-support/workflow-issues/export-issues/my-exported-opacity-map-is-totally-black.html"
breadcrumb-title: ''
description: Erfahre, wie du in Substance 3D Painter die Deckkraft einer exportierten Karte komplett schwarz anzeigst, um sie transparent zu exportieren.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > Export Issues > My exported opacity map is totally black
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Meine exportierte Deckkraftkarte ist komplett schwarz
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '117'
ht-degree: 0%

---


# Meine exportierte Deckkraftkarte ist komplett schwarz

Wenn Sie ein neues Projekt erstellen, kommt die Standardfarbe vom Shader und nicht von den Texturen. Wenn Sie also alle Teile exportieren, die Sie nicht Malen haben, werden sie schwarz sein und einen Alpha-Wert von 0 haben (da für diese Teile keine Daten vorhanden sind).

Der einfachste Weg, dies zu beheben, ist, eine Füllebene am unteren Rand Ihres Ebenenstapels zu platzieren: Es füllt alle UVs mit einer Standardfarbe, die mit der Standardfarbe des Shader identisch ist.
