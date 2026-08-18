---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/iray-renderer/viewer-and-mdl-settings.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie den Viewer und die MDL-Einstellungen für den Iray-Renderer in Substance 3D Painter konfigurieren, um das Rendering von Material anzupassen.
helpx_creative_field: ""
helpx_description: Painter > Features > Iray Renderer > Viewer and MDL Settings
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Viewer- und MDL-Einstellungen
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '733'
ht-degree: 0%

---


# Viewer- und MDL-Einstellungen

![](../../assets/display-settings-iray.png){width="400px"}

## Umgebung

Wie im normalen Viewport wird die Beleuchtung durch die in Irak verwendete Umgebungskarte gesteuert.\
Die Umgebungskarte kann durch Klicken auf den Button oder durch Ziehen und Ablegen einer HDR-Textur geändert werden.

* **Umgebungsbelichtung** : Steuern Sie die Belichtungsstufe der HDR-Umgebungszuordnung.
* **Umgebungsrotation** : , um die Umgebungstextur zu verschieben und die Beleuchtung um die Szene zu drehen.

>[!NOTE]
>
> Da Iray ein physikalisch basierter Renderer ist, bestimmt die Umgebungstextur in hohem Maße die Beleuchtung und den Look deiner Szene.

## Kuppel

Die Kuppel ist die Form, auf die die Umgebungskarte im Hintergrund projiziert wird.\
Es stehen drei Arten von Kuppeln zur Verfügung, die je nach Szene zu verwenden sind:

![](../../assets/dome-type.png)

* **Unendliche Sphäre** : Die Umgebung wird im Hintergrund auf eine Kugel projiziert, um den Horizont zu simulieren, also immer weit weg von der Szene
* **Sphäre** : Die Umgebung wird auf einen regulären Bereich projiziert, der skaliert werden kann
* **Kugel mit Boden** : Ähnlich wie bei der vorherigen Form verfügt diese auch über eine Steuerung, um den Boden der Kugel zu reduzieren, um einen Boden zu simulieren.

>[!NOTE]
>
> Die Kugel mit dem Boden verfügt über eine Steuerung, um die Größe/den Radius des Bodens zu definieren. Ein großer Radius jedoch erzeugt Verzerrungen in der Umgebung.\
>  Je nach gewähltem Typ kann die Beleuchtung beeinflusst werden.

Zusätzliche Einstellungen sind verfügbar:

| *Einstellung* | *Beschreibung* |
| --- | --- |
| **Radius** | Die Größe der Kugel (wenn nicht unendlich) |
| **Texturskala** | Gibt an, wie stark die Textur für den Typ **Sphere with ground** gedehnt wird. |
| **Farbe löschen** | Wenn aktiviert, ersetzen Sie das Hintergrundbild der Umgebungszuordnung durch eine einheitliche Farbe. Dies wirkt sich auf die Beleuchtung aus. |

### Bodeneinstellungen

Mit den Bodeneinstellungen können Sie angeben, wo sich ein Stockwerk befindet.\
Standardmäßig ist der Wert so festgelegt, dass der untere Rand des Begrenzungsrahmens der Szene festgelegt wird.

| ***Einstellung*** | ***Beschreibung*** |
| --- | --- |
| **X, Y, Z Wert** | Definieren Sie die Position des Bodens auf den drei Achsen.   Der Wert 0,0,0 entspricht der Mitte des Begrenzungsrahmens der Szene. |
| **Reflexionsgrad** | Definiert die Intensität und die Farbe der Bodenreflexion.   Ein weißer Helligkeitswert bedeutet, dass der Boden zu 100 % reflektierend ist, während Schwarz bedeutet, dass er überhaupt nicht reflektierend ist. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/reflectivity-optim.gif"/></div> |
| **Glossarität** | Legt fest, wie glänzend (oder rau) die Spiegelung ist. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r3-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/glossiness-optim.gif"/></div> |
| **Schattenintensität** | Dieser Parameter legt die endgültige Deckkraft des Schattens fest, nachdem die Beleuchtung berechnet wurde. |
| **Sichtbar von unten** | Legt fest, ob der Boden von unten sichtbar ist oder nicht. Wenn diese Option aktiviert ist, bedeutet dies, dass der Boden alle darüber liegenden Elemente verdeckt. |

## MDL- und Shader-Parameter

Iray verwendet MDL, um die Materialien zu definieren, die für das Rendern eines Objekts verwendet werden. Weitere Informationen finden Sie auf der [offiziellen Nvidia-Seite im Format ](http://www.nvidia.com/object/material-definition-language.html) .

Standardmäßig ist in Substance 3D Painter eine MDL mit einem GLSL-Shader verknüpft. Sie können zwischen dem regulären Viewport und Iray wechseln, ohne etwas konfigurieren zu müssen.\
Die Parameter der MDL werden dann unten in den Anzeigeeinstellungen angezeigt. Im Folgenden finden Sie die Parameter der Standard-MDL (kompatibel mit dem PBR Metallic/Roughness Shader).

>[!NOTE]
>
> Um benutzerdefinierte MDLs zu laden, ist ein benutzerdefinierter GLS-Shader erforderlich.\
>  Im Shader können einige Metadaten hinzugefügt werden, um den MDL-Pfad anzugeben:
> 
> //- Deklarieren Sie das iray mdl-Material für diesen Shader. //: metadata { //: &quot;mdl&quot;:&quot;mdl::alg::materials::physically\_metal\_roughness::physically\_metal\_roughness&quot; //: }
> 
> * **mdl** : Definieren Sie das Iray mdl -Material, das mit dem Shader verwendet werden soll. Die Pfadsyntax lautet wie folgt:  *mdl::folder1::folder2::mdl\_filename::material\_name* wobei *folder1::folder2::mdl\_filename* der Pfad innerhalb eines Ordners der *mdl*-Ablage zu einer mdl-Datei und *::material\_name* der Name eines in dieser mdl-Datei deklarierten Materials ist. (z. B.: &quot;mdl&quot; : &quot;mdl::alg::materials::physically\_metal\_roughness::physically\_metal\_roughness&quot;)

>[!NOTE]
>
> Für jede Materialinstanz in einem Projekt wird eine MDL festgelegt. Um die Materialeigenschaften zwischen Textursatz zu trennen, legen Sie neue Materialinstanz fest, um die MDLs separat zu konfigurieren.

![](../../assets/mdl.png)

Die Standard-MDL von Substance 3D Painter unterstützt die folgenden Eigenschaften:

| *Einstellung* | *Beschreibung* |
| --- | --- |
| **Emissionsintensität** | Multiplikator des Emissionskanals. Ein hoher Wert beginnt, Licht auszustrahlen. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r1-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/emissive-optim.gif"/></div> |
| **Brechung** | Steuert den Grad der Brechung. |
| **IOR** | Definiert den Brechungsindex des Materials.   Hinweis : Luft = 1,0, Wasser = 1,2, Glas = 1,5. |
| **Streuung** | Steuert, wie viel Licht durch die Oberfläche gestreut wird. |
| **Absorption** | Steuert, wie viel Licht durch die Oberfläche absorbiert wird. |
| **Absorptionsfarbe** | Simuliert Farbverschiebungen, wenn Licht durch die Oberfläche einfällt. |
