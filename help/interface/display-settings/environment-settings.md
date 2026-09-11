---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/interface/display-settings/environment-settings.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie Umgebungseinstellungen in Substance 3D Painter konfigurieren, um Beleuchtung und Hintergrund für die Vorschau des Materials zu steuern.
helpx_creative_field: ""
helpx_description: Painter > Interface > Display settings > Environment settings
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Umgebungseinstellungen
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 1%

---


# Umgebungseinstellungen

Dieser Abschnitt der **Anzeigeeinstellungen** steuert die Beleuchtung des Viewports.

## Umgebung

![](../../assets/env-settings.png)

| *Einstellung* | *Beschreibung* |
| --- | --- |
| **Umgebungs-Map** | Umgebungs-Map-Textur zum Beleuchten der Szene. Sie können im Fenster [Assets](../assets/assets.md) mithilfe der Vorgabe &quot;Umgebung&quot; gefunden werden.Klicken Sie auf die Schaltfläche, um ein Mini-Regal zu öffnen und eine andere Umgebungs-Map auszuwählen. |
| **Umgebungs-Map-Farbraum überschreiben** | Wenn das aktuelle Projekt [Farbmanagement](../../features/color-management/color-management.md) verwendet, kann diese Einstellung aktiviert werden, um den Farbraum der Umgebungs-Map zu überschreiben. |
| **Umgebungsdeckkraft** | Steuert die Sichtbarkeit/Deckkraft der Texturen der Umgebung im Hintergrund des Viewports. Diese Einstellung hat keine Auswirkungen auf die Beleuchtung der Szene. |
| **Umgebungsbelastung** | Der Belichtungswert (EV) ist eine Zahl, die eine Luminanz mit fester Szene darstellt. Bei dieser Einstellung kann der Standardwert für die Luminanz versetzt werden.Diese Einstellung sollte bei der Arbeit mit den Umgebungs-Map, die mit der Anwendung bereitgestellt wurden, auf 0 bleiben. Die Texturierung eines Assets mit einem falschen Belichtungswert kann in anderen Anwendungen zu Problemen bei der Farbkalibrierung führen. |
| **Umgebungsdrehung** | Steuert die horizontale Drehung der Umgebungsdrehung in der Textur. Diese Option ist nützlich, wenn Sie das Licht in der Szene drehen und die Art und Weise ändern möchten, wie das Objekt reagiert. Kann mit einem [Tastaturbefehl](../settings/shortcuts.md) gesteuert werden. |
| **Umgebungsunschärfe** | Steuert, wie scharf oder unscharf die Umgebungsfarbe im Hintergrund des Viewports Textur wird. Diese Einstellungen haben keine Auswirkungen auf die Beleuchtung. |
| **Umgebungsausrichtung** | Steuert, wie sich die Textur der Umgebung im Viewport um den 3D-Modus dreht. Diese Einstellung kann verwendet werden, um Bereiche unter dem 3D-Modell aufzuhellen, wenn sie auf &quot;Lokal&quot; eingestellt ist.Mögliche Werte:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Welt</strong> (Standard): Die Umgebung wird an der Szene ausgerichtet und um die Achse nach oben des 3D-Modells gedreht.</li><li data-preserve-html="true"><strong>Lokal</strong>: Die Umgebung ist an der Kamera ausgerichtet und dreht sich um die Achse nach oben der Kamera.</li></ul> |

## Schatten

![](../../assets/shadow-2.png)

| *Einstellung* | *Beschreibung* |
| --- | --- |
| **Schatten** | Aktivieren/Deaktivieren des Renderns von Schatten im Viewport. |
| **Berechnung-Modus** | Steuert, wie schnell die Schatten berechnet werden.<ul data-preserve-html="true"><li data-preserve-html="true"><strong> Intensiv </strong> : Berechnen Sie schnell, kann aber das Rendern des Viewports einfrieren.</li><li data-preserve-html="true"><strong> Durchschnitt </strong> : Durchschnitt des intensiven und leichten Modus.</li><li data-preserve-html="true"><strong> Lightweight </strong> : (Standard) Die Schatten werden über einige Sekunden langsam berechnet, aber die Leistung des Viewports wird nicht verlangsamt.</li></ul> |
| **Schattendeckkraft** | Steuert, wie viele Tiefen in der Szene zu sehen sind. |
