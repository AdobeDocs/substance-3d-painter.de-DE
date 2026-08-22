---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/getting-started/system-requirements.html"
breadcrumb-title: ''
description: Prüfen Sie die Systemanforderungen für Substance 3D Painter , um sicherzustellen, dass Ihr Computer die Hardware- und Softwarespezifikationen erfüllt.
helpx_creative_field: ""
helpx_description: Painter > Getting Started > System requirements
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Systemanforderungen
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '779'
ht-degree: 1%

---


# Unterstützte Systeme

Im Folgenden finden Sie eine Liste der von der Anwendung unterstützten Hardware und Systeme:

## Windows

|  | Minimum | Empfohlen | Optimal |
| --- | --- | --- | --- |
| <b>Betriebssystem</b> | Windows 11 64-Bit Version 23H2 | Windows 11 64-Bit Version 24H1 | Windows 11 64-Bit Version 24H2 |
| <b>CPU</b> | Intel Core i5 AMD Ryzen 5 | Intel Core i7 AMD Ryzen 7 | Intel Core i9 AMD Ryzen 9 |
| <b>GPU</b> | NVIDIA GeForce RTX 2060 Super NVIDIA Quadro RTX 4000 AMD Radeon RX 5700 XT AMD Radeon Pro W5700 | NVIDIA GeForce RTX 3080 NVIDIA Quadro RTX A4000 AMD Radeon RX 6800 XT AMD Radeon Pro W7700 | NVIDIA GeForce RTX 4090 NVIDIA Quadro RTX 5000 ADA Generation AMD Radeon RX 7900 XTX AMD Radeon Pro W7800 |
| <b>VRAM</b> | 8 GB | 16 GB | 24 GB |
| <b>RAM</b> | 16 GB | 32 GB | 64 GB |
| <b>Speicher</b> | SSD mit 30 GB verfügbarem Speicherplatz | SSD mit 50 GB verfügbarem Speicherplatz | SSD mit 70 GB verfügbarem Speicherplatz |

### MacOS

|  | Minimum | Empfohlen | Optimal |
| --- | --- | --- | --- |
| <b>Betriebssystem</b> | macOS 12 Monterey | macOS 13 Ventura | macOS 14 Sonoma |
| <b>CPU</b> | Apple M1 | Apple M2 Pro | Apple M4 Pro |
| <b>GPU</b> | Apple M1 | Apple M2 Pro | Apple M4 Pro |
| <b>RAM</b> | 16 GB | 32 GB | 64 GB |
| <b>Speicher</b> | SSD mit 30 GB verfügbarem Speicherplatz | SSD mit 50 GB verfügbarem Speicherplatz | SSD mit 70 GB verfügbarem Speicherplatz |

### Linux

| Unternehmen | dämpfen |
| --- | --- |
| RHEL 8</br>RHEL 9 | Ubuntu 22,04 |

## Allgemeine Empfehlungen

Um eine gute Leistung bei der Verwendung des UV-Kachel-Arbeitsablaufs zu erzielen, empfehlen wir die Verwendung von:

* 32 GB RAM
* GPU mit 8 GB VRAM
* SSD zum Speichern sowohl des Projekt- als auch des Anwendungscaches.

Sonstiges:

* Viele Substance-Apps sind für RHEL8/9-Kompatibilität auf OpenSSL 1.1.1 angewiesen. Bei Systemen mit neueren OpenSSL-Versionen muss der Kunde diese manuell bereitstellen.
* Für die Arbeit unter angenehmen Bedingungen empfehlen wir einen Monitor mit einer vertikalen Auflösung größer als 1000 Pixel und breiter als 1280 Pixel.
* Für den Export mit <b>8K</b> (8192\*8192 Pixel) ist eine GPU mit <b> mehr als </b> 2 GB VRam erforderlich.
* Nur die Versionen 2019.x und höher wurden notariell beglaubigt, um auf MacOS 10.15 (Catalina) ausgeführt zu werden.
* Informationen zum Verwenden der Software über RDP (Remote Desktop) finden Sie auf der dedizierten [Dokumentationsseite](../pipeline-and-integration/configuration/remote-desktop.md).
* Absturz auf Ryzen CPU beim Backen, kann durch Aktualisierung des BIOS behoben werden.

## Nicht unterstützte Konfigurationen

<b>Windows</b>

* Virtuelle Computer werden nicht unterstützt.
* Windows Server wird nicht unterstützt.

<b>Mac</b>

* Es werden nur offizielle Apple-Konfigurationen unterstützt.
* eGPUs werden derzeit nicht unterstützt und haben möglicherweise Stabilitätsprobleme.

<b>Linux</b>

