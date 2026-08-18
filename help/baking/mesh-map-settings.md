---
helpx_url: 'https://helpx.adobe.com/de/substance-3d-painter/baking/mesh-map-settings.html'
breadcrumb-title: ''
description: Erfahren Sie, wie Sie die Einstellungen für die Gitterzuordnung in Substance 3D Painter konfigurieren, um Backparameter und Ausgabequalität zu steuern.
helpx_creative_field: ''
helpx_description: Substance 3D Painter
helpx_experience_level: ''
helpx_learn_topic: ''
helpx_tags: ''
title: Einstellungen für Mesh-Maps
user-guide-description: ''
user-guide-title: ''
source-git-commit: 7b5f6e6c9623cb51253b6e49c8dbcbb22856418c
workflow-type: tm+mt
source-wordcount: '1348'
ht-degree: 10%

---


# Einstellungen für Mesh-Maps

<b>Das Einstellungsfenster für die Gitterzuordnung &quot;</b>&quot; ist im Backmodus verfügbar und verfügt über Steuerelemente, mit denen das Gitter für das Backen vorbereitet wird. Um die Einstellungen für die Mesh-Map für eine bestimmte Map anzupassen, wählen Sie die Map im Bedienfeld &quot;<b>Mesh-Map-Bäcker&quot; aus</b>. Für jede Mesh-Map können unterschiedliche Einstellungen verfügbar sein. Eine Sammlung von <b>Allgemeine Einstellungen </b>, die von allen Gitterzuordnungen gemeinsam genutzt werden, ist oben im Fenster Gitterzuordnungs-Bäcker verfügbar.

Alle Einstellungen, die über Gitterzuordnungen hinweg gemeinsam genutzt werden, werden auf der Seite Allgemeine Einstellungen und nicht auf jeder einzelnen Gitterzuordnung angezeigt.

## Allgemeine Einstellungen

Die Seite &quot;Allgemeine Einstellungen&quot; enthält Steuerelemente, die beeinflussen, wie alle Gitterzuordnungen gebacken werden.

### Ausgabeeinstellungen

| Einstellung | Funktion |
| --- | --- |
| Ausgabegröße | Definieren Sie die X- und Y-Auflösung generierter Gitterzuordnungen. Klicken Sie auf das Schloss, um nicht quadratische Auflösungen zuzulassen. |
| Dehnungsbreite | Passen Sie an, wie weit die gespeicherten Informationen über die Grenzen von UV-Inseln hinausgehen. |
| Diffusion anwenden | Aktivieren Sie dieses Kontrollkästchen, um Diffusion auf die Kanten der generierten Informationen anzuwenden. |

### High-Poly-Parameter

| Einstellung | Funktion |
| --- | --- |
| Niedriges Polygitter als hohes Polygitter verwenden | Aktivieren Sie diese Einstellung, um Maps basierend auf Ihrem Projektgitter zu backen. |
| Hochauflösende Meshes | Fügen Sie Ihrem Projekt hohe Poly-Meshes hinzu, um aus einem hohen Poly-Mesh ein niedriges Poly-Mesh in Ihrem Projekt zu erstellen. Es können mehrere Gitter importiert werden. |
| Käfig | Legen Sie fest, wie der Backkäfig erzeugt wird.<ul data-preserve-html="true"> <li data-preserve-html="true">Entfernungsabhängig: Blasen Sie die Scheitelpunkte vom Gitter aus in einem gleichmäßigen Abstand über das Modell auf, um einen Käfig zu erstellen.</li> <li data-preserve-html="true">Automatisch (experimentell): Painter analysiert dein Gitter und generiert automatisch einen Käfig. Der Käfig bleibt nahe an der Oberfläche, ohne Schnittpunkte zu erstellen.</li> <li data-preserve-html="true">Benutzerdefinierte Datei: Importieren Sie eine Datei, die Sie erstellt haben, um sie als Käfig zu verwenden. Beachten Sie, dass importierte Dateien dieselbe Anzahl an Scheitelpunkten wie das Basisgitter haben müssen, damit sie ordnungsgemäß funktionieren.</li> </ul> |
| Rückseite ignorieren | Stellt ein, ob die Rückseiten beim Backen ignoriert werden. Dies kann Artefakte reduzieren, aber auch in bestimmten Fällen zu Fehlern führen. |
| Abgleichen | Ändern Sie, wie der Bäcker bestimmt, ob Objekte beim Backen einbezogen werden:<ul data-preserve-html="true"> <li data-preserve-html="true">Immer: Schließen Sie alle hohen Poly-Maschen ein, die beim Backen im Käfig getroffen werden.</li> <li data-preserve-html="true">Nach Maschenname: Backen Sie für jeden Käfig die Gitter nur mit dem entsprechenden Gittersuffix.</li> </ul> |
| Suffix für Low-Poly-Mesh | Verwenden Sie dieses Suffix, wenn Sie den Netznamen &quot;Angleichen nach&quot; verwenden, um niedrige Poly-Meshes zu definieren. |
| Suffix für High-Poly-Mesh | Verwenden Sie dieses Suffix, wenn Sie den Netznamen &quot;Angleichen nach&quot; verwenden, um hohe Polygitter zu definieren und mit dem entsprechenden niedrigen Polygitter abzugleichen. |
| Antialiasing | Passen Sie den Grad des Antialiasing in den generierten Maps an. |

