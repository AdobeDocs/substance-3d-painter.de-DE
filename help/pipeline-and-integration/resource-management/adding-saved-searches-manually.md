---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/pipeline-and-integration/resource-management/adding-saved-searches-manually.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie in Substance 3D Painter gespeicherte Suchvorgänge manuell hinzufügen, um schnell auf häufig verwendete Ressourcenfilter zuzugreifen.
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Resource management > Adding saved searches manually
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Manuelles Hinzufügen gespeicherter Suchen
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '240'
ht-degree: 2%

---


# Manuelles Hinzufügen gespeicherter Suchen

Assets-Suchabfragen (oder gespeicherte Suchvorgänge) können durch Bearbeiten einer Konfigurationsdatei definiert werden. Auf dieser Seite wird erläutert, wie das geht.

## Speicherort der Konfigurationsdatei

Zum Hinzufügen benutzerdefinierter gespeicherter Abfragen navigieren Sie zum Ordner Dokumente des Benutzers und öffnen Sie die Datei **Shelf.ini**.

<table data-preserve-html="true" style="width: 100.0%;"> <colgroup> <col style="width: 15.0%;"/> <col style="width: 15.0%;"/> <col style="width: 70.0%;"/> </colgroup> <tbody> <tr> <th>Plattform</th> <th>Version</th> <th>Pfad</th> </tr> <tr> <td rowspan="2"><strong>Windows</strong></td> <td><strong>7.2</strong> oder höher</td> <td colspan="1">C:\Users\username\Documents\Adobe\Adobe Substance 3D Painter</td> </tr> <tr> <td colspan="1">Alte Version</td> <td colspan="1">C:\Users\username\Documents\Allegorithmic\Substance Painter</td> </tr> <tr> <td rowspan="2"><strong>Mac</strong></td> <td colspan="1"><strong>7.2</strong> oder höher</td> <td colspan="1">/Users/Benutzername/Documents/Adobe/Adobe Substance 3D Painter</td> </tr> <tr> <td colspan="1">Alte Version</td> <td colspan="1">/Users/Benutzername/Documents/Allegorithmic/Substance Painter</td> </tr> <tr> <td rowspan="2"><strong>Linux</strong></td> <td colspan="1"><strong>7.2</strong> oder höher</td> <td colspan="1">/home/username/Documents/Adobe/Adobe Substance 3D Painter</td> </tr> <tr> <td>Alte Version</td> <td colspan="1">/home/username/Documents/Allegorithmic/Substance Painter</td> </tr> </tbody> </table>

## Beispiel

Im Folgenden finden Sie ein Beispiel für den Inhalt, der in die Konfigurationsdatei eingefügt werden kann:

```
[filters] 

size=4 

1name=Grunge 

1query="u:basematerial=,smartmaterial=,smartmask=,texture=,procedural=,brush=,alpha= grunge" 

2name=Procedural 

2query="u:procedural=" 

3name=Environment 

3query="u:environment=" 

4name=Default Filters 

4query="p:/allegorithmic/^ u:filters="
```


So funktioniert die Syntax:

* **Größe**: bestimmt die Anzahl der benutzerdefinierten Vorgaben, die von der Anwendung gelesen und geladen werden müssen.
* **Zahl**: am Anfang der Zeile definiert die aktuelle Vorgabe, die sie als Ziel hat (z. B.:  **1/**).
* **Abfrage**: (nach der Zahl) definiert die tatsächlich verwendeten Suchbegriffe. Im Beispiel wird **u:** für Verwendungen, **p:** für Pfade oder eine Zeichenfolge für einen Suchbegriff verwendet. Der Inhalt der Abfrage muss in Anführungszeichen eingeschlossen werden. Weitere Informationen zu den verwendbaren Begriffen finden Sie auf [dieser Seite](../../interface/assets/advanced-search-queries.md).
* **Name**: den Namen der Vorgabe an.
