---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/technical-support/technical-issues/rendering-issues/broken-viewport-ubuntu.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie fehlerhafte oder nicht reagierende Viewport-Probleme auf Ubuntu in Substance 3D Painter für ein ordnungsgemäßes 3D-Rendering beheben.
helpx_creative_field: ""
helpx_description: Viewport appears broken or unresponsive on Ubuntu
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Viewport wird unter Ubuntu als defekt oder nicht reagierend angezeigt
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 0%

---


# Viewport wird unter Ubuntu als defekt oder nicht reagierend angezeigt

Wenn Sie Painter von Steam auf Ubuntu ab Version 11.1 ausführen, kann der Viewport defekt oder nicht reagierend erscheinen.

Dies hängt damit zusammen, dass Painter nicht mit der richtigen zugewiesenen GPU startet. Auf Ubuntu die integrierte GPU statt der diskreten kann man am Ende ausgewählt werden. Painter übernimmt diese Konfiguration über Steam , was zu Problemen führen kann.

Es gibt einige Lösungen:

1. Führen Sie Steam von einem Terminal aus. Dies erzwingt einen anderen Kontext und sollte dazu führen, dass Steam und Painter auf der richtigen GPU laufen.
1. Bearbeiten Sie den Steam-Shortcut, um die Einstellung <b>Mit dedizierter Grafikkarte ausführen</b> zu deaktivieren. Führen Sie dann Steam wie gewohnt aus.

Weitere Informationen finden Sie unter [diesem GitHub-Problem](https://github.com/ValveSoftware/steam-for-linux/issues/9940).
