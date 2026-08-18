---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/performances-guidelines/gpu-drivers.html"
breadcrumb-title: ''
description: Erfahren Sie mehr über den GPU-VRAM und die Treiberanforderungen für Substance 3D Painter zum Optimieren der Rendering-Leistung und -Stabilität.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Performances guidelines > GPU Drivers
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: GPU VRAM und Treiber
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 0%

---


# GPU-Treiber

Wir können keine Leistung garantieren ohne die Verwendung von empfohlenen Treibern. Nicht-WHQL-Treiber müssen vermieden werden.\
GPU-Treiber sind wie jede Software, jede neue Version kann Leistungsprobleme verursachen. Wenn nach dem Aktualisieren auf eine neuere Treiberversion Probleme auftreten, empfehlen wir, die Treiber auf eine frühere Version herunterzustufen.

## NVIDIA-Treibereinstellungen

Einige NVIDIA-Standardeinstellungen können sich auf die Leistung auswirken. Wir empfehlen, ein Profil zu erstellen und die folgenden Parameter zu deaktivieren (deaktivieren Sie sie):

* Thread-Optimierung
* Vertikale Synchronisierung

## Wie andere Anwendungen die GPU nutzen können

Substance 3D Painter arbeitet nicht nur mit der GPU, sondern auch mit anderen Anwendungen. Nahezu jede 3D-Anwendung nutzt die GPU und den VRAM, einschließlich der häufig zusammen mit Painter verwendeten Anwendungen wie Blender, Maya, Unreal Engine, Unity, C4D und anderen. Eine Lösung, die eine gute Leistung gewährleistet, während diese Anwendungen geöffnet bleiben, besteht darin, sicherzustellen, dass Substance 3D Painter zuerst gestartet wird, um eine eigene VRAM-Zuweisung anzufordern. Einige Software kann jedoch Teile des VRAM dynamisch erwerben und dennoch Konflikte mit Substance 3D Painter verursachen, selbst wenn sie nach Painter gestartet wird.

Im Allgemeinen gilt: Je mehr VRAM Painter hat, desto schneller wird es ausgeführt. Versuchen Sie daher, die Menge an VRAM zu minimieren, die von anderen Anwendungen verwendet wird, die gleichzeitig mit Painter ausgeführt werden.

## GPU VRAM-Größe und Bandbreite

Substance 3D Painter ist für die meisten Berechnungen stark von der GPU abhängig. Aus diesem Grund ist es wichtig, eine GPU zu haben, die den [Systemanforderungen](../../getting-started/system-requirements.md) entspricht.

Painter überträgt Texturen in den GPU-Speicher (VRAM), um die Berechnungen durchzuführen (z. B. Füllvorgänge, um die endgültigen Texturen zu erstellen). Wenn der VRAM jedoch voll wird, werden die nicht verwendeten Texturen zurück in den RAM des Computers übertragen, um VRAM-Speicherplatz freizugeben. Substance 3D Painter schreibt und liest bei der Arbeit GBs Daten. Dies bedeutet, dass sowohl die Kapazität des VRAM (Menge) als auch die Bandbreitengeschwindigkeit bei Übertragungen wichtig sind. Sie können Tools wie [MSI AfterBurner](https://www.msi.com/page/afterburner) verwenden, um dieses Verhalten zu überwachen.

>[!NOTE]
>
> Es ist bekannt, dass die <b>Nvidia GTX 970</b> hinsichtlich ihres GPU-Speichers ein problematisches Design aufweist, das sich auf Substance 3D Painter auswirkt. Die letzten 500 MB der gesamten 4 GB funktionieren langsamer als die restlichen 3,5 GB. Wenn Substance 3D Painter mit den letzten 500 MB funktioniert, kann die Leistung um das Zehnfache reduziert werden (gemessen an dem, was wir gemessen haben). Weitere technische Einzelheiten finden Sie unter: <https://www.pcper.com/news/Graphics-Cards/NVIDIA-Responds-GTX-970-35GB-Memory-Issue>
