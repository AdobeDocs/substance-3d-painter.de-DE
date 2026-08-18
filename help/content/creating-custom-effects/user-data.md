---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/content/creating-custom-effects/user-data.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie Benutzerdaten in benutzerdefinierten Effekten für Substance 3D Painter verwenden, um benutzerdefinierte Informationen an Shader-Effekte zu übergeben.
helpx_creative_field: ""
helpx_description: Painter > Content > Creating custom effects > User data
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Benutzerdaten
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '1175'
ht-degree: 1%

---


# Benutzerdaten

Auf dieser Seite werden benutzerdefinierte Eigenschaften (Benutzerdaten) beschrieben, die dem Substance-Diagramm hinzugefügt werden können, um bestimmte Verhaltensweisen auszuführen.\
Die Benutzerdateneinstellungen werden in der Regel auf Eingabe- oder Ausgabeknoten eines Diagramms angewendet, um anzugeben, wie die Anwendung sie interpretieren soll. Dies ermöglicht es, die Eingabe eines Diagramms anzufordern, um auf eine bestimmte Weise Effekte anzuwenden, ist ein bekannter Kontext (z. B.: die Anforderung eines bestimmten Farbraums) oder die Angabe, wie eine Ausgabe erstellt wurde, falls die Anwendung danach zusätzliche Konvertierungen anwenden muss.

* Dateneinstellungen verwenden sind als **Schlüssel = Wert** definiert.
* Mehrere Einstellungen werden durch ein Semikolon ( **;** ) getrennt.

## Farbraum

Die Einstellung **Farbraum** kann verwendet werden, um Substance-Diagrammeingaben mit einem bestimmten Farbraum anzufordern oder eine Ausgabe zu definieren, die auf eine bestimmte Art konfiguriert ist. Beispiel: Angeben des Formats der normalen Map-Ausgabe.

Syntaxbeispiel: **colorspace=$working**

Kontextübersicht:

* **Farbschaltfläche**: Ein Farbschaltflächen-Widget in den Eigenschaften eines Substance-Diagramms.
* **Diagrammeingabe/-ausgabe**: Eingangs- oder Ausgangsknoten eines Graphen, der mit einem Kanal verbunden ist (z. B.: BaseColor).
* **Image-Eingabe**: generische Eingabe eines Graphen, die nicht mit bestimmten Kanälen zusammenhängt.

>[!NOTE]
>
> Mit der Einführung des Farbmanagements haben sich mehrere Verhaltensweisen im Zusammenhang mit der Farbraumeinstellung geändert:
> 
> * In der folgenden Tabelle werden zuerst die Farbraumeinstellungen aufgeführt, die vor Version 8.1 kompatibel sind. Der zweite Abschnitt gilt ausschließlich für Version 8.1 und höher.
> * In Bezug auf die Kontexte, in denen die Farbraumeinstellung verwendet werden kann, nur da in Version 8.1 Farbschaltflächen einen Farbraum definieren können. In früheren Versionen wurde davon ausgegangen, dass sie sich im Anzeigebereich (sRGB) befinden.
> 
> **snorm** und **unorm** Farbraum/Transformationen sollten nicht mit GPU-Texturformaten gemischt werden. Ihr Zweck ist unterschiedlich.

