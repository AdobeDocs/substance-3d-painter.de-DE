---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/automatic-uv-unwrapping.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie das automatische Ausgliedern von UV-Licht in Substance 3D Painter verwenden, um UV-Layouts für Ihre 3D-Modelle automatisch zu generieren.
helpx_creative_field: ""
helpx_description: Painter > Features > Automatic UV Unwrapping
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Automatisches Ausgliedern von UVs
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 0%

---


# Automatisches Ausgliedern von UVs

![](../assets/auto-unwrap-update-810.jpg)\
Mit dem automatischen Ausgliedern von UVs können beim Importieren eines 3D-Modells automatisch UV-Inseln generiert werden. Es kann verwendet werden, um auf einem 3D-Modell zu malen, das keine vorhandenen UVs hat.

## Aktivieren der automatischen UV-Entpackung

![](../assets/uv-new-project.png)

Stellen Sie beim Erstellen eines neuen Projekts oder beim erneuten Importieren eines Gitters in ein vorhandenes Projekt sicher, dass die Einstellung &quot;Automatisch entpacken&quot; aktiviert ist. Wenn diese Option deaktiviert ist, wird der Prozess übersprungen und die Gitter-UVs bleiben unverändert.

## Einstellungen für das Ausgliedern von UV

![](../assets/unwrap-settings.png)

Beim Importieren eines Gitters und beim Ausgliedern sind die folgenden Einstellungen verfügbar. Einige Einstellungen sind über die Schaltfläche &quot;Optionen&quot; in der Benutzeroberfläche verfügbar.

| Abschnitt | ***Einstellung*** | ***Beschreibung*** |
| --- | --- | --- |
| **Sequenz ausgliedern** | **Nähte** | Steuert, ob die Nahtstellen (UV-Inseln-Rahmen) nur für Gitter generiert werden sollen, in denen sie nicht vorhanden sind oder immer neu generiert werden.Mögliche Werte:<ul data-preserve-html="true"><li data-preserve-html="true"><strong> Fehlende Daten </strong> generieren (Standard): Es werden Nähte für Gitter erzeugt, in denen sie fehlen.</li><li data-preserve-html="true"><strong> Alle </strong> neu berechnen : Für alle Maschen werden Nähte erzeugt.</li></ul> |
| **UV-Inseln** | Steuert, ob die UV-Entpackung aus Gittern ohne UVs oder für beliebige Gitter generiert werden soll. Mögliche Werte:<ul data-preserve-html="true"><li data-preserve-html="true"><strong> Fehlende Daten </strong> generieren (Standard): UV-Entpackung wird für Gitter generiert, denen UVs fehlen.</li><li data-preserve-html="true"><strong> Alle </strong> neu berechnen : UV-Entpackung wird für alle Gitter generiert.</li></ul> |  |
| **Packing** | Steuert das Packing/Layout der UV-Inseln der Gitter.Mögliche Werte:<ul data-preserve-html="true"><li data-preserve-html="true"><strong> Fehlende Daten </strong> generieren (Standard): Packen von UV-Inseln für Gitter, bei denen UVs fehlten.</li><li data-preserve-html="true"><strong> Alle </strong> neu berechnen : Packen Sie alle UV-Inseln.</li></ul> |  |
|  |  |  |
| **Layoutanpassung** | **Randgröße** | Definiert den Abstand zwischen den UV-Inseln. Diese Einstellung gilt für einen allgemeinen Prozentsatz, der unabhängig von der Auflösung ist.Mögliche Werte:<ul data-preserve-html="true"><li data-preserve-html="true"><strong> Kein Rand </strong> : 0 %</li><li data-preserve-html="true"><strong> Klein </strong> (Standard): 0,2%</li><li data-preserve-html="true"><strong> Medium </strong> : 0,5%</li><li data-preserve-html="true"><strong> Groß </strong> : 1 %</li></ul> |
|  | **Ausrichtung der UV-Insel** | Steuern Sie die Ausrichtung der UV-Inseln während des Packings.Mögliche Werte:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Nicht eingeschränkt</strong> (Standard): Es wird keine Einschränkung angewendet, um die Ausrichtung zu berechnen.</li><li data-preserve-html="true"><strong>An 3D-Gitter ausrichten</strong>: die UV-Insel auf die Gitterrichtung zu beschränken</li></ul> |
|  |  |  |
| **UV-Kacheln** | **Maximale Anzahl von UV-Kacheln** | Wenn der Arbeitsablauf für UV-Kacheln aktiviert ist, wird mit diesen Einstellungen die maximale Anzahl der Kacheln festgelegt, die für die Verteilung auf den UV-Inseln erzeugt werden sollen. |
|  |  |  |
| **Optimierung** | **Längliche UV-Inseln vermeiden** | Wenn diese Option aktiviert ist, wird dieser Prozess UV-Inseln teilen, die als zu lang angesehen werden, um die Nutzung des Texturraums zu verbessern.Beispiel für vorher (oben) und nachher (unten): <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r10-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../assets/uv-before-after.jpg" width="400px"/></div> |

## Bekannte Einschränkungen

Im Folgenden finden Sie eine Liste der Einschränkungen im Zusammenhang mit dem Ausgliederungsprozess:

* Die Verarbeitung von Polygonzügen kann lange dauern.
* Eckpunkte mit genau denselben Koordinaten werden zusammengeführt
* In seltenen Fällen kann die UV-Generierung an einigen Netzteilen fehlschlagen
* Uneinheitliches oder stark verzerrtes Textilverhältnis in einer einzigen UV-Insel in einigen Fällen
* Nicht einheitliches Textilverhältnis zwischen Textursätzen
* Die erzeugte UV-Insel kann sehr lang sein und passt in manchen Fällen nicht in den UV-Raum.
* Entartete Flächen oder nicht dreieckige Gitterflächen mit kleinen oder überlappenden Kanten werden möglicherweise nicht von UV ausgepackt.
