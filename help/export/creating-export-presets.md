---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/getting-started/export/creating-export-presets.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie benutzerdefinierte Ausgabevorlagen in Substance 3D Painter erstellen, um Ihre eigenen Exportkonfigurationen für Texturen zu definieren.
helpx_creative_field: ""
helpx_description: Painter > Getting Started > Export > Creating Output templates
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Erstellen von Ausgabevorlagen
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '963'
ht-degree: 0%

---


# Ausgabevorlagen erstellen

Auf dieser Seite wird erläutert, wie benutzerdefinierte Ausgabevorlagen erstellt und geändert werden. Ausgabevorlagen steuern die Benennung und Konfiguration der exportierten Texturen. Mit einer benutzerdefinierten Ausgabevorlage können Sie Ihre Exporte so konfigurieren, dass sie perfekt zu Ihrem Workflow passen.

Die Registerkarte &quot;Konfiguration&quot; des Exportfensters ist in drei Hauptteile unterteilt:

* <b>Die Vorgabenliste:</b> (links) ermöglicht es, die zu bearbeitende oder zu duplizierende Vorlage auszuwählen und vorhandene Vorlagen umzubenennen.
* <b>Textur der Ausgabe</b>: (Mitte) den Inhalt einer ausgewählten Vorgabe und zeigt die Benennungskonvention und die Optionen für das Kanal-Packing an.
* <b>Kanalliste</b> und <b>Konvertierte Texturen</b>: (rechts) Liste der Kanäle und Texturen, die zum Zusammensetzen des Inhalts einer exportierten Textur verwendet werden sollen.

![](../assets/image2018-4-25-13-36-44.png){width="800px"}

>[!NOTE]
>
> Ausgabevorlagen werden auf dem Datenträger als <b>Einzeldateien</b> gespeichert und können für andere Substance 3D Painter-Benutzer freigegeben werden.\
> Die lokalen Dateien für benutzerdefinierte Vorlagen, die Sie erstellt haben, finden Sie im Ordner assets/export-presets Ihrer [Substance 3D Painter-Dateien](../pipeline-and-integration/resource-management/shelf-and-assets-location.md).

>[!NOTE]
>
> Wenn eine Vorlage zum Exportieren von Texturen verwendet wird, wird die Vorlagendatei bei nachfolgenden Speichervorgängen automatisch in die Projektdatei aufgenommen.\
> Dies ermöglicht die Freigabe und/oder das Verschieben eines Projekts auf einen anderen Computer, während die Vorlagen für den Export der Texturen beibehalten werden.\
> Nur die zuletzt verwendete Vorgabe wird im Projekt gespeichert. Wenn Substance 3D Painter jedoch eine Vorgabe mit demselben Namen erkennt, wird die Vorgabe innerhalb des Projekts in der Liste als &quot;Veraltet&quot; markiert.

## Erstellen einer Vorlage

Oben in der Liste der Vorgaben befinden sich drei Schaltflächen:

![](../assets/image2018-4-25-13-39-6.png)

* <b> Duplikat</b> : eine vorhandene Vorlage zu duplizieren.
* <b> Entfernen</b> : Löschen Sie alle ausgewählten Vorlagen.
* <b> Erstellen</b> : Erstellen Sie eine neue und leere Vorlage.

Sie können auch auf eine Vorlage doppelklicken oder <b>mit der rechten Maustaste auf &quot;</b>&quot; klicken, um den Namen einer Vorlage zu ändern.

## Erstellen von Ausgabemaps

Nachdem eine Vorlage ausgewählt wurde, können Sie neue Ausgabemaps mithilfe der entsprechenden Schaltflächen hinzufügen, die oben im mittleren Abschnitt des Fensters verfügbar sind.

![](../assets/output-buttons.png)

![](../assets/output-map.gif)

Nachdem eine Karte erstellt wurde, können Sie sie benennen und dann Eingabe-Map in einen der verfügbaren Kanalsteckplätze ziehen und dort ablegen.\
Sobald eine Eingabe-Map in den Abschnitt &quot;Ausgabemaps&quot; abgelegt wurde, wird ein Menü mit der Frage geöffnet, welcher Inhaltstyp in diesen Steckplatz geladen werden soll.

Die Optionen reichen von <b>RGB</b> und <b>individual</b>-Kanälen bis zum <b>Alpha</b> und der <b>Graustufen</b>-Konvertierung der Eingabe.

