---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/performances-guidelines/layer-management.html"
breadcrumb-title: ''
description: Lernen Sie Best Practices für die Ebenenverwaltung in Substance 3D Painter kennen, mit denen Sie die Leistung optimieren und strukturierte Projekte beibehalten können.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Performances guidelines > Layer management
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Ebenenmanagement
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '677'
ht-degree: 0%

---


# Ebenenmanagement

Painter berechnet den Ebenenstapel von unten nach oben. Wenn Sie also Änderungen an der obersten Ebene auf dem Stapel vornehmen, muss Painter nur die Änderungen dieser Ebene berechnen. Wenn Sie jedoch eine Ebene am unteren Rand des Stapels ändern, muss Painter alle Ebenen über dieser Ebene berechnen, um das Endergebnis zu berechnen.

Es gibt verschiedene Optionen, mit denen Sie die Leistungskosten für Änderungen an Ebenen auf einer niedrigeren Ebene im Stapel senken können:

+++Verwenden von Geometrie-Masken
Geometriemasken sind das beste Optimierungswerkzeug. Wann immer Sie einen Teil Ihres Meshs zum Arbeiten isolieren können, tun Sie dies, entweder durch Maskieren von Ebenen oder Ordnern. Geometriemasken arbeiten, indem sie entweder durch UDIM oder durch einen Mesh-Teil isoliert werden, sodass Bereiche, die nicht in der Maske enthalten sind, nicht verarbeitet werden, was die Leistung verbessert. Außerdem kannst du diese Bereiche im Viewport isolieren, um die Texturierung zu vereinfachen.

Sie können [mehr über Geometriemasken in diesem Tutorial erfahren](https://www.youtube.com/watch?v=TGASuIGSUns) oder indem Sie [auf die Dokumentation verweisen](../../interface/layer-stack/geometry-mask.md).

+++

+++Ebenen ausblenden
Um Verzögerungen zu vermeiden, wenn Sie Änderungen auf einer niedrigeren Ebene im Ebenenstapel vornehmen, können Sie Ebenen über der bearbeiteten Ebene ausblenden, bis Sie mit den Korrekturen fertig sind. Painter verarbeitet keine ausgeblendeten Ebenen. Wenn also alle Ebenen über Ihrer Ebene ausgeblendet sind, ist es so, als ob Sie die oberste Ebene im Stapel bearbeiten. Auf diese Weise werden die Ebenen darüber nur einmal berechnet, wenn Sie sie einblenden, anstatt nach jeder Änderung, die Sie vornehmen.

+++

+++Ebenen deaktivieren
Wie beim Ausblenden von Ebenen verhindert auch die Deaktivierung des Mischmodus, dass Ebenen berechnet werden. Es kann hilfreich sein, Ebenen mit geringer Auswirkung auf den Mischmodus &quot;Deaktivieren&quot; festzulegen, während Bereiche geändert werden, in denen sie nicht wichtig sind.

+++

+++Ordner verwenden
Versuchen Sie, Ebenen nach Möglichkeit zu gruppieren, da sich Ordner wie ein unsichtbarer Zwischenspeicherpunkt verhalten. Wenn Sie Änderungen unterhalb oder oberhalb eines bestimmten Ordners vornehmen, werden die Ebenen innerhalb des Ordners nicht alle einzeln neu berechnet, sondern ihre Gruppenergebnisse werden neu berechnet.

+++

+++Die Verwendung von Filtern am oberen Rand des Ebenenstapels beschränken
Filter können teuer sein. Wenn Sie einen Filter in der Nähe des oberen Rands des Ebenenstapels verwenden müssen, können Sie Geometriemasken verwenden, um die Leistungskosten zu senken.

+++

+++Verwendung des Mischmodus &quot;Passthrough&quot; beschränken
Passthrough wird häufig mit Filtern oder Pinselstrichebenen verwendet. Dieser Mischmodus ist sehr kostspielig, da er auf alle darunterliegenden Ebenen angewendet wird und deren Ergebnis transformieren, anstatt das Ergebnis wie bei einem normalen Mischmodus zu überschreiben. Versuchen Sie bei der Verwendung von Passthrough, sie mit Geometriemasken und Ordnern zu kombinieren, um die Auswirkungen auf die Leistung zu minimieren.

+++

+++Tiefe der Projektion klein halten
Halten Sie den Wert für die Tiefe der Projektion mit allen Werkzeugen oder Modi, die eine Einstellung für die Tiefe der Projektion haben (Verformen, planar, Pfad usw.), so klein wie möglich. Je weiter sich die Tiefe der Projektion erstreckt, desto weniger performant ist sie.

+++

+++Sei vorsichtig bei Pinseln mit Dynamischen Pinselstrichen
Pinsel und Werkzeuge mit einem orangefarbenen Tag haben einen dynamischen Parameter. Dieser dynamische Parameter kann auf &quot;Unlimited&quot; gesetzt werden, was bedeutet, dass jeder Stempel in einer Kontur eindeutig ist. Dies kann sich erheblich auf die Leistung auswirken, wenn Hunderte oder Tausende von Pinselstrichen verwendet werden. In den meisten Fällen ist es schwierig, den Unterschied nach 16-32 Variationen zu erkennen, sodass es im Allgemeinen unwahrscheinlich ist, dass eine Überquerung einen großen visuellen Einfluss hat.

[Weitere Informationen zu Dynamischen Pinselstrichen finden Sie in der Dokumentation.](../../painting/dynamic-strokes/dynamic-strokes.md)

+++

+++Arbeiten mit einer niedrigeren Textur
Die Reduzierung der Dokumentauflösung ist der schnellste Weg zur Leistungssteigerung. Eine Verdoppelung der Auflösung bedeutet eine 4-mal größere Karte, sodass eine Erhöhung von 1 auf 2 K eine bis zu 4-mal höhere Performance-Kosten bedeutet. Daher ist es oft nützlich, so lange wie möglich mit einer niedrigeren Auflösung zu arbeiten.

+++

+++Aufkleber auf Planare Projektion einstellen
Der Standard-Aufklebermodus ist &quot;Verformen&quot;. Wenn Sie den Aufkleber jedoch nicht durch Verschieben der Ankerpunkte verformen, ist das Umschalten in den Planaren Modus viel kostengünstiger.

+++
