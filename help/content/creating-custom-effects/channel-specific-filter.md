---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/content/creating-custom-effects/channel-specific-filter.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie kanalspezifische Filtereffekte für Substance 3D Painter erstellen, um einzelne Texturkanäle zu verarbeiten.
helpx_creative_field: ""
helpx_description: Painter > Content > Creating custom effects > Channel specific filter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Kanalspezifischer Filter
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '455'
ht-degree: 0%

---


# Kanalspezifischer Filter

Ein Effekt kann für einen bestimmten Kanal spezifisch sein. Wenn Sie in diesem Fall einen bestimmten Kanal beeinflussen möchten, müssen Sie eine Eingabe UND eine Ausgabe erstellen, die diesen Kanal identifiziert. In der Regel sollte bei der Eingabe-/Ausgabestruktur immer eine 1:1-Regel eingehalten werden. Wenn Sie einen bestimmten Kanal eingeben möchten, müssen Sie denselben Kanal ausgeben.

Beispiel für einen Filter, der nur den Kanal **basecolor** betrifft:

![](../../assets/specific-filter-basecolor.png)

>[!NOTE]
>
> Es ist nicht möglich, generische Einstellungen (Eingabe-/Ausgabeknoten) und spezifische Kanäle (Grundfarbe/Grundfarbe) zu kombinieren.

## Alpha Component Management

Als RGBA gespeicherte Kanäle unterstützen Alpha (zum Beispiel Grundfarbe). Für diesen Kanal kann der Alpha-Eingang/Ausgang direkt in der Substance-Farbausgabe abgelegt werden. Die Substance-Engine unterstützt jedoch kein Alpha für Graustufenbilder: Es muss mithilfe einer sekundären Karte verwaltet werden. Um die Alphakomponente eines bestimmten Kanals in einem Substanzdiagramm abzurufen, erstellen Sie eine Graustufeneingabe mit dem Namen &quot;**Kanalname\_Alpha**&quot;. Beispiel: **Grundfarbe\_Alpha**, **Raueit\_Alpha** usw.\
Erstellen Sie zum Ausgeben dieser Alphakomponente einen Ausgabeknoten mit der gleichen Namenskonvention.

>[!NOTE]
>
> Die spezifische &quot;**\_Alpha**&quot;-Ausgabe pro Kanal funktioniert nicht mit regulären **Materialien**. Um einen Kanal mit einer Maske auszublenden, muss eine bestimmte Ausgabe mit der folgenden Namenskonvention erstellt werden:
> 
> * Kennung: **Channels\_Alpha**
> * Verwendung : **Channels\_Alpha**

## Liste der Ein-/Ausgabenutzungen und Kennungen

>[!NOTE]
>
> Es ist möglich, in einem Eingabeknoten entweder **usage** oder **identifier** zu verwenden (die Verwendung hat die Priorität).

| Kanalname | Nutzung | Bezeichner-/Bezeichner-Alpha |
| --- | --- | --- |
| *Umgebungs-Verdeckung* | **ambientOcclusion** | **ambientOcclusion / ambientOcclusion\_Alpha** |
| *Anisotropie Winkel* | **Anisotropiewinkel** | **AnisotropyAngle/AnisotropyAngle\_Alpha** |
| *Anisotropie* | **Anisotropiestufe** | **AnisotropyLevel/AnisotropyLevel\_Alpha** |
| *Grundfarbe* | **Grundfarbe** | **baseColor / baseColor\_Alpha** |
| *Füllmaske* | **Mischmaske** | **Mischmaske/Mischmaske\_Alpha** |
| *Diffus* | **diffuse** | **diffuse / diffuse\_Alpha** |
| *Versatz* | **Versatz** | **Versatz/Versatz\_Alpha** |
| *Ausstrahlend* | **emissiv** | **emittierend/emissiv\_Alpha** |
| *Glossarität* | **Glanz** | **Glanz/Glanz\_Alpha** |
| *Height* | **Height** | **Height/Height\_Alpha** |
| *IOR* | **ior** | **ior / ior\_Alpha** |
| *Metallisch* | **metallisch** | **metallisch / metallisch\_Alpha** |
| *Normal* | **normal** | **normal / normal\_Alpha** |
| *Deckkraft* | **Deckkraft** | **Deckkraft/Deckkraft\_Alpha** |
| *Spiegelung* | **Spiegelung** | **Spiegelung/Spiegelung\_Alpha** |
| *Raueit* | **Raueit** | **Raueit/Raueit\_Alpha** |
| *Streuung* | **Streuung** | **Streuung/Streuung\_Alpha** |
| *Specular* | **Specular** | **Specular/Specular\_Alpha** |
| *Specular level* | **Glanzstufe** | **specularLevel / specularLevel\_Alpha** |
| *Transmissiv* | **transmissiv** | **transmissiv/transmissiv\_Alpha** |
| *Benutzer 0* | **Benutzer0** | **user0 / user0\_Alpha** |
| *Benutzer 1* | **Benutzer1** | **Benutzer1 / Benutzer1\_Alpha** |
| *Benutzer 2* | **Benutzer2** | **Benutzer2 / Benutzer2\_Alpha** |
| *Benutzer 3* | **Benutzer3** | **Benutzer3 / Benutzer3\_Alpha** |
| *Benutzer 4* | **Benutzer4** | **Benutzer4 / Benutzer4\_Alpha** |
| *Benutzer 5* | **Benutzer5** | **Benutzer5 / Benutzer5\_Alpha** |
| *Benutzer 6* | **Benutzer6** | **Benutzer6 / Benutzer6\_Alpha** |
| *Benutzer 7* | **Benutzer7** | **Benutzer7 / Benutzer7\_Alpha** |

## Beispiele

![](../../assets/single-channel.png){width="650px"}

In diesem Beispiel wird der Alphakanal der Grundfarbe über einen Graustufenknoten extrahiert, um den Kanal **Raueit** zu überschreiben.

![](../../assets/mix-channel.png){width="650px"}

In diesem Beispiel wird der **Raueit**-Kanal mit der **Grundfarbe** multipliziert.
