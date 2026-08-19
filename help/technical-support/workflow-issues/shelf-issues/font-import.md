---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/technical-support/workflow-issues/shelf-issues/font-import.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie Probleme beim Importieren von Schriftdateien in Substance 3D Painter beheben können, um Schriftartenressourcen erfolgreich zu importieren und zu verwenden.
helpx_creative_field: ""
helpx_description: Substance 3D Painter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Schriftdatei kann nicht importiert werden
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---


# Schriftdatei kann nicht importiert werden

Mit der Einführung der [Textressource](../../../painting/text-resource.md) werden Schriftartendateien beim Start automatisch erfasst. Schriftdateien können auch manuell importiert werden.

In diesen Fällen können einige Fehlermeldungen angezeigt werden:

* Wenn Sie eine Datei per Drag &amp; Drop in die Oberfläche von Painter ziehen.
* Wenn Painter Schriften auf der Festplatte erkennt (Library Crawling).

## Wie behebt man das Problem

Wenn eine Fehlermeldung zu einer <b>beschädigten Datei</b> ausgelöst wird, suchen Sie nach einer alternativen Version, und Painter kann diese möglicherweise laden. Beachten Sie, dass nur die Formate <b>.ttf</b> und <b>.otf</b> unterstützt werden.

Wenn eine Fehlermeldung zu einem <b>Lizenzierungsproblem</b> ausgelöst wird, ist die Schriftart einfach nicht mit Painter kompatibel und kann nicht importiert werden.

### Nachrichtenübersicht

|  |  |
| --- | --- |
| <b>Fehlermeldung</b> | <b>Erklärung</b> |
| In der Bibliothek &quot;LIBRARYNAME&quot; gibt es Probleme mit 4 Schriftdateien: FONTNAME, FONTNAME, FONTNAME,... | Diese Meldung erfasst eine kurze Liste von Schriftdateinamen, die identifiziert wurden, aber nicht in Painter importiert werden können. Diese Dateien werden ignoriert und nicht im Fenster &quot;Elemente&quot; angezeigt. |
| Es wurden Schriftprobleme gefunden. Weitere Informationen finden Sie unter https://... | Generische Meldung, die darauf hinweist, dass ein Problem mit Schriftarten gefunden wurde. |
| FONTNAME kann aufgrund von Lizenzbeschränkungen nicht importiert werden. Weitere Informationen finden Sie unter https://... | Painter muss in der Lage sein, Schriftarten in seine Projektdatei einzubetten, um sie verwenden zu können. Schriftarten, die dies nicht zulassen (in ihren Metadaten angegeben), können daher nicht importiert werden. |
| FONTNAME kann nicht importiert werden, da die Datei beschädigt ist oder ein nicht unterstützter Typ vorliegt. Weitere Informationen finden Sie unter https://... | Painter kann die bereitgestellte Schriftdatei nicht lesen. |
