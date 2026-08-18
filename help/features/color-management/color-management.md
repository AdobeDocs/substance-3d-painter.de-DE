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

Farbmanagement ist die Handhabung und Konvertierung von Farben. Vom Import von Ressourcen über die Anzeige von Farben auf dem Bildschirm bis hin zum Export von Texturen. Die Farbkalibrierung ist wichtig, um in allen Anwendungen dasselbe Aussehen zu gewährleisten.

In der Anwendung wird das Farbmanagement über die Integration von [OpenColorIO](https://opencolorio.org/) (kurz OCIO) Version 2 ausgeführt. OCIO ist der Standard für Film- und Animationsvorlagen zur Konvertierung und Anzeige von Farben. Um das Farb-Management zu aktivieren, erstellen Sie einfach ein neues Projekt oder öffnen Sie ein vorhandenes und aktivieren Sie die dedizierten Einstellungen.

>[!NOTE]
>
> Das Farbmanagement ist seit Version 7.4.0 verfügbar.

## Projekteinstellungen

Einstellungen für das Farbmanagement:

* [Farbmanagement mit Adobe ACE - ICC](color-management-with-adobe-ace-icc.md)
* [Farbmanagement mit OpenColorIO](color-management-with-opencolorio.md)

## Vokabular

Es kann hilfreich sein, einige technische Begriffe im Zusammenhang mit dem Farbmanagement zu kennen, um den zugehörigen Arbeitsablauf besser zu verstehen:

| Stichwort | Beschreibung |
| --- | --- |
| **Farbraum** | Koordinatensystem, in dem Farben definiert sind. |
| **Arbeitsbereich** | Der Farbraum, der in der Anwendung zum Mischen von Textur, Farbe usw. verwendet wird. |
| **Transformation anzeigen** | Mit &quot;Transformation anzeigen&quot; werden die linearen Farben aus dem Arbeitsfarbraum in den Farbraum des Bildschirms konvertiert, um Farben wahrnehmbar anzuzeigen (für das menschliche Auge sichtbar). Display-Transformationen beinhalten häufig einen Tonzuordnungs-Pass zur Komprimierung von Farben, um sie an den begrenzten Wertebereich anzupassen, der von einem Bildschirm zugelassen ist. |
| **Konfiguration** | Eine OCIO-Konfigurationsdatei Er definiert den Arbeitsfarbraum, eine Liste der Farbräume und eine Liste der Anzeigetransformation. |
| **ACES** | ACES steht für Academy Color Encoding System und ist in vielen Anwendungen der Standard für den Austausch digitaler Bilddateien. Zwei Versionen dieses Standards sind standardmäßig in der Anwendung enthalten. |
| **Tonzuordnung** | Hierbei handelt es sich um den Prozess der Zuordnung von Farbwerten von HDR (High Dynamic Range) zu LDR (niedriger Dynamikbereich). Dieser Vorgang hilft bei der Anzeige einer ungefähren Anzeige einer Vielzahl von Farben. |

## Liste der farbverwalteten Kanäle

Innerhalb der Anwendung ist vordefiniert, welche Kanäle farbverwaltet sind (Daten/Passthrough) oder nicht.

| Kanal | Ist farbverwaltet |
| --- | --- |
| **Umgebungs-Verdeckung** | Nein |
| **Anistotropiewinkel** | Nein |
| **Anisotropie** | Nein |
| **Grundfarbe** | **Ja** |
| **Füllmaske** | Nein |
| **Mantelfarbe** | **Ja** |
| **Coat normal** | Nein |
| **Deckkraft der Beschichtung** | Nein |
| **Raueit der Beschichtung** | Nein |
| **Specular level beschichten** | Nein |
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
| **Glanzdeckkraft** | Nein |
| **Raueit des Glanzes** | Nein |
| **Specular** | **Ja** |
| **Specular edge color** | **Ja** |
| **Specular level** | Nein |
| **Lichtdurchlässigkeit** | Nein |
| **Transmissiv** | **Ja** |
| **UserX (0-15)** | Abhängig von [Textursatzeinstellungen](../../interface/texture-set/texture-set-settings.md). Standardmäßig werden Benutzerkanäle nicht farbverwaltet. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r31-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/user-demo.png"/></div> |

## Farbwähler

Wenn das Farbmanagement aktiviert ist, ändert sich das Verhalten der [Farbauswahl](../../interface/color-picker.md) leicht:

* Die Farben werden auf der Grundlage der aktuell ausgewählten Anzeige bearbeitet.
* Der Benutzeroberfläche werden einige zusätzliche Informationen hinzugefügt.

Weitere Informationen finden Sie auf der Dokumentationsseite &quot;[&#128279;](../../interface/color-picker.md)&quot; des Farbwählers &quot;&quot;.

## Viewport-Steuerelemente

Sowohl die 2D- als auch die 3D-Ansicht sind farbverwaltet und verfügen über spezielle Einstellungen oben im Viewport, mit denen Sie steuern können, welche Bildschirmtransformation verwendet werden soll:

![](../../assets/viewport-cm.png)

* **Linke Schaltfläche**: Aktivieren/Deaktivieren der Anzeigetransformation des Ansichtsfensters. Wenn diese Option deaktiviert ist, zeigt der Viewport die Farben als Raw/Passthrough an. Diese Schaltfläche ist standardmäßig aktiviert.
* **Dropdown rechts**: Legen Sie fest, welche Anzeigetransformation zum Konvertieren der Farben für die Anzeige auf dem Bildschirm verwendet werden soll. Der Standardwert basiert auf der OCIO-Konfiguration. Diese Einstellung wird nicht zusammen mit dem Projekt gespeichert, da sie monitorabhängig sein kann.

>[!NOTE]
>
> Im Solomodus (Kanäle einzeln anzeigen) wird das Farbmanagement beim Anzeigen von Datenkanälen automatisch deaktiviert (siehe obige Liste).

## Exporteinstellungen

Die Hauptexporteinstellungen werden von der Projektkonfiguration gesteuert (siehe oben).

Im Fenster &quot;[Texturen exportieren](../../export/export.md)&quot; befindet sich ein Stichwort, das verwendet werden kann, um den Farbraum, der pro Textur verwendet wird, an die Dateinamen anzuhängen: **$colorSpace**.

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

### Ändern des Farbraums der Umgebungskarte

Aktivieren Sie in den [Anzeigeeinstellungen](../../interface/display-settings/display-settings.md) den **Farbraum der Umgebungszuordnung überschreiben** und wählen Sie dann einen Farbraum in der Liste aus, der Ihrer Ressource entspricht.

![](../../assets/color-sace-menu-env.png)