>[!NOTE]
>
> Jedes Mal, wenn eine Eingabe-Map per Drag &amp; Drop verschoben wird, wird eine zufällige Farbe generiert. Dadurch erhalten Sie einen visuellen Hinweis für die Kanäle und die zugehörige geladene Eingabe-Map.\
> Die Schaltfläche zeigt auch an, was in den Steckplatz geladen wird:
> 
> * Hintergrundfarbe: zeigt an, welche <b>Eingabe</b>-Zuordnungen geladen sind.
> * RGB: zeigen an, dass die <b>R</b>-, <b>G</b>- und <b>B</b>-Kanäle von der Eingabe-Map geladen sind.
> * Roter Balken: zeigen an, dass der <b>rote</b>-Kanal von der Eingabe-Map geladen ist.
> * Grüne Leiste : zeigen an, dass der <b>grüne</b>-Kanal von der Eingabe-Map geladen ist.
> * Blue bar: zeigen an, dass der <b>Blue</b>-Kanal von der Eingabe-Map geladen ist.
> * Graue Leiste: geben an, dass die Eingabe-Map als <b>Graustufen</b> geladen ist (entweder von einer RGB-in-Graustufen-Konvertierung oder weil die Eingabe bereits in Graustufen vorliegt).
> * Schwarz-Weiß-Linie: zeigen an, dass der <b>Alpha</b>-Kanal von der Eingabe-Map geladen ist. In Substance 3D Painter entspricht das Alpha einer Eingabe der gesamten gemalten Fläche.

## Benennen von Ausgabemaps

![](../assets/output-name.gif)

Einige Flags sind verfügbar, um den Namen der Textur während des Exportvorgangs automatisch zu generieren.

* <b> $Mesh</b> : Name der im Projekt geladenen Meshdatei
* <b> $textureSet</b> : Name des Textursatzes
* <b> /</b> (Schrägstrich): Ordnerseparation

<b> Beispiel </b> : cymourai.fbx mit einem Textursatz namens &quot;MaterialBase&quot;

* <b>$Mesh\_$textureSet\_BaseColor</b> generiert <b>Cymourai\_MaterialBase\_BaseColor.png.</b>
* <b>$Mesh/$textureSet\_BaseColor</b> generiert einen Ordner mit dem Namen <b>cymourai</b>, in dem sich eine Textur mit dem Namen <b>MaterialBase\_BaseColor.png</b> befindet.

>[!NOTE]
>
> Ordner werden automatisch als Gruppen konvertiert, falls das Exportformat auf das Dateiformat **PSD** (Photoshop) festgelegt ist.

## Zuweisen von Kanälen zu Ausgabemaps

![](../assets/empty-channel.gif)

Es ist möglich, einige Kanäle (der Ausgabemap) vollständig leer zu lassen. In diesem Fall wird eine Standardfarbe zugewiesen.

>[!NOTE]
>
> Wenn sich ein Slot auf einen Kanal bezieht, der während des Exports nicht im Textursatz vorhanden ist, wird ebenfalls eine Standardfarbe generiert.\
> Diese Farbe ändert sich je nach Kanal, der den besten neutralen Wert ergibt.\
>  **Beispiel** : Wenn das Height fehlt, wird der Kanal mit einem Grauwert erzeugt.

Es gibt verschiedene Arten von Karten:

* <b>Eingabe-Map</b>: Direktkanäle, die in einem Textursatz hinzugefügt werden können. Über das Einstellungsbedienfeld TextureSet.
* <b> Mesh-Map</b>: Texturen in den zusätzlichen Kartensteckplätzen eines Textursatzes (Baking geführt Texturen).
* <b> konvertierte Maps:</b> virtuelle Texturen. Diese werden während des Exports auf der Grundlage der im Dokument vorhandenen Kanäle generiert.
  * <b>Normales OpenGL/DirectX</b> : Gibt eine Normale im dedizierten Raum aus, indem die Normale aus den zusätzlichen Karten, dem Height und dem Normalkanal kombiniert wird.
  * <b>Gemischte AO</b>: Kombinieren Sie die zusätzliche Ambient occlusion-Map mit dem Ambient occlusion-Kanal.
  * <b>Diffuse</b>: Diffuse, die aus der BaseColor und den Metallic Kanälen generiert wird (metallic Teile werden durch eine schwarze ersetzt).
  * <b>Specular</b>: Specular-Farbe, die aus der BaseColor und Metallic Kanälen generiert wurde.
  * <b>Glanz</b>: Umgekehrt zur Rauheit.
  * <b>Unity4-Diffusen</b>: Von der BaseColor generierte Diffuse, die mit Unity4-Shadern übereinstimmt.
  * <b>Unity4 Gloss</b>: Glanz, der aus der Rauheit und dem Metallic Kanal generiert wird, um Unity4-Shadern zu entsprechen.
  * <b>Reflexion</b>: Exportieren einer Map, wobei Weiß ein dielektrisches Material und andere Farben für metallic Material angibt
  * <b>1/ior</b>: 1 dividiert durch den Seniorwert, Senior wird aus der metallic Karte generiert: 1.4 für Dielektrika, 100 für Metalle (schwarze Farbe)
  * <b>Glanz<sup>2</sup></b>: Quadratische Version des Glanz-Kanals (Glanz \* Glanz)
  * <b>f0</b>: Reflexionswert bei Fresnel 0 (0,04 für Dielektrika, 1,0 für metallic)
