---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/interface/texture-set/texture-set-settings.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie die Kanaleinstellungen in Substance 3D Painter konfigurieren, um die Auflösung der Textur und die Kanaleigenschaften zu steuern.
helpx_creative_field: ""
helpx_description: Painter > Interface > Texture Set > Texture Set settings
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Einstellungen für "Textursatz"
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '1146'
ht-degree: 0%

---


# Einstellungen für &quot;Textursatz&quot;

![](../../assets/texture-set-settings.png){width="300px"}

Die **Parametereinstellungen** steuern die Textursatz des aktuell ausgewählten Textursatzes. Hier können die Auflösung, die Kanäle und die zugehörigen Mesh-Map verwaltet werden.

## Allgemeine Eigenschaften

![](../../assets/txtset-general-properties.png)

| Einstellung | Beschreibung |
| --- | --- |
| **Name** | Name des Textursatzes. Geerbt für den Modellnamen, der dem 3D-Material zugewiesen ist. |
| **Beschreibung** | Textfeld zum Hinzufügen von Informationen über einen Textursatz. Dieser Textursatz wird in den Fenstern [Textliste](texture-set-list.md) und [Baking](../../baking/baking.md) angezeigt. |
| **Größe** | Steuert die Kanalauflösung in Pixel innerhalb eines Textursatzes. Um **nicht quadratische** Auflösungen (z. B. 2048x1024) zu verwenden, deaktivieren Sie die **Sperrschaltfläche** zwischen den beiden Dropdown-Listen.Textursatz-Auflösungen sind **dynamisch** aufgrund des **nicht-destruktiven Workflows**. Dies bedeutet, dass es möglich ist, mit einer niedrigen Auflösung zu arbeiten, um gute Leistungen zu erhalten, und dann später mit einer höheren Auflösung eine bessere Qualität zu erzielen. Innerhalb der Anwendung beträgt die maximale Auflösung eines Kanals 4096x4096 Pixel, während beim Exportieren das Maximum stattdessen 8192x8192 beträgt (sofern von der GPU unterstützt). Eine Änderung der Auflösung kann eine lange Berechnung des Engine auslösen. |
| **Shader-Instanz** | Definieren Sie, welcher [Shader](../shader-settings/shader-settings.md) zum Rendern des angegebenen Textursatzes im [Viewport](../viewport/viewport.md) verwendet werden soll. |

## Kanäle

### Kanalliste

![](../../assets/txtset-channels.png)

Die Liste kann jederzeit durch Hinzufügen oder Entfernen von Kanälen geändert werden (es sei denn, sie wird vom [Material-Ebenen](../../features/dynamic-material-layering.md)Workflow überschrieben).

