---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/scripting-and-development/api-reference/shader-api/libraries-shader-api/lib-sparse-shader-api.html"
breadcrumb-title: ''
description: Greifen Sie auf die Referenz "Lib Sparse Shader-API" für Substance 3D Painter zu, um mit Spare Texture Sampling in benutzerdefinierten Shadern zu arbeiten.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Libraries - Shader API > Lib Sparse - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Lib Sparse - Shader-API
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---


# Lib Sparse - Shader-API

## lib-sparse.glsl

Diese Datei enthält nützliche Funktionen, um sicherzustellen, dass die Sampling-Richtigkeit von &quot;spärlichen Texturen&quot; (ARB\_sparse\_texture) gewährleistet ist. Ermöglicht das Sampeln nur eines Teils der Texturen, die wirklich im Videospeicher vorhanden sind.

**Öffentliche Funktionen:** *getSparseCoord* *getSparseCoordLod0* *textureSparseQueryLod* *textureSparse*

**Öffentliche Strukturen:** *SamplerSparse* *SparseCode*

Das Makro *FEATURE\_SPARSE\_TEXTURE* ist nur definiert, wenn die Erweiterung für virtuelle Texturen mit geringer Dichte aktiviert ist.

Wenn diese Option aktiviert ist, können Sie zusätzliche Textursuchprüfungen verarbeiten, um die Mipmap-Pyramide nach oben zu klettern, wenn Texel fehlen.

```
## ifdef FEATURE_SPARSE_TEXTURE

//: param auto material_lod_check_needed 

uniform bool material_lod_check_needed = false; 

//: param auto material_lod_mask 

uniform usampler2D material_lod_mask; 

## endif // FEATURE_SPARSE_TEXTURE

//: param auto uvtile_reference_sampler 

uniform sampler2D uvtile_reference_sampler; 

//: param auto uvtile_size 

uniform vec2 uvtile_size; 

//: param auto uvtile_inverse_size 

uniform vec2 uvtile_inverse_size; 

//: param auto uvtile_lod_bias 

uniform float uvtile_lod_bias;
```


Informationsstruktur für Sampler und Spare Texture

Wird zum Abfragen aller Sampler-bezogenen Uniformen mit einer einzigen automatischen Bindung verwendet.

```
struct SamplerSparse { 

  sampler2D tex; 

  vec4 size; // width, height, 1/width, 1/height 

  bool is_set; // a boolean indicating whether the texture is in the texture set or not 

  uvec3 lod_mask_select; // masking operations description allowing to retrieve loaded mipmaps information 

};
```


Koordinaten für spärliches Sampling

UV-Koordinaten und materialsparse LoD-Maske speichern

```
struct SparseCoord { 

  vec2 tex_coord; 

  vec2 dfdx; 

  vec2 dfdy; 

  float lod; 

  uint material_lod_mask; 

}; 

 

 

## if defined(SHADER_FRAGMENT)
```


Struktur der Texturkoordinaten erstellen, die von der *textureSparse()*-Sampling-Funktion verwendet wird (muss vom Fragmentshader aufgerufen werden)

Beispiel: *SparseCoord uv1coord = getSparseCoord(inputs.multi\_tex\_coord[1]);*

```
SparseCoord getSparseCoord(vec2 tex_coord) { 

  SparseCoord res; 

  res.tex_coord = tex_coord; 

  res.dfdx = dFdx(tex_coord); 

  res.dfdy = dFdy(tex_coord); 

## ifdef FEATURE_SPARSE_TEXTURE

  res.material_lod_mask = material_lod_check_needed ? 

    textureLod(material_lod_mask,tex_coord,0.0).r : 

    0u; 

  res.lod = getLodFromReferenceSampler(tex_coord); 

## endif // FEATURE_SPARSE_TEXTURE

  return res; 

} 

## endif
```


Struktur der Texturkoordinaten erstellen, die von *textureSparse()*-Sampling-Funktion verwendet wird Sampling-Version auf Basisebene (kann verwendet werden, wenn sich der Fragmentshader außerhalb des Fragments befindet)

