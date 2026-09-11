---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/color-management/color-management-with-adobe-ace-icc.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie das Adobe-ACE und das ICC-Farbmanagement in Substance 3D Painter für konsistente Farbarbeitsabläufe verwenden.
helpx_creative_field: ""
helpx_description: Painter > Features > Color management > Color management with Adobe ACE - ICC
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Farbmanagement mit Adobe ACE - ICC
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 0%

---


# Farbmanagement mit Adobe ACE - ICC

Auf dieser Seite werden die Farbmanagementeinstellungen für das Adobe Color Engine (ACE) aufgeführt, das mit ICC-Profilen verwendet werden soll.

## Projekteinstellungen

![](../../assets/cm-ace.png)

Die Projekteinstellungen können beim Erstellen eines neuen Projekts über das Fenster &quot;[Neues Projekt](../../getting-started/project-creation.md)&quot; oder mithilfe des Fensters &quot;[Projektkonfiguration](../../interface/project-configuration.md)&quot; festgelegt werden.

>[!NOTE]
>
> Wenn eine Umgebungsvariable (siehe unten) oder eine Vorgabedatei geladen wird, werden die Einstellungen in der Benutzeroberfläche deaktiviert.

Die verfügbaren Einstellungen sind:

| Abschnitt | Einstellung | Beschreibung |
| --- | --- | --- |
| **Konfiguration** | **Farbmanagement** | Legen Sie fest, welches Engine zum Verwalten von Farben verwendet werden soll.Mögliche Werte:<ul data-preserve-html="true"> <li data-preserve-html="true"><strong>Legacy</strong> (Standard): Verwenden Sie die vordefinierte sRGB/Linear sRGB Gamma-Farbkorrektur.</li> <li data-preserve-html="true"><strong>OpenColorIO</strong>: Nutze OCIO.</li> <li data-preserve-html="true"><strong>Adobe ACE</strong>: Adobe Color Engine, um ICC-Profile zu unterstützen.</li> </ul> |
|  | **Vorgabedatei verwenden** | Wenn diese Option aktiviert ist, können Sie die Farbmanagementeinstellungen über eine JSON-Konfigurationsdatei steuern. |
|  | **Vorgabedatei** | Pfad zur Voreinstellungsdatei im JSON-Format. Weitere Informationen finden Sie unten. |
|  |  |  |
| **Farbeinstellungen** | **Arbeitsfarbraum** | Der Farbraum, der vom Engine für die Arbeit in der Anwendung verwendet wird. Dies ist der Farbraum, aus dem Texturen konvertiert werden können in (Import) oder aus (Export). Mögliche Werte sind:<ul data-preserve-html="true"> <li data-preserve-html="true"><strong>Linear sRGB IEC61966-2.1</strong> (Standard)</li> <li data-preserve-html="true"><strong>ACEScg ACE Arbeitsfarbraum AMPAS S-2014-004</strong></li> <li data-preserve-html="true"><strong>Linearer Adobe RGB (1998)</strong></li> </ul> |
|  | **Renderpriorität** | Geben Sie die Methode an, die zum Konvertieren von Farben zwischen Farbräumen verwendet wird.Mögliche Werte:<ul data-preserve-html="true"> <li data-preserve-html="true"><strong>Perzeptiv</strong></li> <li data-preserve-html="true"><strong>Sättigung</strong> (Standard)</li> <li data-preserve-html="true"><strong>Relativ chromatisch</strong></li> <li data-preserve-html="true"><strong>Absolut chromatisch</strong></li> </ul> |
|  |  |  |
| **Standardwerte für den Bitmapimport-Farbraum** | **8-Bit-Bilder** | Standardmäßig zu verwendender Farbraum beim Importieren von 8-Bit-Bilddateien. |
|  | **16-Bit-Bilder** | Standardmäßig zu verwendender Farbraum beim Importieren von 16-Bit-Bilddateien. |
|  | **Gleitkommabilder** | Standardmäßig zu verwendender Farbraum beim Importieren von HDR./EXR Bilddateien. |
|  | **Integrierte ICC-Profile verwenden, wenn verfügbar (empfohlen)** | Wenn diese Option aktiviert ist, können Sie die Farben der ICC-Profile seit der Bilddatei anpassen. |
|  |  |  |
| **Substance Material** | **Standardfarbraum für Material** | Legen Sie fest, welcher Farbraum für das Substance von Materialien mit Farb-Management für Ein-/Ausgabe verwendet werden soll. |
|  |  |  |
| **Farbraum exportieren** | **8-Bit-Bilder** | Standardmäßig zu verwendender Farbraum beim Exportieren von 8-Bit-Bilddateien. |
|  | **16-Bit-Bilder** | Standardmäßig zu verwendender Farbraum beim Exportieren von 16-Bit-Bilddateien. |
|  | **Gleitkommabilder** | Beim Exportieren von HDR./EXR Bilddateien standardmäßig zu verwendender Farbraum. |

## Verwenden einer Vorgabedatei

![](../../assets/cm-ace-env-var.png)

Es ist möglich, eine Vorgabedatei (im JSON-Format) zu verwenden, um die ACE beim Erstellen neuer Projekte zu steuern.

### Umgebungsvariable

Die Umgebungsvariable **PAINTER\_ACE\_CONFIG** kann verwendet werden, um den Pfad einer Vorgabedatei anzugeben. Wenn vorhanden, verwendet die Anwendung immer eine Vorgabedatei, um die Farbmanagementeinstellungen zu steuern. Die Einstellungen werden in der Benutzeroberfläche deaktiviert.

Weitere Informationen finden Sie auf der Seite [Umgebungsvariablen](../../pipeline-and-integration/configuration/environment-variables.md).

### Beispiel für Vorgabe

Im Folgenden finden Sie ein Beispiel für eine JSON-Datei, die als Vorgabedatei verwendet werden kann:

```
{ 

  "color settings": { 

    "working color space": "Linear Adobe RGB (1998)", 

    "rendering intent": "Saturation" 

  }, 

  "bitmap import color space defaults" : { 

    "8 bit images": "image P3", 

    "16 bit images": "image P3", 

    "floating point images": "Raw", 

    "use embedded ICC profiles when available": false 

  }, 

  "substance material": { 

    "material color space default": "image P3" 

  }, 

  "export colors spaces" : { 

    "8 bit images": "image P3", 

    "16 bit images": "image P3", 

    "floating point images": "Raw" 

  } 

} 
```
