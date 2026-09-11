---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/painting/presets/photoshop-brush-presets-abr/photoshop-brush-parameters-compatibility.html"
breadcrumb-title: ''
description: Erfahren Sie mehr über die Kompatibilität von Photoshop-Pinselparametern in Substance 3D Painter beim Importieren von ABR-Pinselvorgaben.
helpx_creative_field: ""
helpx_description: Painter > Painting > Presets > Photoshop Brush Presets (ABR) > Photoshop Brush Parameters Compatibility
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Kompatibilität mit Photoshop-Pinselparametern
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '645'
ht-degree: 1%

---


# Kompatibilität mit Photoshop-Pinselparametern

Auf dieser Seite werden alle Photoshop-Pinselparameter und ihre Kompatibilität mit dem Substance 3D Painter-Pinsel-Engine aufgeführt.

## Allgemeine Kompatibilität

Wenn Sie in die ABR-Datei schauen, ruft Substance 3D Painter nur bestimmte Pinsel/Werkzeugvorgaben ab:

| *Vorgabentyp* | *Support* | *Beschreibung* |
| --- | --- | --- |
| **Pinsel (Bitmap)** | Importiert | Pinselvorgaben, die auf Bitmaps basieren, da ihre Alphate importiert werden. |
| **Pinsel (prozedural)** | Ignoriert | Pinselvorgaben, die auf prozeduralen Formen basieren (z. B. ein Kreis), werden nicht importiert. |
| **Pinsel (Airbrush)** | Ignoriert | Pinselvorgaben mit Airbrush-Einstellungen werden nicht importiert. |
| **Pinsel (Borste)** | Ignoriert | Pinselvorgaben mit Borsteneinstellungen werden nicht importiert. |
| **Pinsel (erodierbar)** | Ignoriert | Pinselvorgaben mit erodierbaren Einstellungen werden nicht importiert. |
| **Bleistift** | Ignoriert | Stiftvorgaben werden nicht importiert. |
| **Mischpinsel** | Ignoriert | Pinselvorgaben des Mischers werden nicht importiert. |
| **Klon-Stempel** | Ignoriert | Klon-Stempelvorgaben werden nicht importiert. |
| **Verwischen** | Ignoriert | Verwisch-Vorgaben werden nicht importiert. |

## Parameter

