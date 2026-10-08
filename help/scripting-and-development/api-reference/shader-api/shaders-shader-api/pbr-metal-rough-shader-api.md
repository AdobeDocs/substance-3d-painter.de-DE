---
breadcrumb-title: ""
description: Greifen Sie auf die PBR Metal Rough-Shader-API-Referenz für Substance 3D Painter zu, um physikalisch basierte Materialien zu erstellen.
title: PBR Metal Rough - Shader-API
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '57'
ht-degree: 0%
---

# PBR Metal Rough - Shader-API

## Allegorithmic Metal/Rough PBR Shader

Aus Bibliotheken importieren.

```
import lib-sss.glsl 

import lib-pbr.glsl 

import lib-emissive.glsl 

import lib-pom.glsl 

import lib-utils.glsl
```


Deklarieren Sie das Material iray mdl für diesen Shader.

```
//: metadata { 

//:   "mdl":"mdl::alg::materials::skin_metallic_roughness::skin_metallic_roughness" 

//: }
```


Hier sind die für den Metall-/Grobarbeitsablauf erforderlichen Kanäle gebunden.

```
//: param auto channel_basecolor 

uniform SamplerSparse basecolor_tex; 

//: param auto channel_roughness 

uniform SamplerSparse roughness_tex; 

//: param auto channel_metallic 

uniform SamplerSparse metallic_tex; 

//: param auto channel_specularlevel 

uniform SamplerSparse specularlevel_tex;
```


Shader-Einstiegspunkt.

```
void shade(V2F inputs) 

{ 

  // Apply parallax occlusion mapping if possible 

  vec3 viewTS = worldSpaceToTangentSpace(getEyeVec(inputs.position), inputs); 

  applyParallaxOffset(inputs, viewTS); 

 

  // Fetch material parameters, and conversion to the specular/roughness model 

  float roughness = getRoughness(roughness_tex, inputs.sparse_coord); 

  vec3 baseColor = getBaseColor(basecolor_tex, inputs.sparse_coord); 

  float metallic = getMetallic(metallic_tex, inputs.sparse_coord); 

  float specularLevel = getSpecularLevel(specularlevel_tex, inputs.sparse_coord); 

  vec3 diffColor = generateDiffuseColor(baseColor, metallic); 

  vec3 specColor = generateSpecularColor(specularLevel, baseColor, metallic); 

  // Get detail (ambient occlusion) and global (shadow) occlusion factors 

  float occlusion = getAO(inputs.sparse_coord) * getShadowFactor(); 

  float specOcclusion = specularOcclusionCorrection(occlusion, metallic, roughness); 

 

  LocalVectors vectors = computeLocalFrame(inputs); 

 

  // Feed parameters for a physically based BRDF integration 

  emissiveColorOutput(pbrComputeEmissive(emissive_tex, inputs.sparse_coord)); 

  albedoOutput(diffColor); 

  diffuseShadingOutput(occlusion * envIrradiance(vectors.normal)); 

  specularShadingOutput(specOcclusion * pbrComputeSpecular(vectors, specColor, roughness)); 

  sssCoefficientsOutput(getSSSCoefficients(inputs.sparse_coord)); 

} 

 
```
