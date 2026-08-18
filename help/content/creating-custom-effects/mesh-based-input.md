---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/content/creating-custom-effects/mesh-based-input.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie netzbasierte Eingaben in benutzerdefinierten Effekten für Substance 3D Painter verwenden, um geometrieabhängige Textureffekte zu erstellen.
helpx_creative_field: ""
helpx_description: Painter > Content > Creating custom effects > Mesh Based Input
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Gitterbasierte Eingabe
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '228'
ht-degree: 1%

---


# Gitterbasierte Eingabe

&quot;Gitterbasierte Eingabe&quot; sind Texturen, die vom Modul von Substance 3D Painter bereitgestellt werden und aus dem Gitter im aktuellen Projekt extrahiert werden. Diese Texturen können verwendet werden, um erweiterte Effekte basierend auf der Gittertopologie zu erstellen.

>[!NOTE]
>
> Diese Mesh-Informationen basieren auf der Topologie selbst und berücksichtigen nicht die Mesh-Map (baked textures).
> 
> Der Eingang, den der Motor liefert, ist eine 32-bit-Gleitkommatextur, die auf den Wert des Eingangs im Substance-Graphen herunterskaliert/geklemmt wird.

| Gitterinformationen | Kennung | Nutzung | Beschreibung |
| --- | --- | --- | --- |
| *Position (RGB)* | **mesh\_position** | **meshPosition** | Rufen Sie eine Textur ab, die die Scheitelpunktposition enthält. |
| *Normaler Weltraum (RGB)* | **mesh\_world\_space\_normal** | **meshNormalWS** | Rufen Sie eine Textur ab, die die Scheitelpunktnormale im Welt-Raum enthält. |
| *World Space Tangent (RGB)* | **mesh\_world\_space\_tangent** | **meshTangentWS** | Rufen Sie eine Textur ab, die die Scheitelpunkttangente im Weltraum enthält. |
| *World Space Bitangent (RGB)* | **mesh\_world\_space\_bitangent** | **meshBitangentWS** | Rufen Sie eine Textur ab, die den Scheitelpunkt &quot;Bi-Tangente&quot; (Bi-Normal) im Weltraum enthält. |
| *Texelgröße (Graustufen)* | **mesh\_texel\_size** | **meshTexelSize** | Rufen Sie eine Textur ab, die die Texelgröße (Differenz zwischen Pixeldichte und Netz-UV) enthält. |
| *UV-Maske (Graustufen)* | **mesh\_uv\_mask** | **meshUVMask** | Rufen Sie eine Struktur als schwarze (außen) und weiße (innen) Maske der Gitter-UV-Inseln ab. |