| Schaltfläche/Symbol | Beschreibung |
| --- | --- |
| <b>Kanal hinzufügen</b>  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c0_image" src="../../assets/channel-add.png" width="40px"/></div> | Klicken Sie auf diese Schaltfläche, um einen neuen Kanal zur Liste hinzuzufügen.Das Popupmenü wird in drei Kategorien unterteilt:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Unterstützte Kanäle</strong>: Diese Kanäle können vom aktuellen Shader im Viewport genutzt werden.</li><li data-preserve-html="true"><strong>Nicht unterstützte Kanäle</strong>: Diese Kanäle werden vom aktuellen Shader im Viewport ignoriert.</li><li data-preserve-html="true"><strong>Benutzerkanäle</strong>: zusätzliche Kanäle zum Malen weiterer Informationen, in der Regel nicht von den Shadern unterstützt.</li></ul>  **Hinweis:** Die Anzahl der Kanäle ist nicht begrenzt. Allerdings können zu viele Kanäle die Leistung stark beeinträchtigen und erfordern mehr Speicher. |
| <b>Kanal entfernen</b>  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c0_image" src="../../assets/channel-remove.png" width="40px"/></div> | Entfernen Sie einen Kanal aus der Liste.  **Hinweis:** Die Malinformationen innerhalb des Projekts werden mit dem Kanal nicht gelöscht. Daher kann der Kanal später wieder hinzugefügt werden, falls er für die Wiederherstellung der Texturierung (nach einer Neuberechnung) erforderlich ist. |
| <b>Kanalname</b>  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r3-column-c0_image" src="../../assets/channel-name.png" width="100px"/></div> | Der Name eines bestimmten Kanals.Benutzerkanäle können umbenannt werden, indem Sie auf den aktuellen Namen doppelklicken: <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r3-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/user-channel-rename.gif"/></div> |
| <b>Kanaleinstellungen</b>  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r4-column-c0_image_79857878" src="../../assets/channel-settings-1.png" width="40px"/></div> | Mit dieser Schaltfläche wird das Einstellungsmenü des Kanals mit mehreren Aktionen geöffnet.Die erste Aktionsliste steuert den Speichertyp und die Genauigkeit des Kanals:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>sRGB8</strong>: RGB-Farben, gamma-korrigierte Werte, gespeichert auf 8 Bit.</li><li data-preserve-html="true"><strong>L8</strong>: Graustufenwerte, gespeichert auf 8 Bit.</li><li data-preserve-html="true"><strong>RGB </strong>: RGB-Farben, gespeichert auf 8 Bit.</li><li data-preserve-html="true"><strong>L16</strong>: Graustufenwerte, gespeichert auf 16 Bit.</li><li data-preserve-html="true"><strong>RGB16</strong>: RGB-Farben, gespeichert auf 16bit.</li><li data-preserve-html="true"><strong>L16F</strong>: Graustufenwerte - positive und negative Werte, gespeichert auf gleitenden 16-Bit-Werten.</li><li data-preserve-html="true"><strong>RGB16F</strong>: RGB-Farben - positiv und negativ, gespeichert auf 16bit schwebend.</li><li data-preserve-html="true"><strong>L32F</strong>: Graustufenwerte - positive und negative Werte, gespeichert auf gleitenden 32-Bit-Werten.</li><li data-preserve-html="true"><strong>RGB32F</strong>: RGB-Farben - positiv und negativ, gespeichert auf 32bit Floating.</li></ul>  **Hinweis:** Der Speichertyp **ist kein Farbraum-/Gammasteuerelement**. Die Daten, die zur Speicherung der Informationen eines Kanals (z. B. sRGB8 oder L32F) verwendet werden, haben keine Auswirkungen auf die Art und Weise, wie die Anwendung sie liest. Beispielsweise wird der Rauheit-Kanal weiterhin als &quot;data/raw&quot; und die Grundfarbe weiterhin als &quot;gamma-korrigiert&quot; betrachtet.  Die letzte Aktion des Menüs kann verwendet werden, um [Farbmanagement](../../features/color-management/color-management.md) auf dem Kanal zu aktivieren oder zu deaktivieren:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Farbkanal</strong>: Wenn diese Option aktiviert ist, wird der Kanal farbverwaltet. Diese Option kann nur manuell für Benutzerkanäle geändert werden.</li></ul> |
| <b>Farbmanagement</b>  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r5-column-c0_image" src="../../assets/icon-cm.png" width="40px"/></div> | Gibt an, dass der Kanal farbverwaltet ist, sofern vorhanden. Nur Benutzerkanäle können als farbverwaltet markiert werden oder nicht, das Verhalten anderer Kanäle ist festgelegt.Eine detaillierte Liste der Kanäle, die farbverwaltet werden oder nicht, finden Sie unter: [Farbmanagement](../../features/color-management/color-management.md). |

### Mischeinstellungen

![](../../assets/mixing.png)

Diese Einstellungen steuern verschiedene Verhaltensweisen bei der Kanalgenerierung, insbesondere die Kombination von Kanälen mit den Baking geführt Texturen (Mesh-Map).

