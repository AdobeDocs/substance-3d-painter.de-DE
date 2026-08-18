---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/getting-started/export/export-presets/predefined-presets/usd-pbr-metal-roughness-preset.html"
breadcrumb-title: ''
description: Lerne, wie du in Substance 3D Painter mit der Exportvorgabe "USDz (Apple AR)" Texturen für Apple AR-Workflows exportieren kannst.
helpx_creative_field: ""
helpx_description: Painter > Getting Started > Export > Export presets > Predefined Presets > USDz (Apple AR) Preset
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: USDz (Apple AR)
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '220'
ht-degree: 0%

---


# Vordefinierte USDz-Vorlage (Apple AR)

>[!NOTE]
>
> Verwenden Sie zum Exportieren in USD mit einer benutzerdefinierten Ausgabevorlage nicht die Vorlage USDz (Apple AR). Verwenden Sie stattdessen Ihre ausgewählte Ausgabevorlage und aktivieren Sie <b>USD-Asset exportieren</b> am unteren Rand der Registerkarte <b>Einstellungen</b>.

Die vordefinierte USDz (Apple AR)-Ausgabevorlage exportiert Ihr Element, das für die Verwendung mit Apple AR-Anwendungen konfiguriert ist.

Verwenden der Vorlage &quot;USDz (Apple AR)&quot;:

1. Öffnen Sie das Exportfenster mit <b>Datei > Texturen exportieren</b> oder mit der Tastenkombination <b>Strg + Umschalt + E</b>.
1. Öffnen Sie auf der Registerkarte <b>Einstellungen</b> das Dropdown-Menü <b>Ausgabevorlage</b> und wählen Sie <b>USDz (Apple AR)</b> aus.

![Ein Bild des Exportfensters mit geöffnetem Ausgabevorlagen-Dropdown und ausgewähltem USDz (Apple AR).](../../../assets/export-usd.png){zoomable="yes"}

Es werden fünf Texturdateien erstellt und gespeichert (Grundfarbe, Metall, Normal, Verdeckung und Raueit). Alle Dateien werden als JPG gespeichert, mit Ausnahme der normalen Map, die als PNG gespeichert wird, um Artefakte aufgrund der verlustbehafteten Komprimierung zu vermeiden.

Darüber hinaus werden zwei weitere Dateien mit der Erweiterung usdc und usdz erstellt:

Hier ist ein Beispiel für die JadeToad, die direkt in MacOS vom Finder aus geöffnet wurde:

![](../../../assets/usdz.png){width="400px"}

Hier ist ein Beispiel für eine USDZ-Datei, die an einen iPhone gesendet wurde und den AR-Modus verwendet, um das JadeToad-Modell in einer realen Umgebung zu platzieren:

![](../../../assets/3d-usdz.jpg){width="500px"}
