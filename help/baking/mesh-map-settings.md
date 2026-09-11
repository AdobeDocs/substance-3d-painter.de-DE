---
helpx_url: 'https://helpx.adobe.com/de/substance-3d-painter/baking/mesh-map-settings.html'
breadcrumb-title: ''
description: Erfahren Sie, wie Sie die Mesh-Map-Einstellungen in Substance 3D Painter konfigurieren, um die Parameter für das Baking und die Ausgabequalität zu steuern.
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

<b>Das Bedienfeld &quot;Mesh-Map-Einstellungen&quot; </b> ist im Baking-Modus verfügbar und verfügt über Steuerelemente, mit denen Sie Ihren Mesh für das Baking vorbereiten können. Um die Mesh-Map-Einstellungen für eine bestimmte Map anzupassen, wählen Sie die Map im <b>Mesh-Map-Baker-Bedienfeld</b> aus. Für jede Mesh-Map können unterschiedliche Einstellungen verfügbar sein. Eine Sammlung von <b>allgemeinen Einstellungen </b>, die von allen Mesh-Map gemeinsam genutzt werden, ist oben im Bedienfeld &quot;Mesh-Map-Baker&quot; verfügbar.

Alle von Mesh-Map gemeinsam genutzten Einstellungen werden auf der Seite &quot;Allgemeine Einstellungen&quot; und nicht auf den einzelnen Mesh-Map angezeigt.

## Allgemeine Einstellungen

Die Seite &quot;Allgemeine Einstellungen&quot; enthält Steuerelemente, die beeinflussen, wie alle Mesh-Map Baking geführt werden.

### Ausgabeeinstellungen

| Einstellung | Funktion |
| --- | --- |
| Ausgabegröße | Definieren Sie die X- und Y-Auflösung generierter Mesh-Map. Klicken Sie auf das Schloss, um nicht quadratische Auflösungen zuzulassen. |
| Dehnungsbreite | Passen Sie an, wie weit die gespeicherten Informationen über die Grenzen von UV-Inseln hinausgehen. |
| Diffusion anwenden | Aktivieren Sie dieses Kontrollkästchen, um Diffusion auf die Kanten der generierten Informationen anzuwenden. |

### High-Poly-Parameter

| Einstellung | Funktion |
| --- | --- |
| Niedriges Polygitter als hohes Polygitter verwenden | Aktivieren Sie diese Einstellung, um Maps auf der Grundlage Ihres Projekt-Meshs Baking führen. |
| Hochauflösende Meshes | Füge hohe Poly-Mesh zu deinem Projekt hinzu, um aus einer High-Poly-Mesh ein Low-Poly-Mesh in deinem Projekt zu machen. Es können mehrere Mesh importiert werden. |
| Käfig | Legen Sie fest, wie der Baking führend Käfig generiert wird.<ul data-preserve-html="true"> <li data-preserve-html="true">Entfernungsabhängig: Blasen Sie die Scheitelpunkt vom Mesh aus in einer gleichmäßigen Entfernung über das Model hinweg auf, um einen Käfig zu erzeugen.</li> <li data-preserve-html="true">Automatisch (experimentell): Painter analysiert Ihren Mesh und generiert automatisch einen Käfig. Dabei wird versucht, den Käfig in der Nähe der Oberfläche zu halten, ohne dass Schnittpunkte erstellt werden, um optimale Ergebnisse zu erzielen.</li> <li data-preserve-html="true">Benutzerdefinierte Datei: Importieren Sie eine Datei, die Sie erstellt haben, um sie als Käfig zu verwenden. Beachten Sie, dass importierte Dateien dieselbe Anzahl an Scheitelpunkten wie das Basisgitter haben müssen, damit sie ordnungsgemäß funktionieren.</li> </ul> |
| Rückseite ignorieren | Stellt ein, ob rückseitige Flächen beim Baking ignoriert werden. Dies kann Artefakte reduzieren, aber auch in bestimmten Fällen zu Fehlern führen. |
| Abgleichen | Ändern Sie, wie der Baker bestimmt, ob Objekte beim Baking einbezogen werden sollen:<ul data-preserve-html="true"> <li data-preserve-html="true">Immer: Schließen Sie alle hohen Poly-Maschen ein, die beim Backen im Käfig getroffen werden.</li> <li data-preserve-html="true">Nach Name des Meshs: Für jeden Käfig werden nur Mesh mit dem entsprechenden Mesh-Suffix Baking geführt.</li> </ul> |
| Suffix für Low-Poly-Mesh | Verwenden Sie bei Verwendung des Namens &quot;Mit Mesh abgleichen&quot; dieses Suffix, um niedrige Poly-Meshs zu definieren. |
| Suffix für High-Poly-Mesh | Verwenden Sie bei Verwendung des Namens &quot;Mit Mesh abgleichen&quot; dieses Suffix, um hohe Poly-Meshs zu definieren und mit den entsprechenden Low-Poly-Mesh abzugleichen. |
| Antialiasing | Passen Sie die Menge des Antialiasings in den generierten Maps an. |

