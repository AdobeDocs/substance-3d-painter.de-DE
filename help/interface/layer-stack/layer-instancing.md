---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/interface/layer-stack/layer-instancing.html"
breadcrumb-title: ''
description: Erfahre, wie du in Substance 3D Painter mithilfe von Ebeneninstanzierungen Ebenen in mehreren Textursätzen effizient wiederverwenden kannst.
helpx_creative_field: ""
helpx_description: Painter > Interface > Layer stack > Layer instancing
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Ebeneninstanzierung
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '631'
ht-degree: 0%

---


# Ebeneninstanzierung

Mit **Ebeneninstanzierung** können Ebenenparameter über mehrere Ebenen und [Textursatz](../texture-set/texture-set.md) synchronisiert werden, während gleichzeitig ein Mesh-abhängiges Ergebnis generiert werden kann.

Wenn eine Ebeneninstanz erstellt wird, wird die ursprüngliche Ebene (oder Quellebene) verwendet, um Parameter über alle vorhandenen Instanzen hinweg zu replizieren. **Nur die Quellebene kann geändert werden**.

>[!WARNING]
>
> Alle Malen-Aktionen (Pinselstriche, Polygonfüllung usw.) funktioniert nur auf dem Textursatz, auf dem sich die Quellebene befindet. Andere Textursatz, die eine Instanz dieser Ebene haben, verwerfen einfach die Malen-Aktionen.

## Erstellen einer Ebeneninstanz

Erstellen einer Ebeneninstanz:

1. Vorhandene Ebene auswählen
1. Kopieren der Ebene (**STRG+C**)
1. Fügen Sie es als Instanz ein (verwenden Sie **STRG+UMSCHALT+V** oder klicken Sie mit der rechten Maustaste, um das Kontextmenü zu öffnen, und wählen Sie **Als Instanz einfügen**).

![](../../assets/paste-as-layer-instance.png)

>[!NOTE]
>
> Instanzen können aus einer beliebigen Ebene erstellt werden, einschließlich **Gruppen**. Das Instanziieren eines Ordners kann eine einfache Möglichkeit sein, mehrere Ebenen über verschiedene Textursatz hinweg zu replizieren. Durch das Hinzufügen von Ebenen innerhalb eines Instanzordners werden sie auch in vorhandene Instanzen repliziert.

Nachdem eine Instanz erstellt wurde, wird auf der Quell- und der Zielebene ein neues Symbol angezeigt. Dieses Symbol ist eine Schaltfläche, mit der Sie einfacher zwischen einer Quellebene und ihren Instanzen navigieren können, ohne manuell zwischen Textursätzen wechseln zu müssen (siehe unten).

| Name | Symbol |
| --- | --- |
| **Nicht instanzierte Ebene** | <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/non-instanced.png"/></div> |
| **Instanzquelle** | <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/instance-source.png"/></div> |
| **Instanzziel** | <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r3-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/instance-target.png"/></div> |

## Erstellen einer Instanz über mehrere Textursatz hinweg

Es ist möglich, eine Ebeneninstanz auf mehreren Textursätzen in einer Aktion zu erstellen und dabei das manuelle Kopieren/Einfügen zu vermeiden.

So erstellen Sie eine Instanz über mehrere Textursatz hinweg:

1. Vorhandene Ebene auswählen
1. Rechtsklicken auf die Ebene, um das Kontextmenü zu öffnen
1. Wählen Sie **Instanziieren zwischen Textursätzen**.
1. Überprüfen Sie im neuen Fenster, welche Textursatz eine Instanz erhalten müssen.
1. Klicken Sie auf OK , um die Instanzen zu validieren und zu erstellen.

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../assets/instance-across-texture-sets.png)

</td>
<td style="border: 0;" valign="top">

![](../../assets/instance-across-texture-sets-dialog.png)

</td>
</tr>
</table>

>[!NOTE]
>
> Der Ausrufezeichen neben einem Kanalnamen weist auf einen Textursatz **nicht übereinstimmend** hin. Das bedeutet, dass eine Instanz, die in diesem Textursatz erstellt wurde, nicht korrekt gerendert wird, da ein Kanal fehlt.

## Wechseln zwischen einer Instanz und ihrer Quelle

Da eine Instanz **nur** aktualisiert werden kann, indem **die Quelle** bearbeitet wird (aus technischen Gründen), muss die Quellebene ausgewählt werden, um ihre Eigenschaften zu bearbeiten.\
Klicken Sie hierzu auf der Ebene im Ebenenstapel auf die Schaltfläche **Instanzeigenschaften**.

![](../../assets/instance-properties-optim.gif)

Wenn auf eine Schaltfläche für Instanzeigenschaften geklickt wird, wechselt das Fenster **Eigenschaften** vom aktuellen Tool/der aktuellen Ebene zu **einer Liste**, in der eine Quellebene und ihre Instanzen angezeigt werden.\
Durch Klicken auf **ein beliebiges Element** der Liste, um automatisch **zu dieser Ebene zu springen** . Dadurch werden **die aktuell ausgewählten** Textursatz **auf der rechten Seite automatisch** geändert.

Die Verwendung der **Instanzenstruktur** ist die beste Methode, um **schnell** von einer Instanz zu ihrer Quelle zu wechseln, während gleichzeitig die **Abhängigkeiten** angezeigt werden.

## Instanzzyklen (und deren Lösung)

Zyklen sind Instanzen, die direkt oder indirekt in der Quellebene selbst verwendet werden. Die **-Zyklen können vom Substance 3D Painter-Engine nicht berechnet werden** und müssen daher **deaktiviert** sein, bis sie behoben oder entfernt wurden.

Beispiel:\
![](../../assets/instance-cycle-optim.gif)

In diesem Beispiel wird die Instanz der Quellebene in diese verschoben (da es sich um einen Ordner handelt). Die Instanz wird beschädigt, weil wir, um ihre Parameter zu generieren, die Parameter von der Quelle abfragen müssen, was von den Parametern der Instanz abhängt. Dadurch entsteht ein Zyklus, der nicht automatisch gelöst werden kann. Die Instanz wird deaktiviert.

Die einzige Möglichkeit, einen Zyklus zu beheben, besteht darin, die Instanz entweder **aus dem Ordner zu verschieben** oder sie zu **löschen**.

Ebeneninstanzen können in Quellebenen verwendet werden, sofern die Instanz selbst auf eine andere Quellebene verweist.