Weitere Informationen zu den Möglichkeiten dieser Parameter finden Sie in der offiziellen [Photoshop-Dokumentation](https://helpx.adobe.com/de/photoshop/using/creating-modifying-brushes.html) .

Nicht alle Photoshop-Pinselparameter werden unterstützt. In der Legende finden Sie Informationen zum Status der einzelnen Parameter, die im Folgenden beschrieben werden:

* **Quadrat (■)** : gibt an, dass der Parameter unterstützt wird, lesen Sie die Beschreibung, um zu erfahren, wie Sie darauf zugreifen können.
* **Kreuz (✖)** : gibt an, dass der Parameter nicht unterstützt wird.

>[!NOTE]
>
> Während Steuerungsparameter in Pinselvorgaben über verschiedene Methoden wie Stift-Neigung, Verblassen-Druck und Stift-Druck gesteuert werden können, wird derzeit nur der **Stift-Druck** unterstützt.

| *Gruppe* | *Parameter* | *Support* | *Beschreibung* |
| --- | --- | --- | --- |
| Form der Pinselspitze | **Größe** | ■ | Mit dem Parameter &quot;Malen-Werkzeuggröße&quot; abgeglichen.  **Hinweis:** Photoshop definiert die Größe in Pixel, während die Größe von Substance 3D Painter auf dem Begrenzungsrahmen des Projekts basiert. Eine exakte Übereinstimmung ist daher nicht möglich und wird nur relativ sein. |
| **X spiegeln** | ■ | Handling via &quot;Brush Maker Photoshop&quot; Substance-Datei. |  |
| **Y spiegeln** | ■ | Handling via &quot;Brush Maker Photoshop&quot; Substance-Datei. |  |
| **Winkel** | ■ | Übereinstimmend mit dem Malen-Werkzeug-Winkelparameter. |  |
| **Rundheit** | ■ | Handling via &quot;Brush Maker Photoshop&quot; Substance-Datei. |  |
| **Härte** | ■ | Handling via &quot;Brush Maker Photoshop&quot; Substance-Datei. |  |
| **Abstand** | ■ | Übereinstimmend mit dem Abstand des Malen-Werkzeugs. |  |
|  |  |  |  |
| Formeigenschaften | **Größe Jitter** | ■ | Übereinstimmend mit dem Jitter &quot;Malen-Werkzeuggröße&quot;. |
| **Steuerelement (für Größe)** | ■ | Abgestimmt auf die Druckeinstellung des Malen-Werkzeugs für den Größenparameter . |  |
| **Mindestdurchmesser** | ■ | Mit dem Parameter &quot;Mindestgröße&quot; des Malwerkzeugs abgestimmt. |  |
| **Neigungsskala** | ✖ |  |  |
| **Winkel-Jitter** | ■ | Mit dem Parameter &quot;Winkel-Jitter&quot; des Malwerkzeugs abgestimmt. |  |
| **Steuerung (für Winkel)** | ✖ |  |  |
| **Rundheits-Jitter** | ■ | Handling via &quot;Brush Maker Photoshop&quot; Substance-Datei. |  |
| **Mindestrundheit** | ■ | Handling via &quot;Brush Maker Photoshop&quot; Substance-Datei. |  |
| **X-Jitter spiegeln** | ■ | Handling via &quot;Brush Maker Photoshop&quot; Substance-Datei. |  |
| **Y-Jitter spiegeln** | ■ | Handling via &quot;Brush Maker Photoshop&quot; Substance-Datei. |  |
| **Pinsel-Projektion** | ✖ |  |  |
|  |  |  |  |
| Streuung | **Streuung** | ■ | Übereinstimmend mit dem Positions-Jitter des Malen-Werkzeugs. |
| **Beide Achsen** | ■ | Mit dem Parameter &quot;Jitter-Achse&quot; für die Position des Malwerkzeugs abgeglichen. |  |
| **Steuerelement (für Streuung)** | ✖ |  |  |
| **Anzahl** | ■ | Kompensiert über den Parameter Abstand des Malwerkzeugs. |  |
| **Jitter zählen** | ✖ |  |  |
| **Steuerelement (für Count Jitter)** | ✖ |  |  |
|  |  |  |  |
| Textur | **Texturen-Pattern** | ✖ |  |
| **Umkehren** | ✖ |  |  |
| **Skalierung** | ✖ |  |  |
| **Helligkeit** | ✖ |  |  |
| **Kontrast** | ✖ |  |  |
| **Textur für jeden Tipp** | ✖ |  |  |
| **Modus** | ✖ |  |  |
| **Tiefe** | ✖ |  |  |
| **Mindestanzahl der Tiefe** | ✖ |  |  |
| **Tiefe Jitter** | ✖ |  |  |
| **Steuerelement (für Tiefe Jitter)** | ✖ |  |  |
|  |  |  |  |
| Dualer Pinsel | **Modus** | ✖ |  |
| **Größe** | ✖ |  |  |
| **Abstand** | ✖ |  |  |
| **Streuung** | ✖ |  |  |
| **Beide Achsen** | ✖ |  |  |
| **Anzahl** | ✖ |  |  |
|  |  |  |  |
| Farbdynamik | **Anwenden pro Tipp** | ✖ |  |
| **Jitter &quot;Vorder-/Hintergrund&quot;** | ✖ |  |  |
| **Steuerelement (für F/B-Jitter)** | ✖ |  |  |
| **Farbton-Jitter** | ✖ |  |  |
| **Sättigungs-Jitter** | ✖ |  |  |
| **Helligkeits-Jitter** | ✖ |  |  |
| **Reinheit** | ✖ |  |  |
|  |  |  |  |
| Transfer | **Deckkraft-Jitter** | ■ | Übereinstimmend mit dem Malen-Werkzeug Stempel Füllparameter auf &quot;Aufhellen&quot; gesetzt. |
| **Steuerelement (für Deckkraft)** | ■ | Abgestimmt auf die Druckeinstellung des Malen-Werkzeugs für den Parameter &quot;Fluss&quot;. |  |
| **Minimum (für Deckkraftsteuerung)** | ■ | Mit dem Malen-Tool-Mindestflussparameter abgeglichen. |  |
| **Flow-Jitter** | ■ | Übereinstimmend mit dem Parameter &quot;Flow-Jitter&quot; des Malen-Werkzeugs. |  |
| **Steuerung (für Flow)** | ■ | Zum Malen-Werkzeug passende Druckeinstellung für den Parameter &quot;Fluss&quot; (wenn niedriger als die Deckkraft) . |  |
| **Minimum (für Flusssteuerung)** | ■ | Mit dem Malen-Werkzeug übereinstimmender Mindestflussparameter (wenn niedriger als die Deckkraft). |  |
| **Wetness-Jitter** | ✖ |  |  |
| **Steuerung (für den Jitter &quot;Nässe&quot;)** | ✖ |  |  |
| **Minimum (für die Wetness-Steuerung)** | ✖ |  |  |
| **Jitter mischen** | ✖ |  |  |
| **Steuerelement (für Mischung)** | ✖ |  |  |
| **Minimum (für Mischsteuerung)** | ✖ |  |  |
|  |  |  |  |
| Pinselhaltung | **Neigung X** | ✖ |  |
| **Neigung X überschreiben** | ✖ |  |  |
| **Neigung Y** | ✖ |  |  |
| **Neigung Y überschreiben** | ✖ |  |  |
| **Drehung** | ✖ |  |  |
| **Drehung überschreiben** | ✖ |  |  |
| **Druck** | ✖ |  |  |
| **Überschreibungsdruck** | ✖ |  |  |
|  |  |  |  |
| Sonstige | **Rauschen** | ✖ |  |
| **Wet Edges** | ✖ |  |  |
| **Aufbau** | ✖ |  |  |
| **Glättung** | ■ | Nicht direkt zugeordnet, kann jedoch über die Einstellung [Verzögerte Mausbewegung](../../lazy-mouse.md) verarbeitet werden. |  |
| **Protect-Textur** | ✖ |  |  |
