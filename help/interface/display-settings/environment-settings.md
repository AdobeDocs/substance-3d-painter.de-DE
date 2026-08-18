---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/interface/display-settings/environment-settings.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie in Substance 3D Painter Umgebungseinstellungen konfigurieren, um Beleuchtung und Hintergrund für die Materialvorschau zu steuern.
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

Dieser Abschnitt der **Anzeigeeinstellungen** steuert die Beleuchtung im Viewport.

## Umgebung

![](../../assets/env-settings.png)

| *Einstellung* | *Beschreibung* |
| --- | --- |
| **Umgebungszuordnung** | Umgebungsmap-Textur, mit der die Szene beleuchtet wird. Sie können im Fenster [Assets](../assets/assets.md) mithilfe der Vorgabe &quot;Umgebung&quot; gefunden werden.Klicken Sie auf die Schaltfläche, um ein Mini-Regal zu öffnen und eine andere Umgebungskarte auszuwählen. |
| **Farbraum für Umgebungszuordnung überschreiben** | Wenn das aktuelle Projekt [Farbmanagement](../../features/color-management/color-management.md) verwendet, kann diese Einstellung aktiviert werden, um den Farbraum der Umgebungszuordnung zu überschreiben. |
| **Umgebungsdeckkraft** | Steuert die Sichtbarkeit/Deckkraft der Umgebungstexturen im Hintergrund des Viewports. Diese Einstellungen haben keinen Einfluss auf die Beleuchtung der Szene. |
| **Umgebungsbelastung** | Der Belichtungswert (EV) ist eine Zahl, die eine feste Szenenluminanz darstellt. Mit dieser Einstellung kann der standardmäßige Luminanzwert versetzt werden.Diese Einstellung sollte bei der Arbeit mit den Umgebungskarten, die mit der Anwendung bereitgestellt werden, auf 0 bleiben. Die Texturierung eines Assets mit einem falschen Belichtungswert kann in anderen Anwendungen zu Problemen bei der Farbkalibrierung führen. |
| **Umgebungsdrehung** | Steuert die horizontale Drehung der Umgebungsstruktur. Diese Option ist nützlich, wenn Sie die Beleuchtung in der Szene drehen und die Art und Weise ändern möchten, wie das Objekt reagiert. Kann mit einem [Tastaturbefehl](../settings/shortcuts.md) gesteuert werden. |
| **Umgebungsunschärfe** | Steuert, wie scharf oder unscharf die Umgebungstextur im Hintergrund des Viewports erscheinen soll. Diese Einstellungen haben keine Auswirkungen auf die Beleuchtung. |
| **Umgebungsausrichtung** | Steuert, wie sich die Umgebungstextur im Ansichtsfenster um den 3D-Modus dreht. Diese Einstellung kann verwendet werden, um Bereiche unter dem 3D-Modell aufzuhellen, wenn sie auf &quot;Lokal&quot; eingestellt ist.Mögliche Werte:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Welt</strong> (Standard): Die Umgebung wird an der Szene ausgerichtet und um die Hochachse des 3D-Modells gedreht.</li><li data-preserve-html="true"><strong>Lokal</strong>: Die Umgebung wird an der Kamera ausgerichtet und um die Hochachse der Kamera gedreht.</li></ul> |

## Schatten

![](../../assets/shadow-2.png)

| *Einstellung* | *Beschreibung* |
| --- | --- |
| **Schatten** | Aktivieren/Deaktivieren des Renderns von Schatten im Viewport. |
| **Berechnungsmodus** | Steuert, wie schnell die Schatten berechnet werden.<ul data-preserve-html="true"><li data-preserve-html="true"><strong> Intensiv </strong> : Berechnen Sie schnell, kann aber das Rendern des Ansichtsfensters einfrieren.</li><li data-preserve-html="true"><strong> Durchschnitt </strong> : Durchschnitt des intensiven und leichten Modus.</li><li data-preserve-html="true"><strong> Lightweight </strong> : (Standard) Die Schatten werden über einige Sekunden langsam berechnet, die Leistung des Ansichtsports wird jedoch nicht verlangsamt.</li></ul> |
| **Schattendeckkraft** | Steuert, wie viel Schatten in der Szene sichtbar sein werden. |
