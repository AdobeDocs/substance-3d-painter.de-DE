---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/features/uv-tiles/image-sequence.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie Bildsequenzen mit UV-Kacheln in Substance 3D Painter für animierte Textur-Workflows verwenden.
helpx_creative_field: ""
helpx_description: Painter > Features > UV Tiles > Image Sequence
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Bildsequenz
user-guide-description: ''
user-guide-title: ''
source-git-commit: 8b892d2d6c9d0f1a3b5d9d3ab9b180a7c2770a83
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 0%

---


# Bildsequenz

Bildsequenzen sind eine Zusammenstellung von Bildern, die als eine einzige Ressource im Regal gruppiert sind. Bilder werden anhand eines bestimmten Musters in ihren Dateinamen gruppiert.

## Bilder als Sequenz importieren

Wenn der Dateiname beim Importieren einer Bilddatei mit einem bestimmten Muster übereinstimmt, wird er automatisch als Sequenz importiert. Wenn sich neben der importierten Datei weitere Bilder befinden, werden diese ebenfalls berücksichtigt. Es ist daher nicht erforderlich, alle Dateien aus einer Sequenz manuell zu importieren, da es genügt, die erste Datei auszuwählen.

Beispiele für passende Dateinamen:

Die folgenden Dateinamen können eine Bildsequenz erfolgreich importieren, da sie erkennen, dass der letzte Teil des Dateinamens auf eine UDIM-Nummer 1032 verweist:

* Datei\_22.1032.jpg
* Datei\_22-223.1032.jpg
* Datei\_22-223-1032.jpg
* Datei\_22-223\_1032.jpg

Die folgenden Dateinamen werden nicht als Bildsequenz importiert, da sie nicht korrekt strukturiert sind:

* Datei\_22-2232032.jpg
* Datei\_22-223PM2032.jpg
* Datei\_22-223-0032.jpg
* Datei\_22-223\_Rec2020.jpg

Der Dateinamenabgleich basiert auf dem folgenden regulären Ausdruck:

```
 ^(.+?)[\.\-\_](?
```


## Bildsequenzen verwenden

Bildsequenzen können wie jede andere Ressource in einen beliebigen Ressourcenplatz der Schnittstelle geladen werden. In einigen Fällen können jedoch zusätzliche Einstellungen erforderlich sein, um ordnungsgemäß verwendet zu werden.

Stellen Sie in [Füllebenen](../../painting/fill-projections/fill-projections.md) (und Fülleffekte) sicher, dass der Sequenzmodus auf **Projektion (Übereinstimmung pro UV-Kachel)** festgelegt ist, um sicherzustellen, dass jedes Bild aus der Sequenz der rechten [UV-Kachel](uv-tiles.md) im Textursatz zugewiesen ist.
