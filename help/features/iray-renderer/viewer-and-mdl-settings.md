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

Wie im regulären Viewport steuert die in Iray verwendete Umgebungs-Map die Beleuchtung.\
Die Umgebungskarte kann durch Klicken auf den Button oder durch Ziehen und Ablegen einer HDR Textur verändert werden.

* **Umgebungsbelichtung** : Steuern Sie die Belichtungsstufe der HDR. Umgebungs-Map.
* **Umgebungsrotation** : , um die Umgebungstextur zu verschieben und die Beleuchtung um die Szene zu drehen.

>[!NOTE]
>
> Da Iray ein physikalisch basierter Renderer ist, bestimmt die Umgebungsbeleuchtung in hohem Maße die Textur und den Look deiner Szene.

## Kuppel

Die Kuppel ist die Form, auf die die Umgebungskarte im Hintergrund projiziert wird.\
Es stehen drei Arten von Kuppeln zur Verfügung, die je nach Szene verwendet werden können:

![](../../assets/dome-type.png)

* **Unendliche Kugel** : Die Umgebung ist im Hintergrund auf eine Kugel projiziert, um den Horizont zu simulieren, so immer weit von der Szene entfernt
* **Sphäre** : Die Umgebung wird auf einen regulären Bereich projiziert, der skaliert werden kann
* **Kugel mit Boden** : Ähnlich wie bei der vorherigen Form verfügt diese auch über eine Steuerung, um den Boden der Kugel zu reduzieren, um einen Boden zu simulieren.

>[!NOTE]
>
> Die Kugel mit Boden kann die Größe/den Radius des Bodens festlegen. Ein großer Radius erzeugt jedoch Verzerrungen in der Umgebung.\
>  Je nach gewähltem Typ kann die Beleuchtung beeinflusst werden.

Zusätzliche Einstellungen sind verfügbar:

| *Einstellung* | *Beschreibung* |
| --- | --- |
| **Radius** | Die Größe der Kugel (wenn nicht unendlich) |
| **Skalierung der Textur** | Gibt an, wie viel die Textur für den Typ **Kugel mit Boden** gedehnt wird. |
| **Farbe löschen** | Wenn aktiviert, ersetzen Sie das Hintergrundbild der Umgebungs-Map durch eine einheitliche Farbe. Dies wirkt sich auf die Beleuchtung aus. |

### Boden-Einstellungen

Mit den Bodeneinstellungen können Sie festlegen, wo sich der Boden befindet.\
Standardmäßig ist der Wert so festgelegt, dass der untere Rand des Begrenzungsrahmens der Szene festgelegt wird.

| ***Einstellung*** | ***Beschreibung*** |
| --- | --- |
| **X, Y, Z Wert** | Definieren Sie die Position des Bodens auf den drei Achsen.   Der Wert 0,0,0 entspricht der Mitte des Begrenzungsrahmens der Szene. |
| **Reflexionsgrad** | Definiert Intensität und Farbe der Boden-Reflexion.   Ein Weißwert bedeutet, dass der Boden zu 100 % reflektierend ist, während Schwarz bedeutet, dass er überhaupt nicht reflektierend ist. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/reflectivity-optim.gif"/></div> |
| **Glanz** | Legt fest, wie glänzend (oder rau) die Spiegelung ist. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r3-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/glossiness-optim.gif"/></div> |
| **Schattenintensität** | Dieser Parameter legt die endgültige Deckkraft des Schattens fest, nachdem die Beleuchtung berechnet wurde. |
| **Sichtbar von unten** | Definiert, ob der Boden von unten sichtbar ist oder nicht. Wenn diese Option aktiviert ist, bedeutet dies, dass der Boden alle darüber liegenden Elemente ausschließt. |

## MDL- und Shader-Parameter

Iray verwendet MDL zum Definieren der Material, die für das Rendern eines Objekts verwendet werden. Weitere Informationen finden Sie auf der [offiziellen Nvidia-Seite im Format ](http://www.nvidia.com/object/material-definition-language.html) .

Standardmäßig ist in Substance 3D Painter eine MDL einem GLSL-Shader zugeordnet. Sie können zwischen dem regulären Viewport und dem Iray wechseln, ohne etwas konfigurieren zu müssen.\
Die Parameter der MDL werden dann unten in den Anzeigeeinstellungen angezeigt. Im Folgenden finden Sie die Parameter der Standard-MDL (kompatibel mit dem PBR-Shader Metallic/Rauheit).

>[!NOTE]
>
> Zum Laden benutzerdefinierter MDLs ist ein benutzerdefinierter GLS-Shader erforderlich.\
>  Im Shader können einige Metadaten hinzugefügt werden, um den MDL-Pfad anzugeben:
> 
> //- Deklarieren Sie das Material iray mdl für diesen Shader. //: metadata { //: &quot;mdl&quot;:&quot;mdl::alg::materials::physically\_metallic\_Rauheit::physically\_metallic\_Rauheit&quot; //: }
> 
> * **mdl** : Definieren Sie das Iray mdl -Material, das mit dem Shader verwendet werden soll. Die Pfadsyntax lautet wie folgt:  *mdl::folder1::folder2::mdl\_filename::Material\_name* wobei *folder1::folder2::mdl\_filename* der Pfad innerhalb eines Ordners Ihres Regals *mdl* zu einer mdl-Datei ist und *::Material\_name* der Name eines in dieser mdl-Datei deklarierten Materials ist. (z. B.: &quot;mdl&quot; : &quot;mdl::alg::materials::physically\_metallic\_Rauheit::physically\_metallic\_Rauheit&quot;)

>[!NOTE]
>
> Für jede Material-Instanz in einem Projekt wird eine MDL festgelegt. Um daher die Materialien-Eigenschaften zwischen Textursätzen zu trennen, legen Sie die neue Materialien-Instanz fest, um die MDLs separat zu konfigurieren.

![](../../assets/mdl.png)

Die Standard-MDL von Substance 3D Painter unterstützt die folgenden Eigenschaften:

| *Einstellung* | *Beschreibung* |
| --- | --- |
| **Emissive-Intensität** | Multiplikator des Emissive-Kanals. Ein hoher Wert beginnt, Licht auszustrahlen. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r1-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/emissive-optim.gif"/></div> |
| **Brechung** | Steuert den Grad der Brechung. |
| **IOR** | Definiert den Brechungsindex des Materials.   Hinweis : Luft = 1,0, Wasser = 1,2, Glas = 1,5. |
| **Streuung** | Steuert, wie viel Licht durch die Oberfläche gestreut wird. |
| **Absorption** | Steuert, wie viel Licht durch die Oberfläche absorbiert wird. |
| **Absorptionsfarbe** | Simuliert Farbverschiebungen, wenn Licht durch die Oberfläche einfällt. |
