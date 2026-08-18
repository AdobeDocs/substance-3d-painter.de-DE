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

Mit dem Substance Bridge-Plug-in müssen Sie nicht den langen Prozess durchlaufen, separate Dateien mit niedrigem und hohem Poly zu exportieren, sie in Painter zu importieren und Backs zu konfigurieren und auszuführen.

So verwenden Sie die Zbrush-zu-Painter-Brücke:

1. Stellen Sie sicher, dass mindestens Version 2026.2.0 von ZBrush installiert ist.
1. Aktivieren Sie das Plug-in in Painter, indem Sie sicherstellen, dass **Python > zbrush_painter_plugin** aktiviert ist.
1. In ZBrush ist **An Painter senden** in **Texture > Substance Bridge verfügbar**

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
| PolyPaint senden | Konvertiert PolyPaint in eine Texturmap und wendet diese auf dem Substance als Füllebene an, auf der Sie darüber malen und mit ihr mischen können. |
| Normale Glättung | Glättet Tangentennormalen beim Export, sodass facettierte Meshes auf dem Substance glatt erscheinen, was der Darstellung von Game-Engines entspricht. Deaktivieren Sie diese Option, um die tatsächliche Facettierung der Geometrie anzuzeigen. |
| Karten automatisch backen | Führt die Backalgorithmen von Substance automatisch nach Ankunft des Modells aus und generiert Normalmaps, Umgebungs-Verdeckungen, Krümmungen und andere Detailkarten aus dem Vergleich der hohen/niedrigen Maschenöffnungen. |
| Automatisches Ausgliedern von UVs erzwingen | Löst den UV-Entpackungsalgorithmus von Substance für jedes eintreffende SubTool aus. Lassen Sie die Option weg, wenn Ihr Modell bereits über gute UVs verfügt, da sie dadurch überschrieben werden. |
| Unterteilungsebene | Steuert, welche Unterteilungsebenen gesendet werden. Mit &quot;Aktuell&quot; wird nur der angezeigte Pegel gesendet. &quot;Niedrig &amp; Hoch&quot; sendet sowohl die niedrigsten als auch die höchsten Stufen für das Backen und ist die empfohlene Option für die meisten Arbeitsabläufe. |
| Textur-Sets | Steuert, wie der UV-Raum in Substance aufgeteilt wird: Pro SubTool (ein Texturensatz pro SubTool) oder pro PolyGroup (ein Texturensatz pro PolyGroup innerhalb jedes SubTool). |

Wenn Painter das Modell erhält und &quot;Automatisch backen&quot; aktiviert ist, wird das Backen gestartet. Die unterste Unterteilung des Modells ist das Mesh, das als Low-Poly-Mesh importiert wird, und die höchste Unterteilung wird als High-Poly-Mesh verwendet, um Details zu backen. ZBrush kann eine viel höhere Anzahl von Polygonen verarbeiten als Painter. Stellen Sie daher sicher, dass das niedrige Polygitter eine optimale Arbeitsgröße hat (dies hängt von der Maschine ab, ist aber am besten unter 1 Million).

Struktursammlungen in Painter stellen Materialzuweisungen dar. Ein Textursatz entspricht einem UV-Raum.

* Pro SubTool wird für jedes SubTool ein Textursatz erstellt (alle Unterwerkzeugteile würden den gleichen UV-Raum nutzen), was die einfachere Option ist.
* Pro PolyGroup wird pro PolyGroup in jedem SubTool ein Textursatz erstellt, der Ihnen eine feinere Kontrolle über Materialzuweisungen ermöglicht.

>[!NOTE]
>
>Bei der Steam-Version von Painter muss Painter geöffnet sein, um das ZBrush-Modell zu erhalten.


## Weitere Informationsquellen

[Sehen Sie sich dieses Video an](https://www.youtube.com/watch?v=fLkkwV4BzrU), um die Bridge in Aktion zu sehen, oder greifen Sie auf die [ZBrush-Dokumentation](https://help.maxon.net/zbr/en-us/Default.htm#html/reference-guide/texture/substance-bridge/substance-bridge.html?Highlight=painter) zu, um weitere Informationen zu erhalten.
