---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/technical-support/performances-guidelines/mesh-and-uv-setup.html"
breadcrumb-title: ''
description: Lernen Sie Best Practices für die Einrichtung von Gittern und UVs in Substance 3D Painter kennen, um die Leistung und die Texturqualität zu optimieren.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Performances guidelines > Mesh and UV setup
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Gitter- und UV-Einrichtung
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 0%

---


# Gitter- und UV-Einrichtung

Mit ein paar Minuten Vorbereitung deines Gitters für Painter kannst du den Texturierungsprozess schneller und einfacher gestalten.

+++Modelle mit hoher Polyzahl
Es gibt keine spezielle Benchmark für Polycount, die Painter verarbeiten kann, da sie weitgehend von Maschinenspezifikationen, Textursatz-Zuweisung und Ebenenstapeleigenschaften abhängt. Bei Berücksichtigung der Ebenenstapeloptimierungen sollten jedoch weniger als 10 Millionen Polys problemlos verarbeitet werden.

+++

+++Modelle mit niedrigem Polyanzahlwert
Es gibt so etwas wie zu wenig Poly. Das liegt daran, dass die Textur-Engine die Polygone verwendet, um zu wissen, welcher Teil des Gitters gerendert werden soll, um die Pinselstriche zu berechnen. Gitter mit einer sehr niedrigen Polycount-Zahl können auch mit winzigen Pinselstrichen vollständig neu gerendert werden, was die GPU unnötig überarbeiten kann.

Wenn Sie beispielsweise eine einzelne Quad-Ebene texturieren, ist es besser, das Gitter zu unterteilen, insbesondere beim Handmalen mit vielen Strichen, da die Informationen über mehr Scheitelpunkte verteilt sind.

+++

+++Aufteilen von Texturen auf mehrere Texturensätze
Es ist am besten, größere Gitter mit komplexeren Materialzuweisungen in mehrere Textursets aufzuteilen. Mit Textursätzen können Sie verschiedene Einstellungen pro Textursatz zuweisen, z. B. Auflösung und Shader-Eigenschaften. Wenn beispielsweise nur ein Teil des Gitters Lichtdurchlässigkeit oder SSS verwendet, empfiehlt es sich, diesem Teil einen anderen Textursatz und eine andere Shader-Instanz zuzuweisen. Auf diese Weise müssen diese komplexeren Eigenschaften nicht berechnet werden, wenn sie nicht verwendet werden.

+++

+++UV-Inseln dicht beieinander halten.
Versuche, UV-Inseln, die Nachbarn im 3D-Raum sind, nah beieinander zu halten. Dies gilt sowohl für das UDIM-Layout als auch für das klassische UV-Raum-Layout. Wenn sie über gemeinsame Malstriche oder Texturierung verfügen, ist es einfacher, sie zu berechnen, wenn sie sich im selben Bereich des UV-Raums befinden, als wenn sie sich an gegenüberliegenden Enden befinden.

Die Textur-Engine teilt eine Textur in kleinere Blöcke auf, um die Berechnung zu beschleunigen. Dies bedeutet, dass mit jeder Kontur nur die zu ändernden Blöcke aktualisiert werden, anstatt die gesamte Textur mit jeder Kontur zu aktualisieren. Durch die Nähe benachbarter UV-Inseln wird die Anzahl der Blöcke minimiert, die von einem einzigen Strich betroffen sind.

+++

+++Vermeiden Sie zu viele Objekte
Die Leistung sollte beim Importieren eines Gitters mit weniger als 8000 Unterobjekten komfortabel bleiben. Wenn Sie diesen Grenzwert überschreiten, kann sich dies auf den Viewport und die Malleistung auswirken. Wenn dieser Grenzwert erreicht wird, wird empfohlen, Objekte zusammenzuführen, um den Rendering-Overhead zu reduzieren.

+++
