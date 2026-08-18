---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/interface/texture-set/texture-set-list.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie die Textursatzliste in Substance 3D Painter verwenden, um mehrere Textursätze in Ihrem Projekt zu verwalten und zu organisieren.
helpx_creative_field: ""
helpx_description: Painter > Interface > Texture Set > Texture Set list
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Textursatzliste
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '609'
ht-degree: 0%

---


# Textursatzliste

![](../../assets/texture-set-list.png)

Im Fenster **Textursatzliste** werden alle Material-IDs des aktuellen 3D-Modells in einem Projekt angezeigt. So können Sie zwischen den Ebenen wechseln, die den einzelnen Materialien auf dem Modell zugeordnet sind, und deren Einstellungen sehen.

Das Hauptziel des Fensters &quot;Texturensatz-Liste&quot; besteht darin, den Wechsel von einem Material zum anderen zu ermöglichen, um auf den Ebenenstapel zuzugreifen, der jedem Material zugeordnet ist.\
Im Fall des Arbeitsablaufs [Materialschichtung](../../features/dynamic-material-layering.md) werden die **Unterstapel** **unter dem Namen des Textursatzes** angezeigt.

>[!WARNING]
>
> Es kann jeweils nur ein Textursatz bearbeitet/gemalt werden.

## Textursatzstatus

Textursätze können mehrere Zustände haben:

![](../../assets/txtset-status.png)

* **Ausgewählt** : Der aktuell bearbeitete Textursatz. Wenn Sie einen Textursatz auswählen, werden der [Ebenenstapel](../layer-stack/layer-stack.md) und das Fenster [Shader-Einstellungen](../shader-settings/shader-settings.md) entsprechend aktualisiert.
* **Sichtbar/Ausgeblendet** : Weitere Informationen finden Sie im Abschnitt zur Sichtbarkeit weiter unten.
* **Deaktiviert** : Das bedeutet, dass die Textursätze und der zugehörige Ebenenstapel nicht mit einem Material im Gitter verbunden werden können. Weitere Informationen finden Sie unter [Neuzuweisung von Textursätzen](texture-set-reassignment.md).

## Sichtbarkeit

![](../../assets/texturesetlist.png)

Die Anzeige eines Textursatzes kann über die dedizierten Symbole verwaltet werden:

| *Symbol* | *Aktion* | *Beschreibung* |
| --- | --- | --- |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/txtsetlist-icon-menu.png"/></div> | Menü öffnen | Öffnen Sie ein neues Menü mit den folgenden Aktionen:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Alle anzeigen</strong>: Zeigt alle Textursätze im Viewport an.</li><li data-preserve-html="true"><strong>Alle ausblenden</strong>: Blendet alle Struktursammlungen im Viewport aus.</li><li data-preserve-html="true"><strong>Einblenden/Ausblenden umkehren</strong>: Sichtbare Textursätze werden ausgeblendet, ausgeblendete Textursätze werden sichtbar.</li></ul> |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/txtsetlist-icon-isolate.png"/></div> | Fokussiermodus | Isolieren Sie den aktuell aktiven Textursatz und blenden Sie alle anderen aus, während dieser Modus aktiv ist. Klicken Sie erneut auf diese Schaltfläche, um den Modus zu beenden. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r3-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/txtsetlist-icon-visible.png"/></div> | Sichtbarkeit | Klicken Sie auf diese Schaltfläche neben einem Textursatz, um einen Textursatz im Ansichtsfenster auszublenden oder sichtbar zu machen. |

>[!NOTE]
>
> Beim **Malen** wird standardmäßig nur der ausgewählte Textursatz angezeigt. Sie können dieses Verhalten in den [Voreinstellungen](../settings/settings.md) ändern, indem Sie das Kontrollkästchen &quot;**Nur beim Malen ausgewähltes Material anzeigen**&quot; deaktivieren.\
> Hinweis : Das Ausblenden anderer Textursätze beim Malen von **verbessert die Leistung**.

## Kontextmenü

![](../../assets/txtset-list-contextualmenu.png)

Wenn Sie mit der rechten Maustaste auf einen Textursatz-Namen klicken, wird ein Kontextmenü mit den folgenden Aktionen geöffnet:

* **Textursatz anzeigen/ausblenden** : die Sichtbarkeit des Textursatzes ein-/ausschalten (wie im vorherigen Abschnitt beschrieben)
* **Name bearbeiten** : &quot; können Sie einen Textursatz umbenennen. Dieser Name wird auch während des Exportvorgangs für die Texturen verwendet. Umbenennen ist auch möglich, indem Sie auf den Namen des Textursatzes doppelklicken.
* **Setzen Sie den Namen auf \*ursprünglichen Namen\*** zurück: Stellt den ursprünglichen Textursatz-Namen aus dem Gittermaterial wieder her, wenn er geändert wurde.
* **Beschreibung bearbeiten** : ermöglicht das Hinzufügen/Ändern der einem Textursatz zugeordneten Beschreibung.

## Shader Management

Mit der Schaltfläche rechts neben jedem Textursatz-Namen kann die Shader-Zuweisung verwaltet werden.\
Standardmäßig hat jeder Textursatz dieselbe Shader-Instanz. Manchmal kann es jedoch zweckmäßig sein, einen anderen Shader nur für einen bestimmten Teil des Gitters zu verwenden. Klicken Sie dazu auf die Schaltfläche und wählen Sie &quot;**Neue Shader-Instanz**&quot; aus. Von dort aus können Sie im Fenster &quot;[Shader settings](../shader-settings/shader-settings.md)&quot; den Shader und seine Parameter ändern, ohne andere Textursätze zu beeinflussen.

![](../../assets/capture-d-e-cran-2018-07-12-a-15-45-32.png){width="500px"}

## Einstellungen

Über die Schaltfläche Einstellungen wird ein neues Menü geöffnet, in dem mehrere Aktionen angezeigt werden:

* **Leere Beschreibungen ausblenden** (Standard) : Ausblenden der Beschreibungsfelder, wenn diese leer sind
* **Alle Beschreibungen ausblenden** : Die Beschreibungsfelder ausblenden, auch wenn sie nicht leer sind
* **Alle Beschreibungen anzeigen** : Beschreibungsfelder anzeigen, auch wenn sie leer sind
* **Shader-Parameter importieren** : Importieren einer JSON-Datei zum Konfigurieren der Shader-Parameter der Textursätze zulassen
* **Textursätze erneut zuweisen** : Weitere Informationen finden Sie unter [Neuzuweisung von Textursätzen](texture-set-reassignment.md).
