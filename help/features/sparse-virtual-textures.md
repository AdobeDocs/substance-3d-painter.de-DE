---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/sparse-virtual-textures.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie in Substance 3D Painter virtuelle Texturen mit geringer Dichte verwenden, um effizient mit Texturen mit ultrahoher Auflösung zu arbeiten.
helpx_creative_field: ""
helpx_description: Painter > Features > Sparse Virtual Textures
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Virtuelle Strukturen mit geringer Dichte
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '748'
ht-degree: 0%

---


# Virtuelle Strukturen mit geringer Dichte

![](../assets/svt-header.jpg)

Ab Version **2018.3** verwendet Substance 3D Painter **Virtuelle Texturen mit geringer Dichte** (**SVT** ) in seinem Echtzeit-Viewport, um eine große Anzahl von Texturen zu verwalten. Diese Technologie ermöglicht das Streamen von Texturen, die nur aus einem bestimmten Blickwinkel erforderlich sind, um eine bestimmte Stellfläche auf dem GPU-Speicher beizubehalten. Es verbessert die Leistung bei Projekten mit einer großen Anzahl von Textursets (oder UDIMs).

## Unterstützte Plattformen

![](../assets/sparse-settings.png)

Geringe Texturen erfordern eine spezielle Hardware-Konfiguration, um voll leistungsfähig zu sein. Wenn die aktuelle Konfiguration sie nicht ordnungsgemäß unterstützt, **fallback** zu einer Softwareimplementierung (die weniger präzise und weniger leistungsfähig ist).

Es ist möglich, Substance 3D Painter zu zwingen, den Software-Fallback anstelle der Hardwarebeschleunigung zu verwenden, indem Sie in [Einstellungen](../interface/settings/settings.md) nachsehen.

Hier sind die Konfigurationen, die die hardwarebeschleunigten virtuellen Sparse-Texturen unterstützen:

| Plattform | Unterstützt (Hardware-beschleunigt) | Nicht unterstützt (Software-Fallback) |
| --- | --- | --- |
| **Windows** | <ul data-preserve-html="true"><li data-preserve-html="true">Nvidia GeForce (Treiber 411.63 oder höher)</li><li data-preserve-html="true">NVIDIA Quadro (Treiber 411.63 oder höher)</li><li data-preserve-html="true">AMD FirePro und Radeon Pro (Treiber 18.9.3 oder höher) <strong> &#42; </strong></li><li data-preserve-html="true">AMD Radeon (Treiber 18.9.3 oder höher)&#42;</li></ul> | <ul data-preserve-html="true"><li data-preserve-html="true"> NVIDIA Quadro M2000 </li><li data-preserve-html="true">  NVIDIA Geforce GTX 970 </li><li data-preserve-html="true"> Intel GPUs </li></ul> |
| **Mac-Betriebssystem** | <ul data-preserve-html="true"><li data-preserve-html="true"> Hardwarefunktion wird vom Betriebssystem nicht unterstützt </li></ul> | <ul data-preserve-html="true"><li data-preserve-html="true">Beliebiges GPU-Modell</li></ul> |
| **Linux** | <ul data-preserve-html="true"><li data-preserve-html="true">Nvidia GeForce (Treiber 410.73 oder höher)</li><li data-preserve-html="true">NVIDIA Quadro (Treiber 410.73 oder höher)</li><li data-preserve-html="true">AMD FirePro und Radeon Pro (Treiber 18.9.3 oder höher) <strong> &#42; </strong></li><li data-preserve-html="true">AMD Radeon (Treiber 18.9.3 oder höher)&#42;</li></ul> | <ul data-preserve-html="true"><li data-preserve-html="true">Intel-GPU</li></ul> |


* **\*** : Hardwarebeschleunigung ist standardmäßig deaktiviert und kann manuell in den [Einstellungen](../interface/settings/settings.md) aktiviert werden.

## Warum verwendet Substance 3D Painter virtuelle Texturen mit geringer Dichte?