#### Verzerrungskorrektur

| Einstellung | Beschreibung |
| --- | --- |
| **Malen Verzerrungskorrektur** | Rufen Sie den Verzerrungskorrektur-Malmodus auf. |
| **Kantenschutz** | Aktiviere/deaktiviere die Option &quot;Kantenschutz&quot;, um die Werte für die gemalte Verzerrungskorrektur in der Nähe harter Kanten zu maskieren. |
| **Kantenabstand** | Legt fest, wie weit der Kantenschutz von harten Kanten reicht. |
| **Kantenkontrast** | Legt fest, wie stark der Kantenschutzverlauf vom vollständigen Schutz zum Nichtschutz übergeht. |

## ID-Map-Einstellungen

| Einstellung | Funktion |
| --- | --- |
| Farbquelle | Ändern Sie, wie die Baking geführt Farben der ID-Map bestimmt werden:<ul data-preserve-html="true"> <li data-preserve-html="true">Vertexfarbe</li> <li data-preserve-html="true">Materialfarbe</li> <li data-preserve-html="true">Datei-ID</li> <li data-preserve-html="true">Mesh-ID/Polygruppe</li> </ul> |
| Farbgenerator | Wenn Sie die Datei-ID oder Mesh-ID/Polygruppe als Farbquelle verwenden, bestimmen Sie, wie Farben generiert werden:<ul data-preserve-html="true"> <li data-preserve-html="true">Zufallswert</li> <li data-preserve-html="true">Farbtonverschiebung</li> <li data-preserve-html="true">Graustufen</li> </ul> |

## Umgebungszuordnungseinstellungen für die Verdeckung

| Einstellung | Funktion |
| --- | --- |
| Sekundäre Strahlen | Ändern Sie die Anzahl der Sekundärstrahlen. Mehr Strahlen können bessere Ergebnisse liefern, was auf Kosten einer erhöhten Verarbeitungszeit geht. |
| Min Occluder-Abstand | Passen Sie den Mindestabstand für die Strahlen so an, dass sie auf eine hohe Poly-Geometrie treffen und auf die resultierende AO-Karte wirken. |
| Max. Occluder-Distanz | Strahlen, die sich über diese Entfernung hinaus erstrecken, ohne die High-Poly-Mesh zu treffen, gelten als nicht verdeckt und wirken sich nicht auf die AO-Karte aus. |
| Relativ zum Begrenzungsrahmen | Wenn dieses Kontrollkästchen aktiviert ist, werden andere Einstellungen, die sich auf den Abstand beziehen, auf den Begrenzungsrahmen des Projekt-Meshs angewendet. Ein Abstand von 1 entspricht der Größe des Begrenzungsrahmens. |
| Ausbreitungswinkel | Passen Sie den angular-Bereich der generierten Strahlen an. Ein höherer Spreizwinkel ermöglicht es, eine Oberfläche leichter durch Geometrie zu verschließen, die nicht senkrecht von der Oberfläche weg angeordnet ist. |
| Verteilung | Legen Sie fest, wie die Strahlen verteilt werden. |
| Rückseite ignorieren | Ändert, ob Flächen hinter Objekten verborgen werden. |
| Selbstverdeckung | Wählen Sie aus, welche Mesh das ambient occlusion für den aktuellen Mesh betreffen sollen. |
| Abmilderung | Ändert, wie Verdeckung durch Verdeckungsabstand gedämpft wird. |
| Grundebene | Aktivieren Sie diese Option, um eine Boden-Ebene zu erstellen, die als Okklusion fungiert. |
| Versatz der Grundebene | Ändern Sie die Position des Bodens. |

## Krümmungs-Map-Einstellungen

