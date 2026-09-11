---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/getting-started/export.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie Texturen aus Substance 3D Painter in verschiedenen Formaten für die Verwendung in anderen Anwendungen und Game-Enginen exportieren.
helpx_creative_field: ""
helpx_description: Painter > Getting Started > Export
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Exportieren
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 1%

---


# Exportieren

## Exportieren von Texturen

Texturen werden als Bitmapsammlung exportiert. Painter bietet durch Ausgabevorlagen viel Flexibilität beim Exportieren von Texturen. Mit Ausgabevorlagen können Sie z. B. die Benennung der exportierten Dateien, die Art und Weise, wie Texturen in Kanälen gepackt werden, sowie das Format und die Bittiefe der exportierten Dateien steuern. Wenn das einschüchternd klingt, keine Sorge, Painter umfasst Dutzende von Standard-Ausgabevorlagen, die für häufig verwendete 3D-Anwendungen und Anwendungsfälle konfiguriert sind.

Sie öffnen das <b>Exportfenster</b> und beginnen mit dem Exportieren von Texturen mit <b>Datei > Texturen exportieren</b>, oder verwenden Sie den Tastaturbefehl <b>STRG + UMSCHALT + E</b>. Unter den folgenden Links finden Sie weitere Informationen zum Exportieren von Texturen:

* [Exportfenster](../export/export-window/export-window.md)
* [Ausgabevorlagen](../export/export-presets/export-presets.md)
* [Ändern oder Erstellen von Ausgabevorlagen](creating-export-presets.md)

### Mesh exportieren

Painter kann den importierten Mesh ändern, indem es beispielsweise automatisch UVs generiert. Wenn Sie in Painter Änderungen am Mesh vorgenommen haben, können Sie den Mesh mit <b>Datei > Mesh exportieren</b> exportieren.

Beim Exportieren eines Meshs stehen Ihnen einige Optionen zur Verfügung:

* <b>Ohne Versatz/Tessellation</b>: exportiert den Basis-Mesh, ohne die Geometrie anhand der Material zu ändern.
  * <b>Triangulation anwenden</b>: Wenn der importierte Mesh aus Quads oder Polygonen bestand, können Sie diese Option aktivieren, um die triangulierte Painter-Version des Meshs zu exportieren. Dies kann dazu beitragen, visuelle Triangulationsfehler zu vermeiden, falls andere Anwendungen anders triangulieren.
* <b>Mit Versatz/Tesselierung</b>: Painter tesseliert den Mesh, fügt weitere Polygone hinzu und verwendet Versatz oder Height, um die Oberflächengeometrie des Meshs zu ändern.
  * <b>Normale des Scheitelpunkts erneut berechnen</b>: Die Änderung der Oberfläche des Meshs kann zu fehlerhaften Normalen bereits vorhandener Scheitelpunkt führen. Wenn diese Option aktiviert ist, aktualisiert Painter die Normalen des Scheitelpunkts automatisch auf den richtigen Wert für die neue Fläche.

![](../assets/export-render.jpg){width="500px"}
