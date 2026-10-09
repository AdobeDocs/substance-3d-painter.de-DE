---
breadcrumb-title: ""
description: Erfahren Sie, wie Sie Probleme mit defektem oder nicht reagierendem Viewport auf Ubuntu in Substance 3D Painter für ein ordnungsgemäßes 3D-Rendering beheben.
title: Viewport erscheint defekt oder reagiert nicht auf Ubuntu
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 0%
---

# Viewport erscheint defekt oder reagiert nicht auf Ubuntu

Wenn Sie Painter von Steam auf Ubuntu ab Version 11.1 ausführen, kann der Viewport beschädigt erscheinen oder nicht mehr reagieren.

Dies hängt damit zusammen, dass Painter nicht mit der richtigen zugewiesenen GPU startet. Auf Ubuntu die integrierte GPU statt der diskreten kann man am Ende ausgewählt werden. Painter übernimmt diese Konfiguration über Steam , was zu Problemen führen kann.

Es gibt einige Lösungen:

1. Führen Sie Steam von einem Terminal aus. Dies erzwingt einen anderen Kontext und sollte dazu führen, dass Steam und Painter auf der richtigen GPU laufen.
1. Bearbeiten Sie den Steam-Tastaturbefehl, um die Einstellung <b>Mit dedizierter Grafikkarte ausführen</b> zu deaktivieren. Führen Sie dann Steam wie gewohnt aus.

Weitere Informationen finden Sie unter [diesem GitHub-Problem](https://github.com/ValveSoftware/steam-for-linux/issues/9940).
