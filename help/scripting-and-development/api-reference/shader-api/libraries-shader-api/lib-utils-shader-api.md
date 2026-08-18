---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/scripting-and-development/api-reference/shader-api/libraries-shader-api/lib-utils-shader-api.html"
breadcrumb-title: ''
description: Greifen Sie auf die Referenz "Lib Utils Shader-API" für Substance 3D Painter zu, um Dienstprogrammfunktionen in der Entwicklung benutzerdefinierter Shader zu verwenden.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Libraries - Shader API > Lib Utils - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Lib Utils - Shader-API
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '238'
ht-degree: 1%

---


# Lib Utils - Shader-API

## Allegorithmic Utility-Funktionen

## Tone Mapping

Dies sind Beispiele für Farbtonzuordnungen, die Sie in Ihrem Shader verwenden können. Painter wendet keine Tonzuordnung an, außer der optionalen, die von Yebis angewendet wird. Wenn du in deinem Shader eine Farbtonzuordnung vornehmen willst, wird diese vor der Farbtonzuordnung auf Yebis angewendet.

Führen Sie die S-Gradationskurvenzuordnung basierend auf den Parametern sigma und n durch.

```
vec3 tonemapSCurve(vec3 value, float sigma, float n) 

{ 

  vec3 pow_value = pow(value, vec3(n)); 

  return pow_value / (pow_value + pow(sigma, n)); 

}
```


## sRGB-Konvertierungen

Dies sind die in Painter verwendeten Konvertierungen. Sie können die automatische Konvertierung von linear -> sRGB im Viewport überschreiben, indem Sie diese Zeile in Ihren benutzerdefinierten Shader einfügen:

*#define DISABLE\_FRAMEBUFFER\_SRGB\_CONVERSION*

und führen Sie Ihre eigene benutzerdefinierte Konvertierung durch.

sRGB in lineare Farbkonvertierung. Skalare Version.

```
float sRGB2linear(float x) 

{ 

  return x <= 0.04045 ? 

    x * 0.0773993808 : // 1.0/12.92 

    pow((x + 0.055) / 1.055, 2.4); 

}
```


sRGB in lineare Farbkonvertierung. RGB.

```
vec3 sRGB2linear(vec3 rgb) 

{ 

  return vec3( 

    sRGB2linear(rgb.r), 

    sRGB2linear(rgb.g), 

    sRGB2linear(rgb.b)); 

}
```


sRGB in lineare Farbkonvertierung. RGB + Alpha.

```
vec4 sRGB2linear(vec4 rgba) 

{ 

  return vec4(sRGB2linear(rgba.rgb), rgba.a); 

}
```


Linear in sRGB. Skalare Version.

```
float linear2sRGB(float x) 

{ 

  return x <= 0.0031308 ? 

      12.92 * x : 

      1.055 * pow(x, 0.41666) - 0.055; 

}
```


Linear in sRGB. RGB.

```
vec3 linear2sRGB(vec3 rgb) 

{ 

  return vec3( 

      linear2sRGB(rgb.r), 

      linear2sRGB(rgb.g), 

      linear2sRGB(rgb.b)); 

}
```


Linear in sRGB. RGB + Alpha.

```
vec4 linear2sRGB(vec4 rgba) 

{ 

  return vec4(linear2sRGB(rgba.rgb), rgba.a); 

}
```


Linear in sRGB; Farbkonvertierung optional. Skalare Version.

```
//: param auto conversion_linear_to_srgb 

uniform bool convert_to_srgb_opt; 

float linear2sRGBOpt(float x) 

{ 

  return convert_to_srgb_opt ? linear2sRGB(x) : x; 

}
```


Linear in sRGB; Farbkonvertierung optional. RGB.

```
vec3 linear2sRGBOpt(vec3 rgb) 

{ 

  return convert_to_srgb_opt ? linear2sRGB(rgb) : rgb; 

}
```


Linear in sRGB; Farbkonvertierung optional. RGB + Alpha.

```
vec4 linear2sRGBOpt(vec4 rgba) 

{ 

  return convert_to_srgb_opt ? linear2sRGB(rgba) : rgba; 

}
```


Farbkonvertierung. Skalare Version.

```
uniform int output_conversion_method; 

float convertOutput(float x) 

{ 

 if (output_conversion_method == 0) return x; 

 else if (output_conversion_method == 1) return linear2sRGB(x); 

 else return sRGB2linear(x); 

}
```


Farbkonvertierung. RGB.

```
vec3 convertOutput(vec3 rgb) 

{ 

 if (output_conversion_method == 0) return rgb; 

 else if (output_conversion_method == 1) return linear2sRGB(rgb); 

 else return sRGB2linear(rgb); 

}
```


Farbkonvertierung. RGB + Alpha.

```
vec4 convertOutput(vec4 rgba) 

{ 

 if (output_conversion_method == 0) return rgba; 

 else if (output_conversion_method == 1) return linear2sRGB(rgba); 

 else return sRGB2linear(rgba); 

}
```


## Dither

Dies sind einige Hilfsmittel, um Shadern Dithering hinzuzufügen.

8x8 Bayer-Matrix für Dithering-Modus verwenden

```
import lib-bayer.glsl 

 

float getDitherThreshold(uvec2 coords) 

{ 

  return bayerMatrix8(coords); 

} 

 

 

vec4 RGB2Gray(vec4 rgba) 

{ 

  float gray = 0.299 * rgba.r + 0.587 * rgba.g + 0.114 * rgba.b; 

  return vec4(vec3(gray), rgba.a); 

}
```


Entfernen von AO und Schatten auf glänzenden Metalloberflächen (nahe bei Spiegeln)

```
float specularOcclusionCorrection(float diffuseOcclusion, float metallic, float roughness) 

{ 

  return mix(diffuseOcclusion, 1.0, metallic * (1.0 - roughness) * (1.0 - roughness)); 

} 

 
```
