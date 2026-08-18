---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/scripting-and-development/api-reference/shader-api/parameters-shader-api/all-engine-params-shader-api.html"
breadcrumb-title: ''
description: Greifen Sie auf die Substance 3D Painter-Shader-API-Referenz "Alle Motorparameter" zu, um Shader-Parameter auf Engine-Ebene zu steuern.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Parameters - Shader API > All Engine Params - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Alle Motorparameter - Shader-API
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---


# Alle Motorparameter - Shader-API

## Beispiele für Motorparameter

## Texturparameter

Substance Painter verwendet ein SVT-System (Sparse Virtual Texture), um Texturen im Viewport anzuzeigen.

Weitere Informationen zu diesem System finden Sie in der [Onlinedokumentation](../../../../features/sparse-virtual-textures.md).

Dieses System hat Auswirkungen auf das Schreiben von Shader-Code. Wir stellen Helfer zur Verfügung, um die Verwendung mit der Struktur *SamplerSparse* und den Textursuchfunktionen zu vereinfachen (siehe [lib-sparse.glsl](../libraries-shader-api/lib-sparse-shader-api.md)).

Allgemeine Verwendung:

```
// Defines the SamplerSparse structure 

import lib-sparse.glsl 

 

//: param auto TEXTURE_TAG 

uniform SamplerSparse uniform_tex;   // Texture sampler and its information
```


Mit Texturparametern kann der Operator &quot;or&quot; zum Definieren eines Fallbacks verwendet werden:

```
//: param auto TEXTURE_TAG_1 or TEXTURE_TAG_2 

uniform SamplerSparse uniform_tex; // if TEXTURE_TAG_1 exists then TEXTURE_TAG_1 else TEXTURE_TAG_2
```


Dabei ist *TEXTURE\_TAG* eines der unten beschriebenen Tags.

### Tags für Dokumentkanäle

Alle diese Texturen sind **vormultipliziert** und **erweitert**, um Nahtprobleme zu vermeiden.

**Kanäle für Textursatz**

*channel\_ambientocclusion* *channel\_anisotropyangle* *channel\_anisotropylevel* *channel\_basecolor* *channel\_blendingmask* *channel\_diffuse* *channel\_Versatz* *channel\_emissive* *channel\_glossiness* 8&rbrace;Kanal\_Height **&#x200B; Kanal\_Senior &#x200B;** Kanal\_metallisch **&#x200B; Kanal\_normal &#x200B;** Kanal\_Deckkraft **&#x200B; Kanal\_Spiegelung &#x200B;** Kanal\_Raueit **&#x200B; Kanal\_Streuung &#x200B;** Kanal\_Specular *36&rbrace;channel\_specularlevel* *channel\_transmissive***

**Benutzerkanäle**

*Kanal\_Benutzer0* *Kanal\_Benutzer1* *Kanal\_Benutzer2* *Kanal\_Benutzer3* *Kanal\_Benutzer4* *Kanal\_Benutzer5* *Kanal\_Benutzer6* *Kanal\_Benutzer7*

### Mesh-Maps

*texture\_ambientocclusion* : Umgebungskarte Verdeckung\
*Textur\_Krümmung* : Krümmungskarte\
*texture\_id* : ID-Map\
*Textur\_normal* : Normale Tangentialraumkarte\
*texture\_normal\_ws* : Normale Weltraumkarte\
*texture\_position* : Weltkarte der Weltraumposition\
*Textur\_Thickness* : Thickness Map

## Zusätzliche Texturparameter

Allgemeine Verwendung:

```
//: param auto TEXTURE_TAG 

uniform sampler2D uniform_tex;   // The texture itself 

 

//: param auto TEXTURE_TAG_size 

uniform vec4 uniform_tex_size;   // The size of the texture (width, height, 1/width, 1/height)
```


Mit Texturparametern kann der Operator &quot;or&quot; zum Definieren eines Fallbacks verwendet werden:

```
//: param auto TEXTURE_TAG_1 or TEXTURE_TAG_2 

uniform sampler2D uniform_tex; // if TEXTURE_TAG_1 exists then TEXTURE_TAG_1 else TEXTURE_TAG_2 

 

//: param auto TEX_TAG_1_size or TEX_TAG_2_size 

uniform vec4 uniform_tex_size; // if TEX_TAG_1 exists then TEX_TAG_1_size else TEX_TAG_2_size
```


