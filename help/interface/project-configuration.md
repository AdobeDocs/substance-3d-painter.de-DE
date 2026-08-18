---
helpx_url: 'https://helpx.adobe.com/de/substance-3d-painter/interface/project-configuration.html'
breadcrumb-title: ''
description: Erfahren Sie, wie Sie in Substance 3D Painter Projekteinstellungen konfigurieren, um die Texturauflösung, Kanäle und Projekteigenschaften einzurichten.
helpx_creative_field: ''
helpx_description: Painter > Interface > Project configuration
helpx_experience_level: ''
helpx_learn_topic: ''
helpx_tags: ''
title: Projektkonfiguration
user-guide-description: ''
user-guide-title: ''
source-git-commit: 3e4ef9bd5897f042b01d6c0819ec06cc21ba208a
workflow-type: tm+mt
source-wordcount: '839'
ht-degree: 4%

---


# Projektkonfiguration

![](../assets/project-configuration-full.png)

Das Projektkonfigurationsfenster enthält Steuerelemente zum Ändern von Projekteinstellungen. Projekteinstellungen werden in der Regel beim Erstellen eines neuen Projekts festgelegt, in einigen Fällen müssen Sie diese Einstellungen jedoch zu einem späteren Zeitpunkt im Projekt ändern.

## 3D-Mesh

Wenn Änderungen am 3D-Gitter oder an der Gitterdatei vorgenommen wurden, können Sie das Gitter erneut importieren, während die anderen Projektdaten beibehalten werden. Überprüfen Sie **Mesh erneut importieren**, und stellen Sie sicher, dass die richtige Datei importiert wird.

Ein erneutes Importieren des Gitters ist häufig nützlich, wenn Sie Folgendes benötigen:

* Aktualisieren der 3D-Modell-Topologie
* Aktualisieren der UVs
* [Textursätze](texture-set/texture-set.md) hinzufügen oder entfernen

| **Parameter** | **Beschreibung** |
| --- | --- |
| **3D-Mesh** | Gibt den Pfad zur 3D-Modelldatei an. Verwenden Sie die **Schaltfläche &quot;Auswählen&quot;**, um die Quelldatei für das Projekt zu ändern. |
| **Mesh erneut importieren** | Wenn diese Option aktiviert ist, wird die Gitterdatei erneut importiert, wenn Sie unten auf der Benutzeroberfläche auf &quot;OK&quot; klicken. Dieser Parameter wird automatisch überprüft, wenn die Schaltfläche &quot;Auswählen&quot; verwendet wird, um eine Gitterdatei anzugeben, die sich von der ursprünglichen Gitterdatei unterscheidet. |

>[!NOTE]
>
> Wenn sich die Material-IDs ändern oder beim Importieren des Projektgitters umbenannt werden, können die vorherigen Textursätze im Projekt deaktiviert werden, wodurch das Aussehen fehlender Texturen entsteht. Dies kann mit dem [Neuzuweisungsfenster](texture-set/texture-set-reassignment.md) aus der **Textursatzliste** behoben werden.

## Projekteinstellungen

Dieser Abschnitt steuert mehrere projektbezogene Einstellungen:

<table>
  <tr>
    <th><em>Einstellung</em></th>
    <th><em>Beschreibung</em></th>
  </tr>
  <tr>
    <td><strong>Normalen-Map-Format</strong></td>
    <td>Definiert das Format der Normalmap, die für das Gitter im Viewport verwendet wird. Dieser Parameter betrifft nur die <a href="shader-settings/shader-settings.md">Shader</a> in der Viewport- und Mesh-Maps in <a href="../baking/baking.md">bakers</a>. Der Ebenenstapel ist unabhängig. Empfohlener Wert für gängige Anwendungen:<br><br><ul><li><strong>Einheit</strong>: OpenGL</li><li><strong>Unreale Engine</strong>: DirectX</li><li><strong>Maya</strong>: OpenGL</li><li><strong>3DS Max.</strong>: DirectX</li><li><strong>Blender</strong>: OpenGL</li></ul></td>
  </tr>
  <tr>
    <td><strong>Berechnen des Tangentialraums pro Fragment</strong></td>
    <td>Bestimmt, wie Normalmaps im Viewport für Schattierung und Beleuchtung berechnet und angezeigt werden. Wenn diese Option aktiviert ist, werden die Tangente und die Binormale des Gitters pro Pixel und nicht pro Scheitelpunkt berechnet.<br>Empfohlener Wert für häufige Anwendungen:<br><br><ul><li><strong>Einheit</strong>: Deaktiviert (aktiviert, wenn HDRP verwendet wird)</li><li><strong>Unreale Engine</strong>: Aktiviert</li></ul></td>
  </tr>
</table>

>[!NOTE]
>
> Wenn Sie das Normalformat oder die Tangentenberechnung ändern, müssen Sie die Gitterzuordnungen erneut backen, um sicherzustellen, dass das Erscheinungsbild in den Viewports korrekt ist.

