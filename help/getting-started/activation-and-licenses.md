---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/getting-started/activation-and-licenses.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie Substance 3D Painter aktivieren und Lizenzen verwalten, um die Anwendung für das Texturmalen zu verwenden.
helpx_creative_field: ""
helpx_description: Painter > Getting Started > Activation and licenses
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Aktivierung und Lizenzen
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 1%

---


# Aktivierung und Lizenzen

Auf dieser Seite wird erläutert, wie Sie Ihre Lizenzen aktivieren und verwalten, damit Sie Painter verwenden können.

## Aktivierungsprozess nach Anwendungstyp

Der Aktivierungsprozess hängt davon ab, wo Sie Painter erworben haben oder Zugriff darauf haben:

| Anwendungstyp | Aktivierungsprozess |
| --- | --- |
| Creative Cloud Desktop | Weitere Informationen finden Sie auf der entsprechenden Seite in der [HilfeX-Dokumentation](https://helpx.adobe.com/de/download-install/using/download-creative-cloud-apps.html). Falls Probleme auftreten, kann die [Creative Cloud-Dokumentation](https://helpx.adobe.com/de/creative-cloud/user-guide.html) zusätzliche Antworten liefern. |
| dämpfen | Starten Sie das Produkt direkt aus Ihrer Steam-Bibliothek. |
| Substance 3D als eigenständiges Produkt | Weitere Informationen finden Sie im unten beschriebenen Aktivierungsprozess. |

## Schritte zur eigenständigen Aktivierung

### Der Aktivierungsassistent

Der Aktivierungsassistent wird in bestimmten älteren Versionen von Substance 3D Painter angezeigt.

Wenn Sie vor dem 30. September 2022 eine unbefristete Lizenzdatei von der Substance 3D-Website heruntergeladen haben, können Sie sie dennoch verwenden, um geeignete Versionen von Substance 3D Painter über den Aktivierungsassistenten zu aktivieren. [Weitere Informationen zu älteren Substance-Lizenzen und -Konten finden Sie hier.](https://substance3d.adobe.com/faq-end-of-life-accounts/)

![](../assets/activation-wizard.png){width="350px"}

Der Aktivierungsassistent verfügt über drei Optionen:

* <b>Dieses Produkt auswerten</b>: Ältere Testversionen sind nicht mehr verfügbar. [Sie können stattdessen eine 30-tägige Testversion für jede Substance 3D-Anwendung hier &#x200B;](https://www.adobe.com/de/products/substance3d/free-trial-download.html?msockid=35568f9be2b964ec22d09c04e3eb65af) oder mit Creative Cloud Desktop starten.
* <b>Mit einer Lizenzdatei aktivieren</b>: Aktivieren Sie das Produkt mit einer Lizenzdatei (<b>\*.key</b>), die Sie vor dem 30. September 2022 von Ihrer Kontoseite auf der Substance 3D-Website heruntergeladen haben.
* <b>Aktivieren mit Ihrem Konto</b>: Ältere Substanzkonten können nicht mehr für die Aktivierung verwendet werden.

>[!WARNING]
>
> Um die Lizenzdatei mit dem Aktivierungsassistenten zu installieren, müssen Sie Painter als Administrator ausführen und das Antivirenprogramm vorübergehend deaktivieren.

### Manuelle Aktivierung

Sie können Substance Painter manuell aktivieren, indem Sie die Datei license.key in den folgenden Ordner kopieren:

>[!NOTE]
>
> Stellen Sie sicher, dass die Datei &quot;**license.key**&quot; heißt, andernfalls kann sie von der Anwendung nicht gefunden werden.

<table data-preserve-html="true"><colgroup> <col/> <col/> <col/> <col/> </colgroup><tbody><tr><th>Plattform</th><th>Version</th><th colspan="2">Pfad</th></tr><tr><td rowspan="4"><strong>Windows</strong></td><td rowspan="2"><strong>7.2</strong> oder höher</td><td colspan="1">App-Daten (lokal)</td><td colspan="1">C:\Users\[Benutzername]\AppData\Local\Adobe\Adobe Substance 3D Painter</td></tr><tr><td colspan="1">App-Daten (Roaming)</td><td colspan="1">C:\Users\[Benutzername]\AppData\Roaming\Adobe\Adobe Substance 3D Painter</td></tr><tr><td rowspan="2">Alte Version</td><td colspan="1">App-Daten (lokal)</td><td colspan="1">C:\Users\[Benutzername]\AppData\Local\Allegorithmic\Substance Painter</td></tr><tr><td colspan="1">App-Daten (Roaming)</td><td colspan="1">C:\Users\[Benutzername]\AppData\Roaming\Allegorithmic\Substance Painter</td></tr><tr><td rowspan="2"><strong>Mac</strong></td><td colspan="1"><strong>7.2</strong> oder höher</td><td colspan="2">/Users/[Benutzername]/Library/Application Support/Adobe/Adobe Substance 3D Painter</td></tr><tr><td colspan="1">Alte Version</td><td colspan="2">/Users/[Benutzername]/Library/Application Support/Allegorithmic/Substance Painter</td></tr><tr><td rowspan="2"><strong>Linux</strong></td><td colspan="1"><strong>7.2</strong> oder höher</td><td colspan="2">/home/[Benutzername]/.local/share/Adobe/Adobe Substance 3D Painter</td></tr><tr><td>Alte Version</td><td colspan="2">/home/[Benutzername]/.local/share/Allegorithmic/Substance Painter</td></tr></tbody></table>

>[!NOTE]
>
> Einige der Verzeichnisse in den oben genannten Pfaden sind möglicherweise standardmäßig ausgeblendet. Geben Sie den Pfad manuell im Datei-Explorer ein oder zeigen Sie ausgeblendete Dateien an, um sie anzuzeigen.

### Umgebungsvariable

Sie können den Speicherort, an dem Painter die Datei **license.key** sucht, mit einer [Umgebungsvariablen](../pipeline-and-integration/configuration/environment-variables.md) überschreiben.