#### Verzerrungskorrektur

| Einstellung | Beschreibung |
| --- | --- |
| **Korrektur der Farbneigung** | Wechseln Sie in den Skew-Korrekturmodus. |
| **Kantenschutz** | Schalten Sie den Kantenschutz um, um die Werte der bemalten Neigungskorrektur in der Nähe harter Kanten zu maskieren. |
| **Kantenabstand** | Legt fest, wie weit der Kantenschutz von harten Kanten reicht. |
| **Kantenkontrast** | Legt fest, wie stark der Kantenschutzverlauf vom vollständigen Schutz zum Nichtschutz übergeht. |

## ID-Zuordnungseinstellungen

| Einstellung | Funktion |
| --- | --- |
| Farbquelle | Ändern Sie, wie die vordefinierten Farben der ID-Map bestimmt werden:<ul data-preserve-html="true"> <li data-preserve-html="true">Vertexfarbe</li> <li data-preserve-html="true">Materialfarbe</li> <li data-preserve-html="true">Datei-ID</li> <li data-preserve-html="true">Gitter-ID/Polygruppe</li> </ul> |
| Farbgenerator | Wenn Sie die Datei-ID oder die Gitter-ID/Polygruppe als Farbquelle verwenden, bestimmen Sie, wie Farben generiert werden:<ul data-preserve-html="true"> <li data-preserve-html="true">Zufallswert</li> <li data-preserve-html="true">Farbtonverschiebung</li> <li data-preserve-html="true">Graustufen</li> </ul> |

## Umgebungszuordnungseinstellungen für die Verdeckung

| Einstellung | Funktion |
| --- | --- |
| Sekundäre Strahlen | Ändern Sie die Anzahl der Sekundärstrahlen. Mehr Strahlen können bessere Ergebnisse liefern, was auf Kosten einer erhöhten Verarbeitungszeit geht. |
| Min Occluder-Abstand | Passen Sie den Mindestabstand für die Strahlen so an, dass sie auf eine hohe Poly-Geometrie treffen und auf die resultierende AO-Karte wirken. |
| Max. Occluder-Distanz | Strahlen, die sich über diese Entfernung hinaus erstrecken, ohne das hohe Polygitter zu treffen, gelten als nicht verdeckt und wirken sich nicht auf die AO-Karte aus. |
| Relativ zum Begrenzungsrahmen | Wenn dieses Kontrollkästchen aktiviert ist, werden andere Einstellungen, die sich auf den Abstand beziehen, auf den Begrenzungsrahmen des Projektnetzes angewendet. Ein Abstand von 1 entspricht der Größe des Begrenzungsrahmens. |
| Ausbreitungswinkel | Passen Sie den angular-Bereich der generierten Strahlen an. Ein höherer Spreizwinkel ermöglicht es, eine Oberfläche leichter durch Geometrie zu verschließen, die nicht senkrecht von der Oberfläche weg angeordnet ist. |
| Verteilung | Legen Sie fest, wie die Strahlen verteilt werden. |
| Rückseite ignorieren | Ändert, ob Flächen hinter Objekten verborgen werden. |
| Selbstverdeckung | Wählen Sie aus, welche Gitter die Verdeckung des aktuellen Gitters beeinflussen sollen. |
| Abmilderung | Ändere, wie die Verdeckung durch die Entfernung der Augenringe gedämpft wird. |
| Grundebene | Aktivieren Sie diese Option, um eine Grundebene zu erstellen, die als Okklusion fungiert. |
| Versatz der Grundebene | Ändern Sie die Position der Grundebene. |

## Einstellungen für die Krümmungskarte

| Einstellung | Funktion |
| --- | --- |
| Methode | Wählen Sie, wie die Krümmungszuordnung generiert werden soll. |
| Sekundäre Strahlen | Passen Sie an, wie viele Sekundärstrahlen zum Generieren der Krümmungszuordnung verwendet werden. Mehr Sekundärstrahlen können bessere Ergebnisse erzielen, was auf Kosten einer höheren Verarbeitungszeit geht. |
| Sampling-Radius | Passen Sie an, wie weit der Bäcker sucht, um die Rundung des aktuellen Punktes zu berechnen. |
| Relativ zum Begrenzungsrahmen | Wenn diese Option aktiviert ist, basieren alle Abstände auf der Größe des Gitterbegrenzungsrahmens. |
| Selbstüberschneidung | Wählen Sie aus, welche Objekte bei der Bestimmung der Krümmung berücksichtigt werden sollen. |
| Automatisches Tonemapping (pro UV-Kachel) | Lassen Sie diese Option aktiviert, um die Tonemap-Krümmungszuordnungen automatisch auf Basis einer UV-Kachel anzupassen. |
| Min. Tonemapping | Wenn die automatische Tonzuordnung deaktiviert ist, passen Sie den Mindestwert für die Tonzuordnung an. |
| Max. Tonemapping | Wenn die automatische Tonzuordnung deaktiviert ist, passen Sie den Höchstwert für die Tonzuordnung an. |

