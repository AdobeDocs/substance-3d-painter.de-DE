---
breadcrumb-title: ""
description: Erfahren Sie, wie Sie GPU-Erkennungsprobleme beheben, die in Substance 3D Painter als "GDI Generic" angezeigt werden, um die GPU-Beschleunigung zu gewährleisten.
title: GPU wird nicht erkannt und wird als GDI-generisch bezeichnet
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '134'
ht-degree: 0%
---

# GPU wird nicht erkannt und wird als GDI-generisch bezeichnet

Dieses Problem ist etwas kompliziert zu verfolgen und kann durch mehrere Quellen verursacht werden:

* Wenn Sie sich auf einem Computer mit Nvidia Optimus befinden, finden Sie weitere Informationen unter dem folgenden Link: [GPU wird nicht erkannt](gpu-is-not-recognized.md)
* Überprüfen Sie, ob Ihr Monitor an die primäre GPU angeschlossen ist (und ob dieser Monitor unter Windows als Hauptanzeige eingestellt ist).
* Überprüfen Sie, ob die Bittiefe des Hauptbildschirms unter Windows auf 32 Bit festgelegt ist.
* Wenn Sie immer noch Probleme haben, versuchen Sie, Ihre GPU-Treiber neu zu installieren (die vollständige Deinstallation mit der Bereinigung der bleibt in der Windows-Registrierung erhalten).
