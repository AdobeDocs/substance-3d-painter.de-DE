---
title: Einen Blendenfleck erzeugen
description: ''
helpx_description: "Substance 3D Painter"
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/post-processing/lens-flare.html"
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '262'
ht-degree: 7%

---


# Blendenflecke

![](../../assets/v12_post_flare.jpg)

Simuliert optische Artefakte, die entstehen, wenn helle Lichtquellen mit Kameraobjektiven interagieren, und erzeugt Halos, Streifen und Geisterreflexionen.

| <b>Parameter</b> | <b>Beschreibung</b> |
| --- | --- |
| <b>Auflösung</b> | Legt die interne Renderauflösung für den Blendenflecken-Effekt fest. Höhere Werte führen zu schärferen Streifen, können aber auch die Leistung beeinträchtigen. |
| <b>Kamera</b> | Wählt das Kameramodell aus, mit dem der Blendenfleck simuliert wird. Mögliche Werte sind:<ul data-preserve-html="true"> <li data-preserve-html="true"><b>Panoramaobjektiv</b> (kürzere Brennweite) </li> <li data-preserve-html="true"><b>Teleobjektiv</b> (längere Brennweite).</li> </ul> |
| <b>Betrag</b> | Steuert die Gesamtintensität des Blendenflecken-Effekts. Der Wert kann über 1,0 hinausgehen, um die Intensität zu erhöhen. |
| <b>Schwellenwert</b> | Bestimmt die minimale Luminanz des Bildes, die erforderlich ist, um einen Blendenfleck zu erzeugen. Niedrigere Werte führen dazu, dass mehr Bereiche Blendenflecken erzeugen, während höhere Werte den Effekt auf sehr helle Lichtquellen beschränken. |
| <b>Blendenskala</b> | Legt die Größe der Blendenform fest, die für die Berechnung des Blendenflecks verwendet wird. Dies wirkt sich auf die Gesamtgröße der Blendenelemente aus. |
| <b>Beschichtungsdicke</b> | Simuliert die Antireflexionsbeschichtung auf Linsenelementen. Die Thickness der Beschichtung wirkt sich darauf aus, wie leichte Streuungen aussehen, und ändert so die Farbe der Blendenflecken. |
| <b>IOR-Beschichtung</b> | Simuliert den Brechungsindex der Linse: wie das Licht seine Thickness durchdringt. Niedrigere Werte führen zu konzentrierteren Geistern. |
| <b>Verdeckung skalieren</b> | Legt die Größe des betroffenen mittleren Bereichs fest. |
| <b>Verdeckung Smoothness</b> | Steuert, wie allmählich der Blendenfleck verblasst. Höhere Werte erzeugen weichere Übergänge. |
| <b>Eindeutige Geister</b> | Definiert, wie variiert die Blendenformen sind. Höhere Werte können sich erheblich auf die Leistung auswirken. |
| <b>Ghost-Positionsskala</b> | Steuert die Ausbreitung und die Größe der Blendenfleckphantome. |
| <b>Blendenstruktur</b> | Definiert die Form der Blendenöffnung, die zum Erzeugen des Blendenflecks verwendet wird. Die Textur steuert die Beugung und die Geisterformen. |
