---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/features/effects/compare-mask.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie den Effekt "Maske vergleichen" in Substance 3D Painter verwenden, um Masken auf der Grundlage von Texturvergleichen zu erstellen.
helpx_creative_field: ""
helpx_description: Painter > Features > Effects > Compare Mask
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Vergleichsmaske
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 1%

---


# Vergleichsmaske

![](../../assets/compare-mask.png)

Mit diesem Effekt können Sie schnell und einfach zwei Kanäle vergleichen und eine Maske erstellen. Dieser Effekt ist nur für die Ebenenmaske verfügbar.

Im Folgenden sind die verfügbaren Einstellungen für diesen Effekt aufgeführt:

| Einstellung | Beschreibung |
| --- | --- |
| **Kanal** | Der Kanal, der zwischen Quelle und Ziel verglichen werden soll, aus dem eine Maske erstellt werden soll. Diese Liste basiert auf dem Kanal, der in den [Einstellungen für den Textursatz](../../interface/texture-set/texture-set-settings.md) verfügbar ist. |
| **Vergleichen** | Hier stehen drei Parameter zur Auswahl, wie die Maske berechnet werden soll. Die Dropdown-Liste in der Mitte definiert den Vergleichsvorgang (kleiner als, innerhalb der Toleranz, größer als). <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/compare-mode.png"/></div> Quell- und Zielmodus sind :<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Ebenen darunter</strong> : Berücksichtigen Sie die reduzierte Version aller Ebenen unter der aktuellen.</li><li data-preserve-html="true"><strong>Diese Ebene</strong> : Berücksichtigen Sie nur diese Ebene.</li><li data-preserve-html="true"><strong>Diese Maske</strong> : Berücksichtigen Sie den vorhandenen Inhalt der Maske (z. B. wenn bereits ein Effekt &quot;Füllen&quot; oder ein Effekt &quot;Generator&quot; vorhanden ist).</li><li data-preserve-html="true"><strong>Konstante</strong> : Einheitlicher Wert.</li></ul>Die Maßnahmen umfassen:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Kleiner als </strong> : Wenn die Quelle (linke Dropdown-Liste) niedrigere Werte als das Ziel (rechte Dropdown-Liste) hat, werden weiße Werte in der Maske ausgegeben.</li><li data-preserve-html="true"><strong>Innerhalb der Toleranz</strong> : Wenn die Quelle (linke Dropdown-Liste) ähnliche Werte wie das Ziel (rechte Dropdown-Liste) hat, werden Weißwerte in der Maske ausgegeben.</li><li data-preserve-html="true"><strong>Größer als </strong> : Wenn die Quelle (linke Dropdown-Liste) höhere Werte als das Ziel (rechte Dropdown-Liste) hat, werden Weißwerte in der Maske ausgegeben.</li></ul> |
| **Konstante** | Wert, mit dem verglichen werden soll, wenn die Vergleichseinstellung auf &quot;konstant&quot; festgelegt ist. |
| **Härte** | Steuert die Smoothness/Härte des resultierenden Maskenvergleichs. |
| **Histogramm der Quellkanäle** | Bereitstellen einer Histogrammansicht der Quelle und des Ziels. Nützlich, um zu wissen, ob sie sich ein bisschen oder überhaupt nicht überlappen (wenn sie sich nicht überlappen, ist die Maske leer).Weitere Informationen über die Funktionsweise des Histogramms finden Sie unter : [Stufen](https://experienceleague.adobe.com/en/docs/substance-3d-designer/using/substance-graphs/nodes-reference-for-substance-graphs/atomic-nodes/levels). |

>[!NOTE]
>
> Es ist möglich, mit der rechten Maustaste auf eine Ebene zu klicken und den Tastaturbefehl &quot;**Height mit Maskenkombination hinzufügen**&quot; auszuwählen, um diesen neuen Effekt schnell auf einer Ebene hinzuzufügen. Mit diesem Tastaturbefehl wird auch der Mischmodus &quot;**&quot; für den Height-Kanal &quot;**&quot; auf &quot;**Normal**&quot; umgeschaltet, anstelle des Standardmodus &quot;**Linear Abwedeln (Hinzufügen)**&quot;.\
> ![](../../assets/compare-shortcut.png)
