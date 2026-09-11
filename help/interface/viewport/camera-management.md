---
helpx_url: 'https://helpx.adobe.com/substance-3d-painter/interface/viewport/camera-management.html'
breadcrumb-title: ''
description: Erfahre, wie du in Substance 3D Painter Viewport die Ansicht einer Kamera verwaltest, um deine 3D-Modelle effektiv zu navigieren und mit Rahmen zu versehen.
helpx_creative_field: ''
helpx_description: Painter > Interface > Viewport > Camera management
helpx_experience_level: ''
helpx_learn_topic: ''
helpx_tags: ''
title: Kameramanagement
user-guide-description: ''
user-guide-title: ''
source-git-commit: e370ba212d3e90f71e09b75ff41be6123d37c5eb
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---


# Kameramanagement

In Maya, Max, Blender, Modo und DAE erstellte Kameras können in Substance 3D Painter importiert werden.

>[!NOTE]
>
> Orthografische Kameras und Anzeigeverhältnisse werden im ABC-Format (Alembic) nicht korrekt unterstützt.

## Kameras in Substance 3D Painter importieren

Die Kameras sollten in die Meshdatei aufgenommen werden, entweder im FBX- oder im ABC-Format (Alembic).

Der Name, die Transformationsparameter, das FOV und das Seitenverhältnis (sofern vorhanden) werden importiert.

Wählen Sie im Fenster Neues Projekt die Meshdatei aus, in der die Kameras enthalten sind, und überprüfen Sie, ob das Kontrollkästchen **Kameras importieren** aktiviert ist. Wenn Sie im **Bearbeiten > Projektkonfigurationsfenster** auf **Mesh neu importieren** umschalten, können Sie auch **Kameras importieren** aktivieren, wenn Sie sie bei der ersten Projekterstellung verpasst haben.

Klicken Sie dann auf **OK**:

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../assets/New-project-window-full.png" alt=""/></td>
    <td style="border: 0;" valign="top"><img src="../../assets/project-configuration-full.png" alt=""/></td>
  </tr>
</table>

## Kameras auswählen

Wenn Kameras in Ihr aktuelles Projekt importiert wurden, können Sie im **Dropdown** im **3D-Viewport** auswählen, welche Kamera aktiviert ist.

Standardmäßig ist die Painter-Kamera mit dem Namen &quot;Standardkamera&quot; ausgewählt und befindet sich im Perspektivmodus.

![](../../assets/camera-select.png)

Im obigen Beispiel werden 3 Kameras importiert. Wenn die Standard -Kamera einbezogen wird, werden insgesamt 4 Kameras in der Dropdown-Liste angezeigt.

## Steuern der Kameras

Wenn eine importierte Kamera ausgewählt ist, wird das Verschieben der Kamera durch Schwenken, Zoomen oder Drehen im Viewport auf die Standard-Kamera umgeschaltet. Dadurch wird verhindert, dass importierte Kameras in die Szene verschoben werden.

>[!NOTE]
>
> Wenn Sie die importierte Kameraposition ändern müssen, können Sie diese in der ausgewählten Szenenbearbeitungsanwendung aktualisieren und die Szene mit **Bearbeiten > Projektkonfiguration** erneut importieren.

Sie können die Parameter der importierten Kameras im **Einstellungsfenster anzeigen** steuern.

![](../../assets/display-settings-cameras.png)

Wählen Sie im Dropdown-Menü **Vorgabe** die zu ändernde Kamera aus.

Wenn eines der Attribute geändert wird, können Sie mit der Schaltfläche **Wiederherstellen** die ursprünglichen Werte wiederherstellen.

![](../../assets/camera-restore.png)

Wenn ein Parameter für eine importierte Kamera geändert wurde, wird der Name der Kamera kursiv dargestellt und ein &quot;\*&quot; wird dem Namen der Kamera hinzugefügt.

### Attribute der Kamera

Das Sichtfeld oder das FOV wird in Grad angegeben.

Die Brennweite wird in mm angegeben.

Im Viewport-Modus (OpenGL) sind Fokusabstand und Blende deaktiviert. Um sie zu aktivieren, müssen Post Effects und DOF aktiviert sein.

### Anzeigeverhältnis

Wenn das Anzeigeverhältnis in der Meshdatei vorhanden ist, wird es im Abschnitt &quot;Kamera&quot; angezeigt. Wenn eine Kamera kein definiertes Anzeigeverhältnis hat, wird sie als **Nicht angegeben** aufgeführt (wie die standardmäßige Kamera).

### Sperren

Eine Kamera kann durch Klicken auf das Schlosssymbol gesperrt werden. Das Sperren einer Kamera verhindert Änderungen an den Parametern der Kamera.

![](../../assets/image2018-7-26-15-47-6.png)

## Kamerarahmen

Der Kamera-Rahmen kann in **Anzeigeeinstellungen > Viewport-Einstellungen** umgeschaltet werden:

![](../../assets/image2018-7-26-15-54-58.png)

Sie können die Deckkraft des Bereichs außerhalb des Rahmens auch mit der **Gate-Maskendeckkraft** anpassen.

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../assets/image2018-7-26-15-58-45.png" alt=""/></td>
    <td style="border: 0;" valign="top"><img src="../../assets/image2018-7-26-15-58-53.png" alt=""/></td>
  </tr>
</table>