Dabei ist *TEXTURE\_TAG* eines der unten beschriebenen Tags.

*Textur\_blau\_Rauschen* : Eine Struktur für blaues Rauschen\
*texture\_environment* : Umgebungszuordnung, **mip-mapped**, verwenden Sie [lib-env.glsl](../libraries-shader-api/lib-env-shader-api.md), um diese zu verwenden

## Andere Parameter

*aspect\_ratio* : ein *float*, das das Ansichtsfenster *width / Height* ratio enthält

```
//: param auto aspect_ratio 

uniform float uniform_aspect_ratio;
```


*Kamera\_Ansicht\_Matrix* : a *mat4* , das die Transformation vom Welt- in den Kameraraum darstellt

```
//: param auto camera_view_matrix 

uniform mat4 uniform_camera_view_matrix;
```


*camera\_view\_matrix\_it* : Inverse-Transpose-Version von *Kamera\_Ansicht\_Matrix*

```
//: param auto camera_view_matrix_it 

uniform mat4 uniform_camera_view_matrix_it;
```


*camera\_vp\_matrix\_inverse* : Umkehrung der *Projektion \* Kamera\_Ansicht\_Matrix* Matrix

```
//: param auto camera_vp_matrix_inverse 

uniform mat4 uniform_camera_vp_matrix_inverse;
```


*Umgebung\_Exposition* : ein *float*, der die Belichtung der Envmap darstellt

```
//: param auto environment_exposure 

uniform float uniform_environment_exposure;
```


*Umgebung\_max\_lod* : ein *float*, der die Tiefe der MIP-Map-Pyramide der Envmap darstellt

```
//: param auto environment_max_lod 

uniform float uniform_max_lod;
```


*Umgebung\_Drehung* : ein *float*, der die Drehung der Envmap um die Hochachse darstellt\
Der Wert liegt im Bereich [0,1] und sollte dem Bereich [0, 2\*pi] zugeordnet werden.

```
//: param auto environment_rotation 

uniform float uniform_environment_rotation;
```


*gegenüberliegend* : eine *Ganzzahl*, die gerenderte Gesichter angibt (-1: Rückseiten, 0: undefiniert, 1: Vorderseiten)\
Wert 0 bedeutet, dass Sie sich sicher auf die integrierte glsl-Variable *gl\_FrontFacing* verlassen können.

```
//: param auto facing 

uniform int uniform_facing;
```


*fovy* : ein *Schwimmer*, der das Kamerafeld entlang der Y-Achse darstellt

```
//: param auto fovy 

uniform float uniform_fovy;
```


*is\_2d\_view* : ein *bool*, der angibt, ob das Rendern für die 2D-Ansicht ausgeführt wird oder nicht

```
//: param auto is_2d_view 

uniform bool uniform_2d_view;
```


*is\_perspective\_projection* : ein *bool*, der angibt, ob die Projektion perspektivisch oder orthografisch ist

```
//: param auto is_perspective_projection 

uniform bool uniform_perspective_projection;
```


*main\_light* : ein *vec4*, das die Position des Hauptlichts in der Umgebung angibt

```
//: param auto main_light 

uniform vec4 uniform_main_light;
```


*mvp\_matrix* : eine *mat4*, die die Projektionsmatrix der Modellansicht darstellt

```
//: param auto mvp_matrix 

uniform mat4 uniform_mvp_matrix;
```


*Szene\_Original\_Radius* : ein *float*, der den Radius der Begrenzungskugel der Szene vor ihrer Normalisierung darstellt

```
//: param auto scene_original_radius 

uniform float uniform_scene_original_radius;
```


*screen\_size* : ein *vec4* mit Bildschirmgrößendaten *(Breite, Height, 1/Breite, 1/Height)*

```
//: param auto screen_size 

uniform vec4 uniform_screen_size;
```


*Welt\_Kamera\_Richtung* : ein *vec3*, das die Weltkameraausrichtung darstellt

```
//: param auto world_camera_direction 

uniform vec3 uniform_world_camera_direction;
```


*Welt\_Auge\_Position* : ein *vec3*, das die Weltaugenposition darstellt

```
//: param auto world_eye_position 

uniform vec3 uniform_world_eye_position; 

 
```