## Positionierungszuordnungseinstellungen

| Einstellung | Funktion |
| --- | --- |
| Modus | Wählen Sie aus, ob eine Positionszuordnung für alle Achsen generiert oder nur die Position für eine ausgewählte Achse berechnet werden soll. |
| Achse | Wenn der Modus Einzelne Achse ausgewählt ist, verwenden Sie diese Einstellung, um auszuwählen, welche Achse berechnet werden soll. |
| Normalisierungstyp | Ändern Sie, wie Positionswerte normalisiert werden, entweder mit einem Begrenzungsrahmen oder einer Begrenzungskugel, oder deaktivieren Sie die Normalisierung. |
| Normalisierungsskala | Ändert die maximale Begrenzung des Positionsraums. |

## Thickness-Map-Einstellungen

| Einstellung | Funktion |
| --- | --- |
| Sekundäre Strahlen | Ändern Sie die Anzahl der Sekundärstrahlen. Mehr Strahlen können bessere Ergebnisse liefern, was auf Kosten einer erhöhten Verarbeitungszeit geht. |
| Min Occluder-Abstand | Passen Sie den Mindestabstand für die zu bewegenden Strahlen an, um auf eine hohe Poly-Geometrie zu treffen und die resultierende Thickness anzuzeigen. |
| Max. Occluder-Entfernung | Strahlen, die sich über diese Entfernung hinaus erstrecken, ohne das hohe Polygitter zu treffen, gelten als nicht verdeckt und wirken sich nicht auf die Thickness aus. |
| Relativ zum Begrenzungsrahmen | Wenn dieses Kontrollkästchen aktiviert ist, werden andere Einstellungen, die sich auf den Abstand beziehen, auf den Begrenzungsrahmen des Projektnetzes angewendet. Ein Abstand von 1 entspricht der Größe des Begrenzungsrahmens. |
| Ausbreitungswinkel | Passen Sie den angular-Bereich der generierten Strahlen an. Ein höherer Spreizwinkel ermöglicht es, eine Oberfläche leichter durch Geometrie zu verschließen, die nicht senkrecht von der Oberfläche weg angeordnet ist. |
| Verteilung | Legen Sie fest, wie die Strahlen verteilt werden. |
| Selbstverdeckung | Wählen Sie aus, welche Gitter die Thickness des aktuellen Gitters beeinflussen sollen. |
| Normalisierung | Ändern Sie, wie Werte für Thicknessen normalisiert werden. |

## Height-Map-Einstellungen

| Einstellung | Funktion |
| --- | --- |
| Normalisierung | Ändern Sie, wie die Werte von Heights normalisiert werden. |
| Skalierungsdivisor | Wenn &quot;Normalisierung&quot; auf &quot;Manuell&quot; eingestellt ist, können Sie mit diesem Schieberegler den Skalierungs-Divisor anpassen und die Normalisierung der Height-Map anpassen. |

## Gebeugte Normal-Zuordnungseinstellungen

| Einstellung | Funktion |
| --- | --- |
| Sekundäre Strahlen | Ändern Sie die Anzahl der Sekundärstrahlen. Mehr Strahlen können bessere Ergebnisse liefern, was auf Kosten einer erhöhten Verarbeitungszeit geht. |
| Min Occluder-Abstand | Passen Sie den minimalen Abstand für die Strahlen an, um auf eine hohe Poly-Geometrie zu treffen und die resultierende gebogene Normal-Map zu treffen. |
| Max. Occluder-Entfernung | Strahlen, die sich über diese Entfernung hinaus erstrecken, ohne das hohe Polygitter zu treffen, gelten als nicht verdeckt und wirken sich nicht auf die gebogene Normalenmaske aus. |
| Relativ zum Begrenzungsrahmen | Wenn dieses Kontrollkästchen aktiviert ist, werden andere Einstellungen, die sich auf den Abstand beziehen, auf den Begrenzungsrahmen des Projektgitters angewendet. Ein Abstand von 1 entspricht der Größe des Begrenzungsrahmens. |
| Ausbreitungswinkel | Passen Sie den angular-Bereich der generierten Strahlen an. Ein höherer Spreizwinkel ermöglicht es, eine Oberfläche leichter durch Geometrie zu verschließen, die nicht senkrecht von der Oberfläche weg angeordnet ist. |
| Verteilung | Legen Sie fest, wie die Strahlen verteilt werden. |
| Rückseite ignorieren | Legen Sie fest, ob die Rückseiten als Okklusionen behandelt werden sollen. |
| Selbstverdeckung | Wählen Sie aus, welche Gitter die gebogenen Normalen des aktuellen Gitters beeinflussen sollen. |
