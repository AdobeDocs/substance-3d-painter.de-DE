---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/rendering-issues/blocky-artifacts-appear-on-textures-in-the-viewport.html"
breadcrumb-title: ''
description: Hier erfahren Sie, wie Sie blockartige Artefakte auf Texturen in Substance 3D Painter Viewport korrigieren, um eine klare Bildqualität zu erzielen.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Rendering Issues > Blocky artifacts appear on textures in the viewport
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Blockige Artefakte erscheinen auf Texturen im Viewport
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 0%

---


# Blockige Artefakte erscheinen auf Texturen im Viewport

Ab Version 2018.3.0 können folgende Artefakte im Viewport auftreten:

![](../../../assets/viewport-artifacts.jpg){width="400px"}

Diese Artefakte beziehen sich auf Probleme mit Nvidia-GPU-Treibern.\
Um die Artefakte zu vermeiden, muss der Hardware-Support der Dünn besetzte virtuelle Textur deaktiviert werden.

Die GeForce **Treiber 440.97** haben dieses Problem jetzt **behoben** . Wir haben empfohlen, auf diese Treiber zu aktualisieren und SVT aktiviert zu lassen, um gute Leistungen zu erzielen.

Neue Treiber sind auf der Nvidia-Website verfügbar: <https://www.nvidia.com/Download/index.aspx>

## Deaktivieren der Dünn besetzte virtuelle Textur Hardwarebeschleunigung

### 1 - Starten Sie Substance 3D Painter und öffnen Sie die Einstellungen.

![](../../../assets/settings-34.png)

Öffnen Sie die Haupteinstellungen über Bearbeiten > Einstellungen.

### 2 - Suchen Sie den Abschnitt &quot;Dünn besetzte virtuelle Texturen&quot;

![](../../../assets/svt-subsection.png)

Scrollen Sie im Abschnitt &quot;Allgemein&quot; nach unten und suchen Sie nach dem Unterabschnitt &quot;Dünn besetzte virtuelle Texturen&quot;.

### 3 - Deaktivieren Sie die Einstellung

![](../../../assets/uncheck-hardware.png)

Deaktivieren Sie die Einstellung &quot;Beschleunigung des Hardware-Supports&quot;, indem Sie sie deaktivieren.

### 4 - Substance 3D Painter validieren und neu starten

![](../../../assets/validate-1.png)

Bestätigen Sie die Änderung, indem Sie auf &quot;OK&quot; klicken.

![](../../../assets/restart-3.png)

Starten Sie Substance 3D Painter neu, indem Sie auf die Schaltfläche &quot;Ja&quot; klicken, um die Änderung anzuwenden.
