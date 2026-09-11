---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/painting/dynamic-strokes/creating-custom-dynamic-strokes.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie in Substance 3D Painter benutzerdefinierte Dynamische Pinselstriche erstellen, um einzigartige Verhalten und Effekte für Pinselstriche zu entwerfen.
helpx_creative_field: ""
helpx_description: Painter > Painting > Dynamic strokes > Creating Custom Dynamic Strokes
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Erstellen benutzerdefinierter Dynamische Pinselstriche
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---


# Erstellen benutzerdefinierter Dynamische Pinselstriche

Zum Erstellen benutzerdefinierter Dynamische Pinselstriche sind zwei Optionen verfügbar:

* Verwenden einer vorhandenen Substance-Ressource zum Erstellen eines neuen Pinsels/einer neuen Werkzeugvorgabe
* Erstellen Sie eine neue Substance-Ressource von Grund auf neu (erfordert [Substance 3D Designer](https://substance3d.adobe.com/display/SDDOC/Substance+Designer) ).

Es wird außerdem empfohlen, die [Dynamic Stroke Performances](dynamic-stroke-performances.md) zu lesen, bevor benutzerdefinierte Substance-Dateien erstellt werden, um Schuldige zu vermeiden.

## Vorhandene Ressource wiederverwenden

Das Erstellen neuer Dynamische Pinselstriche von Grund auf kann schwierig sein. Vorhandene Ressourcen zu nutzen, anzupassen und sie dann als neue Vorgaben zu speichern, kann ein guter Ausgangspunkt sein.

Suchen Sie im Regal nach kompatiblen Ressourcen, die Ihren Anforderungen entsprechen, und sehen Sie sich dann unsere Seite zu [Vorgaben](../presets/presets.md) an.

## Erstellen benutzerdefinierter Substance-Dateien für Dynamische Pinselstriche

Im Folgenden finden Sie eine Liste der unterstützten Parameter für Dynamische Pinselstriche in Substance-Grafen.

| Variable Identifizierung | Beschreibung |
| --- | --- |
| <b>Zufallsparameter</b> | Wenn eine Substance-Datei mit gelegt Zufallsverteilung gekocht wird, kann sie mit der Funktion &quot;Dynamischer Strich&quot; gesteuert werden. |
| <b>stampIndex</b> | <b>Ganzzahl1</b> Wird beim Malen des Pinselstrichs von Substance 3D Painter zugeführt. Die Minimal- und Maximalwerte haben keine Auswirkungen, sie werden von Substance 3D Painter ignoriert. |
| <b>stampCycleCount</b> | <b>Ganzzahl1</b> Painter liest den Parameterstandardwert, den Minimal- und den Maximalwert, um den Parameter &quot;Stempelzyklusanzahl&quot; legen. Dieser Parameter steuert, wie viele eindeutige Substance-Varianten erstellt werden. |
| <b>$time</b> | <b>Fließkommazahl1</b> Wird von Substance 3D Painter gespeist, wenn der Pinselstrich auf der Grundlage der verstrichenen Malzeit (pro Strich) gemalt wird. Diese Eigenschaft kann viele Substance-Varianten generieren und sich daher auf die Leistung auswirken. |
| <b>strokeSpacing</b> | <b>float1</b> Der aktuelle Abstandswert für den gesamten gemalten Strich. |
| <b>strokeSize</b> | <b>float1</b> Der aktuelle Größenwert für den gesamten gemalten Strich. |
| <b>stampStrokePosition</b> | <b>Ganzzahl1</b> Wird verwendet, um den Beginn/Anfang einer Kontur anzugeben. Der Endwert ist nur auf dem Pfadstrich verfügbar, nicht beim manuellen Malen. Mögliche Werte:<ul data-preserve-html="true"> <li data-preserve-html="true">0 = Mitte</li> <li data-preserve-html="true">1 = Start</li> <li data-preserve-html="true">2 = Ende</li> </ul>Kann mit dem isstrokepositionactive Benutzertag deaktiviert werden. |
| <b>distanceAlongCurve</b> | <b>float1</b> Der aktuelle Abstand am angegebenen Stempel entlang eines Pfads. Diese Eigenschaft kann viele Substance-Varianten generieren und sich daher auf die Leistung auswirken. Kann mit dem <b>iscurvedistanceactive</b>-Benutzer-Tag deaktiviert werden. |
| <b>distanceMaxCurve</b> | <b>float1</b> Die Gesamtlänge eines mit dem Pfadwerkzeug erstellten Pfads. Kann mit dem <b>iscurvedistanceactive</b>-Benutzer-Tag deaktiviert werden. |
| <b>pathCorner</b> | <b>Ganzzahl1</b> Geben Sie an, welchen Eckentyp ein Menüband verwendet. Mögliche Werte:<ul data-preserve-html="true"> <li data-preserve-html="true">0 = Keine Ecke</li> <li data-preserve-html="true">1 = Linke Ecke</li> <li data-preserve-html="true">2 = Rechte Ecke</li> </ul> |
| <b>pathCornerAngle</b> | <b>Gleitend</b> Winkel (im Radianten) der Ecke auf einem Bandpfad. Kann verwendet werden, um das Aussehen einer Ecke basierend auf einem genauen Winkelwert zu kompensieren oder anzupassen. |
| <b>patchLengthOnCurve</b> | <b>float</b> Größe eines Abschnitts (Patches) auf einem Bandpfad. In Kombination mit <b>distanceAlongCurve</b> und <b>distanceMaxCurve</b> kann sie beispielsweise verwendet werden, um die Größe eines Patches zu normalisieren. |
