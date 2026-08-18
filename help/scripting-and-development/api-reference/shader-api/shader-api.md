---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/scripting-and-development/api-reference/shader-api.html"
breadcrumb-title: ''
description: Greifen Sie auf die Shader-API-Referenz für Substance 3D Painter zu, um benutzerdefinierte Shader zu erstellen und die Rendering-Funktionen zu erweitern.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Shader-API
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '702'
ht-degree: 0%

---


# Shader-API

![](../../../assets/header-shader.jpg)

Substance Painter verwendet Shader, um Materialien in seinem Echtzeit-Viewport zu rendern. Es ist möglich, benutzerdefinierte Shader zu schreiben, um neue Verhalten zu implementieren oder den Viewport einfach an andere Renderer anzupassen.

Zusätzliche Shader für Substance Painter finden Sie auf [Substance share](https://share.allegorithmic.com/libraries?by_category_type_id=6).

>[!NOTE]
>
> Der Shader-API ist auch direkt in der Anwendung verfügbar, indem Sie im Menü **Hilfe > Dokumentation > Shader-API** navigieren.

## Shader-Referenz

## Changelog

* [Vollständige Changelog-Datei](changelog-shader-api.md)

## Aufwärmen

Im Substance Painter können Sie eigene Shader in *GLSL* schreiben. Wir erlauben Ihnen, nur einen *Teil* des Fragmentshaders zu schreiben, der manchmal als *Oberflächenshader* bezeichnet wird. Als Nächstes möchten wir den Oberflächenschader &quot;Hello World&quot; für Substance Painter vorstellen:

```
void shade(V2F inputs) { 

  diffuseShadingOutput(vec3(1.0, 0.0, 1.0)); 

}
```


Wenn Sie dieses Snippet jetzt in einer *.glsl*-Datei speichern und in den Substance Painter laden, indem Sie es in die Shader-Registerkarte Ihres Regals ablegen, können Sie es jetzt verwenden und ein schönes gleichmäßiges Rosa auf Ihrem Gitter sehen.

## Surface Shader

* [surface-shader.glsl](shaders-shader-api/surface-shader-shader-api.md)

## Vom Modul bereitgestellte Daten (oder wie kann ich auf meine Kanäle zugreifen?)

Im Substance Painter können Sie auf die Parameter der Rendering-Engine (Dokumentkanäle, zusätzliche Texturen, kamerabezogene Daten und Ähnliches) zugreifen. Hier finden Sie eine vollständige Liste aller Parameter, die für den Motor bereitgestellt wurden:

* [all-engine-params.glsl](parameters-shader-api/all-engine-params-shader-api.md)

## Engine-Einstellungen (oder wie gebe ich Rendering-Status an?)

In einigen Fällen können Sie eine bestimmte Rendering-Konfiguration (Keulung, Füllmethode, Aufnahmeort usw.) für einen Effekt verwenden. Einige Renderstatus werden angezeigt und können im Shader festgelegt werden. Im Folgenden finden Sie eine vollständige Liste aller exponierten Rendering-Status:

* [all-rendering-states-params.glsl](parameters-shader-api/all-rendering-states-params-shader-api.md)

## Benutzerdefinierte Anpassungen (oder wie kann ich meinen Shader anpassen?)

In der Regel werden benutzerdefinierte Anpassungen in einem Shader vorgenommen. Dazu haben wir in den Shadern von Substance Painter eine Möglichkeit eingeführt, benutzerdefinierte Anpassungen festzulegen. Hier finden Sie eine vollständige Liste aller benutzerdefinierten Shader-Tweak-Typen :

* [all-custom-params.glsl](parameters-shader-api/all-custom-params-shader-api.md)

## Integrierte Bibliotheken

Um zu vermeiden, dass Sie in all Ihren Shadern eine Menge Code-Boilerplate schreiben, haben wir eine kleine, aber praktische Bibliothek mit nützlichen Funktionen erstellt. **Bitte beachten Sie, dass Sie es derzeit weder bearbeiten noch eigene erstellen können.**

* [lib-alpha.glsl](libraries-shader-api/lib-alpha-shader-api.md) : enthält Deckkraftbezogene Helfer
* [lib-bayer.glsl](libraries-shader-api/lib-bayer-shader-api.md) : enthält Hilfslinien für die Bayermatrix
* [lib-define.glsl](libraries-shader-api/lib-defines-shader-api.md) : enthält nützliche mathematische Konstanten
* [lib-emissive.glsl](libraries-shader-api/lib-emissive-shader-api.md) : enthält Hilfen für emissive Eigenschaften
* [lib-env.glsl](libraries-shader-api/lib-env-shader-api.md) : enthält Umgebungskarten-bezogene Helfer
* [lib-normal.glsl](libraries-shader-api/lib-normal-shader-api.md) : enthält Hilfsprogramme für Normalmaps (und für Height-Maps generierte Normalmap)
* [lib-pbr.glsl](libraries-shader-api/lib-pbr-shader-api.md) : enthält physikalisch basierte Rendering-Helfer
* [lib-pbr-aniso.glsl](libraries-shader-api/lib-pbr-aniso-shader-api.md) : enthält anisotrope physikalisch basierte Rendering-Helfer
* [lib-pom.glsl](libraries-shader-api/lib-pom-shader-api.md) : enthält Hilfsprogramme für die Parallaxenzuordnung von Verdeckungen
* [lib-random.glsl](libraries-shader-api/lib-random-shader-api.md) : enthält zufällige Dienstprogramme (Sequenzen mit geringer Abweichung)
* [lib-sampler.glsl](libraries-shader-api/lib-sampler-shader-api.md) : enthält Channel-Getter-Helfer
* [lib-sparse.glsl](libraries-shader-api/lib-sparse-shader-api.md) : enthält sichere Spare Texture Sampling Helfer
* [lib-sss.glsl](libraries-shader-api/lib-sss-shader-api.md) : enthält Subsurface-Scattering-Helfer
* [lib-utils.glsl](libraries-shader-api/lib-utils-shader-api.md) : enthält Color-Utility-Funktionen (sRGB-Konvertierungen, Farbtonzuordnung)
* [lib-vectors.glsl](libraries-shader-api/lib-vectors-shader-api.md) : enthält gängige Vektorhilfen

## Metadaten

Sie können zusätzliche nicht erforderliche Informationen deklarieren, um Hinweise auf das Rendering-System zu geben. Syntax:

```
//: metadata { 

//:   "key1":"value1", 

//:   "key2":"value2" 

//: }
```


Unterstützte Schlüssel sind:

* **benutzerdefinierte-Benutzeroberfläche**: Ersetzen Sie die Standardbenutzeroberfläche für Shader-Parameter durch eine benutzerdefinierte Ansicht, die als QML-Modul geschrieben wurde (siehe Scripting-Dokumentation). Der Pfad kann absolut oder relativ zu einem der Ordner &quot;*custom-ui*&quot; in der Ablage sein.
* **mdl**: Definieren Sie das Iray mdl -Material, das mit dem Shader verwendet werden soll. Die Pfadsyntax lautet wie folgt: *mdl::folder1::folder2::mdl\_filename::material\_name* wobei *folder1::folder2::mdl\_filename* der Pfad innerhalb eines Ordners der *mdl*-Ablage zu einer mdl-Datei und *::material\_name* der Name eines in dieser mdl-Datei deklarierten Materials ist. (z. B.: &quot;mdl&quot; : &quot;mdl::alg::materials::physically\_metal\_roughness::physically\_metal\_roughness&quot;)

## Beispiel-Shader (yeah, endlich!)

Um einen Eindruck davon zu bekommen, was wie ein echter Shader aussieht, hier einige Beispiel-Shader, geordnet nach zunehmender Komplexität:

* [pixelated.glsl](shaders-shader-api/pixelated-shader-api.md) : ein pixelierender Shader
* [toon.glsl](shaders-shader-api/toon-shader-api.md) : einen Tonschaber
* [pbr-metal-raw.glsl](shaders-shader-api/pbr-metal-rough-shader-api.md) : der standardmäßige PBR-Shader, der in Substance Painter eingebettet ist

## Dynamische Materialüberlagerung

Die Dynamische Materialüberlagerung ist ein bestimmter Arbeitsablauf, bei dem Materialien in einem Shader zusammengemischt werden und der Benutzer Mischmasken in Substance Painter dynamisch bearbeiten kann. Um diesen Arbeitsablauf zu aktivieren, gibt es zwei neue Funktionen:

* Deklarieren bearbeitbarer Stapel aus einer Shader-Definition: [schichtweise\_deklarieren\_stacks.glsl](parameters-shader-api/layering-declare-stacks-shader-api.md)
* Materialien als Shader-Parameter binden: [Lagern\_bind\_materials.glsl](parameters-shader-api/layering-bind-materials-shader-api.md)