* Mesa-Treiber unter Linux werden nicht unterstützt.

<b>Beliebige Plattform</b>

* Integrierte GPUs werden auf x86-64-CPUs (Intel, AMD) nicht unterstützt.

## Mindestversionen von GPU-Treibern

Im Folgenden finden Sie eine Liste der erforderlichen Mindestversionen von GPU-Treibern, damit die Anwendung problemlos ausgeführt werden kann. Diese Liste kann sich mit der Veröffentlichung neuer Versionen ändern.

Informationen zum Herunterladen neuer Treiber finden Sie unter: [GPU hat veraltete Treiber](../technical-support/technical-issues/gpu-issues/gpu-has-outdated-drivers.md).

| Betriebssystem | NVIDIA | AMD | Intel |
| --- | --- | --- | --- |
| <b>Windows</b> | GeForce 442,50 Quadro 442,50 | Radeon 19.7.1 Radeon Pro/FirePro 18.Q4 | 15.33 |
| <b>Linux</b> | 535.171.04 oder höher | Radeon 22,40,6 | Nicht unterstützt |

>[!NOTE]
>
> Unter **Mac OS** wird der GPU-Treiber vom Betriebssystem selbst bereitgestellt. Aktualisieren Sie auf die neueste Version Ihres Betriebssystems, um auf den neuesten Treiber zuzugreifen.

### Kompatibilitätsprobleme mit Treibern

Eine detaillierte Liste der Probleme mit GPU-Treibern pro Konstruktor finden Sie auf der [Seite zur dedizierten Dokumentation](../technical-support/technical-issues/gpu-issues/gpu-drivers-compatibility.md).

## GPU-Raytracing zum Backen

Um GPU-Raytracing über Optix oder DXR zu aktivieren, müssen die oben empfohlenen Mindesttreiber installiert sein.

<b>DXR</b> erfordert ebenfalls die folgende Mindestkonfiguration:

* <b>Windows 10</b> Version 1809. Weitere Informationen finden Sie auf [dieser Seite](https://experienceleague.adobe.com/de/docs/substance-3d/bakers/features/gpu-raytracing).
* <b> GPU mit Pascal-Architektur</b> (Nvidia GeForce 10XX)

>[!TIP]
>
> GPU-Raytracing läuft optimal auf dedizierter Raytracing-Hardware wie NVIDIA GeForce RTX oder NVIDIA Quadro RTX GPUs.

## Unterstützte Grafiktabletts

Im Folgenden finden Sie eine Liste der kompatiblen Grafiktabletts, die mit der Substance 3D Painter-Version <b>7.4.2</b> getestet wurden:

+++Wacom
<b>Modelle:</b> Intuos Pro (M-Größe), Intuos (S-Größe)


| Betriebssystem | Treiberversion |
| --- | --- |
| Windows | 6.3.45-1 |
| macOS | 6.3.45-3 |


+++

+++XPen
<b>Modell:</b> Deco 01


| Betriebssystem | Treiberversion |
| --- | --- |
| Windows | XP-PENWin\_3.2.2.211027 |
| macOS | XP-PENMac\_3.2.3\_211203 |
| Linux | XP-PEN-pentablet-3.2.1.211019-1 |


+++

+++Huion
<b>Modell:</b> Q11K


| Betriebssystem | Treiberversion |
| --- | --- |
| Windows | XP-PENWin\_3.2.2.211027 |
| macOS | XP-PENMac\_3.2.3\_211203 |


+++

+++Xencelabs
<b>Modell:</b> Stifttablettmedium


| Betriebssystem | Treiberversion |
| --- | --- |
| Windows | XencelabsWin\_1.2.1-14 |
| macOS | XencelabsMac\_1.2.1-18 |
| Linux | XencelabsLinux\_1.1.0-2 |


+++

## Unterstützte 3Dconnection SpaceMouse-Modelle

Im Folgenden finden Sie eine Liste der kompatiblen Treiberversionen für die [3Dconnection Space Mouse](https://3dconnection.com/us/spacemouse/), die mit der Substance 3D Painter-Version <b>8.1.</b> getestet wurden.

Die Treiberversionen gelten für die Modelle <b>Compact</b>, <b>Pro</b> und <b>Enterprise</b>.

| Betriebssystem | Treiberversion |
| --- | --- |
| Windows | 10.8.6.3431 |
| macOS | 10.7.2.3454 |

## Sprachen

Die Software-Benutzeroberfläche ist in den folgenden Sprachen verfügbar:

* Englisch (Vereinigte Staaten)
* Deutsch
* Spanisch
* Français
* Italienisch
* 日本語
* Koreanisch
* Portugiesisch (Brasilien)
* Chinesisch (vereinfacht)
