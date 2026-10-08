---
breadcrumb-title: ""
description: Lesen Sie die Versionshinweise für Substance 3D Painter 2017.2, um mehr über neue Funktionen, Verbesserungen und Fehlerbehebungen zu erfahren.
title: Version 2017.2
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 0%
---

# Version 2017.2

Mit **Substance Painter 2017.2** wird eine neue leistungsstarke Funktion über das Ankerpunktsystem eingeführt. Es ermöglicht die Erstellung erweiterter Konfigurationen im Ebenenstapel, was viele neue Möglichkeiten eröffnet.

Freigabedatum: *27. Juli 2017*

## Wichtigste Funktionen

### Effekt &quot;Neuer Ankerpunkt&quot;

![](../../assets/anchor-height-blend-optim.gif)

**Ein neuer Effekttyp** wurde dem Substance Painter hinzugefügt. Neben den bereits vorhandenen Effekttypen **Filter** und **Ebene** finden Sie jetzt den neuen **Ankerpunkt**. Mit diesem neuen Effekt kann ein **Speicherort** im **Ebenenstapel** definiert werden, auf den dann **verwiesen** für den Rest des Projekts in allen anderen Ebenen verwendet werden kann. So kannst du z. B. die Height-Informationen einer Ebene in die Maske einer Ebene direkt darüber einfügen, um eine natürlichere Überblendung zu ermöglichen (siehe GIF oben).

Da der Anker als Effekt fungiert, kann in **vielen Situationen** erstellt werden: den **Inhalt** einer Ebene, die **Maske** und sogar als **Pass-Through**-Filter. Der Effekt funktioniert auch, wenn die Ebene, in der er sich befindet, deaktiviert ist. Beachten Sie, dass der Anker nur einen Speicherort definiert, nicht den, den Sie daraus abrufen können. Diese Informationen werden an der Stelle definiert, an der der Verweis auf den Anker erstellt wird.

Weitere technische Einzelheiten und Beispiele finden Sie auf der entsprechenden Seite: [Ankerpunkt](../../features/effects/anchor-point.md)

### Verschiedene neue Verbesserungen

Neben dem neuen Ankerpunkt-Effekt arbeiteten wir auch an folgenden Themen:

* Die Möglichkeit, einige Effekte umzubenennen, z. B. die Füllung und die Malen
* Neue Skriptfunktionen, die das Erstellen einer Live-Verknüpfung mit anderen Anwendungen wie Unity ermöglichen

## Tutorial

Die neuen Funktionen werden in den neuesten Videos ausführlich erläutert:

## Versionshinweise

### 2017.2

(Release 27. Juli 2017)

**Hinzugefügt:**

* [Effekt] Neuer Ankerpunkt, der Ebenen- und Maskenreferenzen zulässt
* [Ebenen] Möglichkeit, Füll- und Malen-Effekte umzubenennen
* [Plug-In] Aktualisiertes Substance Source-Plug-In
* [Scripting] Abfrage der Auflösung des Textursatzes zulassen
* [Scripting] Ermöglicht das Abrufen des Status des Painting-Engine
* [Leistung] Verbessertes Laden des Projekts und Optimieren des Pinselstempels

**Fest:**

* [Tool] Leistungsprobleme beim Anpassen von Material-Parametern
* [Engine] Verschwindende Pinselstriche bei Änderung der Auflösung (4K>2K)
* [3D-Ansicht] Tangente-Speicherplatz wird nicht mit Bakern synchronisiert
* [Regal] Der Regal-Pfad in den Benutzerdokumenten wird nicht automatisch erstellt
* [Regal] Kompatibilität von Vorgaben mit Vorgängerversionen nach einem Update
* [Shader] Nicht-PBR-Shader funktioniert nicht mehr
* [Baker] ID-Map-Baking schlägt fehl, wenn &quot;Nach Name abgleichen&quot; aktiviert ist
* [Beispiel] Die Namen der Meet Mat-Beispielprojekt-Textursatz sind falsch
* Beim Speichern eines Projekts vor dem Erstellen einer Vorlage werden Schreibberechtigungsfehler zurückgegeben.
