---
breadcrumb-title: ""
description: Erfahren Sie, wie Sie Mesh-basierte Eingaben in benutzerdefinierten Effekten für Substance 3D Painter verwenden, um geometrieabhängige Textur-Effekte zu erzeugen.
title: Mesh-basierte Eingabe
user-guide-description: ""
user-guide-title: ""
source-git-commit: 4432887b652896f77fc3c99010436ef44aeb8a3e
workflow-type: tm+mt
source-wordcount: '279'
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
| *UV Neighbor (RGB)* | **Mesh\_uv\_Nachbar** | **meshUVNeighbor** | Rufen Sie eine Textur mit zwei Informationen ab. Das Innere der UV-Inseln speichert die Koordinaten der regulären UV. Die Außenseite der UV-Inseln speichert die UV-Koordinaten des Pixels auf der anderen Seite der UV-Naht. Diese Textur kann verwendet werden, um nahtlose Effekte zu erzeugen. |
