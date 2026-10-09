---
breadcrumb-title: ""
description: Erfahren Sie, wie Sie leere Asset- und Regal-Vorschauen in Substance 3D Painter korrigieren, um die Miniaturansicht wiederherzustellen.
title: Vorschauen von Elementen (oder Regalen) sind leer
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '90'
ht-degree: 0%
---

# Vorschauen von Elementen (oder Regalen) sind leer

Dieses Problem kann durch andere Software verursacht werden. Siehe: [Softwarekonflikte](../startup-issues/software-conflicts.md).

Wenn Sie nicht feststellen können, welche Software aktualisiert/deinstalliert wird, suchen Sie nach einer Umgebungsvariablen mit dem Namen &quot;QT\_PLUGIN\_PATH&quot; und entfernen Sie diese.

**Unter Windows:**

1. Öffnen Sie **System** in der Systemsteuerung.
1. Klicken Sie auf der Registerkarte &quot;Erweitert&quot; auf **Umgebungsvariablen**
1. Suchen Sie nach der Variablen mit dem Namen **&quot;QT\_PLUGIN\_PATH&quot;**
1. **Entfernen**
1. **Starten Sie Ihren Computer neu**
