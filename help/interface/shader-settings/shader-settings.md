---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/interface/shader-settings.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie in Substance 3D Painter die Shader-Einstellungen konfigurieren, um das Rendern von Materialien und das Erscheinungsbild anzupassen.
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

Das Fenster &quot;**Shaders Settings**&quot; ermöglicht die Steuerung der Parameter &quot;Shader&quot; (und &quot;Iray mdl&quot;) und der Parameter &quot;Geometrie-Versatz&quot;.

Ein Shader ist eine Funktion, die definiert, wie ein Objekt aussehen soll, wenn es mit Licht und Schatten in den Viewporten interagiert. In dieser Anwendung werden Shader verwendet, um zu wissen, wie die Textursatz-Kanäle zu lesen und den 3D-Mesh in den Viewporten zu rendern.

## Stapel und Shader rückgängig machen

![](../../assets/shader-undo.png)

Dieser Abschnitt im Fenster &quot;Shader-Einstellungen&quot; steuert die Hauptparameter beim Bearbeiten von Shadern.\
Der Stapel &quot;Rückgängig/Wiederholen&quot; für den Shader ist unabhängig vom Hauptverlauf [1}, sodass beim Malen keine Konflikte entstehen.](https://substance3d.adobe.com/display/DRAFTPAINTER/History)

Wenn die Shader-Datei als &quot;Veraltet&quot; markiert ist, wird empfohlen, sie nach Möglichkeit zu aktualisieren. Siehe :  [Shader wird aktualisiert](https://substance3d.adobe.com/display/DRAFTPAINTER/Updating+a+Shader)

| *Einstellung* | *Beschreibung* |
| --- | --- |
| **Rückgängig** | Shader-Dateiänderung oder Shader-Parameteränderung rückgängig machen/rückgängig machen |
| **Wiederholen** | Wenden Sie erneut eine Änderung an, die über die Funktion &quot;Rückgängig&quot; abgebrochen wurde. |
| **Shader-Datei** | Schaltfläche mit der aktuell verwendeten Shader-Datei. Klicken Sie auf den Knopf, um ein Mini-Regal zu öffnen und einen anderen Shader zu wählen. |
| **Instanzname** | Name der Shader-Instanz. |
| **Standardwerte wiederherstellen** | Stellen Sie die Standardwerte aller Shader-Parameter wieder her (wie in der Shader-Datei). |

### Shader-Instanz

Eine Shader-Instanz ist ein Shader, der auf einer originalen Shader-Datei basiert, jedoch benutzerdefinierte Parameter aufweist. Eine Shader-Instanz kann für mehrere Textursatz freigegeben werden, und ein Textursatz kann eine eindeutige Shader-Instanz haben.

**Beispiel:** Ein Projekt kann einen Basis-Shader verwenden, während ein Textursatz einen benutzerdefinierten Shader verwendet, um die Deckkraft zu unterstützen.

Informationen zum Erstellen und Verwalten von Shader-Instanzen finden Sie im Fenster &quot;[Textursatz list](../texture-set/texture-set-list.md)&quot;.

## Shader-Parameter

![](../../assets/shader-parameters-1.png)

Shader-Parameter hängen von der aktuell geladenen Shader-Datei ab.

## Versatz und Tesselierung

![](../../assets/disp-parameters.png)

Versatz und Tesselierung sind zwei Funktionen, mit denen Sie die Form eines Objekts ändern können, um weitere Details hinzuzufügen.

* **Versatz**: Schieben oder verschieben Sie die Geometrie basierend auf einem Eingabekanal.
* **Tesselation**: Unterteilen Sie die Geometrie, um sie zu verdichten. Mehr Dichte bedeutet, dass der Abstand zwischen den Polygonen kleiner ist, wodurch feinere Details entstehen.

Ein Filter mit dem Namen &quot;**Height in Normal**&quot; ist im Regal verfügbar und kann verwendet werden, um die endgültige Normalen-Map abzurufen (falls die native Konvertierung nicht stark genug ist).

### Verschiebung

Im Folgenden finden Sie die Einstellungen für Versatz:

| *Einstellung* | *Beschreibung* |
| --- | --- |
| <b> Quellkanal </b> | Kanal, auf dem die Mesh-Deformation basiert. Der Standardwert ist &quot;Height&quot;, kann aber auch auf &quot;Versatz&quot; festgelegt werden. |
| <b>Einheit skalieren</b> | Legen Sie fest, wie die Versatz-Skalierung definiert wird:<ul data-preserve-html="true"> <li data-preserve-html="true"><b>Normalisiert: Die </b>-Versatz-Skala ist relativ zur Größe des Begrenzungsrahmens des Meshs.</li> <li data-preserve-html="true"><b>Szene: Die </b>-Versatz-Skalierung ist relativ zu den Einheiten der importierten Szene.</li> <li data-preserve-html="true"><b>Physische Größe (cm)</b>: Der Maßstab des Versatzes wird in cm anhand der Physische Größe des Objekts gemessen.</li> </ul> |
| <b> Skalierungsbetrag </b> | Steuert den Grad der Verformung, die auf den Mesh im Projekt angewendet wird, basierend auf der ausgewählten Skalierungseinheit. |

>[!NOTE]
>
> Für die <b>Szene</b> und die <b>Physische Größe (cm) </b>Skalierungseinheitseinstellungen ist es erforderlich, dass das importierte Modell für die Messung der Physische Größe vorbereitet wurde. Wenn die Maßeinheiten in der importierten Physische Größe nicht korrekt eingerichtet sind oder der importierte Dateityp die Maßeinheiten nicht unterstützt, funktioniert der Versatz weiterhin. Unter Umständen werden die Ergebnisse jedoch nicht an Ihre Anforderungen angepasst.

### Tessellierung

Im Folgenden sind die Einstellungen für die Tesselierung aufgeführt:

| *Einstellung* | *Beschreibung* |
| --- | --- |
| **Unterteilungsmodus** | Bestimmt, wie der Betrag der Unterteilung berechnet wird. Verfügbare Konfigurationen sind:<ul data-preserve-html="true"><li data-preserve-html="true"> Einheitlich (Standard) </li><li data-preserve-html="true"> Kantenlänge </li></ul> |
| **Anzahl der Unterteilungen** | (Modus gleichmäßig) Von 1 bis 32. Bei einem hohen Wert werden mehr Polygone erzeugt, die mehr Details enthalten, aber Leistungsprobleme verursachen können. |
| **Maximale Länge** | (Modus Kantenlänge)1 / Wert. Jeder Polygonrand wird unterteilt, bis jedes Segment dieser Zahl entspricht oder kleiner ist; 1/1 ist dabei die Größe der Szene. |
