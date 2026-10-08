---
breadcrumb-title: ""
description: Rufen Sie die Bibliothek Bayer Shader-API reference für Substance 3D Painter auf, um Bayer Dithering-Muster in benutzerdefinierten Shadern zu erstellen.
title: Lib Bayer - Shader-API
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '32'
ht-degree: 0%
---

# Lib Bayer - Shader-API

## lib-bayer.glsl

**Öffentliche Funktionen:** *bayerMatrix8*

```
float bayerMatrix8(uvec2 coords) { 

  return (float(bayer(coords.x, coords.y)) + 0.5) / 64.0; 

} 

 
```
