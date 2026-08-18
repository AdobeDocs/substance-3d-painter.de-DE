---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/color-management/color-management-with-opencolorio.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie das OpenColorIO-Farbmanagement in Substance 3D Painter für konsistente Farb-Workflows über Pipelines hinweg verwenden.
helpx_creative_field: ""
helpx_description: Painter > Features > Color management > Color management with OpenColorIO
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Farbmanagement mit OpenColorIO
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '675'
ht-degree: 8%

---


# Farbmanagement mit OpenColorIO

Auf dieser Seite werden die Farbmanagementeinstellungen für OpenColorIO (OCIO) aufgeführt.

## Projekteinstellungen

![](../../assets/project-settings-3.png)

Die Projekteinstellungen können beim Erstellen eines neuen Projekts über das Fenster &quot;[Neues Projekt](../../getting-started/project-creation.md)&quot; oder mithilfe des Fensters &quot;[Projektkonfiguration](../../interface/project-configuration.md)&quot; festgelegt werden.

>[!NOTE]
>
> Wenn die **OCIO**-Umgebungsvariable vorhanden ist und eine gültige Konfigurationsdatei angibt, werden die Einstellungen in der Benutzeroberfläche überschrieben und deaktiviert.

Die verfügbaren Einstellungen sind:

<table data-preserve-html="true" style="width: 99.9039%;"><colgroup><col style="width: 12.512%;"/><col style="width: 21.1742%;"/><col style="width: 66.3122%;"/></colgroup><tbody><tr><th style="width: 12.5%;">Abschnitt</th><th style="width: 21.1538%;">Einstellung</th><th style="width: 66.25%;">Beschreibung</th></tr><tr><td rowspan="3" style="width: 12.5%;"><strong>Konfiguration</strong></td><td style="width: 21.1538%;"><strong>Farbmanagement</strong></td><td style="width: 66.25%;"><p>Legen Sie fest, mit welcher Engine Farben verwaltet werden.</p><p>Mögliche Werte:</p><ul><li><strong>Legacy</strong> (Standard): Verwenden Sie die vordefinierte sRGB/Linear sRGB Gamma-Farbkorrektur.</li><li><strong>OpenColorIO</strong>: OCIO-Integration.</li><li><strong>Adobe ACE</strong>: Adobe Color Engine, um ICC-Profile zu unterstützen.</li></ul></td></tr><tr><td style="width: 21.1538%;"><strong>OpenColorIO-Konfiguration</strong></td><td style="width: 66.25%;"><p>Welche Konfigurationsdatei zur Steuerung der Farbmanagementeinstellungen verwendet werden soll.</p><p>Mögliche Werte:</p><ul><li><strong>Substance</strong> (Standard): verwenden Linear gamma als Arbeitsraum.</li><li><strong>ACES 1.0.3</strong>: ACEScg als Arbeitsraum verwenden.</li><li><strong>ACES 1.2</strong>: ACEScg als Arbeitsraum verwenden.</li><li><strong>Benutzerdefiniert</strong>: eine benutzerdefinierte Konfigurationsdatei verwenden.</li></ul></td></tr><tr><td style="width: 21.1538%;"><strong>Konfigurationsdatei</strong></td><td style="width: 66.25%;">Pfad zur OCIO-Konfigurationsdatei. Deaktiviert, wenn der Konfigurationsmodus nicht auf <strong>Benutzerdefiniert</strong> festgelegt ist.</td></tr><tr><th style="width: 12.5%;"><br/></th><th style="width: 21.1538%;"><br/></th><th style="width: 66.25%;"><br/></th></tr><tr><td rowspan="2" style="width: 12.5%;"><strong>Farbeinstellungen</strong></td><td style="width: 21.1538%;"><strong>Mit Farbraum arbeiten</strong></td><td style="width: 66.25%;">Der Farbraum, der vom Modul zum Arbeiten innerhalb der Anwendung verwendet wird. Dies ist der Farbraum, aus dem Texturen konvertiert werden können in (Import) oder aus (Export).</td></tr><tr><td colspan="1"><strong>Standard-sRGB-Farbraum</strong></td><td colspan="1"><p>Der Farbraum, der dem [sRGB](https://en.wikipedia.org/wiki/SRGB)-Farbraum entspricht (IEC 61966-2-1:1999).</p><p>Dieser Farbraum wird an mehreren Stellen innerhalb der Anwendung verwendet:</p><ul><li>Zum Konvertieren des Farbsatzes im Hexadezimalfeld des Farbwählers.</li><li>Um Farbfelder innerhalb des Farbwählers zu speichern und zu laden.</li><li>Wird in der Farbwählerliste als Anzeige aufgeführt.</li></ul></td></tr><tr><th style="width: 12.5%;"><br/></th><th style="width: 21.1538%;"><br/></th><th style="width: 66.25%;"><br/></th></tr><tr><td rowspan="4" style="width: 12.5%;"><strong>Farbraumstandard für Bitmap-Import</strong></td><td style="width: 21.1538%;"><strong>8-Bit-Bilder</strong></td><td style="width: 66.25%;">Standardmäßig zu verwendender Farbraum beim Importieren von 8-Bit-Bilddateien.</td></tr><tr><td style="width: 21.1538%;"><strong>16-Bit-Bilder</strong></td><td style="width: 66.25%;">Standardmäßig zu verwendender Farbraum beim Importieren von 16-Bit-Bilddateien.</td></tr><tr><td style="width: 21.1538%;"><strong>Gleitkommabilder</strong></td><td style="width: 66.25%;">Standardmäßig zu verwendender Farbraum beim Importieren von HDR-/EXR-Bilddateien.</td></tr><tr><td style="width: 21.1538%;"><strong>Farbräume automatisch erkennen</strong></td><td style="width: 66.25%;"><p>Lassen Sie zu, dass der Farbraum aus Ressourcen basierend auf bestimmten Einstellungen definiert wird.</p><p>Mögliche Werte:</p><ul><li><strong>Deaktiviert</strong>: die Standardfarbeinstellung verwenden, ignorieren Sie die Ressourcenkonfiguration.</li><li><strong>Name der Analysedatei</strong> (Standard): Verwenden Sie OCIO [Namenskonvention](https://opencolorio.readthedocs.io/en/latest/guides/authoring/rules.html?highlight=filename#strictparsing), um den Namen des von der Ressource verwendeten Farbraums zu extrahieren.</li><li><strong>Konfigurationsdateiregeln verwenden</strong>: Verwenden Sie die OCIO-Konfiguration, um festzulegen, wie Farbräume zugewiesen werden. Dieser Parameter hat Priorität gegenüber den vorherigen Farbraumeinstellungen der Bilddatei.</li></ul></td></tr><tr><th style="width: 12.5%;"><br/></th><th style="width: 21.1538%;"><br/></th><th style="width: 66.25%;"><br/></th></tr><tr><td style="width: 12.5%;"><strong>Substance</strong></td><td style="width: 21.1538%;"><strong>Standardmäßiger Materialfarbraum</strong></td><td style="width: 66.25%;"><p>Legen Sie fest, welcher Farbraum für das Substance von mit Farbmanagement verwalteten Ein-/Ausgaben von Materialien verwendet werden soll (die Kanalliste finden Sie unten).</p></td></tr><tr><th style="width: 12.5%;"><br/></th><th style="width: 21.1538%;"><br/></th><th style="width: 66.25%;"><br/></th></tr><tr><td rowspan="3" style="width: 12.5%;"><strong>Farbräume exportieren</strong><br/><br/><br/></td><td style="width: 21.1538%;"><strong>8-Bit-Bilder</strong></td><td style="width: 66.25%;">Standardmäßig zu verwendender Farbraum beim Exportieren von 8-Bit-Bilddateien.</td></tr><tr><td style="width: 21.1538%;"><strong>16-Bit-Bilder</strong></td><td style="width: 66.25%;">Standardmäßig zu verwendender Farbraum beim Exportieren von 16-Bit-Bilddateien.</td></tr><tr><td style="width: 21.1538%;"><strong>Gleitkommabilder</strong></td><td style="width: 66.25%;">Standardmäßig zu verwendender Farbraum beim Exportieren von HDR-/EXR-Bilddateien.</td></tr></tbody></table>

### OpenColorIO-Rollen

Die folgenden Rollen werden unterstützt und ermöglichen es, die Standardauswahl von Farbräumen zu ändern:

| Rollenname | Beschreibung |
| --- | --- |
| **substance\_3d\_painter\_standard\_srgb** | Rolle, um den Farbraum anzugeben, der dem [Standard sRGB](https://en.wikipedia.org/wiki/SRGB) entspricht (IEC 61966-2-1:1999). |
| **substance\_3d\_painter\_bitmap\_import\_8bit** | Rolle, um den Farbraum anzugeben, der zum Importieren von 8-Bit-Bildern verwendet wird. |
| **substance\_3d\_painter\_bitmap\_import\_16bit** | Rolle, um den Farbraum anzugeben, der zum Importieren von 16-Bit-Bildern verwendet wird. |
| **substance\_3d\_painter\_bitmap\_import\_floating** | Rolle, um den Farbraum anzugeben, der zum Importieren von HDR-Bildern verwendet wird. |
| **substance\_3d\_painter\_substance\_material** | Rolle, um den Farbraum anzugeben, der für farbverwaltete Kanäle in Substance-Materialien verwendet wird. |
| **substance\_3d\_painter\_bitmap\_export\_8bit** | Rolle, um den Farbraum anzugeben, der beim Exportieren von 8-Bit-Texturen verwendet wird. |
| **substance\_3d\_painter\_bitmap\_export\_16bit** | Rolle, um den Farbraum anzugeben, der beim Exportieren von 16-Bit-Texturen verwendet wird. |
| **substance\_3d\_painter\_bitmap\_export\_floating** | Rolle, um den Farbraum anzugeben, der beim Exportieren von HDR-Texturen verwendet wird. |

>[!NOTE]
>
> Die mit der Anwendung bereitgestellten OCIO-Konfigurationen können als Beispiele für die Verwendung dieser spezifischen Rollen verwendet werden.
