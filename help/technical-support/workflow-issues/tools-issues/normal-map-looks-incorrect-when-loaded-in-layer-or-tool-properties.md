---
breadcrumb-title: ""
description: Erfahren Sie, wie Sie Probleme mit der Normalen-Map-Anzeige in den Ebenen- und Werkzeugeigenschaften von Substance 3D Painter beheben, um präzise Oberflächendetails zu erhalten.
title: Normalen-Map sieht beim Laden in Ebenen- oder Werkzeugeigenschaften falsch aus
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '105'
ht-degree: 0%
---

# Normalen-Map sieht beim Laden in Ebenen- oder Werkzeugeigenschaften falsch aus

Wenn Sie eine Normalität in das aktuelle Tool von Füllebene laden, kann diese fehlerhaft erscheinen, wenn es sich um eine OpenGL-Normalen-Map handelt.\
Der Grund ist ganz einfach: Das Engine von Substance 3D Painter nimmt an, dass geladene Normalen-Map standardmäßig DirectX sind.

Dieses Material lässt sich einfach bearbeiten, indem man auf den kleinen Pfeil neben dem Substance-Kanal oder dem dedizierten Kanal klickt:

![](../../../assets/channel-format-override.png)
