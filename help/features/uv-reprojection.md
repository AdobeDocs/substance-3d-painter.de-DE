---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/features/uv-reprojection.html"
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

Die UV-Projektion ist ein automatischer Prozess, der ausgeführt wird, wenn Sie die Strukturauflösung geändert haben oder ein neues Gitter importieren.\
Wenn Sie ein neues Gitter in Ihr Dokument laden (über das Fenster [Projektkonfiguration](https://substance3d.adobe.com/display/draftpainter/project%20configuration) ), werden alle Ihre Aktionen auf dieses neue Gitter neu projiziert. Es spielt keine Rolle, ob sich die Topologie geändert hat (solange sie ähnlich ist) oder ob sich die UVs geändert haben. Da für die Neuprojektion alle Ebenen und Pinselstriche neu berechnet werden, kann dies etwas Zeit in Anspruch nehmen (insbesondere bei hohen Texturauflösungen).

Malen in der 2D-Ansicht

Da jeder in der 2D-Ansicht ausgeführte Strich im UV-Raum ausgeführt wird, gibt es keine Möglichkeit, ihn korrekt neu zu projizieren, falls sich die UV-Werte des Gitters nach einem erneuten Import dramatisch ändern. Die beste Möglichkeit, die Projektreprojektion nachvollziehbar zu machen, besteht darin, sich auf die Maskierung durch eine ID-Karte und andere Arten der Auswahl zu verlassen und stattdessen in der 3D-Ansicht zu malen.

## Wie funktioniert die Neuprojektion?

Substance 3D Painter speichert seine Daten im dreidimensionalen Raum, um sicherzustellen, dass alles verlustfrei bleibt. Das bedeutet, dass Substance 3D Painter beim Importieren eines Gitters versucht, an der Stelle zu malen, an der sich das Gitter vor dem erneuten Import befand, und nicht weiß, wohin einige Teile verschoben werden konnten.

Auch beim Importieren eines Gitters in Substance 3D Painter wird der Begrenzungsrahmen berechnet, um den Raum zu registrieren und eine relative Skalierung für die Werkzeuge (Pinsel, Partikel usw.) zu definieren. Dieser Bounding Box ist auf jeder Achse 1 Einheit breit. Wenn Sie beim Importieren eines neuen Gitters die Option &quot;Kontur beibehalten&quot; deaktivieren, wird der Begrenzungsrahmen auf das neue Gitter normalisiert. Daher können sich die Striche bewegen, wenn sich die Größe des Gitters drastisch geändert hat. Wenn Sie jedoch &quot;Konturen beibehalten&quot; aktivieren, skalieren wir den ursprünglichen Begrenzungsrahmen auf den neuen, um die Pinselstriche neu zu projizieren.

>[!WARNING]
>
> Das Ändern der Einheiten des 3D-Meshs kann dazu führen, dass die UV-Projektion nicht funktioniert. Das alte und das neue Gitter können, obwohl sich die Topologie nicht geändert hat, als sehr unterschiedliche Maßstäbe interpretiert werden. Im Idealfall vermeiden Sie eine Änderung der Geräteinstallation, da dies schwierig zu beheben sein kann.