| ColorSpace | Kontextverfügbarkeit | Beschreibung |
| --- | --- | --- |
| **auto** | Farbschaltfläche Diagrammeingabe/-ausgabe Bildeingabe | Standard. Die Anwendung entscheidet, welche Farbraumkonvertierung durchgeführt wird, abhängig von den Eigenschaften des Eingabeknotens und dem Bild, das an den Eingang angeschlossen ist. |
| **linear** | Farbschaltfläche Diagrammeingabe/-ausgabe Bildeingabe | Standard-sRGB IEC 61966-2-1:1999-Farbraum mit linearer Gamma-/Tonwertkurve. Nur verfügbar mit dem Farbmanagementmodus **Legacy**. |
| **srgb** | Farbschaltfläche Diagrammeingabe/-ausgabe Bildeingabe | sRGB IEC 61966-2-1:1999-Farbraum. Nur verfügbar mit dem Farbmanagementmodus **Legacy**. |
| **Kennwort** | Farbschaltfläche Diagrammeingabe/-ausgabe Bildeingabe | Veraltet. Wird als **linear** im alten Farbmanagementmodus und **raw** mit OCIO/ACE interpretiert. Sollte stattdessen durch **raw** ersetzt werden. |
| **snorm** | Diagrammeingabe/-ausgabe Bildeingabe | Signiert normalisiert. Anfordern, dass das Eingabebild im Bereich [0, 1] liegt. Bei 8-Bit-Eingabebildern bedeutet dies, dass der mittlere Wert 127 ist. Bei schwebenden Bildeingaben beträgt die mittlere 0,5 und es erfolgt keine Klemmung. |
| **normalxyzright** | Diagrammeingabe/-ausgabe Bildeingabe | OpenGL-Normalen-Map-Format. |
| **normalxyzleft** | Diagrammeingabe/-ausgabe Bildeingabe | DirectX Normalen-Map-Format. |
|  |  |  |
| **unorm** | Diagrammeingabe/-ausgabe Bildeingabe | Schwimmereingang, ohne Bereich/Klemmung. |
| **Daten** | Farbschaltfläche Diagrammeingabe/-ausgabe Bildeingabe | Nicht signiert, normalisiert oder Gleitkommawert. Informationen ohne Farbe. |
| **raw** | Farbschaltfläche Diagrammeingabe/-ausgabe Bildeingabe | Bei Verwendung dieser Einstellung werden keine Farbtransformationen angewendet. |
| **$standardsrgb** | Farbschaltfläche Diagrammeingabe/-ausgabe Bildeingabe | sRGB IEC 61966-2-1:1999-Farbraum. |
| **$Working** | Farbschaltfläche Diagrammeingabe/-ausgabe Bildeingabe | Der Arbeitsfarbraum hängt von den Farbmanagementeinstellungen ab. Sind identisch mit Daten für nicht farbverwaltete Kanäle und Monokanal (Schablone, Alpha, Maske) |
| **$raw** | Farbschaltfläche Diagrammeingabe/-ausgabe Bildeingabe | Alias für **RAW**. |
| **$auto** | Farbschaltfläche Diagrammeingabe/-ausgabe Bildeingabe | Alias für **auto**. |

## Alpha

Die Einstellung **alpha** kann verwendet werden, um anzugeben, wie das Alpha einer Farbeingabe oder -ausgabe (RGBA) kombiniert wird.

Syntaxbeispiel: **alpha=premultiplied**

| Einstellung | Beschreibung |
| --- | --- |
| gerade | Fordern Sie einen geraden Wert an, oder definieren Sie den Alphawert. |
| vormultipliziert | Anfordern oder definieren Sie den Alpha-Wert als vormultipliziert. |
| Keine | Passthrough, verwenden Sie das angegebene Alpha wie vorhanden. |

>[!NOTE]
>
> Der Kanal **Deckkraft** gilt standardmäßig als **gerade**.

## Standardfarbe für Bildeingabe

Die Standardfarbe eines Substance-Diagrammbildes ist Schwarz, wobei der Alphawert auf 0 gesetzt ist. Mit der Einstellung **defaultcolor** kann ein anderer Wert definiert werden, wenn die Bildeingabe eines Diagramms leer ist.

Gleitende Werte (Bereich [0, 1]) oder ganzzahlige Werte (Bereich [0, 255]) können verwendet werden, um die Farbe anzugeben. Jeder Komponentenwert ist durch ein Komma getrennt, während Gleitkommawerte einen Punkt als Dezimaltrennzeichen verwenden. Wenn ein Gleitkomma keinen Punkt hat, wird es als Ganzzahl betrachtet.

Syntaxbeispiel:

* **defaultcolor=(1.0,0.5,0.0)**
* **defaultcolor=(0,128,255)**

