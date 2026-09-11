---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/scripting-and-development/api-reference/shader-api/changelog-shader-api.html"
breadcrumb-title: ''
description: Prüfen Sie das Änderungsprotokoll für Substance 3D Painter Shader-API, um Updates, neue Funktionen und Änderungen im Zeitverlauf zu verfolgen.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Changelog - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Changelog - Shader-API
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '837'
ht-degree: 3%

---


# Changelog - Shader-API

## Changelog

## 2018.3.2

* [lib-sparse.glsl](libraries-shader-api/lib-sparse-shader-api.md): Sampling-Funktionen verwenden Textur-Derivate anstelle von einfachen Mipmap-Stufen. Dies ist eine Voraussetzung für die Unterstützung von Anisotropie-Sampling. Signaturen für Sampling-Funktionen werden nicht geändert.
* [lib-pom.glsl](libraries-shader-api/lib-pom-shader-api.md): Die Funktionssignatur *getParallaxOffset* wurde geändert, um Textur-Ableitungen zu verwenden.

## 2018.3.0

* Fügen Sie eine neue [lib-pbr-aniso.glsl](libraries-shader-api/lib-pbr-aniso-shader-api.md)-Bibliothek hinzu, um die Visualisierung anisotroper Specular-Highlights zu erleichtern
* Fügen Sie eine neue [lib-sparse.glsl](libraries-shader-api/lib-sparse-shader-api.md)-Bibliothek hinzu, um die Kanalabtastung zu erleichtern, indem Sie die Verfügbarkeit von Mipmaps sicherstellen.
* Update Shader Libraries-Schnittstellen, um dieses sichere Sampling zu gewährleisten
* **Verfall**: Die bisherigen Funktionen, die auf den vec2-Texturen-Koordinaten und dem Texturen-Sampler basieren, sind veraltet (bitte neue Signaturen verwenden).
* [lib-pom.glsl](libraries-shader-api/lib-pom-shader-api.md): Fügen Sie eine *applyParallaxOffset*-Funktion hinzu, um die Verwendung des Effekts &quot;Parallax-Verdeckung&quot; zu vereinfachen.
* [lib-random.glsl](libraries-shader-api/lib-random-shader-api.md): Hinzufügen eines Blue Rauschen-Zufallswertgenerators und temporaler Alternativen
* [lib-sampler.glsl](libraries-shader-api/lib-sampler-shader-api.md): Teilen Sie alle Kanal-Sampling-Helfer auf, um sowohl Wertermittlung als auch Sampling-Helfer zu erhalten

## 2018.2.0

* **Änderung des Shaders-API an der Oberfläche**: Die Funktionssignatur *shade* wurde geändert. Weitere Informationen finden Sie unter [surface-Shader.glsl](shaders-shader-api/surface-shader-shader-api.md).
* Die *shadeShadow*-Funktion wird nicht mehr verwendet und kann sicher aus benutzerdefinierten Oberflächenschattierungen entfernt werden.
* Unterstützung für das Hinzufügen von Volumenstreuungen finden Sie unter [surface-Shader.glsl](shaders-shader-api/surface-shader-shader-api.md) und [lib-sss.glsl](libraries-shader-api/lib-sss-shader-api.md).
* [lib-pbr.glsl](libraries-shader-api/lib-pbr-shader-api.md): Die *pbrComputeBRDF*-Funktion wurde entfernt. Im Beispiel [pbr-metal-raw.glsl](shaders-shader-api/pbr-metal-rough-shader-api.md) erfahren Sie, wie Sie die Bibliothek jetzt verwenden.
* Neue Motorparameter wurden hinzugefügt: *Textur\_blau\_Rauschen*, *Seitenverhältnis\_Seitenverhältnis*, *camera\_vp\_matrix\_inverse*, *Umgebung\_Belichtung*, *Umgebung\_Drehung*, *Fovy*, *Hauptlicht\_Belichtung* und *Bildschirm\_Größe*. Weitere Informationen finden Sie unter [all-Engine-params.glsl](parameters-shader-api/all-engine-params-shader-api.md)
* Fügen Sie die *description*-Metadaten hinzu, um QuickInfos für benutzerdefinierte Shader-Parameter bereitzustellen.

## 2017.4.2

* Fehlende Shader in Dokumentationsbeispielen korrigieren (verpixelte und toon Shader)
* Dithering für hohe Auflösung korrigieren
  * [lib-bayer.glsl](libraries-shader-api/lib-bayer-shader-api.md): **bayerMatrix8()** gibt gültige Werte für Datensätze > 4k zurück.

## 2017.4.1

* PBR-beschichteter Shader reparieren
  * [lib-vectors.glsl](libraries-shader-api/lib-vectors-shader-api.md): **tangentSpaceToWorldSpace()** und **worldSpaceToTangentSpace()** Ausgaben werden jetzt normalisiert

## 2017.4.0

* Falsche Specular-Spiegelung in der 2D-Ansicht für bestimmte Gitter

## 2017.3.1

* Günstigeres Dithering

## 2017.2.0

* Entfernen der interpolierten Tabulatornormalisierung, um das Verhalten von Substance Designer und Bakern abzugleichen
* [Viewport] Ersetzen Sie den Hammersley-Tisch durch eine Fibonacci-Spirale

## 2.6.0

