---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/technical-support/workflow-issues/project-issues/a-project-has-been-processed-as-a-text-file-and-is-now-corrupted.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie beschädigte Substance 3D Painter-Projektdateien wiederherstellen, die als Textdateien verarbeitet wurden.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > Project Issues > Corrupted project file
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Beschädigte Projektdatei
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '119'
ht-degree: 0%

---


# Ein Projekt wurde als Textdatei verarbeitet und ist jetzt beschädigt

Manchmal kann der folgende Fehler beim Laden eines Projekts auftreten:

```
[Hdf5Archive] Archive 'project.spp' appears to have been processed as a text file and is irremediably corrupted. 

[Project management] The selected project 'project.spp' isn't valid!
```


Dieser Fehler bedeutet, dass das Projekt außerhalb von Substance 3D Painter geändert wurde und **nicht ordnungsgemäß zurückgelesen werden kann** .\
Dies geschieht in der Regel, wenn eine Versionsverwaltungssoftware (z. B. **Perforce** ) das Substance 3D Painter-Projekt **als Textdatei statt als Binärdatei** verarbeitet. Die einzige Lösung besteht darin, der Versionsverwaltungssoftware eine neue Regel/Ausnahme hinzuzufügen, um die Verarbeitung von **spp.-Dateien als binär** zu erzwingen. Weitere Informationen zu **Perforce** finden Sie in der dedizierten Dokumentation : 2<https://www.perforce.com/perforce/r16.1/manuals/cmdref/p4_typemap.html>
