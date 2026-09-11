---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/features/iray-renderer/iray-settings.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie in Substance 3D Painter Iray-Renderereinstellungen konfigurieren, um die Rendering-Qualität und -Performance zu steuern.
helpx_creative_field: ""
helpx_description: Painter > Features > Iray Renderer > Iray Settings
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Iray-Einstellungen
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '369'
ht-degree: 0%

---


# Iray-Einstellungen

![](../../assets/iray-settings.png)

Die Iray-Einstellungen steuern das Rendering des IRay-Viewports, seine Laufzeit und seine Qualität.

## Information über Iray

Im oberen Bereich des Fensters wird der Status des Irays neben anderen Informationen angezeigt.

| *Einstellung* | *Beschreibung* |
| --- | --- |
| **Status** | Der Status zeigt an, wie das Iray funktioniert :<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Rendern</strong> (Iray berechnet das Bild)</li><li data-preserve-html="true"><strong>Angehalten</strong> (Iray wurde beendet, aber nicht beendet)</li><li data-preserve-html="true"><strong>Fertig</strong> (Iray-Berechnung abgeschlossen oder Einstellungswerte erreicht)</li></ul> |
| **Auflösung** | Die Auflösung des Iray-Bildes (standardmäßig abhängig von der Viewport-Größe). |
| **Größe der Szene** | Die Größe des Begrenzungsrahmens der Szene/des 3D-Mesh. Es gibt keine Einheit, aber es wird angenommen, dass es in Zentimetern ist. |
| **Iterationen** | Die Anzahl der Berechnungen, die von Irays über den in den Einstellungen festgelegten Höchstwert durchgeführt werden. |
| **Renderzeit** | Die verstrichene Zeit beim Rendern über die in den Einstellungen definierte maximale Zeit. |

>[!NOTE]
>
> Die Anzahl der Iterationen bestimmt die endgültige Qualität des Renderings: mehr Iterationen = bessere Qualität.\
> Iterationen können jedoch etwas Zeit in Anspruch nehmen, weshalb es möglich ist, eine Höchstzeit festzulegen. Eine Iteration wird durch die Anzahl der Samples definiert.

## Einstellungen

Sobald eine Einstellung modifiziert wurde, beginnt Iray mit der Berechnung des Renderings.\
Es ist möglich, das Iray anzuhalten, um dieses Verhalten mit der dedizierten Schaltfläche zu vermeiden:

![](../../assets/pause-2.png)

| *Einstellung* | *Beschreibung* |
| --- | --- |
| **Min. Beispiel** | Minimale Anzahl von Samples, die von Pixeln durchgeführt werden |
| **Max. Beispiel** | Maximale Anzahl von Samples, die von Pixeln ausgeführt werden |
| **Max. Zeit** | Die Höchstdauer, die Irays für die Berechnung eingeräumt wird.  Mit der Dropdown-Liste auf der rechten Seite können Sie die Einheit (Sekunden, Minuten oder Stunden) festlegen. |
| **Kaustisches Sampler aktiviert** | Mit dieser Option können Sie fortschrittlichere Beleuchtungsreflexionen (Kaustik) berechnen. |
| **Firefly-Filter aktiviert** | Mit dieser Option können Sie isolierte und sehr helle Pixel entfernen, die manchmal auftreten können. |
| **Viewport-Auflösung überschreiben** | Mit dieser Einstellung können Sie eine benutzerdefinierte Größe für das Rendering definieren, anstatt die aktuelle Größe des Viewports zu verwenden. Mit der folgenden Einstellung **Breite** und **Height** können Sie die Breite in Pixel definieren. |
| **Render speichern** | Aktion zum Exportieren des aktuellen Renderings (auch wenn es noch nicht abgeschlossen ist) in eine Datei. |
| **Freigeben** | Erlaubt das Freigeben/Exportieren des aktuellen Renderings in [ArtStation](https://www.artstation.com/). |