* Anpassen der Füllmethoden für Shader
* Dithering nachbearbeiten. Wenn ich nun ein lineares Rendering verwende, wenden wir es nach dem Farbprofil an

## 2.5.0

* Unterstützung für Farbprofile (LUT) in Viewporten hinzufügen (optional sRGB-Konvertierung)
* Dithering zur Deckkraft in Shadern hinzufügen
* Parallaxe-Verdeckung-Zuordnung zu PBR-Shadern hinzufügen
* Hinzufügen einer Möglichkeit zum Ausblenden benutzerdefinierter Parameter in der Standard-Shader-Benutzeroberfläche
* Link zur Liste der Channel-Tags in der Shader-Dokumentation mit Ebenen hinzufügen
* Tag &quot;channel\_ao&quot; durch &quot;channel\_ambientocclusion&quot; ersetzen
* [Viewport] Einige Normalmaps haben festgeklemmte Werte, die als Artefakte angezeigt werden
* Dokument zu verfügbaren Kanälen im Shader-Format bearbeiten
* Definieren einer benutzerdefinierten Shader-Benutzeroberfläche zulassen
* Standard-UI für Shader mit Ebenen für Material hinzufügen
* Benutzerdefinierte UI-Dateien werden jetzt relativ zum Ordner &quot;shaders/custom-ui&quot; in den Regale durchsucht (wie beim mdl)
* Verwenden des Specular level-Kanals in Standard-Shadern
* Beispiel für vec3-Shader-Parameter beheben
* Upgrade von Painter auf das OpenGL-Kernprofil

## 2.4.0

* Beheben Sie den Unterschied zwischen der exportierten und der im Viewport angezeigten Normalen-Map-Version

## 2.2.0

* Hinzufügen von Unterstützung für bindungslose Texturen in generischen Materialien für Nicht-Dokument-Texturen
* Dokumentation zu benutzerdefinierten Shader-Schiebereglern aktualisieren
* Festlegen der Schrittgenauigkeit für Schieberegler
* Dokumentation für die dynamische Materialüberlagerung

## 2.1.1

* Hinzufügen einer &#39;RGB2Gray&#39;-Funktion in lib-utils

## 2.1.0

* Erlaubt das Definieren von Gruppen für Shader-Parameter und Materialien/Masken.
* Hinzufügen fehlender Kanäle in der Dokumentation (&quot;ao&quot;, &quot;diffuse&quot;, &quot;spiegelnde Ebene&quot;)

## 2.0.4

* Normale Entpackungsfunktion falsch mit niedrigen Alpha-Werten
* Lesen der Scheitelpunkt-Farben des Meshs in benutzerdefiniertem Shader zulassen
* [Viewport] Gedehnt Umgebungs-Map auf einigen Computern

## 2.0.0

* Überschreiben zusätzlicher Normal/AO-Maps durch dedizierten Kanal zulassen
* Ändern der Height2Normal-Funktion, um die Sobel-Methode zu verwenden
* Hinzufügen der Möglichkeit, eine MDL pro Shader zu definieren
* Hinzufügen eines neuen MDL-Ordners zum Regal
* Hinzufügen von Diffus- und Specular level-Kanalvorgaben
* Aktualisierung der Dokumentation für die Tonzuordnung
* Reparieren von Reflexionen im orthografischen Modus
* Die vertikale weiße Störung, die an einer bestimmten Position auf der Umrandung angezeigt wurde, wurde behoben.
* Definieren von &quot;default\_color&quot; für Parameter von Texturen zulassen

## 1.7.0

* Zulassen, dass externe Texturen aufgenommen werden (vom Regal)

## 1.6.0

* Leg einer Gamma-/Tonzuordnungsfunktion, um sie überschreiben zu können
* Leg mehrerer Texcoords

## 1.5.0

* Hinzufügen von Zeilennummer und Dateiname im Shader-Fehlerbericht

## 1.4.1

* Alle sRGB-Konvertierungen folgen dem sRGB-Standard, mit Ausnahme der Konvertierungen in Shadern mit enger Näherung
* Height-Kanal auf Normalen-Map wird in den falschen Farbraum konvertiert

## 1.4.0

* Ambient occlusion-Kanal hinzufügen
* Neuen Arbeitsablauf für die normale Edition hinzufügen
* Hinzufügen der Ausdruckssyntax &quot;or&quot; für die Textur zugehörige automatische Parameter
* pbr-Shader für Intel-GPU unter OSX korrigieren

## 1.3.4

* Binormales in Fragment-Shader interpolieren
* Mikkt-Tangente korrigieren

## 1.3.3

* Festlegen von sphärischen Oberwellen, die eine negative Lichtintensität erzeugen
* Die Belichtungszeit unterscheidet sich von der Berechnung des Substance Designers (und passen Sie den Belichtungsregler an)
* Schatten sollten auf 100 % metallic Fläche nicht sichtbar sein.

## 1.3.0

* Schattenfunktion hinzufügen
* Unterstützung für Deckkraft hinzufügen (&#39;alpha\_test&#39; und &#39;alpha\_blend&#39;)

## 1.2.0

* Möglichkeit, erforderliche OpenGL-Status in benutzerdefinierte Shader umzuwandeln
* Umgekehrte Bitangenten reparieren
* Unterstützung für normalen Kanal hinzufügen

## 1.0

* Unterstützung für benutzerdefinierte Shader hinzufügen
