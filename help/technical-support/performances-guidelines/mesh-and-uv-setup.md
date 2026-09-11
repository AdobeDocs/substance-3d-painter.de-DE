---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/technical-support/performances-guidelines/mesh-and-uv-setup.html"
breadcrumb-title: ''
description: Informieren Sie sich über Best Practices für die Einrichtung von Meshs und UV in Substance 3D Painter, um die Performance und die Qualität der Textur zu optimieren.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Performances guidelines > Mesh and UV setup
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Mesh- und UV-Setup
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 0%

---


# Mesh- und UV-Setup

Die Vorbereitung deines Meshs für Painter dauert nur wenige Minuten und beschleunigt und vereinfacht den Texturierungsprozess.

+++Modelle mit hoher Polyzahl
Es gibt keine spezielle Benchmark für Polycount, die Painter verarbeiten kann, da sie weitgehend von Maschinenspezifikationen, der Zuweisung von Textursätzen und den Eigenschaften von Ebenenstapeln abhängt. Bei Berücksichtigung der Ebenenstapel-Optimierungen sollten jedoch weniger als 10 Millionen Polys ausreichend verrechnet werden.

+++

+++Modelle mit niedrigem Polyanzahlwert
Es gibt so etwas wie zu wenig Poly. Das liegt daran, dass das Engine &quot;Textur&quot; die Polygone verwendet, um zu wissen, welcher Teil des Meshs gerendert werden soll, um die Pinselstriche zu berechnen. Mesh mit einer sehr niedrigen Polycount-Rate können auch mit winzigen Pinselstrichen vollständig neu gerendert werden, was die GPU unnötig überarbeiten kann.

Wenn Sie beispielsweise eine einzelne Quad-Ebene texturieren, ist es besser, den Mesh zu unterteilen, insbesondere beim Handmalen mit vielen Strichen, da die Informationen über mehr Scheitelpunkt verteilt sind.

+++

+++Dividieren von Texturen über mehrere Textursatz hinweg
Es ist am besten, größere Mesh mit komplizierteren Material-Zuweisungen in mehrere Textursatz aufzuteilen. Mithilfe von Textursätzen können Sie verschiedene Einstellungen pro Textursatz festlegen, z. B. Auflösung und Shader-Eigenschaften. Wenn beispielsweise nur ein Teil des Meshs translucency oder SSS verwendet, empfiehlt es sich, diesem Teil einen anderen Textursatz und eine andere Shader-Instanz zuzuweisen. Auf diese Weise müssen diese komplexeren Eigenschaften nicht berechnet werden, wenn sie nicht verwendet werden.

+++

+++UV-Inseln dicht beieinander halten.
Versuche, UV-Inseln, die Nachbarn im 3D-Raum sind, nah beieinander zu halten. Dies gilt sowohl für das UDIM-Layout als auch für das klassische UV-Space-Layout. Wenn sie über gemeinsame Malen-Konturen oder Texturierung verfügen, ist es einfacher, sie zu berechnen, wenn sie sich im selben Bereich des UV-Bereichs befinden, als wenn sie sich an gegenüberliegenden Enden befinden.

Das Engine &quot;Textur&quot; teilt eine Textur in kleinere Blöcke auf, um die Berechnung zu beschleunigen. Dies bedeutet, dass mit jeder Kontur nur die zu ändernden Blöcke aktualisiert werden, anstatt die gesamte Textur mit jeder Kontur zu aktualisieren. Durch die Nähe benachbarter UV-Inseln wird die Anzahl der Blöcke minimiert, die von einem einzigen Strich betroffen sind.

+++

+++Vermeiden Sie zu viele Objekte
Die Leistung sollte auch beim Importieren eines Meshs mit weniger als 8000 Unterobjekten komfortabel sein. Wenn Sie diesen Grenzwert überschreiten, kann sich dies auf die Viewport- und Malleistung auswirken. Wenn dieser Grenzwert erreicht wird, wird empfohlen, Objekte zusammenzuführen, um den Rendering-Overhead zu reduzieren.

+++
