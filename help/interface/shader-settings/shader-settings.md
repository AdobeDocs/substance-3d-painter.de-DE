---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/interface/shader-settings.html"
breadcrumb-title: ''
description: Lerne, wie du in Substance 3D Painter die Shader-Einstellungen für die Anpassung von Rendering und Erscheinungsbild von Material änderst.
helpx_creative_field: ""
helpx_description: Painter > Interface > Shader settings
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Shader-Einstellungen
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '633'
ht-degree: 5%

---


# Shader-Einstellungen

![](../../assets/shader-settings.png)

Das Fenster &quot;**Shaders Settings**&quot; ermöglicht die Steuerung der Parameter &quot;shader&quot; (und &quot;Iray mdl&quot;) sowie der Parameter für den Geometrie-Versatz.

Ein Shader ist eine Funktion, die definiert, wie ein Objekt aussehen soll, wenn es mit Beleuchtung und Schatten in den Viewports interagiert. In dieser Anwendung werden Shader verwendet, um zu wissen, wie die Textursatz-Kanäle gelesen und das 3D-Gitter in den Viewports gerendert werden.

## Stapel- und Shader-Datei rückgängig machen

![](../../assets/shader-undo.png)

Dieser Abschnitt des Fensters &quot;Schattierungseinstellungen&quot; steuert die Hauptparameter bei der Bearbeitung von Schattierungen.\
Der Stapel &quot;Rückgängig/Wiederholen&quot; für den Shader ist vom [Hauptverlauf](https://substance3d.adobe.com/display/DRAFTPAINTER/History) unabhängig, sodass beim Malen keine Konflikte entstehen.

Wenn die Shader-Datei als &quot;Veraltet&quot; markiert ist, wird empfohlen, sie nach Möglichkeit zu aktualisieren. Siehe :  [Shader wird aktualisiert](https://substance3d.adobe.com/display/DRAFTPAINTER/Updating+a+Shader)

| *Einstellung* | *Beschreibung* |
| --- | --- |
| **Rückgängig** | Änderungen an der Shader-Datei oder an Shader-Parametern rückgängig machen/abbrechen |
| **Wiederholen** | Wenden Sie erneut eine Änderung an, die über die Funktion &quot;Rückgängig&quot; abgebrochen wurde. |
| **Shader-Datei** | Schaltfläche, die die aktuell verwendete Shader-Datei anzeigt. Klicken Sie auf die Schaltfläche, um ein Mini-Regal zu öffnen und einen anderen Shader auszuwählen. |
| **Instanzname** | Name der Shader-Instanz. |
| **Standardwerte wiederherstellen** | Stellen Sie die Standardwerte aller Shader-Parameter wieder her (wie in der Shader-Datei). |

### Shader-Instanz

Eine Shader-Instanz ist ein Shader, der auf einer ursprünglichen Shader-Datei basiert, jedoch benutzerdefinierte Parameter aufweist. Eine Shader-Instanz kann für alle Textursätze freigegeben werden, und ein Textursatz kann eine eindeutige Shader-Instanz haben.

**Beispiel:** Ein Projekt kann einen Basis-Shader verwenden, während ein Textursatz einen benutzerdefinierten Shader verwendet, um die Deckkraft zu unterstützen.

Informationen zum Erstellen und Verwalten von Shader-Instanzen finden Sie im Fenster [Textursatz-Liste](../texture-set/texture-set-list.md).

## Shader-Parameter

![](../../assets/shader-parameters-1.png)

Shader-Parameter sind von der aktuell geladenen Shader-Datei abhängig.

## Versatz und Tesselierung

![](../../assets/disp-parameters.png)

Versatz und Tesselierung sind zwei Funktionen, mit denen Sie die Form eines Objekts ändern können, um weitere Details hinzuzufügen.

* **Versatz**: Schieben oder verschieben Sie die Geometrie basierend auf einem Eingabekanal.
* **Tesselation**: Unterteilen Sie die Geometrie, um sie zu verdichten. Mehr Dichte bedeutet, dass der Abstand zwischen den Polygonen kürzer ist, was feinere Details ergibt.

Ein Filter mit dem Namen &quot;**Height zu Normal**&quot; ist im Shelf verfügbar und kann verwendet werden, um die endgültige Normalzuordnung abzurufen (falls die native Konvertierung nicht stark genug ist).

### Verschiebung

Im Folgenden finden Sie die Einstellungen für Versatz:

| *Einstellung* | *Beschreibung* |
| --- | --- |
| <b> Quellkanal </b> | Kanal, auf dem die Gitterverformung basiert. Der Standardwert ist &quot;Height&quot;, kann aber auch auf &quot;Versatz&quot; festgelegt werden. |
| <b>Einheit skalieren</b> | Legen Sie fest, wie die Versatz-Skalierung definiert wird:<ul data-preserve-html="true"> <li data-preserve-html="true"><b>Normalisiert: Die </b>-Versatz-Skala ist relativ zur Größe des Begrenzungsrahmens des Gitters.</li> <li data-preserve-html="true"><b>Szene: Die </b>-Versatz-Skalierung ist relativ zu den Einheiten der importierten Szenendatei.</li> <li data-preserve-html="true"><b>Physische Größe (cm)</b>: Der Maßstab des Versatzes wird in cm anhand der Physische Größe des Objekts gemessen.</li> </ul> |
| <b> Skalierungsbetrag </b> | Steuert den Grad der Verformung, die auf das Gitter im Projekt angewendet wird, basierend auf der ausgewählten Skalierungseinheit. |

>[!NOTE]
>
> Für die <b>Szeneneinstellungen</b> und die <b>Physische Größe (cm) </b>Maßeinheit muss das importierte Modell für die Messung der Physische Größe vorbereitet werden. Wenn die Maßeinheiten in der importierten Physische Größe nicht korrekt eingerichtet sind oder der importierte Dateityp die Maßeinheiten nicht unterstützt, funktioniert der Versatz weiterhin. Unter Umständen werden die Ergebnisse jedoch nicht an Ihre Anforderungen angepasst.

### Tessellierung

Im Folgenden sind die Einstellungen für die Tesselierung aufgeführt:

| *Einstellung* | *Beschreibung* |
| --- | --- |
| **Unterteilungsmodus** | Bestimmt, wie der Betrag der Unterteilung berechnet wird. Verfügbare Konfigurationen sind:<ul data-preserve-html="true"><li data-preserve-html="true"> Einheitlich (Standard) </li><li data-preserve-html="true"> Kantenlänge </li></ul> |
| **Anzahl der Unterteilungen** | (Modus gleichmäßig) Von 1 bis 32. Bei einem hohen Wert werden mehr Polygone erzeugt, die mehr Details enthalten, aber Leistungsprobleme verursachen können. |
| **Maximale Länge** | (Modus Kantenlänge)1 / Wert. Jeder Polygonrand wird unterteilt, bis jedes Segment dieser Zahl entspricht oder kleiner ist; 1/1 ist dabei die Größe der Szene. |