Substance 3D Painter verwendet seine Haupt-Engine für die Berechnung von Texturen, die dann in den Viewports angezeigt werden. Das bedeutet, dass Engine und Viewport den GPU-Speicher (VRam) gemeinsam nutzen müssen, um diese Texturen zu berechnen und anzuzeigen. Je mehr **Textursätze** (oder UV-Kacheln) ein Projekt enthält, desto mehr Speicher wird für den Viewport benötigt. Wenn der Viewport zu viel Speicher auf der GPU belegt, hat die Haupt-Engine nicht genügend Platz, um Texturen zu berechnen, und muss Texturen in den Systemspeicher (RAM) auslagern. Dies führt zu schlechten Leistungen und langsamen Berechnungen.

Ziel der SVT ist es, den Viewport so viel wie möglich vom GPU-Speicher zu verwenden und der Engine so viel Platz wie möglich für die Berechnungen zu lassen. Der Vorteil des Systems besteht darin, dass es auch die Möglichkeit bietet, viel größere Projekte in Substance 3D Painter zu laden, während es gleichzeitig wie gewohnt funktioniert.

## Wie funktioniert Sparse Textures ?

Virtuelle Texturen mit geringer Dichte sind eine Art von Texturen, die nicht vollständig sind. Das bedeutet, dass die Anwendung nur Teile von Texturen im Speicher lädt. Es wird nur das geladen, was benötigt wird, und der Rest wird in den Systemspeicher oder auf die Festplatte (Cache) geladen. Bei Bedarf werden die Texturen aus dem Cache abgerufen und wieder in den Viewport verschoben. Um die Übertragung schnell genug zu gestalten, verwendet das System **MIPMAPS** und springt schnell zwischen verschiedenen Auflösungen der Textur. Aus diesem Grund kann ein schnelles Öffnen des Viewports dazu führen, dass Texturen zunächst unscharf erscheinen und sich die Qualität nach einigen Sekunden erhöht.

Weitere technische Informationen finden Sie unter:  [Virtuelle Strukturen mit geringer Dichte](https://silverspaceship.com/src/svt/) .

## Cachespeicherort

![](../assets/settings-temp.png)

Wenn nicht genügend Systemspeicher (Ram) zum Speichern des SVT-Caches verfügbar ist, wechselt Substance 3D Painter zur Computerfestplatte, um den Cache zu speichern.\
Der Speicherort dieses Cache befindet sich standardmäßig im Ordner Temporäre Dateien des Betriebssystems. Dieser Speicherort kann über die Haupteinstellungen der Anwendung geändert werden. Weitere Informationen finden Sie unter [Allgemeine Voreinstellungen](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/general-71008262.html) .

## Shader-Kompatibilität

Um die Vorteile der SVT voll ausschöpfen zu können, müssen Shader Texturen aus dem Sparse-System anfordern und lesen. Aus diesem Grund wurden vorherige Funktionen, die auf **vec2-Texturkoordinaten** und **Samplern** basieren, veraltet. Stattdessen stehen nun Hilfsfunktionen zur Verfügung, um die Sparse-Texturen zu verwenden.

So aktualisieren Sie Ihre Schattierungen :

* Für **Standard-Substance 3D Painter-Shader** : Befolgen Sie die schrittweise Anleitung auf der Seite [Aktualisieren eines Shaders](../interface/shader-settings/updating-a-shader.md).
* Für **Benutzerdefinierter Shader** : Sehen Sie sich die Fehlermeldung(en) im Protokoll sowie die [Shader-API](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/custom-shader-api-89686018.html)-Seite an.

>[!WARNING]
>
> Ältere Projekte zeigen möglicherweise weiße Blitze an, wenn ihre Shader nicht auf dem neuesten Stand sind. Weitere Informationen finden Sie auf dieser Seite : [Mesh-Blitz auf Weiß beim Verschieben der Kamera](../technical-support/technical-issues/rendering-issues/mesh-flash-to-white-when-moving-camera.md).
