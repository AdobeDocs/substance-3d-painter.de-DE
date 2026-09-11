---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/content/importing-assets/adding-content-on-the-hard-drive.html"
breadcrumb-title: ''
description: Hier erfahren Sie, wie Sie Inhalte von Ihrer Festplatte zu Substance 3D Painter hinzufügen, um Ihre Ressourcenbibliothek mit lokalen Dateien zu erweitern.
helpx_creative_field: ""
helpx_description: Painter > Content > Importing assets > Adding content on the hard drive
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Hinzufügen von Inhalten auf der Festplatte
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '488'
ht-degree: 2%

---


# Hinzufügen von Inhalten auf der Festplatte

Es ist möglich, Ressourcen zu Ihren Bibliotheken hinzuzufügen, indem Sie neue Inhalte direkt auf der Festplatte am richtigen Ort platzieren.

Standardmäßig wird ein Standardordner für Benutzerelemente bereitgestellt, in dem Sie Ihren neuen Inhalt entweder über die Anwendungsoberfläche oder durch manuelles Ablegen am folgenden Speicherort hinzufügen können. Diese Standardbibliothek wird auch beim Erstellen neuer Vorgaben wie Pinsel, Werkzeuge, intelligente Materialien usw. verwendet. Weitere Informationen finden Sie in der Dokumentation [Vorgaben](../../painting/presets/presets.md).

## Wo werden Assets platziert?

Im Folgenden finden Sie die Speicherorte der standardmäßigen **Bibliothek &quot;Ihre Assets**&quot;, in der Ihre eigenen benutzerdefinierten Inhalte standardmäßig erstellt werden:

<table data-preserve-html="true" style="width: 100.0%;"><colgroup> <col style="width: 15.0%;"/> <col style="width: 15.0%;"/> <col style="width: 70.0%;"/> </colgroup><tbody><tr><th>Plattform</th><th>Version</th><th>Pfad</th></tr><tr><td rowspan="2"><strong>Windows</strong></td><td><strong>7.2</strong> oder höher</td><td colspan="1">C:\Users\username\Documents\Adobe\Adobe Substance 3D Painter</td></tr><tr><td colspan="1">Alte Version</td><td colspan="1">C:\Users\username\Documents\Allegorithmic\Substance Painter</td></tr><tr><td rowspan="2"><strong>Mac</strong></td><td colspan="1"><strong>7.2</strong> oder höher</td><td colspan="1">/Users/Benutzername/Documents/Adobe/Adobe Substance 3D Painter</td></tr><tr><td colspan="1">Alte Version</td><td colspan="1">/Users/Benutzername/Documents/Allegorithmic/Substance Painter</td></tr><tr><td rowspan="2"><strong>Linux</strong></td><td colspan="1"><strong>7.2</strong> oder höher</td><td colspan="1">/home/username/Documents/Adobe/Adobe Substance 3D Painter</td></tr><tr><td>Alte Version</td><td colspan="1">/home/username/Documents/Allegorithmic/Substance Painter</td></tr></tbody></table>

>[!WARNING]
>
> Die **Starter-Assets**, die mit der Anwendung geliefert wurden, befinden sich im Installationsordner und werden in jeder neuen Version ersetzt. Es wird nicht empfohlen, persönliche Inhalte an diesem Speicherort abzulegen, da sie bei jedem Update **&#x200B;**&#x200B;gelöscht werden und sogar Lese-/Schreibberechtigungsprobleme verursachen können.\
> Es empfiehlt sich, den Speicherort **Ihre Assets** oder einen anderen benutzerdefinierten Speicherort zu verwenden. Weitere Informationen zum Hinzufügen eines benutzerdefinierten Bibliothekspfads finden Sie unter [Hinzufügen einer neuen Bibliothek](../../interface/assets/adding-a-new-library.md).

## Dateiformate und Verwendungen

Sie können verschiedene Dateitypen in Ihre Substance 3D Painter-Bibliothek importieren. Sie werden in den angegebenen Ordnern abgelegt (z. B. *alphas*, *colorluts*, *effects*...). weist dem Asset eine Nutzungsart zu. Daher ist es wichtig, den richtigen Ordner auszuwählen, wenn Sie neue Inhalte hinzufügen. Wenn Sie einen benutzerdefinierten Speicherort für die Bibliothek hinzufügen, werden automatisch die entsprechenden Ordner an diesem Speicherort erstellt.

| *Dateiformat* | *Nutzung* | *Ordner* |
| --- | --- | --- |
| **SBSAR** | Substance-Material | Assets/Materials |
| **SBSAR** | Filter | Assets/Effekte |
| **SBSAR** | Generatoren | Assets/Generatoren |
| **PNG, TGA, JPEG usw.** | Textur oder Alpha | Assets/Texturen **oder** Regal/Alphas |
| **HDR., EXR** | Umgebung oder Farb-Lut | Assets/Umgebungen **oder** Regal/Colorlut |
| **GLSL** | Shader | assets / Shaders |
| **SPPR** | Pinselvorgabe | Elemente/Vorgaben/Pinsel |
| **SPPR** | Vorgabe &quot;Partikel&quot; | Assets/Vorgaben/Partikeln |
| **SPPR** | Materialvorgabe | Assets/Vorgaben/Materials **oder** Assets/Materials |
| **SPPR** | Werkzeugvorgabe | Assets/Vorgaben/Tools |
| **SPSM** | Intelligentes Material | Elemente/Smart-Material |
| **SPMSK** | Smart-Maske | Elemente / Smart-Masken |
| **SPEXP** | Exportvorgabe | Regal/Exportvorgaben |

>[!NOTE]
>
> Ab Version 7.2.0 können benutzerdefinierte Ordner und Kategorien in einer Bibliothek verwendet werden. Sie sind im Fenster &quot;Elemente&quot; über [Filter nach Pfad](../../interface/assets/filter-by-path.md) oder [Breadcrumbs](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/navigating-in-the-shelf-147095659.html) zugänglich.

>[!WARNING]
>
> **SBS** (nicht SBSAR)-Dateien können nicht direkt verwendet werden. Sie müssen als SBSAR aus Substance 3D Designer exportiert werden.