### Dateitypspezifische Einstellungen

Wenn ein USD-Gitterformat ausgewählt ist, werden andere dateitypspezifische Einstellungen verfügbar.

![](../assets/image2023-1-30-11-16-6.png){width="473px"}

<table>
  <tr>
    <th><em>Parameter</em></th>
    <th><em>Beschreibung</em></th>
  </tr>
  <tr>
    <td><strong>Umfang und Varianten</strong></td>
    <td>Wählen Sie einen bestimmten Teil einer USD-Datei aus. Standardmäßig ist sie auf "Root" festgelegt, was bedeutet, dass die gesamte USD-Datei im Painter-Projekt verwendet wird. <strong>Änderung...</strong> öffnet ein neues Fenster, in dem der Inhalt des USD angezeigt wird. Wenn Varianten erkannt werden, können Sie eine bestimmte Variante auswählen, die in das Projekt geladen werden soll.<br><br>Hinweis:<br><ul><li>Nur die Modellvariantenauswahl hat Auswirkungen.</li><li>Innerhalb von Varianten verschachtelte Varianten werden derzeit nicht erkannt.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Unterteilungsebene</strong></td>
    <td>Gilt für Geometrie mit Unterteilung. Geben Sie in Painter an, wie stark das Gitter für die Texturierung unterteilt werden soll. Wenn in der USD-Datei explizit "none" als Unterteilung festgelegt ist, wird diese Einstellung ausgegraut. Die Unterteilung wird nach dem UV-Entpacken angewendet, sodass die Form der UVs des Gitters nicht geändert wird.</td>
  </tr>
  <tr>
    <td><strong>Rahmen</strong></td>
    <td>Gilt für USDs, in denen Animationen erkannt werden. Wählen Sie den Frame aus, der in das Painter-Projekt geladen werden soll. Wenn die ausgewählte USD-Datei keine Animation enthält, ist diese Einstellung ausgegraut.</td>
  </tr>
</table>

## Einstellungen für UV-Kacheln

Dieser Abschnitt enthält Steuerelemente, mit denen Sie die Verwendung von UDIMs im Projekt umschalten können. Es ist nicht möglich, diese Einstellungen zu ändern, nachdem das Projekt erstellt wurde, aber Sie können die Einstellungen für das Projekt hier anzeigen. Weitere Informationen finden Sie in der Dokumentation zu [UV-Kacheln](../features/uv-tiles/uv-tiles.md).

## Importeinstellungen

Diese Einstellungen steuern, wie das ausgewählte Gitter importiert wird:

| *Einstellung* | *Beschreibung* |
| --- | --- |
| **Kameras importieren** | Wenn diese Option aktiviert ist, werden die in der Gitterdatei vorhandenen Kameras auch importiert und im 3D-Viewport verfügbar. |
| **Konturpositionen im Gitter beibehalten** | Diese Einstellung steuert, wie Pinselstriche nach dem Importieren eines neuen 3D-Gitters neu berechnet werden. Es wird empfohlen, diese Einstellung in den meisten Fällen aktiviert zu lassen. Weitere Informationen finden Sie in der Dokumentation [UV-Projektion](../features/uv-reprojection.md). |
| **Automatisches Ausgliedern** | Automatisches Ausgliedern von UV-Licht. Klicken Sie auf die Schaltfläche Option, um den Prozess zu konfigurieren. Weitere Informationen finden Sie in der [Dokumentation zum automatischen Ausgliedern von UVs](../features/automatic-uv-unwrapping.md). |

### Physische Größe

Passen Sie die [Physische Größe](../features/physical-size.md) des importierten Gitters an.

| *Einstellung* | *Beschreibung* |
| --- | --- |
| **Interne Einheitenskalierung der Gitterdatei verwenden** | Wenn das Gitter mit physikalisch akkuraten Messungen erstellt wurde, lassen Sie diese Option aktiviert, um dieselbe Physische Größe in Painter beizubehalten. |
| **Benutzerdefinierte Einheitenskalierung** | Wenn das Gitter nicht unter Berücksichtigung der Physische Größe erstellt wurde, können Sie mit dieser Option die Größe des Gitters anpassen. Sie müssen die gewünschte Physische Größe und die Größe (in Einheiten) des importierten Gitters kennen, um diesen Wert zu bestimmen. |
| **Skalierung der Füllebenen auf Physische Größe umstellen, wenn Materialien zugewiesen werden** | Wenn diese Option aktiviert ist, wechseln Füllebenen und -effekte automatisch die Skalierungsmethode in die Physische Größe, wenn Sie ein Material zuweisen, das Physische Größe-Eigenschaften aufweist. |

### Einstellungen für das Farbmanagement

Dieser Abschnitt steuert die Einstellungen für die Farbkonvertierung. Weitere Informationen finden Sie in der Dokumentation zum [Farbmanagement](../features/color-management/color-management.md).
