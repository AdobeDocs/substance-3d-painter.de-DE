---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/uv-reprojection.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie die UV-Reprojektion in Substance 3D Painter verwenden, um Texturen zwischen verschiedenen UV-Layouts zu übertragen.
helpx_creative_field: ""
helpx_description: Painter > Features > UV Reprojection
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: UV-Reprojektion
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 0%

---


# UV-Reprojektion

UV-Reprojektion ist ein automatischer Prozess, der ausgeführt wird, wenn Sie die Auflösung der Textur geändert haben oder einen neuen Mesh importieren.\
Wenn Sie einen neuen Mesh in Ihr Dokument laden (über das Fenster [Projektkonfiguration](https://substance3d.adobe.com/display/draftpainter/project%20configuration) ), werden alle Ihre Aktionen auf diesen neuen Mesh neu projiziert. Es spielt keine Rolle, ob sich die Topologie geändert hat (solange sie ähnlich ist) oder ob sich die UVs geändert haben. Da für die Neuprojektion alle Ebenen und Pinselstriche neu berechnet werden, kann dies etwas Zeit in Anspruch nehmen (insbesondere bei hohen Auflösungen der Textur).

Malen in der 2D-Ansicht

Da jeder in der 2D-Ansicht ausgeführte Strich im UV-Bereich ausgeführt wird, gibt es keine Möglichkeit, ihn erneut zu projizieren, falls sich die UV des Meshs nach einem erneuten Import dramatisch ändert. Die beste Methode, um die Projektreprojektion nachahmenswert zu machen, besteht darin, sich auf die Maskierung durch einen ID-Map und andere Auswahlmöglichkeiten zu verlassen und anstelle der 3D-Ansichten zu malen.

## Wie funktioniert die erneute Projektion?

Substance 3D Painter speichert seine Daten im 3D-Welt-Raum, damit nichts zerstört wird. Das bedeutet, dass Substance 3D Painter beim Importieren eines Meshs versucht, auf dem Malen zu machen, wo sich der Mesh vor dem erneuten Import befand, und nicht wissen kann, wohin einige Teile verschoben werden konnten.

Auch beim Importieren eines Meshs in Substance 3D Painter wird der Begrenzungsrahmen berechnet, um den Abstand zu registrieren und eine relative Skalierung für die Werkzeuge (Malen-Pinsel, Partikeln usw.) zu definieren. Dieser Bounding Box ist auf jeder Achse 1 Einheit breit. Wenn Sie beim Importieren eines neuen Meshs die Option &quot;Kontur beibehalten&quot; deaktivieren, normalisieren wir den Begrenzungsrahmen auf den neuen Mesh neu. Wenn sich der Mesh also stark skaliert hat, können sich die Konturen verschieben. Wenn Sie jedoch &quot;Konturen beibehalten&quot; aktivieren, skalieren wir den ursprünglichen Begrenzungsrahmen auf den neuen, um die Pinselstriche neu zu projizieren.

>[!WARNING]
>
> Das Ändern der Einheiten Ihres 3D-Mesh kann dazu führen, dass die UV-Neuprojektion nicht funktioniert. Der alte und der neue Mesh können, obwohl sich die Topologie nicht geändert hat, als sehr unterschiedliche Maßstäbe interpretiert werden. Im Idealfall vermeiden Sie eine Änderung der Geräteinstallation, da dies schwierig zu beheben sein kann.
