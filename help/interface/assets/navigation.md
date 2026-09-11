---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/interface/assets/navigation.html"
breadcrumb-title: ''
description: Im Bedienfeld "Elemente" in Substance 3D Painter können Sie Ihre Ressourcenbibliothek durchsuchen und effizient darauf zugreifen.
helpx_creative_field: ""
helpx_description: Painter > Interface > Assets > Navigation
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Navigation
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '830'
ht-degree: 1%

---


# Navigation

Im Bedienfeld &quot;Elemente&quot; gibt es verschiedene Navigationsmöglichkeiten: Breadcrumbs, Suchfelder und das Symbol für Elementtypen. Alle Navigationstypen sind koabhängig, sodass Sie diese Suchvorgänge zu Ihrem Vorteil kombinieren können.\
Wenn Sie beispielsweise in Ihren Symbolen für Elementtypen Materialien ausgewählt haben, aber die Breadcrumbs verwendet haben, um zum Bibliotheksordner zu navigieren, zeigt das Bedienfeld &quot;Elemente&quot; keine Ergebnisse an. Sie müssen zu &quot;Alle Intelligente Masken&quot; zurückkehren, wenn Sie Materialien anzeigen möchten, oder die Auswahl von Materialien aufheben, wenn Sie die Intelligente Masken durchsuchen möchten.

## Breadcrumbs

Mit Breadcrumbs können Sie schnell durch die Bibliothek navigieren. Wenn Sie auf die Pfeile klicken, wird angezeigt, wie die Assets auf dem Datenträger gespeichert werden, und Sie können einen der angezeigten Speicherorte auswählen. Wenn sie ausgegraut ist, bedeutet dies, dass es in diesem Ordner keine Assets des ausgewählten Typs gibt, Sie jedoch zu diesem Ordner navigieren können.

![](../../assets/00-05-breadcrumbs.jpg)

## Suchfeld

Das Suchfeld kann verwendet werden, um Ressourcen zu filtern, die die typisierte Abfrage enthalten. Beachten Sie, dass nicht nur nach dem Titel der Ressourcen gesucht wird, sondern auch nach ihrem Speicherort und allen in der Ressource enthaltenen Tags.\
Eingegebene Suchvorgänge können auch komplexer sein als nur Stichwörter. Siehe [Erweiterte Suchabfragen](advanced-search-queries.md).

![](../../assets/00-05-searchfield.jpg)

## Elementtypen

>[!NOTE]
>
> Die Symbole des Elementtyps können mehrfach ausgewählt werden, indem **Strg** beim Klicken beibehalten wird.

Die Standardauswahl ist &quot;Materialien&quot;. Wenn Sie jedoch auf andere Symbole für Elementtypen klicken, werden andere Ressourcen angezeigt.

![](../../assets/00-05-assettypeicons.jpg)

