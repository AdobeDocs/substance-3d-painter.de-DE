---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/scripting-and-development/api-reference/shader-api/shaders-shader-api/surface-shader-shader-api.html"
breadcrumb-title: ''
description: Greifen Sie auf die Surface Shader-API-Referenz für Substance 3D Painter zu, um benutzerdefinierte Surface Shader-Effekte und -Materialien zu erstellen.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Shaders - Shader API > Surface Shader - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Surface Shader - Shader-API
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '114'
ht-degree: 0%

---


# Surface Shader - Shader-API

## surface-Shader.glsl

Um eine Shader-Ressource zu erstellen, die in Substance Painter verwendet werden kann, erstellen Sie einfach eine GLS-Datei, die eine einzelne Funktion namens *shade* mit dem folgenden Profil enthält:

```
void shade(V2F inputs);
```


## V2F-Eingabetypdefinition:

```
struct V2F { 

  vec3 normal;               // interpolated normal 

  vec3 tangent;              // interpolated tangent 

  vec3 bitangent;            // interpolated bitangent 

  vec3 position;             // interpolated position 

  vec4 color[1];             // interpolated vertex colors (color0) 

  vec2 tex_coord;            // interpolated texture coordinates (uv0) 

  SparseCoord sparse_coord;  // interpolated sparse texture coordinates used by textureSparse() sampling function 

  vec2 multi_tex_coord[8];   // interpolated texture coordinates (uv0-uv7) 

};
```


Hinweis: Um einen SparseCoord für uv1-uv7 zu erhalten, müssen Sie explizit *getSparseCoord(vec2)* aufrufen, definiert in [lib-sparse.glsl](../libraries-shader-api/lib-sparse-shader-api.md)

## Surface Shader Outputs:

Die folgenden Funktionen können innerhalb der *shade*-Funktion aufgerufen werden, um Fragmenteigenschaften zu beschreiben:

```
// fragment opacity. default value: 1.0 

void alphaOutput(float); 

// diffuse lighting contribution. default value: vec3(0.0) 

void diffuseShadingOutput(vec3); 

// specular lighting contribution. default value: vec3(0.0) 

void specularShadingOutput(vec3); 

// color emitted by the fragment. default value: vec3(0.0) 

void emissiveColorOutput(vec3); 

// fragment color. default value: vec3(1.0) 

void albedoOutput(vec3); 

// subsurface scattering properties, see lib-sss.glsl for details. default value: vec4(0.0) 

void sssCoefficientsOutput(vec4);
```


Die grundlegendste Rendering-Gleichung für die Berechnung der Fragmentfarbe ist beispielsweise: *emissiveColor + Albedo \* diffuseShading + specularShading*