## Bildeingabenabstände

Standardmäßig haben Bildeingaben eines Substance-Graphen keine Auffüllung, der Bereich außerhalb der UV-Insel wird aus Leistungsgründen in der Regel mit einer einheitlichen Farbe gefüllt. Die Füllungseinstellung kann stattdessen verwendet werden, um eine unendliche Dilatation anzufordern, die für Filter verwendet werden kann, um z. B. das Erzeugen von Nähten zu vermeiden.

Syntaxbeispiel: **p**&#x200B;**adding=extend**

## Deaktivieren einer Ausgabe standardmäßig

Beim Hinzufügen einer Substanz in einen Schlitz (wie der Materialschlitz des Werkzeugs einer Füllschicht) kann über das Metadaten-Textfeld angegeben werden, dass kein bestimmter Kanal aktiviert werden soll:

* Auf einem bestimmten Ausgabeknoten (wie ein Material) :  **disable=(true)**
* Auf einem generischen Ausgabeknoten (wie bei einem Filter) :  **disable=(Height,diffuse,Specular)**

Beim Laden der Substanz wird dieser Kanal nicht in der Benutzeroberfläche aktiviert und hat daher keine Auswirkungen auf den Ebenenstapel. Der Benutzer kann den Kanal weiterhin wieder aktivieren.

## Ausgabe als gemeinsame Maske/Alpha-Maske festlegen

Die Ausgabe eines Substance-Graphen kann als gemeinsamer Alphakanal/Maske auf den anderen Ausgaben verwendet werden.

Dazu gibt es zwei Möglichkeiten:

* Erstellen Sie einen Ausgabeknoten mit der Kennung **Channels\_Alpha**.
* Oder fügen Sie die folgenden Benutzerdaten zu einem bestimmten Ausgabeknoten hinzu:  **IsChannelsAlpha=true**

Es können einige Bedingungen gelten:

* Wenn ein Ausgabeknoten mit der Kennung **Channels\_Alpha** vorhanden ist und andere Ausgaben nicht über die Benutzerdaten verfügen, wird dieser Knoten als Kanalmaske verwendet.
* Wenn eine Ausgabe über die Benutzerdaten verfügt, wird sie als Kanalmaske verwendet, solange kein Knoten **Channels\_Alpha** vorhanden ist.
* Wenn sowohl ein **Channels\_Alpha**-Knoten als auch ein Knoten mit den Benutzerdaten vorhanden ist, wird zuerst der **Channels\_Alpha**-Ausgabeknoten verwendet.
* Wenn die Benutzerdaten über mehrere Knoten verfügen, wird der erste von der Anwendung gefundene Knoten als Kanalmaske verwendet. Die Reihenfolge, in der die Ausgaben gefunden werden, ist nicht unbedingt dieselbe wie im Substance-Diagramm.

>[!NOTE]
>
> Diese Einstellungen gelten nur für das Substance-Diagramm, das im **Materialmodus** verwendet wird. Es gilt nicht für Filter, Generatoren usw.

## Standardfüllmodus für Materialausgaben festlegen

Es ist möglich festzulegen, wie die Füllmethode einer bestimmten Ausgabe in einem Substance-Diagramm aussehen soll, wenn Sie Materialien vom Shelf in den Viewport oder Ebenenstapel ziehen und ablegen.

* Auf einem bestimmten Ausgabeknoten:  **blendingmode=normal**

Liste der unterstützten Füllmethoden:

* normal
* Passthrough
* deaktivieren
* ersetzen
* multiplizieren
* teilen
* inversedividieren
* verdunkeln
* aufhellen
* Linearumgehung
* subtrahieren
* umgekehrt subtrahieren
* Differenz
* Ausschluss
* unterschriebene Addition
* Überlagerung
* Gitter
* Linearburn
* Buntbrand
* Farbabdruck
* Weichlicht
* grelles Licht
* hell
* Nadellicht
* Tönung
* Sättigung
* Farbe
* Wert
* Normalkombination
* Normaldetail
* Normalinversedetail
