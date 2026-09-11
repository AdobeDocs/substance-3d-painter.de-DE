---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/painting/tool-list/eraser.html"
breadcrumb-title: ''
description: Entferne Malen und Texturen präzise und mit dem Radiergummi-Werkzeug von Substance 3D Painter.
helpx_creative_field: ""
helpx_description: Painter > Painting > Tool list > Eraser
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Radiergummi
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '235'
ht-degree: 1%

---


# Radiergummi

Der Radiergummi ist ein Malen-Werkzeug, mit dem zuvor von anderen Tools gemalte Elemente gelöscht oder ausgeblendet werden. Dieses Werkzeug wirkt sich jeweils nur auf eine Ebene aus.

Die Radiergummi verwenden das Malen-Werkzeug, um dieselben Parameter und dieselben Verhaltensweisen zu nutzen. Weitere Informationen zum Pinsel sowie zu den Alpha- und Schablone-Steuerelementen finden Sie auf der [Malen-Werkzeugseite](paint-brush.md).

>[!NOTE]
>
> Technisch gesehen entfernt **der Radiergummi die Informationen nicht wirklich**. Die Alpha-Ebene wird einfach wieder auf Null gesetzt, wodurch die vorherigen Malinformationen gelöscht bzw. ausgeblendet werden. Dies bedeutet:
> 
> * Alle vorherigen Pinselstriche, die gemalt wurden, werden weiterhin berechnet, wenn ein Projekt erneut geöffnet wird, bevor die Pinselstriche mit dem Radiergummi angewendet werden.
> * Ein Substance-Filter kann die Malen-Informationen abrufen, wenn er die Alpha-Informationen ignoriert.
> 
> Aus diesem Grund ist es manchmal ratsam, eine Ebene **zu löschen und neu zu erstellen**, anstatt den Radiergummi zu verwenden, da dies die Leistung verbessern kann.

## Material

Beim Löschen von Informationen kann es vorkommen, dass nur bestimmte Kanäle betroffen sind.

>[!NOTE]
>
> Im Gegensatz zum Malen-Tool kann der Radiergummi nur festlegen, welche Kanäle betroffen sind. Es ist nicht möglich, eine Ressource aus dem Shelf zu laden, um jeden Kanal zu beeinflussen.

* Wenn alle Kanäle aktiviert sind, entfernt der Radiergummi Informationen aus allen Kanälen:

  ![](../../assets/eraser-all-channels-selection.png)

  ![](../../assets/erase-all-channel-optim.gif){width="325px"}
* Wenn bestimmte Kanäle ausgewählt sind, entfernt der Radiergummi nur Informationen aus diesen Kanälen:

  ![](../../assets/eraser-one-channel-selection.png)

  ![](../../assets/erase-one-channel-optim.gif){width="325px"}
