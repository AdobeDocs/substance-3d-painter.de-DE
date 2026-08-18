---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/effects/anchor-point.html"
breadcrumb-title: ''
description: Lerne, wie du in Substance 3D Painter für komplexere Kompositionen Ankerpunkte verwenden kannst, um Strukturen aus anderen Ebenen zu referenzieren.
helpx_creative_field: ""
helpx_description: Painter > Features > Effects > Anchor Point
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Ankerpunkt
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '303'
ht-degree: 0%

---


# Ankerpunkt

Ein Ankerpunkt ist eine Möglichkeit, eine beliebige Ressource oder ein Element im Ebenenstapel anzuzeigen und in verschiedenen Bereichen des Ebenenstapels zu referenzieren, und zwar für unterschiedliche Zwecke und mit unterschiedlichen Korrekturen. Mit ihnen eröffnen sich völlig neue Möglichkeiten. Ebenen und Masken können miteinander verknüpft werden. Ein einziger Ankerpunkt wirkt sich auf mehrere Aspekte deines Projekts aus und verwandelt Substance 3D Painter in ein wirklich nichtlineares Erlebnis.

>[!NOTE]
>
> Ein Ankerpunkt kann nur innerhalb der gleichen Struktur referenziert werden, die erstellt wurde. Das Erstellen von Verknüpfungen zwischen einem Anker und seinen Referenzen ist in Textursätzen nicht möglich.

## Ankerpunkt hinzufügen

Ankerpunkte sind im Menü &quot;Effekte&quot; verfügbar. Sie können sowohl auf Ebenen als auch auf Masken hinzugefügt werden.

![](../../assets/add-anchor-point.png)

## Ankerpunkt als Referenz verwenden.

Ein Ankerpunkt kann von einer anderen Ebene referenziert werden: Dadurch wird der Inhalt des Ankerpunkts in die Ebene instanziiert, die ihn referenziert.

Ankerpunkte können in den folgenden Ressourcen als Referenz verwendet werden:

* Füllebene
* Fülleffekt
* Eingabe eines Substance-Filters (Effekt, Procedural, Generator)

![](../../assets/anchor-point-resource.png)

Nur Ankerpunkte, die **unterhalb von** der Ebene liegen, auf die verwiesen wird, können als Verweise verwendet werden.\
Wenn Sie einen Ankerpunkt über eine Ebene bewegen, die darauf verweist, wird der Verweis beschädigt. Sie können diese Aktion rückgängig machen, wenn Sie sie abbrechen möchten.

![](../../assets/layer-broken.png)![](../../assets/reference-broken.png)

## Suchen nach Referenzen für einen Ankerpunkt

Wenn Sie auf einen Ankerpunkt klicken, können Sie in den Eigenschaften die Liste der Ebenen sehen, auf denen dieser Ankerpunkt als Referenz dient.

![](../../assets/references.png)

## Ankerpunkt suchen

Wenn Sie eine Füllebene/ein Effekt sind, der einen Ankerpunkt als Referenz verwendet, können Sie zum Ankerpunkt springen.

![](../../assets/jump-to-anchor-point.png)
