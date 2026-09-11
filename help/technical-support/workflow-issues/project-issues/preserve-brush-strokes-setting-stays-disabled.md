---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/technical-support/workflow-issues/project-issues/preserve-brush-strokes-setting-stays-disabled.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie die Einstellung "Pinselstriche erhalten" korrigieren, die in Substance 3D Painter deaktiviert bleibt, um den Pinselstrich korrekt beizubehalten.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > Project Issues > Preserve brush strokes setting stays disabled
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Die Einstellung "Pinselstriche beibehalten" bleibt deaktiviert
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 0%

---


# Die Einstellung &quot;Pinselstriche beibehalten&quot; bleibt deaktiviert

Aufgrund eines unglücklichen Fehlers, der in Substance 3D Painter 1.5 eingeführt wurde (teilweise behoben in 1.7), haben einige Projekte Metadaten im Zusammenhang mit dem Mesh verloren. Dieser Fehler führt dazu, dass die Einstellung &quot;Konturpositionen auf dem Mesh beibehalten&quot; im Fenster [Projektkonfiguration](../../../interface/project-configuration.md) deaktiviert bleibt.

Um das Problem zu lösen, müssen einige spezifische Schritte befolgt werden:

* Öffnen Sie das Projekt mit dem Problem in Substance 3D Painter 1.7 oder höher
* Gehen Sie zu Bearbeiten > Projektkonfiguration.
* Den ursprünglichen Mesh, den Sie im aktuellen Projekt verwendet haben (nicht die aktualisierte Version), auswählen und erneut importieren
* Validieren Sie die Ebenen und lassen Sie Substance 3D Painter die Ebenen berechnen. Wenn es sich um denselben Mesh handelt, sollte sich nichts ändern.
* Gehen Sie erneut zu Bearbeiten > Projektkonfiguration
* Die Option &quot;Konturpositionen auf dem Mesh beibehalten&quot; sollte jetzt wieder aktiviert werden, sodass Sie den neuen Mesh importieren können.
