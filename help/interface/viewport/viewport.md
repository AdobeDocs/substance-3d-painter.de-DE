---
helpx_url: 'https://helpx.adobe.com/substance-3d-painter/interface/viewport.html'
description: Lerne, wie du mit dem Viewport von Substance 3D Painter deine 3D-Modelle und Texturen während des Malens visualisieren kannst.
helpx_description: Painter > Interface > Viewport
title: Viewport
source-git-commit: 307c4f1121ae6841d68f8ea5dc597790e0d18a14
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 2%

---


# Viewport

![](../../assets/viewports-progress.jpg){width="600px"}

Im Viewport werden der 3D-Mesh und seine Texturen angezeigt. Hier ist es auch möglich, auf die 3D-Meshfläche zu malen.

## Überblick

Der Viewport ist in vier Teile unterteilt:

* **Kontextabhängige Symbolleiste**: Diese Symbolleiste befindet sich am oberen Rand des Viewports und bietet je nach dem aktuellen Kontext (Pinselparameter beim Malen zum Beispiel) Tastaturbefehle zu verschiedenen Eigenschaften.
* **3D-Ansicht**: Diese Ansicht zeigt das 3D-Gitter aus einem bestimmten Winkel, der durch eine Kamera definiert wird.
* **2D-Ansicht**: Diese Ansicht zeigt den entpack des 3D-Meshs für den aktuell ausgewählten [Textursatz](../texture-set/texture-set-list.md) in UV an.
* **Fortschrittsleiste**: Diese graugrüne Leiste am unteren Rand des Viewports wird angezeigt, wenn eine Berechnung ausgeführt wird (z. B. wenn das Engine Texturen generiert).

Weitere Informationen finden Sie auf den entsprechenden Seiten:

* [2D-Ansicht](2d-view.md)
* [3D-Ansicht](3d-view.md)
* [Kameramanagement](camera-management.md)

Die 3D- und 2D-Ansichten können angepasst werden, um zusätzliche oder andere Informationen über die [Anzeigeeinstellungen](../../interface/display-settings/display-settings.md) anzuzeigen.

## Viewport-Navigationssteuerelemente

Die Steuerelemente für das Navigieren im Viewport sind in den 2D- und 3D-Ansichten ähnlich.

<table>
  <tr>
    <th>Bewegungstyp</th>
    <th>Tastaturbefehl</th>
    <th>Beschreibung</th>
  </tr>
  <tr>
    <td>Kreisen/Drehen<br></td>
    <td><strong>Alt + Linksklick</strong></td>
    <td><ul><li>3D-Ansicht: Drehen Sie die Kamera um die Cursorposition.</li><li>2D-Ansicht: Drehen Sie den UV-Bereich um die Cursorposition.</li></ul></td>
  </tr>
  <tr>
    <td>Schwenken</td>
    <td><strong>Alt + Mitte-Klick</strong></td>
    <td>Bewegen Sie die Kamera nach oben, unten, links oder rechts.</td>
  </tr>
  <tr>
    <td>Zoom/Dolly</td>
    <td><strong>Alt + Rechtsklick</strong></td>
    <td>Zoomen Sie näher an den Mesh/die UVs heran oder weiter davon.</td>
  </tr>
</table>

>[!NOTE]
> Sowohl in der 2D- als auch in der 3D-Ansicht können Sie mit **Alt + Umschalt + Linksklick** orthogonale Winkel beim Umkreisen/Drehen einrasten werden.

## Layout ändern

Beim Standardlayout wird die 3D-Ansicht links und die 2D-Ansicht rechts platziert. In der **Kontextsymbolleiste** sind einige Parameter verfügbar, mit denen das Layout geändert werden kann:

<table>
  <tr>
    <th><em>Einstellung</em></th>
    <th><em>Beschreibung</em></th>
  </tr>
  <tr>
    <td><strong>Viewport Mode</strong><br><img src="../../assets/viewport-viewmode.png"/></td>
    <td>Diese Einstellungen steuern das Layout des Viewports:<br><ul><li><strong>3D/2D</strong> (Standard): sowohl die 3D- als auch die 2D-Ansicht im Viewport anzeigen</li><li><strong>Nur 3D</strong>: Maximieren Sie die 3D-Ansicht und blenden Sie die 2D-Ansicht aus.</li><li><strong>Nur 2D</strong>: Maximieren Sie die 2D-Ansicht und blenden Sie die 3D-Ansicht aus.</li><li><strong>3D/2D austauschen</strong>: die Reihenfolge austauschen, in der die Ansichten angezeigt werden. Wenn die 3D-Ansicht auf der linken Seite war, wird sie nach Auswahl dieser Aktion auf der rechten Seite angezeigt.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Perspektive Mode</strong><br><img src="../../assets/viewport-camera-projection.png"/></td>
    <td>Mit diesen Einstellungen wird gesteuert, wie das 3D-Mesh in der 3D-Ansicht angezeigt wird:<br><ul><li><strong>Perpektiven-Ansicht</strong> (Standard): zeigt den 3D-Mesh so an, wie er vom menschlichen Auge oder einer Kamera wahrgenommen würde.</li><li><strong>Orthografische Ansicht</strong>: zeigt den 3D-Mesh an, wenn jede Richtung dieselbe Länge misst.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Kamera-Drehmodus</strong><br><img src="../../assets/viewport-camera-axis.png"/></td>
    <td>Diese Einstellungen steuern, wie viele Achsen die Viewport-Kamera drehen kann.<br><ul><li><strong>Freie Drehung</strong>: Die Kamera wird auf der X-, Y- und Z-Achse gedreht.</li><li><strong>Eingeschränkte Drehung</strong> (Standard): Die Kamera wird nur auf der X- und Y-Achse gedreht (keine Rolle).</li></ul></td>
  </tr>
  <tr>
    <td><strong>Rendermodus</strong><br><img src="../../assets/viewport-rendering.png"/></td>
    <td>Wechseln Sie in den <a href="../../features/iray-renderer/iray-renderer.md">-Rendermodus </a>.</td>
  </tr>
</table>
