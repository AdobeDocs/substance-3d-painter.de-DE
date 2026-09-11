---
breadcrumb-title: ''
description: Prüfe alle Änderungen und Updates in den verschiedenen Substance 3D Painter-Versionen, um den Funktionsverlauf und Verbesserungen im Laufe der Zeit nachzuverfolgen.
title: ZBrush zu Painter Bridge
user-guide-description: ''
user-guide-title: ''
source-git-commit: c50b48e520277293b9ddef466baf8e27db4891ab
workflow-type: tm+mt
source-wordcount: '609'
ht-degree: 2%

---


# ZBrush zu Painter Bridge

Ab ZBrush 2026.2.0 (Maxon One April 2026-Update) und Substance 3D Painter 12.0.2 (Steam- und CC-Version) ist es möglich, Modelle direkt von ZBrush über ein Plug-in an Painter zu senden, das automatisch mit der neuesten Version von ZBrush installiert wird.

![Ein Werbebild, das ein Element zeigt, das gerendert wurde, während es von demselben Element in Zbrush und in Painter überlagert wurde.](../../assets/zbrush_promotional.png)

Mit dem Substance Bridge-Plug-in müssen Sie nicht den langen Prozess durchlaufen, separate Dateien mit niedrigem und hohem Poly zu exportieren, sie in Painter zu importieren und Baking führte zu konfigurieren und auszuführen.

So verwenden Sie die Zbrush-zu-Painter-Brücke:

1. Stellen Sie sicher, dass mindestens Version 2026.2.0 von ZBrush installiert ist.
1. Aktivieren Sie das Plug-in in Painter, indem Sie sicherstellen, dass **Python > zbrush_painter_plugin** aktiviert ist.
1. In ZBrush ist **An Painter senden** in **Textur > Substance Bridge verfügbar**

![Ein Bild des Substance Bridge-Plug-ins in ZBrush](../../assets/zbrush_painterSendTo.png)

## Konfiguration

Sie können die folgenden Einstellungen für die automatische Projekterstellung in Painter konfigurieren:

| Einstellung | Beschreibung |
| --- | --- |
| An Painter senden | Sendet das Modell an Substance 3D Painter, wobei die aktuellen Einstellungen angewendet werden. Mit jedem Klick wird ein neues Substance-Projekt erstellt. |
| **Untertools** | |
| Alle | Sendet jedes SubTool unabhängig von der Sichtbarkeit. Egal ob der Augapfel ein- oder ausgeschaltet ist, alles wird gesendet. |
| Sichtbar | Sendet nur SubTools mit aktiviertem Augensymbol in der SubTool-Liste. |
| Aktiv | Sendet nur das aktuell ausgewählte SubTool |
| PolyPaint senden | Konvertiert PolyPaint in eine Textur-Map und wendet diese auf dem Substance als Füllebene an, auf der Sie mit dem Malen darüber malen und die Überblendung damit durchführen können. |
| Normale Glättung | Glättet Tangente-Normalen beim Export, sodass facettierte Meshs auf dem Substance glatt erscheinen, was der Art und Weise entspricht, wie Game-Engine sie rendern. Deaktivieren Sie diese Option, um die tatsächliche Facettierung der Geometrie anzuzeigen. |
| Karten mit automatischem Baking | Führt die Baking führend Algorithmen von Substance automatisch nach Ankunft des Modells aus und generiert Normalen-Map, ambient occlusion, Krümmung und andere Detailkarten aus dem Mesh-Vergleich. |
| UV Automatisches Entpacken erzwingen | Löst den entpackend UV-Algorithmus von Substance für jedes eintreffende SubTool aus. Lassen Sie die Option weg, wenn Ihr Modell bereits über gute UVs verfügt, da sie dadurch überschrieben werden. |
| Unterteilungsebene | Steuert, welche Unterteilungsebenen gesendet werden. Mit &quot;Aktuell&quot; wird nur der angezeigte Pegel gesendet. &quot;Niedrig &amp; Hoch&quot; sendet sowohl die niedrigsten als auch die höchsten Stufen für das Baking und ist die empfohlene Option für die meisten Workflows. |
| Textur-Sets | Steuert, wie UV-Leerzeichen beim Substance unterteilt werden: Pro SubTool (ein Textursatz pro SubTool) oder pro PolyGroup (ein Textursatz pro PolyGroup innerhalb jedes SubTool). |

Wenn Painter das Modell erhält und &quot;Auto-Baking&quot; aktiviert ist, wird das Baking gestartet. Die unterste Unterteilung des Modells ist der Mesh, der als Low-Poly-Mesh importiert wird, und die oberste Unterteilung wird als High-Poly-Baking verwendet. ZBrush kann eine viel höhere Anzahl von Polygonen verarbeiten als Painter, stellen Sie daher sicher, dass die Low-Poly-Mesh eine optimale Arbeitsgröße hat (dies hängt von der Maschine ab, ist aber unter 1 Million am besten).

Textursatz in Painter stellen Zuweisungen von Materialien dar. Ein Textursatz entspricht einem UV-Leerzeichen.

* Pro SubTool wird ein Textursatz für jedes SubTool erstellt (alle Unterwerkzeugteile würden den gleichen UV-Speicherplatz nutzen), was die einfachere Option ist.
* Pro PolyGroup wird innerhalb jedes SubTool ein Textursatz pro PolyGroup erstellt, sodass Sie die Zuweisung von Materialien genauer steuern können.

>[!NOTE]
>
>Bei der Steam-Version von Painter muss Painter geöffnet sein, um das ZBrush-Modell zu erhalten.


## Weitere Informationsquellen

[Sehen Sie sich dieses Video an](https://www.youtube.com/watch?v=fLkkwV4BzrU), um die Bridge in Aktion zu sehen, oder greifen Sie auf die [ZBrush-Dokumentation](https://help.maxon.net/zbr/en-us/Default.htm#html/reference-guide/texture/substance-bridge/substance-bridge.html?Highlight=painter) zu, um weitere Informationen zu erhalten.
