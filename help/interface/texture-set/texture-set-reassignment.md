---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/interface/texture-set/texture-set-reassignment.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie in Substance 3D Painter Texturensätze neu zuweisen, um Maschenzuweisungen und Texturzuordnung neu zu organisieren.
helpx_creative_field: ""
helpx_description: Painter > Interface > Texture Set > Texture Set reassignment
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Struktur Neuzuweisung festlegen
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 0%

---


# Struktur Neuzuweisung festlegen

![](../../assets/txtset-reassignment-window.png)

Im Fenster &quot;Neuzuweisung des Textursatzes&quot; können Sie die Zuweisung des Ebenenstapels zu einem anderen Teil des Szenengitters ändern. Dies ist beispielsweise nützlich, wenn Sie ein neues Gitter in ein vorhandenes Projekt importieren, in dem einige Textursätze deaktiviert sind. Dies liegt daran, dass der Ebenenstapel einem Material zugewiesen wurde, das nicht mehr existiert. Mit dem Resignment-Fenster ist es möglich, diesen Ebenenstapel wiederherzustellen (siehe &quot;Restoring Disabled Texture Sets&quot; weiter unten).

Um auf das Fenster für die Neuzuweisung von Textursätzen zuzugreifen, öffnen Sie das Fenster [Textursatz-Liste](texture-set-list.md) und wählen Sie **Einstellungen > Textursätze neu zuweisen**.

Das Fenster ist in drei Bereiche unterteilt:

* **Textursätze deaktiviert** : Listet alle derzeit nicht verwendeten Textursätze auf.
* **Project Texture Sets** : Listet alle Textursätze auf, die derzeit einem Gittermaterial zugewiesen sind.
* **Gittermaterialien** : Listet die Gittermaterialien des Projekts auf.

Das Fenster verfügt außerdem über eine zusätzliche Schaltfläche, mit der die folgenden Aktionen ausgeführt werden:

* **Rückgängig** : Zum vorherigen Status des Fensters zurückkehren
* **Wiederholen** : Wenden Sie die rückgängig gemachte Änderung erneut an.
* **Anwenden** : Schließen Sie das Fenster und führen Sie die Neuzuweisung(en) durch.
* **Abbrechen** : Schließen Sie das Fenster und verwerfen Sie alle Änderungen, die gerade vorgenommen wurden.

## Neuzuweisen von Textursätzen

![](../../assets/reassign-existing-sets.gif)

Das Neuzuweisen von Textursätzen kann durch einfaches Ziehen und Ablegen der Schaltflächen erfolgen.

## Wiederherstellen deaktivierter Textursätze

![](../../assets/reassign-disabled-sets.gif)

Ein Textursatz kann deaktiviert werden, wenn er nicht mehr mit einem Gittermaterial verknüpft ist.\
Dies kann beim Importieren eines neuen Gitters in ein Projekt auftreten, in dem die Materialnamen zwischen dem Projekt und dem neuen Gitter unterschiedlich sind.

Um einen Textursatz wiederherzustellen, **vertauschen** Sie einfach seine Position mit einem Textursatz in der Liste &quot;**Project Texture Sets**&quot;.

## Deaktivierte Textursätze löschen

![](../../assets/reassign-delete-sets.gif)

Wenn Sie auf das **Kreuz** neben einem Textursatz in der Liste **Deaktivierte Textursätze** klicken, wird dieser zum Löschen **markiert**.\
Der Löschvorgang erfolgt, wenn Sie auf die Schaltfläche **Anwenden** am unteren Rand des Fensters klicken.

>[!WARNING]
>
> Diese Aktion kann nicht rückgängig gemacht werden, wenn das Fenster mit der Schaltfläche &quot;Anwenden&quot; geschlossen wurde.