```
SparseCoord getSparseCoordLod0(vec2 tex_coord) { 

  SparseCoord res; 

  res.tex_coord = tex_coord; 

  res.dfdx = vec2(0.0); 

  res.dfdy = vec2(0.0); 

## ifdef FEATURE_SPARSE_TEXTURE

  res.material_lod_mask = material_lod_check_needed ? 

    textureLod(material_lod_mask,tex_coord,0.0).r : 

    0u; 

  res.lod = 0.0; 

## endif // FEATURE_SPARSE_TEXTURE

  return res; 

} 

 

## if defined(SHADER_FRAGMENT)
```


Berechnen des Detaillierungsgrads, der zum Aufnehmen einer geringen Textur verwendet werden würde

Mipmap-Pyramide nach oben klettern, wenn Texel fehlen Gibt LoD VOR angewendeter LoD-Voreinstellung zurück

```
float textureSparseQueryLod(SamplerSparse sampler, SparseCoord coord) { 

## ifdef FEATURE_SPARSE_TEXTURE

  float lodfix = coord.lod; 

  if (material_lod_check_needed) { 

    lodfix = getFixedSparseLod(getTextureLodMask(sampler.lod_mask_select, coord.material_lod_mask), lodfix); 

  } 

  return lodfix-uvtile_lod_bias; 

## else // FEATURE_SPARSE_TEXTURE

  return textureQueryLod(sampler.tex, coord.tex_coord).y-uvtile_lod_bias; 

## endif // FEATURE_SPARSE_TEXTURE

} 

## endif // SHADER_FRAGMENT
```


Berechnen der Derivate, die zur Probenahme aus einer spärlichen Textur verwendet werden würden

Bei fehlenden Texeln die Minimappyramide nach oben klettern

```
void textureSparseQueryGrad(out vec2 dfdx, out vec2 dfdy, SamplerSparse sampler, SparseCoord coord) { 

## ifdef FEATURE_SPARSE_TEXTURE

  if (material_lod_check_needed) { 

    float lodfix = getFixedSparseLod(getTextureLodMask(sampler.lod_mask_select, coord.material_lod_mask), coord.lod); 

    if (coord.lod!=lodfix) { 

      // Fix dfdx dfdy, take account offset, no more anisotropy 

      vec2 ddfix = exp2(lodfix-uvtile_lod_bias) * uvtile_inverse_size; 

      dfdx = vec2(ddfix.x,0.0); 

      dfdy = vec2(0.0,ddfix.y); 

      return; 

    } 

  } 

## endif // FEATURE_SPARSE_TEXTURE

  dfdx = coord.dfdx; 

  dfdy = coord.dfdy; 

}
```


Führt eine Textursuche auf einer spärlichen Textur durch, gehen Sie bei Bedarf die Mipmap-Stufen hoch

Diese Funktion ersetzt den Standard *texture(sampler2D, vec2)*, um Texel aus einer spärlichen Textur abzurufen

```
vec4 textureSparse(SamplerSparse sampler, SparseCoord coord) { 

  vec2 dfdx,dfdy; 

  textureSparseQueryGrad(dfdx, dfdy, sampler, coord); 

  return textureGrad(sampler.tex, coord.tex_coord, dfdx, dfdy); 

}
```


Führt bei einer Textur eine optimierte Mehrfachtextursuche mit kleinen Abständen durch

Wir stellen alternative Versionen dieses Helfers für bis zu N=4 zur Verfügung

```
void textureSparseOffsets(SamplerSparse sampler, SparseCoord coord, vec2 offsets[N], out vec4 results[N]) { 

  vec2 dfdx,dfdy; 

  textureSparseQueryGrad(dfdx, dfdy, sampler, coord); 

  for(int i = 0; i < N; ++i) { 

    results[i] = textureGrad(sampler.tex, coord.tex_coord + offsets[i], dfdx, dfdy); 

  } 

} 

 
```
