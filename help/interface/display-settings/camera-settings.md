---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/interface/display-settings/camera-settings.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie Kameraeinstellungen in Substance 3D Painter konfigurieren, um das Kameraverhalten und die Projektion des Ansichtsfensters zu steuern.
helpx_creative_field: ""
helpx_description: Painter > Interface > Display settings > Camera settings
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Kameraeinstellungen
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 3%

---


# Kameraeinstellungen

Dieser Abschnitt der **Anzeigeeinstellungen** steuert das Verhalten der Kamera sowie das endgültige Aussehen des Viewports.

## Kamera

| *Einstellung* | *Beschreibung* |
| --- | --- |
| **Blickfeld** | Ermöglicht die Steuerung des Sichtfelds der Kamera (in Grad) |
| **Fokusentfernung** | Definiert den Abstand, in dem sich der Fokuspunkt befindet.  Dieser Punkt wird von der Tiefe des Effekts &quot;Feld&quot; verwendet. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/focus-distance-optim.gif"/></div> **Hinweis:** Die Fokusentfernung kann automatisch festgelegt werden, indem Sie mit der Tastenkombination **STRG + mittlere Maustaste** auf einen Punkt des Gitters klicken. |
| **Blende** | Definiert die Breite der Tiefe des Felds. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r3-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/dof-aperture-optim.gif"/></div> **Hinweis:** Wenn Iray diesen Parameter steuert, wird durch Ändern des Parameters eine Berechnung erneut ausgelöst. |

## Post-Effekte

![](../../assets/post.png)

Weitere Informationen finden Sie auf der [Seite nach dem Effekt](../../features/post-processing/post-processing.md).

## Temporale Anti-Aliasing

![](../../assets/taa.png)

Wenn die Option **Temporale Anti-Aliasing** (**TAA**) aktiviert ist, werden gezackte Kanten im Viewport entfernt.\
**TAA** sammelt Informationen über mehrere Rendering-Frames hinweg an. Dies bedeutet, dass der Effekt deaktiviert wird, bis die Kamera nicht mehr bewegt wird oder ein anderer Vorgang ausgeführt wird.

| *Einstellung* | *Beschreibung* |
| --- | --- |
| **Akkumulierungen** | Legt fest, wie viele Frames zur Verringerung des Alias-Effekts kumuliert werden.<ul data-preserve-html="true"> <li data-preserve-html="true">16: Empfohlener Wert für die meisten Fälle</li> <li data-preserve-html="true">64: Nützlich zum Bereinigen hoher Kontrastwerte (z. B. Alpha Test Shader und Dithering kombiniert)</li> </ul>  **Hinweis:** Diese Einstellung hat keine Auswirkungen auf die Leistung. Ein hoher Wert kann jedoch länger dauern, bis gute Ergebnisse erzielt werden. |

![](../../assets/temporal-anti-aliasing.gif){width="500px"}

Mit dem Anti-Aliasing kann auch der Shader **Alpha-Test** gefiltert werden, wenn die Einstellung &quot;**Alpha-Dithering**&quot; aktiviert ist:

![](../../assets/dithering-aa.gif){width="500px"}

## Streuung unter der Oberfläche

![](../../assets/subscat.png)

Weitere Informationen finden Sie auf der Seite [Untergrundstreuung](../../features/subsurface-scattering/subsurface-scattering.md).

## Farbprofil

![](../../assets/profile-13.png)

Weitere Informationen finden Sie auf der [Seite des Farbprofils](../../features/post-processing/color-profile.md).

## Tone Mapping

| Einstellung | Beschreibung |
| --- | --- |
| **Funktion** | Geben Sie die Funktion an, die verwendet wird, um Farbwerte anzupassen, die die Monitoranzeigefunktionen überschreiten (Neuzuordnung von HDR-Werten zu einem LDR-Bereich). Mögliche Werte sind:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Linear</strong> (Standard): Bei keiner Transformation werden Werte über 1,0 geklemmt.</li><li data-preserve-html="true"><strong>ACES</strong>: Verwenden Sie die ACES Filmic-Tone-Mapping-Kurve.</li></ul> <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r1-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/linear-vs-aces.jpg" width="450px"/></div> **Hinweis:** Einige Game Engines und Rendering-Software verwenden den ACES-Tonabbildner. Durch Aktivieren dieser Funktion können Sie Farben zwischen Anwendungen abgleichen und Unterschiede vermeiden. |
