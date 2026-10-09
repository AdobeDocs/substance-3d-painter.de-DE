---
breadcrumb-title: ""
description: Erfahren Sie, wie Sie Mesh-basierte Eingaben in benutzerdefinierten Effekten für Substance 3D Painter verwenden, um geometrieabhängige Textur-Effekte zu erzeugen.
title: Mesh-basierte Eingabe
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '228'
ht-degree: 1%
---

# Mesh-basierte Eingabe

&quot;Mesh-basierte Eingabe&quot; sind Texturen, die vom Engine von Substance 3D Painter bereitgestellt werden, das aus dem Mesh innerhalb des aktuellen Projekts extrahiert wurde. Diese Texturen können verwendet werden, um erweiterte Effekte auf der Grundlage der Mesh-Topologie zu erstellen.

>[!NOTE]
>
> Diese Mesh-Informationen basieren auf der Topologie selbst und berücksichtigen nicht die Mesh-Map (Baking geführt Texturen).
> 
> Der vom Engine bereitgestellte Eingang ist eine 32-bit-Gleitkomma-Textur, die auf den Wert des Eingangs im Substance-Graf herunterskaliert/geklemmt wird.

| Informationen zum Mesh | Kennung | Nutzung | Beschreibung |
| --- | --- | --- | --- |
| *Position (RGB)* | **Mesh\_position** | **meshPosition** | Rufen Sie eine Textur ab, die die Position des Scheitelpunkts enthält. |
| *Welt-Raum-Normale (RGB)* | **mesh\_world\_space\_normal** | **meshNormalWS** | Rufen Sie eine Textur ab, die den Scheitelpunkt normal im Welt-Raum enthält. |
| *Welt-Raum-Tangente (RGB)* | **mesh\_world\_space\_tangent** | **meshTangentWS** | Rufen Sie eine Textur ab, die die Scheitelpunkt-Tangente in Welt-Raum enthält. |
| *Welt-Raum Bitangent (RGB)* | **mesh\_world\_space\_bitangent** | **meshBitangentWS** | Rufen Sie eine Textur ab, die den Scheitelpunkt bi-Tangente (bi-normal) im Welt-Raum enthält. |
| *Texelgröße (Graustufen)* | **Mesh\_texel\_size** | **meshTexelSize** | Rufen Sie eine Textur ab, die die Textgröße (Differenz zwischen Pixeldichte und Mesh-UV) enthält. |
| *UV-Maske (Graustufen)* | **Mesh\_uv\_mask** | **meshUVMask** | Rufen Sie eine Textur als schwarze (Außen) und weiße (Innen) Maske der Mesh-UV-Inseln ab. |
