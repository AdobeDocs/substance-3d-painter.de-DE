---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/subsurface-scattering/enabling-subsurface-in-a-project.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie Volumenstreuung in Substance 3D Painter-Projekten aktivieren, um realistische transluzente Material-Effekte zu erstellen.
helpx_creative_field: ""
helpx_description: Painter > Features > Subsurface Scattering > Enabling Subsurface in a Project
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Untergeordnete Oberfläche in einem Projekt aktivieren
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 0%

---


# Untergeordnete Oberfläche in einem Projekt aktivieren

Um die Volumenstreuung in Substance 3D Painter richtig zu aktivieren, müssen zunächst einige Parameter festgelegt werden.\
Auf dieser Seite finden Sie eine Anleitung dazu, welche Parameter aktiviert werden können.

## 1 - Einstellungen für Textursatz

Fügen Sie im [Textursatz](../../interface/texture-set/texture-set.md) einen **Streuungskanal** hinzu, falls dieser noch nicht vorhanden ist:

![](../../assets/add-channel.png)

>[!NOTE]
>
> Der Streuungskanal funktioniert wie eine **Maske** über der **Oberfläche**: Wenn der Kanal schwarz ist, gibt es überhaupt keine Unterfläche, während, wenn er weiß ist, die Untergrundintensität maximal ist. Dieser Kanal ist ein Graustufenwert, der standardmäßig **schwarz** ist. Füge eine Füllebene zum Ebenenstapel hinzu, um die Standardfarbe zu ändern, oder verwende eine Malebene, um die Intensität manuell anzupassen.

## 2 - Globale Untergrundeinstellung

Aktivieren Sie die Einstellung für die Hauptanzeige in den [Anzeigeeinstellungen](../../interface/display-settings/display-settings.md) (unter den Volumenstreuungen für Post-Effects):

![](../../assets/enable-subsurface.png)

>[!NOTE]
>
> Das Aktivieren/Deaktivieren des Unteroberflächeneffekts wirkt sich auf das gesamte Projekt aus. Es kann hilfreich sein, diesen globalen Parameter zu verwenden, wenn er in Bezug auf die Leistung zu umfangreich ist.

## 3 - Shader-Einstellungen

![](../../assets/shader-parameters.png)

Im Fenster &quot;[Shader-Einstellungen](../../interface/shader-settings/shader-settings.md)&quot; mit Standardshadern befindet sich eine Gruppe &quot;**SSS-Parameter**&quot; mit zwei Einstellungen.\
Ändern Sie den Maßstab und die Farbe, um sie an das Zielmaterial anzupassen. Weitere Informationen zu diesen Einstellungen finden Sie unter: [Unteroberflächenparameter](subsurface-parameters.md)

## Bonus: Aktivieren von Schatten

Der Effekt &quot;Volumenstreuung&quot; funktioniert einwandfrei, kann aber seltsam aussehen, wenn er alleine bleibt.\
Aktiviere das Kontrollkästchen &quot;Tiefen&quot;, um den Viewport realistischer wirken zu lassen und das fertige Material realistischer wirken zu lassen.

Aktivieren Sie im Fenster &quot;[Umgebungseinstellungen](../../interface/display-settings/environment-settings.md)&quot; die Einstellung &quot;**Schatten**&quot;:

![](../../assets/shadow-2.png)