| Einstellung | Beschreibung |
| --- | --- |
| **Normale Mischung** | Steuert, wie die &quot;Baking geführt Normalen-Map&quot; mit dem &quot;normalen&quot; Kanal kombiniert werden soll. Mögliche Werte sind:<ul data-preserve-html="true"><li data-preserve-html="true"><strong> Ersetzen von </strong> : Ignorieren Sie den &quot;Baking geführt Normalen-Map&quot; und verwenden Sie nur den &quot;normalen&quot; Kanal für diesen Textursatz. Kann zum Malen über eine Baking geführt Normalen-Map verwendet werden. Weitere Informationen finden Sie in der Dokumentation [Advanced channel painting](../../painting/advanced-channel-painting/normal-map-painting.md). Wenn der Normal-Kanal nicht vorhanden ist oder wenn die Normal-Kanalausgabe leer ist, wird die Baking geführt Normalen-Map weiterhin verwendet.</li><li data-preserve-html="true"><strong> Kombinieren von </strong> (Standard) : Verwenden Sie eine detailorientierte Funktion, um den &quot;Normal&quot;-Kanal und den &quot;Baking geführt Normalen-Map&quot; zu kombinieren.</li></ul>  **Hinweis:** Diese Einstellung ist möglicherweise deaktiviert, wenn der Kanal in der Kanalliste fehlt. Wenn der Kanal fehlt, wird der standardmäßige Mischwert verwendet. |
| **Height zur normalen Methode** | Steuert, welche Methode zum Konvertieren des Height-Kanals in eine Normalen-Map verwendet wird. Mögliche Werte sind:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Sharp</strong>: eine präzisere Normalen-Map zu erstellen, bei der die Gefahr besteht, dass Rauschen und Aliasing entstehen. Geeignet für sich wiederholende Muster wie Stoffe.</li><li data-preserve-html="true"><strong>Glatt (Sobel)</strong> (Standard): eine weichere Normalen-Map mit einem Sobel-Filter zu erstellen, bei der die Gefahr besteht, dass Details verloren gehen. Angepasst für die meisten Fälle.</li></ul> |
| **Mischen von Ambient occlusion** | Steuert, wie die &quot;Baking geführt ambient occlusion&quot; mit dem &quot;Ambient occlusion&quot;-Kanal kombiniert werden soll. Mögliche Werte sind:<ul data-preserve-html="true"><li data-preserve-html="true"><strong> Ersetzen von </strong> : Ignorieren Sie den &quot;Baking geführt ambient occlusion&quot; und verwenden Sie nur den &quot;Ambient occlusion&quot;-Kanal für diesen Textursatz. Kann verwendet werden, um eine gebackene Umgebungs-Verdeckung zu übermalen. Weitere Informationen finden Sie in der Dokumentation [Advanced channel painting](../../painting/advanced-channel-painting/ambient-occlusion-painting.md).  </li><li data-preserve-html="true"><strong> Multiplizieren </strong> (Standard) : Verwenden Sie einen Multiplikationsvorgang, um den Kanal &quot;Ambient occlusion&quot; und den Kanal &quot;Baking geführt ambient occlusion&quot; zu kombinieren.  </li></ul>  **Hinweis:** Diese Einstellung ist möglicherweise deaktiviert, wenn der Kanal in der Kanalliste fehlt. Wenn der Kanal fehlt, wird der standardmäßige Mischwert verwendet. |
| **UV-Auffüllung** | Steuert, wie die Auffüllung außerhalb der UV-Insel generiert wird. Mögliche Werte sind:  <ul class="steps" data-preserve-html="true"> <li class="step" data-preserve-html="true">    <strong>Nachbarraum in 3D</strong> (Standard): Sehen Sie sich die andere Seite der UV-Naht an, um die benachbarte Pixelfarbe zu finden und diese am Rand der UV-Ebene zu verwenden. Diese Einstellung empfiehlt sich beim Malen über UV mit durchgehenden Nähte. Beispiel mit normaler Auffüllung links und dem 3D-Nachbarn rechts:<br/>       <img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r4-column-c1_procedure_proc_par_proc_step_step_par_image_1671759737" src="../../assets/seam-3.png" width="450px"/>   </li> <li class="step" data-preserve-html="true">    <strong>Nachbar des 2D-Raums</strong>: Kopieren Sie den Pixel innerhalb einer UV-Insel in den Rahmen außerhalb der UV-Insel, bevor Sie die Auffüllung generieren. Diese Einstellung empfiehlt sich, wenn UV-Inseln sehr entgegengesetzte Informationen haben und sich nicht überlappen. Beispiel mit einer Kugel, in der die Bänder jeweils eine eindeutige Farbe pro UV-Insel haben, links mit der Einstellung &quot;2D-Nachbar&quot; und rechts mit der Einstellung &quot;3D-Nachbar&quot; (beachten Sie die Blutung):<br/>       <img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r4-column-c1_procedure_proc_par_proc_step1_step_par_image" src="../../assets/2d-neigbor-padding.png" width="450px"/>   </li> </ul>  **Hinweis:** Diese Auffüllungseinstellung wird pro Textursatz gespeichert und beim Exportieren und Visualisieren der Textur in den Viewport berücksichtigt.Da der 3D-Raum-Nachbar funktioniert, kann er nicht mit dem normalen Kanal verwendet werden und verwendet stattdessen die 2D-Version. |

## Mesh-Maps

![](../../assets/mesh-maps.png)

Den Mesh-Map werden Texturen Baking geführt, die spezifisch für den Mesh und den Textursatz sind, die verwendet werden, um die Qualität der Texturierung mithilfe von Filtern, Intelligenten Materialien und Intelligente Masken zu verbessern. Weitere Informationen finden Sie in der Dokumentation [Baking](../../baking/baking.md).
