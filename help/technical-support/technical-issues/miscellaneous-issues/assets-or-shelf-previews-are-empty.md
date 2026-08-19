---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/technical-support/technical-issues/miscellaneous-issues/assets-or-shelf-previews-are-empty.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie leere Asset- und Shelf-Vorschauen in Substance 3D Painter reparieren, um die Miniaturansicht wiederherzustellen.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Miscellaneous Issues > Assets (or shelf) previews are empty
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Vorschauen von Elementen (oder Ablagen) sind leer
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '90'
ht-degree: 0%

---


# Vorschauen von Elementen (oder Ablagen) sind leer

Dieses Problem kann durch andere Software verursacht werden. Siehe: [Softwarekonflikte](../startup-issues/software-conflicts.md).

Wenn Sie nicht feststellen können, welche Software aktualisiert/deinstalliert wird, suchen Sie nach einer Umgebungsvariablen mit dem Namen &quot;QT\_PLUGIN\_PATH&quot; und entfernen Sie diese.

**Unter Windows:**

1. Öffnen Sie **System** in der Systemsteuerung.
1. Klicken Sie auf der Registerkarte &quot;Erweitert&quot; auf **Umgebungsvariablen**
1. Suchen Sie nach der Variablen mit dem Namen **&quot;QT\_PLUGIN\_PATH&quot;**
1. **Entfernen**
1. **Starten Sie Ihren Computer neu**
