---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/pipeline-and-integration/resource-management/excluding-resources-in-a-resource-path.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie bestimmte Ressourcen in Substance 3D Painter von Ressourcenpfaden ausschließen können, um die Organisation Ihres Regals zu verbessern.
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Resource management > Excluding resources in a resource path
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Ausschließen von Ressourcen in einem Ressourcenpfad
user-guide-description: ''
user-guide-title: ''
source-git-commit: 22871eab2f25d09bd82f1292d8b3e5f8c4f1c2cf
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 0%

---


# Ausschließen von Ressourcen in einem Ressourcenpfad

Auf dieser Seite wird erläutert, wie eine Ignorierdatei eingerichtet wird, um Ressourcen und Ordner anzugeben, die während des Crawlvorgangs des Fensters [Assets](../../interface/assets/assets.md) ignoriert werden. So können Sie verhindern, dass unerwünschte Ressourcen angezeigt werden.

>[!NOTE]
>
> Diese Funktion ist seit Version 7.2.3 verfügbar.

## Erstellen einer Ignorierdatei

Navigieren Sie zum Speicherort des Ressourcenordners, in dem Sie Ressourcen ausblenden möchten. Erstellen Sie dann eine Datei mit dem folgenden Namen:

```
.ignore_assets_pt
```


>[!NOTE]
>
> Beachten Sie, dass der Dateiname mit einem Punkt beginnen muss.

Es sollte nach der Erstellung folgendermaßen aussehen:

![](../../assets/ignore-file-location.png)

## Beispiel

Der folgende Dateiinhalt verwirft alle Ressourcen und Ordner außer den Standardbibliotheksordnern:

```
## exclude all

* 

 

## re-include library directories

!alphas 

!colorluts 

!effects 

!emitters 

!environments 

!export-presets 

!generators 

!materials 

!presets 

!procedurals 

!receivers 

!shaders 

!smart-masks 

!smart-materials 

!templates 

!textures
```


## Regeln und Richtlinien

Die folgende Tabelle zeigt die allgemeinen Regeln für die Ignorieren-Datei.

>[!NOTE]
>
> Bei der Musterübereinstimmung der Ignorierungsdatei wird unabhängig vom Verhalten des Betriebssystems zwischen Groß- und Kleinschreibung unterschieden.

| Regel | Beschreibung | Beispiel |
| --- | --- | --- |
| **Leere Zeile** | Leere Zeile, die mit nichts übereinstimmt. Kann als Trennzeichen für die Lesbarkeit verwendet werden. |  |
| **Verzeichnistrennzeichen** | Der Schrägstrich wird als Verzeichnistrennzeichen verwendet. Trennzeichen können am Anfang, in der Mitte oder am Ende eines Suchmusters auftreten.Wenn sich am Anfang oder in der Mitte (oder in beiden) des Musters ein Trennzeichen befindet, ist das Muster relativ zur Verzeichnisebene der Ignorierdatei selbst. Andernfalls kann das Muster auch auf einer beliebigen Ebene unterhalb der Ebene der ignorierten Datei übereinstimmen. Wenn am Ende des Musters ein Trennzeichen steht, wird es ignoriert. Das Muster entspricht dann immer noch den Dateien und Verzeichnissen. | `folder/filename.extension   folder/sub-folder` |
| **Kommentarzeile** | Eine Zeile, die mit dem Nummernzeichen (oder Hash) beginnt, dient als Kommentar. | `# This is a comment` |
| **Sternchen** | Ein Sternchen entspricht einem beliebigen Objekt außer einem Schrägstrich. | `# Match anything starting with Alpha   alpha*   # Match any file with given extension   *.jpg` |
| **Zeichenbereich** | Der Zeichenbereich kann zwischen eckigen Klammern angegeben werden, um den Ordner- und Dateinamen abzugleichen.<ul data-preserve-html="true"> <li data-preserve-html="true"><b>[abc]</b>: Entspricht einem Zeichen in der angegebenen Liste</li> <li data-preserve-html="true"><b>[a-c]</b>: Entspricht einem Zeichen im angegebenen Bereich</li> <li data-preserve-html="true"><b>[ !abc]</b>: Entspricht einem Zeichen, das nicht in der angegebenen Liste enthalten ist</li> <li data-preserve-html="true"><b>[ !a-c]</b>: Entspricht einem Zeichen, das nicht im angegebenen Bereich liegt</li> </ul>Bereich und Liste können auch Zahlen mit dem Format <b>[0-9]</b> sein. | `# Exclude any UDIM image in PNG   *_[0-9][0-9][0-9][0-9].png` |
| **Escapezeichen** | Geben Sie Literalzeichen an, die andernfalls ignoriert oder als Regeln verwendet würden. | `# This is a comment   [#]This/Is/A/Path` |
| **Nachfolgende Leerzeichen** | Nachfolgende Leerzeichen werden ignoriert, es sei denn, sie werden mit Escapezeichen versehen. | `# Match a subfolder with trailing space   folder/subfolder[ ]` |
| **Ausrufepräfix** | Wenn einem Muster ein Ausrufezeichen vorangestellt wird, kann es negiert werden.Jede passende Datei, die durch ein vorheriges Muster ausgeschlossen wurde, wird wieder aufgenommen. Es ist nicht möglich, eine Datei erneut einzuschließen, wenn ein übergeordnetes Verzeichnis dieser Datei ausgeschlossen ist. Beim Crawling werden ausgeschlossene Verzeichnisse aus Leistungsgründen nicht aufgelistet, sodass Muster in enthaltenen Dateien keine Auswirkungen haben, unabhängig davon, wo sie definiert sind. | `# Re-include specific file   !my_file_name.png` |
