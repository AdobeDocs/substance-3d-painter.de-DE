---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/color-management.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie das Farbmanagement in Substance 3D Painter konfigurieren, um über Ihren Workflow hinweg eine konsistente Farbgenauigkeit zu gewährleisten.
helpx_creative_field: ""
helpx_description: Painter > Features > Color management
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Farbmanagement
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '732'
ht-degree: 4%

---


# Farbmanagement

![](../../assets/banner-cm-doc.jpg)

Farbmanagement ist die Handhabung und Konvertierung von Farben. Vom Import von Ressourcen über die Anzeige von Farben auf dem Bildschirm bis hin zum endgültigen Export von Texturen. Die Farbkalibrierung ist wichtig, um in allen Anwendungen dasselbe Aussehen zu gewährleisten.

In der Anwendung erfolgt das Farbmanagement über die Integration von [OpenColorIO](https://opencolorio.org/) (OCIO) Version 2. OCIO ist der Standard für Film- und Animationsvorlagen zum Konvertieren und Anzeigen von Farben. Um das Farb-Management zu aktivieren, erstellen Sie einfach ein neues Projekt oder öffnen Sie ein vorhandenes und aktivieren Sie die dedizierten Einstellungen.

>[!NOTE]
>
> Das Farbmanagement ist seit Version 7.4.0 verfügbar.

## Projekteinstellungen

Einstellungen für das Farbmanagement:

* [Farbmanagement mit Adobe ACE - ICC](color-management-with-adobe-ace-icc.md)
* [Farb-Management mit OpenColorIO](color-management-with-opencolorio.md)

## Vokabular

Es kann hilfreich sein, einige technische Begriffe im Zusammenhang mit dem Farbmanagement zu kennen, um den zugehörigen Arbeitsablauf besser zu verstehen:

| Stichwort | Beschreibung |
| --- | --- |
| **Farbraum** | Koordinatensystem, in dem Farben definiert sind. |
| **Arbeitsbereich** | Der Farbraum, der in der Anwendung zum Überblenden von Textur, Malen usw. verwendet wird. |
| **transformieren anzeigen** | &quot;transformieren anzeigen&quot; konvertiert die Linearfarben aus dem Arbeitsfarbraum in den Farbraum des Bildschirms, um Farben wahrnehmbar anzuzeigen (für das menschliche Auge sichtbar). Die transformieren Optionen enthalten häufig einen Tonzuordnungspass zum Komprimieren von Farben, damit diese an den begrenzten Wertebereich angepasst werden, der von einem Bildschirm zugelassen ist. |
| **Konfiguration** | Eine OCIO Konfigurationsdatei. Er definiert den Arbeitsfarbraum, eine Liste der Farbräume und eine Liste der transformieren Anzeigen. |
| **ACE** | ACE steht für Academy Color Encoding System und ist in vielen Anwendungen der Standard für den Austausch digitaler Bilddateien. Zwei Versionen dieses Standards sind standardmäßig in der Anwendung enthalten. |
| **Tonzuordnung** | Hierbei handelt es sich um den Prozess der Zuordnung von Farbwerten von HDR. (High Dynamic Range) zu LDR (niedriger Dynamikbereich). Dieser Vorgang hilft bei der Anzeige einer ungefähren Anzeige einer Vielzahl von Farben. |

## Liste der farbverwalteten Kanäle

Innerhalb der Anwendung ist vordefiniert, welche Kanäle farbverwaltet sind (Daten/Passthrough) oder nicht.

| Kanal | Ist farbverwaltet |
| --- | --- |
| **Ambient occlusion** | Nein |
| **Anistotropiewinkel** | Nein |
| **Anisotropy level** | Nein |
| **Grundfarbe** | **Ja** |
| **Blending mask** | Nein |
| **Mantelfarbe** | **Ja** |
| **Coat normal** | Nein |
| **Coat opacity** | Nein |
| **Coat roughness** | Nein |
| **Coat specular level** | Nein |
| **Diffus** | **Ja** |
| **Versatz** | Nein |
| **Glossarität** | Nein |
| **Height** | Nein |
| **Ior** | Nein |
| **Metallisch** | Nein |
| **Normal** | Nein |
| **Deckkraft** | Nein |
| **Spiegelung** | Nein |
| **Raueit** | Nein |
| **Streuung** | Nein |
| **Streufarbe** | **Ja** |
| **Glanzfarbe** | **Ja** |
| **Deckkraft des Glanzes** | Nein |
| **Glanz Rauheit** | Nein |
| **Specular** | **Ja** |
| **Specular edge color** | **Ja** |
| **Specular level** | Nein |
| **Translucency** | Nein |
| **Transmissive** | **Ja** |
| **UserX (0-15)** | Abhängig von [Textursatzeinstellungen](../../interface/texture-set/texture-set-settings.md). Standardmäßig werden Benutzerkanäle nicht farbverwaltet. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r31-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/user-demo.png"/></div> |

## Farbwähler

Wenn das Farbmanagement aktiviert ist, ändert sich das Verhalten der [Farbauswahl](../../interface/color-picker.md) leicht:

* Die Farben werden auf der Grundlage der aktuell ausgewählten Anzeige bearbeitet.
* Der Benutzeroberfläche werden einige zusätzliche Informationen hinzugefügt.

Weitere Informationen finden Sie auf der Dokumentationsseite &quot;](../../interface/color-picker.md)&quot; des Farbwählers &quot;[&quot;.

## Viewport-Steuerelemente

Sowohl die 2D- als auch die 3D-Ansicht sind farbverwaltet und verfügen über spezielle Einstellungen oben im Viewport, mit denen Sie steuern können, welche Anzeige transformieren werden soll:

![](../../assets/viewport-cm.png)

* **Linke Schaltfläche**: Aktivieren/Deaktivieren des transformieren Viewports. Wenn diese Option deaktiviert ist, zeigt der Viewport die Farben als RAW/Passthrough an. Diese Schaltfläche ist standardmäßig aktiviert.
* **Dropdown rechts**: Geben Sie an, welcher Anzeigefarb zum Konvertieren der auf dem Bildschirm transformieren Farben verwendet werden soll. Der Standardwert basiert auf der OCIO. Diese Einstellung wird nicht zusammen mit dem Projekt gespeichert, da sie monitorabhängig sein kann.

>[!NOTE]
>
> Im Solomodus (Kanäle einzeln anzeigen) wird das Farbmanagement beim Anzeigen von Datenkanälen automatisch deaktiviert (siehe obige Liste).

## Exporteinstellungen

Die Hauptexporteinstellungen werden von der Projektkonfiguration gesteuert (siehe oben).

Im Fenster &quot;[Texturen exportieren](../../export/export.md)&quot; befindet sich ein Stichwort, mit dem der pro Textur verwendete Farbraum an die Dateinamen angehängt werden kann: **$colorSpace**.

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../assets/export-list-1.png){width="320px"}

</td>
<td style="border: 0;" valign="top">

![](../../assets/export-list-2.png){width="500px"}

</td>
</tr>
</table>

## Außerkraftsetzen von Farbräumen

Möglicherweise müssen Sie einen alternativen Farbraum angeben, damit eine Ressource von den Standardfarbräumen abweicht. Dies kann über das Farbraummenü erfolgen.

### Farbraum einer Ressource ändern

Innerhalb des [Eigenschaftsfensters](../../interface/properties.md) kann der Farbraum einer bestimmten Ressource (in der sie derzeit verwendet wird) überschrieben werden.

Erweitern Sie dazu den Abschnitt &quot;Farbraum&quot; und legen Sie mithilfe der Dropdown-Liste den neuen Farbraum fest:

![](../../assets/color-space-menu.png)

### Ändern des Farbraums der Umgebungs-Map

Aktivieren Sie in den [Anzeigeeinstellungen](../../interface/display-settings/display-settings.md) den **Umgebungs-Map-Farbraum überschreiben**, und wählen Sie dann einen Farbraum in der Liste aus, der Ihrer Ressource entspricht.

![](../../assets/color-sace-menu-env.png)