| Einstellung | Funktion |
| --- | --- |
| Methode | Legen Sie fest, wie die Krümmungs-Map generiert werden soll. |
| Sekundäre Strahlen | Passen Sie an, wie viele Sekundärstrahlen zum Generieren der Krümmungszuordnung verwendet werden. Mehr Sekundärstrahlen können bessere Ergebnisse erzielen, was auf Kosten einer höheren Verarbeitungszeit geht. |
| Sampling-Radius | Passen Sie an, wie weit der Baker sucht, um die Krümmung des aktuellen Punktes zu berechnen. |
| Relativ zum Begrenzungsrahmen | Wenn diese Einstellung aktiviert ist, werden alle Abstände anhand der Größe des Mesh-Begrenzungsrahmens berechnet. |
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

## Dicken-Map-Einstellungen

| Einstellung | Funktion |
| --- | --- |
| Sekundäre Strahlen | Ändern Sie die Anzahl der Sekundärstrahlen. Mehr Strahlen können bessere Ergebnisse liefern, was auf Kosten einer erhöhten Verarbeitungszeit geht. |
| Min Occluder-Abstand | Passen Sie den Mindestabstand für die Strahlen an, damit diese auf die hohe Poly-Geometrie treffen und auf den resultierenden Dicken-Map treffen. |
| Max. Verdeckungsabstand | Strahlen, die sich über diese Entfernung hinaus erstrecken, ohne das hohe Polygitter zu treffen, gelten als nicht verdeckt und wirken sich nicht auf die Thickness aus. |
| Relativ zum Begrenzungsrahmen | Wenn dieses Kontrollkästchen aktiviert ist, werden andere Einstellungen, die sich auf den Abstand beziehen, auf den Begrenzungsrahmen des Projekt-Meshs angewendet. Ein Abstand von 1 entspricht der Größe des Begrenzungsrahmens. |
| Ausbreitungswinkel | Passen Sie den angular-Bereich der generierten Strahlen an. Ein höherer Spreizwinkel ermöglicht es, eine Oberfläche leichter durch Geometrie zu verschließen, die nicht senkrecht von der Oberfläche weg angeordnet ist. |
| Verteilung | Legen Sie fest, wie die Strahlen verteilt werden. |
| Selbstverdeckung | Wählen Sie aus, welche Gitter die Thickness des aktuellen Gitters beeinflussen sollen. |
| Normalisierung | Ändern Sie, wie Werte für Thicknessen normalisiert werden. |

## Höhen-Map-Einstellungen

| Einstellung | Funktion |
| --- | --- |
| Normalisierung | Ändern Sie, wie die Werte von Heights normalisiert werden. |
| Skalierungsdivisor | Wenn &quot;Normalisierung&quot; auf &quot;Manuell&quot; eingestellt ist, können Sie mit diesem Schieberegler den Skalierungs-Divisor anpassen und die Normalisierung der Height-Map anpassen. |

## Bent normals-Map-Einstellungen

| Einstellung | Funktion |
| --- | --- |
| Sekundäre Strahlen | Ändern Sie die Anzahl der Sekundärstrahlen. Mehr Strahlen können bessere Ergebnisse liefern, was auf Kosten einer erhöhten Verarbeitungszeit geht. |
| Min Occluder-Abstand | Passen Sie den Mindestabstand für die Strahlen so an, dass sie auf die hohe Poly-Geometrie treffen und auf die resultierende bent normals-Map wirken. |
| Max. Verdeckungsabstand | Strahlen, die sich über diese Entfernung hinaus erstrecken, ohne das hohe Polygitter zu treffen, gelten als nicht verdeckt und wirken sich nicht auf die gebogene Normalenmaske aus. |
| Relativ zum Begrenzungsrahmen | Wenn dieses Kontrollkästchen aktiviert ist, werden andere Einstellungen, die sich auf den Abstand beziehen, auf den Begrenzungsrahmen des Projekt-Meshs angewendet. Ein Abstand von 1 entspricht der Größe des Begrenzungsrahmens. |
| Ausbreitungswinkel | Passen Sie den angular-Bereich der generierten Strahlen an. Ein höherer Spreizwinkel ermöglicht es, eine Oberfläche leichter durch Geometrie zu verschließen, die nicht senkrecht von der Oberfläche weg angeordnet ist. |
| Verteilung | Legen Sie fest, wie die Strahlen verteilt werden. |
| Rückseite ignorieren | Legen Sie fest, ob die Rückseiten als Okklusionen behandelt werden sollen. |
| Selbstverdeckung | Wählen Sie aus, welche Mesh sich auf die bent normals für den aktuellen Mesh auswirken sollen. |
