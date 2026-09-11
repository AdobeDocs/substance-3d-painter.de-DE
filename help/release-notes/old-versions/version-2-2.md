---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/release-notes/old-versions/version-2-2.html"
breadcrumb-title: ''
description: Lesen Sie die Versionshinweise für Substance 3D Painter 2.2, um mehr über neue Funktionen, Verbesserungen und Fehlerbehebungen zu erfahren.
helpx_creative_field: ""
helpx_description: Painter > Release notes > Old versions > Version 2.2
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Version 2.2
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 0%

---


# Version 2.2

**Substance Painter 2.2** fügt einen neuen Workflow hinzu, der die Dynamische Materialüberlagerung ist.

Freigabedatum: *21. Juli 2016*

## Wichtigste Funktionen

### Neuer Arbeitsablauf für Dynamische Materialüberlagerung

![](../../assets/dynamic-material-blending-materials-preview.jpg)

Mit dieser neuen Version fügen wir einen neuen **Workflow** hinzu, der als **Materialschichtung** bezeichnet wird. Herkömmliche Texturierungs-Workflows basieren auf dem Erstellen von Texturen mit **hoher Auflösung** bis **Details erhalten**, dies ist jedoch **nicht praktisch** für den Anwendungsfall. Ein interessanterer Ansatz ist es, **ein kleines Material zu erstellen** und **es in einem Shader zu wiederholen**. Es ermöglicht, eine bestimmte Qualität beizubehalten und **mit diesem Shader** sehr nah **an das Objekt heranzoomen, ohne dass Einzelheiten verloren gehen**. Das einzige Problem ist, dass es für die Vorschau des Endergebnisses vorher zwingend erforderlich war, zum Engine/Renderer zu gehen, der den endgültigen Shader anzeigt. Das stimmt nicht mehr, da es in dieser neuen Version jetzt möglich ist, einen ähnlichen Shader innerhalb von Substance Painter zu verwenden, mit dem Sie **das Endergebnis visualisieren und gleichzeitig malen können**.

Ein **neues Beispielprojekt** mit dem Namen &quot;**FireHydrant**&quot; wurde hinzugefügt, um den neuen Arbeitsablauf zu präsentieren.

![](../../assets/layer-stacks.png)

Dieser neue Arbeitsablauf eröffnet zwei Arbeitsweisen:

* Materialien sind im Shader definiert, Sie können nur Malen Masken, um sie zu mischen
* Materialien und Masken können gemeinsam bemalt werden

In jedem Fall ist es möglich, jedes Mal einen neuen Ebenenstapel zu definieren, der mehr Spielraum beim Erstellen der Masken und Materialien bietet. Die Verwaltung von Ebenen ist auf diese Weise viel einfacher, und jeder Stapel kann über einen eigenen Satz spezifischer Kanäle verfügen, die im endgültigen Shader überblendet werden können.\
Wir haben auch einen speziellen Shader für Unity 5 und Unreal Engine 4 auf Share :

* [Einheit 5](https://share.allegorithmic.com/libraries/2126)
* [Unreal Engine 4](https://share.allegorithmic.com/libraries/2125)

Weitere Informationen finden Sie auf der entsprechenden Seite der Dokumentation : [Dynamische Materialüberlagerung](../../features/dynamic-material-layering.md)

### Neues Mini-Regal-Suchfeld

![](../../assets/mini-shelf-search.gif)

Wir haben das **Mini-Regal**, das an verschiedenen Stellen der Anwendung angezeigt wird, mit einem dedizierten Suchfeld verbessert. Diese Verbesserung macht die Suche nach Ressourcen viel bequemer und angenehmer zu bedienen. Die benutzerdefinierte Suche bleibt während der aktuellen Sitzung der Anwendung erhalten. Wenn Sie z. B. viele Schmutz-Rauschen verwenden, macht die Verwendung dieses Schlüsselworts

## Tutorial

In unserem neuesten Video-Tutorial lernen Sie die neuen Funktionen kennen:

## Versionshinweise

### 2.2.0

(Release 21. Juli 2016)

**Hinzugefügt:**

* [Shelf] Verbesserung des Suchsystems und der Suchanfragen
* [Shelf] Hinzufügen eines Suchfelds für Mini-Shelfs
* [Shader] Festlegen der Schrittpräzision für Schieberegler
* [Shader] Schaltfläche &quot;Rückgängig/Wiederholen&quot; für Shader-Parameter hinzufügen
* [Shader] Das erneute Laden eines Shaders sollte seine Parameter nicht zurücksetzen
* [MathLayering] Unterstützung für Dynamische Materialüberlagerung und Unterstapel hinzufügen
* [MathLayering] Importieren der JSON-Datei zum Einrichten der Shader-Einstellungen zulassen
* [MathLayering] Entsperren Sie das Limit für Texturaufnehmer (Wechsel zu Bindless-Texturen).
* [Scripting] Baker-Einstellungen festlegen und Berechnung starten
* [Substance] &quot;Verwendung&quot; für Ein-/Ausgangsverbindungen zusätzlich zu Kennungen verwenden
* [Tool] Erlaubt die Auswahl des Vorschaukanals im Ansichtsfenster für das Projektionswerkzeug.

**Fest:**

* Absturz beim Start, wenn sich Substanzen im falschen Ordner befinden
* Absturzbericht funktioniert manchmal nicht aufgrund einer falschen Protokolldatei
* [Iray] Post-Effekte werden nicht aktualisiert, wenn Iray angehalten wird
* [Iray] Kurzbefehl für den automatischen Fokus funktioniert nicht mehr
* [Abray] Verhalten des Blendenreglers ändert sich je nach Elementgröße
* [Ebenen] Der Kanal des ersten Materials ist standardmäßig nicht aktiviert, wenn alle deaktiviert sind
* [Shader] Es werden keine Fehler ausgegeben, wenn ein &quot;param auto&quot; nicht korrekt ist.

**Bekanntes Problem :**

* [Mac] Grenzwert für Textur-Samples auf 16 gesperrt (GPU-Treiberproblem)
