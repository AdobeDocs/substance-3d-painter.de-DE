---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/technical-support/workflow-issues/project-issues/projects-are-really-big.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie die Dateigröße von Substance 3D Painter-Projekten verringern können, um die Performance zu optimieren und die Speicheranforderungen zu optimieren.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > Project Issues > Projects are really big
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Projekte sind wirklich groß
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '883'
ht-degree: 0%

---


# Projekte sind wirklich groß

Substance 3D Painter-Projekte können sehr groß sein und viel Speicherplatz belegen. Diese Seite erklärt, warum und wie Sie sie abschwächen können.

## Welche Art von Ressourcen werden in einem Projekt gespeichert?

Jedes Element oder jede Ressource, die während der Texturierung verwendet wird, wird in der Projektdatei gespeichert. Dazu gehören:

* **Quell-Mesh** (nicht die Originaldatei, sondern eine verarbeitete Datei)
* **Baking geführt Mesh-Map**
* **Materials** (wie Substance von Materials)
* **Bitmaps** oder andere Ressourcen, die von Ebenen/Voreinstellungen/Pinselstrichen verwendet werden.

Die hochpolaren Mesh sind nicht im Projekt enthalten. Sie sind nur verknüpft.

## Warum werden in einem Projekt so viele Ressourcen gespeichert?

Durch das Speichern aller verwendeten Ressourcen wird ein Projekt völlig autonom und kann leicht von einem Computer zum anderen verschoben werden, ohne dass es unterbrochen wird. Der Hauptnachteil ist der potenziell große Dateispeicherplatz auf der Festplatte.

Die Entscheidung, alles in die Projektdatei einzubetten, beruht darauf, dass alles zerstörungsfrei ist. Es bedeutet, dass das Projekt sich selbst &quot;neu aufbaut&quot;, wenn es erneut geöffnet wird. Wenn ein einzelner Pinsel oder ein einzelnes Material im Regal fehlt, kann das Projekt unterbrochen und nicht ordnungsgemäß regeneriert werden. Durch Speichern eines Duplikats der Ressource wird sichergestellt, dass das Projekt beim Speichern wiederhergestellt werden kann.

## Gibt es eine Möglichkeit, die Größe eines Projekts zu reduzieren?

Es gibt mehrere Möglichkeiten, die Größe eines Projekts zu reduzieren:

### Nicht genutzte Ressourcen bereinigen

Wenn Sie viele Ressourcen in einem Projekt verwenden, werden sie von Substance 3D Painter kopiert. Zum Beispiel, wenn Sie ein Alpha zum Malen verwendet haben. Wenn Sie die Ebene später löschen, als das Alpha gemalt wurde, entfernt Substance 3D Painter die Ressource nicht automatisch.

