---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/interface/assets/advanced-search-queries.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie erweiterte Suchabfragen in Substance 3D Painter erstellen, um bestimmte Elemente anhand komplexer Suchkriterien zu finden.
helpx_creative_field: ""
helpx_description: Painter > Interface > Assets > Advanced search queries
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Erweiterte Suchabfragen
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 0%

---


# Erweiterte Suchabfragen

Mit erweiterten Suchabfragen können Sie komplexe Suchvorgänge erstellen und als [Gespeicherte Suchvorgänge](saved-searches.md) wiederverwenden.

Erweiterte Abfragen können in der Suchleiste verwendet werden und Folgendes enthalten:

1. **Pfad** : können Sie das Ergebnis einer Suche anhand einer Ordner-/Ordnerstruktur verfeinern.
1. **Nutzung** : Auflisten aller in der Anwendung verfügbaren Verwendungsmöglichkeiten
1. **Textabfrage** : Zulassen, dass jeder andere Abfragetyp frei hinzugefügt werden kann (z. B. benutzerdefinierte Schlüsselwörter)

Beim Definieren einer neuen Suchabfrage sind mehrere Auswahlmöglichkeiten zulässig.

## Pfad

Mit der Pfadabfrage können Sie eine Abfrage basierend auf einem Pfad verfeinern. Im Bereich &quot;**Nach Pfad filtern**&quot; werden alle verfügbaren Bibliotheken aufgeführt (die Sie selbst über &quot;Bearbeiten&quot; > &quot;Einstellungen&quot; > &quot;Bibliotheken&quot; hinzufügen können).\
Sie können die Pfaddefinition verwenden, um nach einem benutzerdefinierten Bibliothekspfad oder nach bestimmten Unterordnern in der Hierarchie zu filtern.

## Nutzung

Verwendung definieren, was eine Ressource ist und wie sie in Substance 3D Painter verwendet wird. Einige können durch den Dateityp der Ressource definiert werden.\
Beispiel:

* **pbr.glsl**: Eine Shader-Datei - sie kann nur als Shader verwendet werden, sonst nichts.
* **effect.sbsar**: Eine Substance-Datei - es kann ein Generator, ein Filter oder sogar ein Material sein, also wenn ihre Verwendung nicht in der Originalgrafik festgelegt ist (in Designer), muss sie vom Anwender in Painter zum Zeitpunkt des Imports angegeben werden.

## Text

Die Textabfrage unterstützt mehrere Typen von Filterungen, wobei einige komplexer sind als die normale Benutzeroberfläche.\
Sie können aktiviert werden, indem Sie die richtigen Stichwörter eingeben.

* **Verfügbare Suchtypen** :
  * &quot; **n:** &quot;: name
  * &quot; **s:** &quot;: Regal/Bibliothek (einschließlich &quot;Sitzung&quot; und &quot;Projekt&quot;)
  * &quot; **p:** &quot;: Pfad
  * &quot; **u:** &quot;: Brauch
* **Entkommen** : Sie können entweder &quot; **\** &quot; vor dem Zeichen verwenden, das escaped werden muss, oder stattdessen Anführungszeichen verwenden, z. B. :
  * **a\ name\ mit\ Leerzeichen**
  * **&quot;ein Name mit Leerzeichen&quot;**
* **Spezifische Attribute (oder Gruppen)** : , um nach bestimmten Attributen zu suchen, fügen Sie einem oder einer Gruppe eine Typangabe hinzu. Beispiel :
  * **n:a,b,c,d** : name ist a oder b oder c oder d
* **Suchverhalten** :
  * Um bestimmte Verwendungen zu filtern, fügen Sie der Suche das bestimmte **Schlüsselwort** hinzu. Beispiel: &quot;**images** ambient&quot;
  * Um mehrere Anforderungen hinzuzufügen, verwenden Sie ein Komma &quot;**,** &quot;, z. B. : &quot;cobalt **,** gold&quot; (wenn Sie ein Komma verwenden, wird bei der Suche nur eine Ressource angezeigt, die mit beiden Schlüsselwörtern gleichzeitig übereinstimmt)
  * Um nach einem genauen Namen zu suchen, verwenden Sie einen Ausrufezeichen &quot;!&quot; am Ende, Beispiel :  **di!**  (gibt **Dirt**, aber nicht **Tropfen** zurück, dieses Schlüsselwort deaktiviert die Fuzzy-Übereinstimmung)
  * Um ein Muster von einer Suche auszuschließen, verwenden Sie einen Bindestrich &quot;**-** &quot;, z. B. :  **u:image n:-normal** (gibt Bilder zurück, die nicht &quot;normal&quot; enthalten)
* **Zuordnungsfunktionen (Mustersuffix):**
  * **Standard** : ungefähre Übereinstimmung (Fuzzy)
  * **enthält** : !
  * **regex** : #
  * **gleich** : =
  * **beginnt mit** : ^
  * **endet mit** : &amp;
