---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/smart-materials-and-masks.html"
breadcrumb-title: ''
description: Lerne, wie du in Substance 3D Painter mit Smart-Materialien und -Masken prozedurale Strukturen erstellst, die sich an die Geometrie anpassen.
helpx_creative_field: ""
helpx_description: Painter > Features > Smart Materials and Masks
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Smart-Materialien und -Masken
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 0%

---


# Smart-Materialien und -Masken

Substance 3D Painter unterstützt die Verwendung erweiterter **Ebenenvorgaben** . Diese Vorgaben können verwendet werden, um schnell **Textursätze oder Projekte mit**&#x200B;ähnlichem Texturierungsprozess **für** freizugeben, während die Ergebnisse unterschiedlich sind, **angepasst an die Gittertopologie** .

>[!NOTE]
>
> Beachten Sie, dass nach dem Hinzufügen zum Ebenenstapel nicht mehr ermittelt werden kann, welches Smart-Material verwendet wurde. Wenn ein Smart-Material aktualisiert werden muss, muss der Prozess manuell durchgeführt werden.\
> Einzelne Ressourcen können jedoch mit [Resources Updater](plugins/resources-updater.md) aktualisiert werden.

## Wie werden Smart-Materialien/-Masken verwendet?

Smart-Materialien können überall im Ebenenstapel verwendet werden, während Smart-Masken nur im Effektstapel verwendet werden können.\
Weitere Informationen zu den Unterschieden finden Sie unter : [Ebenenstapel](../interface/layer-stack/layer-stack.md) und [Effekte](effects/effects.md)

### Hinzufügen eines Smart-Materials

Smart-Materialien können auf zwei verschiedene Arten hinzugefügt werden:

* Durch Ziehen und Ablegen intelligenter Materialien von der Ablage in den Ebenenstapel :\
  ![](../assets/sm-drop.gif)
* Durch Klicken auf die Schaltfläche Smart Material, um ein Mini-Regal zu öffnen:\
  ![](../assets/sm-button.gif)

### Hinzufügen einer Smart-Maske

Da Smart-Masken Vorgaben für Effekte sind, können sie nur (speziell für Masken) zu Effektstapeln hinzugefügt werden.

* Um eine Smart-Maske hinzuzufügen, ziehen Sie einfach **eine Maske aus dem Shelf auf die Ebene** target **und legen Sie sie dort ab:**\
  ![](../assets/smm-drop.gif)
* Durch Ziehen und Ablegen von **mehreren** intelligenten Masken werden diese akkumuliert:\
  ![](../assets/smm-drop-accum.gif)
* Es ist jedoch möglich, **den gesamten Effektstapel zu ersetzen**, indem Sie **STRG** während des Drag &amp; Drop drücken:\
  ![](../assets/smm-drop-replace.gif)

### Wie erstelle ich Smart-Materialien/Masken?

Zum Erstellen eines Smart Materials ist ein **Ordner** erforderlich.\
Der Inhalt der Smart-Materialien wird in dem Ordner enthalten sein. Klicken Sie dann einfach mit der rechten Maustaste auf den Ordner und wählen Sie &quot;**Smart-Material erstellen** &quot; aus. Das Smart-Material wird dann dem aktuellen Regal hinzugefügt und entsprechend dem ausgewählten Ordner benannt.

![](../assets/create-sm.png)

Klicken Sie zum Erstellen einer Smartmaske einfach mit der rechten Maustaste auf eine Ebene und wählen Sie &quot;**Smartmaske erstellen**&quot; aus.

![](../assets/create-smm.png)

## Wie kann ich ein Smart-Material/eine Smart-Maske freigeben/abrufen?

Die Vorgaben werden **auf dem Datenträger &quot;**&quot; gespeichert und können aus dem entsprechenden Ordner abgerufen werden.\
Informationen zum Speicherort der **Ablage** finden Sie unter : [Hinzufügen von Inhalten auf der Festplatte](../content/importing-assets/adding-content-on-the-hard-drive.md) .

Dann kann jeder die Datei einfach **importieren** in sein Substance 3D Painter-Regal, um die Vorgabe zu verwenden.