Verwenden Sie zum Entfernen nicht verwendeter Ressourcen die Aktion **Bereinigen** im Menü [Datei](https://substance3d.adobe.com/display/DRAFTPAINTER/File+menu) . Speichern Sie dann das Projekt (dies löst das eigentliche Entfernen der Ressource aus).

Ressourcen, die noch in einem Projekt verwendet werden, können nicht entfernt werden. Dies bedeutet, dass deaktivierte Textursatz immer noch auf Ressourcen verweisen und verhindern, dass sie gelöscht werden. Um dies zu vermeiden, entfernen Sie deaktivierte Textursatz im [Fenster für die Neuzuweisung von Textursätzen](../../../interface/texture-set/texture-set-reassignment.md).

### Komprimieren Sie den Textursatz

Wenn ein Projekt gespeichert wird, wird das Endergebnis des Ebenenstapels eines Textursatzes im Projekt gespeichert. Dies ermöglicht es, eine Vorschau im Viewport beizubehalten, wenn das Projekt erneut geöffnet wird, ohne den Textursatz neu berechnen zu müssen. Je größer die Auflösung des Textursatzes auch ist, desto größer ist der Vorschau-Cache.

Um den Cache-Platzbedarf zu reduzieren, ändern Sie einfach die Auflösung in einen niedrigeren Wert wie zum Beispiel 512. Da Substance 3D Painter nicht destruktiv ist, kann diese Auflösung später noch einmal geändert werden, ohne dass die Qualität beeinträchtigt wird.

### Projekt komprimieren

Durch inkrementelles Speichern eines Projekts (über STRG+S) kann eine Menge das Projektdateiarchiv fragmentieren. Obwohl dies kein kritisches Problem ist, kann dies zu leerem Speicherplatz in der Projektdatei führen, wodurch die Größe erhöht werden kann.

Verwenden Sie die Funktion &quot;Speichern und komprimieren&quot; im [Dateimenü](../../../interface/main-menu/file-menu.md), um das Projekt erneut zu speichern und verlorenen Leerraum zu entfernen. Diese Speicheraktion ist länger als eine normale Speicheraktion, kann jedoch den Dateispeicherplatz erheblich reduzieren.

### Baking geführt Größe der Mesh-Map reduzieren

Im Allgemeinen ist der größte Übeltäter und Grund, warum ein Projekt so viel Speicherplatz auf der Festplatte beansprucht, dass die Baking geführt Mesh-Map selbst viele und große sind.

Um die Größe der Mesh-Map zu reduzieren, sind dies einige Dinge, die getan werden können:

* *Geringere Auflösung für das Baking verwenden.*\
  Auch wenn der Normalen-Map von Vorteil sein kann, wenn er in 4K Baking geführt wird, ist dies bei der Positionskarte, die normalerweise nur aus farbigen Farbverläufen besteht, möglicherweise nicht der Fall. Baking in zwei Durchläufen mit zwei verschiedenen Auflösungen, um unterschiedliche Dateigrößen zu mischen.
* *Exportieren Sie die Texturen, und reduzieren Sie den Platzbedarf manuell.*\
  Standardmäßig werden in Substance 3D Painter alle Texturen als RGBA-Bilder in 16 Bit Baking geführt, einschließlich der Graustufen-Baker wie der Ambient occlusion.

  So reduzieren Sie die Baking-Texturen für den Druck:
  1. Deaktivieren Sie die Einstellung &quot;Diffusion anwenden&quot; im Fenster &quot;Baker&quot;.
  1. Setze die &quot;Ausdehnung mit&quot; auf einen angemessenen Wert (z. B. 32 Pixel bei einer Auflösung von 2048).
  1. Alle Texturen werden mit derselben Auflösung Baking geführt
  1. Exportieren Sie die Baking geführt Texturen mit der Exportvorgabe &quot;Mesh-Map&quot; als 16-Bit-PNG mit der Auffüllung auf &quot;Keine Auffüllung (Passthrough)&quot;
  1. Öffnen Sie jede Landkarte in einem Fotobearbeitungsprogramm oder in Substance 3D Designer
  1. Reduzieren Sie die Auflösung für die Texturen, für die sie geeignet scheint. Stellen Sie sicher, dass Ambient occlusion, Krümmung und Thickness von Farbe auf Graustufen umgestellt werden.
  1. Speichern Sie die neuen Textur-Versionen als 16-Bit-PNG.
  1. Importieren Sie die Texturen erneut und ersetzen Sie sie über den ursprünglichen Baking-Texturen in den Textursatz-Einstellungen.
  1. Verwenden Sie die Aktion Bereinigen im Menü Datei , um die alten Mesh-Map zu entfernen.
  1. Verwenden Sie die Aktion &quot;Speichern und komprimieren&quot; im Menü &quot;Datei&quot;, um die Projektdatei zu komprimieren.\
     Nach all diesen Schritten sollte der Projektbedarf deutlich reduziert werden.

Es ist wichtig, dass die Mesh-Map mindestens 16-Bit-Texturen beibehalten. 8-Bit-Texturen können zwar eine kleinere Stellfläche haben, aber Artefakte in Intelligenten Materialien und Maskengeneratoren verursachen. Wir empfehlen PNG, da es ein verlustfreies Komprimierungsformat ist. Das bedeutet, dass die Texturen weiterhin komprimiert werden, ohne dass Artefakte entstehen, und auch 16 Bit unterstützt werden.
