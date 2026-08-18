---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/painting/advanced-channel-painting/flow-map-painting.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie in Substance 3D Painter Flussdiagramme zeichnen, um die Materialflussrichtung und anisotrope Effekte zu steuern.
helpx_creative_field: ""
helpx_description: Painter > Painting > Advanced channel painting > Flow Map Painting
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Flow Map Painting
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 0%

---


# Flow Map Painting

Ein eigener Kanal ist geplant, aber in der Zwischenzeit ist es möglich, mithilfe des Kanals &quot;Normal&quot; und einiger Pinselparameter Flussdiagramme in Substance 3D Painter zu malen.

## Schritt 1: Normale Map erstellen

Erstelle eine normale Map-Textur mit 16 x 16 Pixeln. Die Farbe muss 128, 255, 128 sein, was die folgende Farbe ergeben sollte: ![](../../assets/up-dx.png)\
(Diese Farbe entspricht einer in DirectX nach oben schauenden Vektorgrafik)

## Schritt 2: Hinzufügen eines normalen Kanals

Fügen Sie in Ihrem Substance 3D Painter-Projekt einen **Normal**-Kanal über die **Textursatzeinstellungen** hinzu, wenn dieser Kanal noch nicht vorhanden ist.

## Schritt 3: Pinseleinstellungen

Aktivieren Sie die Funktion &quot;Pfad folgen&quot; in den Pinselparametern. Laden Sie die normale Kartenstruktur (Schritt 1) in den normalen Kanalsteckplatz. Deaktivieren Sie die anderen Kanäle.

![](../../assets/brush-settings-1.png){width="300px"}

## Schritt 4: Malen!

Wenn Sie mit aktivierter Einstellung &quot;Pfad folgen&quot; auf das Gitter malen, zeichnen die Pinselstriche die Richtungen in die normale Karte.

![](../../assets/painting-1.png){width="700px"}
