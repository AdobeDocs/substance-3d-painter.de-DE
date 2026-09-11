---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/post-processing/color-profile.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie die Farbprofil-Nachbearbeitung in Substance 3D Painter verwenden, um Farbkorrekturen und LUT-Transformationen anzuwenden.
helpx_creative_field: ""
helpx_description: Painter > Features > Post Processing > Color Profile
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Farbprofil
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 0%

---


# Farbprofil

![](../../assets/doc-lut-example.jpg){width="700px"}

Substance 3D Painter ermöglicht es, **Farbprofils** den **Viewporten** zuzuweisen, indem **LUT** Texturen geladen werden.\
Mithilfe eines Farbprofils kann die endgültige Farbe des Bildschirms kalibriert werden, um sie an ein Ziel, z. B. eine bestimmte Kamera, anzupassen. Häufig werden Farben durch ein Profil manipuliert, indem die Helligkeit, das Gamma, der Kontrast oder sogar die Farbbalance geändert werden.

>[!NOTE]
>
> **LUT** steht für &quot;**Nachschlagetabelle**&quot;. Dies ist eine optimierte Möglichkeit, Farbkorrekturen als Nachbearbeitungseffekt durchzuführen. Eine LUT wird verwendet, um den Unterschied zwischen einer Quelle und einem Ergebnis auszugleichen.\
>  Substance 3D Painter verwendet **3D** LUTs, die als **2D-Textur** (Gleitend) mit einer beliebigen Auflösung gespeichert sind (Standardauflösung: **2048x128 Pixel** ). Dies bedeutet, dass der Würfel, der die Farboperationen speichert, in Scheiben getrennt ist, die nebeneinander angezeigt werden. Weitere technische Details finden Sie im Artikel **GPU Gem** : 2<http://http.developer.nvidia.com/GPUGems2/gpugems2_chapter24.html>

## Farbprofil verwenden

Ein Farbprofil kann über das Fenster Anzeigeeinstellungen geladen werden.\
Aktivieren Sie das Kontrollkästchen &quot;**Farbprofil aktivieren** &quot;, um den Viewport zu beeinflussen und ein Farbprofil zu aktivieren.

![](../../assets/color-profile-ui.png)

* Wenn &quot;Farbprofil aktivieren&quot; **deaktiviert** ist, erfolgt das Rendern des Viewports in **sRGB** für die Kanalansicht (und linear für einige bestimmte Materialien).
* Wenn &quot;Farbprofil aktivieren&quot; **aktiviert** ist, erfolgt das Rendern des Viewports in **Linear/Raw** für jede Ansicht (einschließlich Solokanälen).

Wenn eine LUT-Textur in den Ressourcensteckplatz geladen wird, wird sie verwendet, um das Rendern des Viewports zu bearbeiten, wenn sie sich in **Materialmodi** befindet.\
Andernfalls wird das Rendering als Linear/Raw angezeigt (z. B. mit Solokanal-Ansichten).

Die Einstellung **Weißpunkt** kann verwendet werden, um die Tonzuordnung des Eingabebildes zu ändern (bevor die LUT wirksam wird).\
Wenn Sie beispielsweise die Sonne betrachten, sollte der Wert höher als 1 (Standard) sein. Für eine perfekte Belichtung muss der Weißpunkt auf den hohen Wert des Bildes gesetzt werden.

Der Weißpunkt lautet wie folgt:

```
float Value = 1.0f / WhitePoint; // Value from the user interface 

float3 Output = clamp( HDR.rgb * Value, 0.0f, 1.0f );
```


Es ist möglich, eine bestimmte Farbtonzuordnung anzuwenden, bevor Sie ein Farbprofil verwenden. Weitere Informationen finden Sie in den Funktionen in [Farbtonzuordnung](tone-mapping.md).\
Substance 3D Painter verarbeitet die Eingabefarbe nur über die Weißpunkt-Einstellung. Es gibt z. B. keine Shaper LUT.

## Erstellen von Farbprofilen

Substance 3D Painter verschiebt den Viewport auf **Linear**-Rendering, wenn **Farbprofil aktivieren** aktiviert ist. Dies bedeutet, dass beim Anwenden einer LUT die Farbe von einem linearen Profil an das gewünschte Ziel Kamera bewogen werden muss.

### Methode 1: Ändern der Identitäts-LUT

Die Bearbeitung der Identitäts-LUT kann in einer Software erfolgen, die <b>32bits floating</b> Texturen unterstützt, wie z. B. <b>Substance 3D Designer</b>. Laden Sie die Identitäts-LUT als Ausgangspunkt herunter, um ein neues Profil zu erstellen:

[Farbe\_Profil\_linear.exr herunterladen](https://github.com/AdobeDocs/painter-python-api/raw/refs/heads/main/static/misc/color_profile_linear.exr)

### Methode 2 : Verwenden von OpenColor IO zum Generieren einer LUT-Textur

Installieren Sie die **OpenColor IO**-Tools. Laden Sie dann die Beispiel-OCIO-Konfiguration herunter, die hier verfügbar ist: <http://opencolorio.org/downloads.html>\
Führen Sie dort das **ociolutimage**-Programm mit den folgenden Argumenten aus:

```
ociolutimage --generate --cubesize 64 --config nuke-default/config.ocio --colorconvert linear srgb --output lutLinearToSRGB.exr
```


**Hinweis**: Es ist auch möglich, die Identity LUT mit **OpenColor IO** zu ändern, indem Sie das Programm **ocioconvert** verwenden, um die Farbkonvertierung auf diese LUT anzuwenden.

### Importieren eines neuen Farbprofils

Öffnen Sie einfach das Importfenster (oder ziehen Sie die LUT per Drag &amp; Drop in das Regal). Stellen Sie beim Importieren der LUT-Textur in Substance 3D Painter sicher, dass Sie der neuen Ressource &quot;**colorlut** &quot; **usage** zuweisen. Andernfalls wird die Ressource nicht korrekt im Regal angezeigt.

Weitere Informationen finden Sie in der Dokumentation zum Import neuer Ressourcen : [Ressourcen werden über das Importfenster hinzugefügt](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/adding-content-via-the-import-window-151584824.html)