| Elementtypen | Beschreibung |
| --- | --- |
| Materialien <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/00-05-assettypes-1-1.png"/></div> | Enthält als *Basismaterial* importierte .sbsar-Dateien und aus einer Füllebene erstellte Materialien (weitere Informationen zur Vorgabenerstellung [hier](https://helpx.adobe.com/de/substance-3d/unlisted/documentation/spdoc/creating-and-saving-a-preset-180191514.html)). Es handelt sich um einfache Materialien, die in Füllebenen verwendet werden können und auf die gesamte Fläche Ihres Meshs oder Textursatzes angewendet werden. |
| Intelligente Materialien <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/00-05-assettypes-7.png"/></div> | Enthält komplexere Materialien, die aus mehreren Ebenen bestehen, die in einem Ordner gespeichert sind (Intelligente Materialien sind auch Vorgaben, die Sie selbst erstellen können). Wie Basismaterialien gelten Intelligente Materialien für den gesamten Mesh/Textursatz, berücksichtigen aber auch die individuellen Informationen Ihres Meshs wie Krümmung, Verdeckung oder andere Oberflächendetails. Um diese Oberflächendetails abzurufen und Intelligente Material richtig zu verwenden, muss Ihr Mesh zunächst [Baking geführt](../../baking/baking.md) sein. |
| Smart-Masken <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r3-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/00-05-assettypes-2.png"/></div> | Enthält komplexere Masken, die Effekte und/oder Generatoren mit mehreren Ebenen verwenden. Sie können [Intelligente Masken-Vorgaben selbst erstellen](https://helpx.adobe.com/de/substance-3d/unlisted/documentation/spdoc/managing-assets-217187091.html).Ähnlich wie bei Intelligenten Materialien benötigen Intelligente Masken Baking geführt Informationen von Ihrem Mesh, um korrekt zu arbeiten. |
| Filter <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r4-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/00-05-assettypes-3.png"/></div> | Enthält als *filter* importierte .sbsar-Dateien.Mit Filtern transformieren du deine bereits vorhandene Textur auf eine Weise. Einige Filter funktionieren nur mit Schwarzweißinformationen, andere nur mit Material-Eingaben, d. h., nicht alle Filter können in Masken verwendet werden. |
| Pinsel <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r5-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/00-05-assettypes-4.png"/></div> | Enthält Pinsel, Partikeln und Werkzeuge. Dies sind alles Vorgaben, die [in Painter erstellt](https://helpx.adobe.com/de/substance-3d/unlisted/documentation/spdoc/managing-assets-217187091.html) werden können.**Pinsel** sind einfache Schwarzweiß-Vorgaben, die einen Alpha-Wert verwenden. Sie können Pinsel zum Malen in einem oder allen Kanälen oder in einer Maske verwenden.**Partikeln** haben die gleichen Eigenschaften wie Pinsel, verfügen aber auch über einen zusätzlichen Parametersatz, der die physische Interaktion mit Ihrem Mesh simuliert. Sie können die Auswirkungen von verschütteten Flüssigkeiten, Tropfen, Regen oder jeder anderen erzeugen, die eine physikalische Simulation erfordern.**Tools** können das Verhalten &quot;Pinsel&quot; und/oder &quot;Partikel&quot; enthalten. Zusätzlich wird diese Vorgabe jedoch auch mit Informationen zu den Material-Kanälen gespeichert. |
| Alphas <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r6-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/00-05-assettypes-5.png"/></div> | Enthält eine Vielzahl von Alphaten sowie mehrere Pinselmacher, mit denen [Pinsel mit aufwändigeren Effekten (Photoshop-ähnliche Pinsel, Dynamische Pinselstriche, Malen-Rolle) erstellt werden können. Alphas sind Graustufenbilder, in denen schwarze Teile transparent erscheinen, wenn sie verwendet werden.](https://helpx.adobe.com/de/substance-3d/unlisted/documentation/spdoc/managing-assets-217187091.html) |
| Texturen <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r7-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/00-05-assettypes-6.png"/></div> | Enthalten Grunges, Prozedurale, durch Baking erzeugte Map, Hardsurface-Normale und LUTs.**Grunges** sind Graustufenbilder mit interessanten Rauschen und Texturen. Mit ihnen kannst du die Oberfläche deines Meshs variieren, entweder über eine Maske oder indem du sie direkt in einen Kanal einfügst.**Procedurals** sind ebenfalls Graustufen-Texturen, die Rauschen oder sogar reguläre Muster umfassen. Im Gegensatz zu einigen statischen Grunges sind Prozedurale jedoch dynamische Bitmaps, die ohne Wiederholung skaliert werden können und unendliche Variationen aufweisen (über Zufallssaatgut).**Durch Baking erzeugte Map** stellen die Oberflächeninformationen und Forminformationen dar, die aus Ihrem Mesh extrahiert wurden. Weitere Informationen zum Baking finden Sie hier.**Normalwerte für die harte Oberfläche** sind Details, die Sie direkt auf Ihren Mesh stempeln können, indem Sie den Kanal &quot;Normal&quot; verwenden.**LUTs** (Nachschlagetabellen) sind Farbprofil-Texturen, die in den Anzeigeeinstellungen verwendet werden können, um ein Farbprofil-Verhalten im Viewport zu simulieren. Weitere Informationen zu Farbprofilen [&#x200B; finden Sie hier:](../../features/post-processing/color-profile.md). |
| Umgebungs-Map <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r8-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/00-05-assettypes-1.jpg"/></div> | Bilder enthalten, die als *Umgebung* (meistens .hdr oder .exr) importiert wurden. Umgebungs-Map sind Hintergrundbilder, die automatisch eine Beleuchtungseinrichtung generieren. Sie können eine Umgebungs-Map verwenden, indem Sie sie direkt in den Viewport ziehen oder die Anzeigeeinstellungen durchsuchen. |
