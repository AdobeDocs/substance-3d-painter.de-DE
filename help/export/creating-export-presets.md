---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/getting-started/export/creating-export-presets.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie in Substance 3D Painter benutzerdefinierte Ausgabevorlagen erstellen, um Ihre eigenen Texturexportkonfigurationen zu definieren.
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
* <b>Ausgabetexturliste </b>: (Mitte) den Inhalt einer ausgewählten Vorgabe und zeigt die Benennungskonvention und die Optionen für das Kanal-Packing an.
* <b>Kanalliste</b> und <b>Konvertierte Texturen</b>: (rechts) Liste der Kanäle und Strukturen, die zum Zusammensetzen des Inhalts einer exportierten Textur verwendet werden sollen.

![](../assets/image2018-4-25-13-36-44.png){width="800px"}

>[!NOTE]
>
> Ausgabevorlagen werden auf dem Datenträger als <b>Einzeldateien</b> gespeichert und können für andere Substance 3D Painter-Benutzer freigegeben werden.\
> Die lokalen Dateien für benutzerdefinierte Vorlagen, die Sie erstellt haben, finden Sie im Ordner assets/export-presets Ihrer [Substance 3D Painter-Dateien](../pipeline-and-integration/resource-management/shelf-and-assets-location.md).

>[!NOTE]
>
> Wenn eine Vorlage zum Exportieren von Texturen verwendet wird, wird die Vorlagendatei in nachfolgenden Speichern automatisch in die Projektdatei aufgenommen.\
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

Nachdem eine Karte erstellt wurde, ist es möglich, sie zu benennen und dann Eingabemaps in einen der verfügbaren Kanalsteckplätze zu ziehen und abzulegen.\
Sobald eine Eingabemap in den Abschnitt &quot;Ausgabemaps&quot; abgelegt wurde, wird ein Menü geöffnet, in dem Sie gefragt werden, welcher Inhaltstyp in diesen Steckplatz geladen werden soll.

Die Optionen reichen von <b>RGB</b> und <b>individual</b>-Kanälen bis zum <b>Alpha</b> und der <b>Graustufen</b>-Konvertierung der Eingabe.

>[!NOTE]
>
> Jedes Mal, wenn eine Eingabemap gezogen und abgelegt wird, wird eine zufällige Farbe generiert. Dadurch erhalten Sie einen visuellen Hinweis für die Kanäle und die entsprechende Eingabezuordnung, die geladen wird.\
> Die Schaltfläche zeigt auch an, was in den Steckplatz geladen wird:
> 
> * Hintergrundfarbe: zeigt an, welche <b>Eingabe</b>-Zuordnungen geladen sind.
> * RGB: zeigen an, dass die <b>R</b>-, <b>G</b>- und <b>B</b>-Kanäle aus der Eingabezuordnung geladen sind.
> * Roter Balken: zeigen an, dass der <b>rote</b> Kanal aus der Eingabezuordnung geladen ist.
> * Grüne Leiste : zeigen an, dass der <b>grüne</b> Kanal aus der Eingabezuordnung geladen ist.
> * Blue bar: zeigen an, dass der <b>blaue</b> Kanal aus der Eingabezuordnung geladen ist.
> * Graue Leiste: geben an, dass die Eingabezuordnung als <b>Graustufen</b> geladen ist (entweder von einer RGB-in-Graustufen-Konvertierung oder weil die Eingabe bereits in Graustufen vorliegt).
> * Schwarz-Weiß-Linie: zeigt an, dass der <b>Alpha</b>-Kanal aus der Eingabezuordnung geladen ist. In Substance 3D Painter entspricht das Alpha einer Eingabe der gesamten gemalten Fläche.

## Benennen von Ausgabemaps

![](../assets/output-name.gif)

Einige Flags sind verfügbar, um den Namen der Textur während des Exportvorgangs automatisch zu generieren.

* <b> $mesh</b> : Name der im Projekt geladenen Gitterdatei
* <b> $textureSet</b> : Name des Struktursatzes
* <b> /</b> (Schrägstrich): Ordnerseparation

<b> Beispiel </b> : cymourai.fbx mit einem Textursatz namens &quot;MaterialBase&quot;

* <b>$mesh\_$textureSet\_BaseColor</b> generiert <b>cymourai\_MaterialBase\_BaseColor.png.</b>
* <b>$mesh/$textureSet\_BaseColor</b> generiert einen Ordner mit dem Namen <b>cymourai</b>, in dem sich eine Textur mit dem Namen <b>MaterialBase\_BaseColor.png</b> befindet.

>[!NOTE]
>
> Ordner werden automatisch als Gruppen konvertiert, falls das Exportformat auf das Dateiformat **PSD** (Photoshop) festgelegt ist.

## Zuweisen von Kanälen zu Ausgabemaps

![](../assets/empty-channel.gif)

Es ist möglich, einige Kanäle (der Ausgabemap) vollständig leer zu lassen. In diesem Fall wird eine Standardfarbe zugewiesen.

>[!NOTE]
>
> Wenn sich ein Slot auf einen Kanal bezieht, der während des Exports nicht im Textursatz vorhanden ist, wird auch eine Standardfarbe generiert.\
> Diese Farbe ändert sich je nach Kanal, der den besten neutralen Wert ergibt.\
>  **Beispiel** : Wenn das Height fehlt, wird der Kanal mit einem Grauwert erzeugt.

Es gibt verschiedene Arten von Karten:

* <b>Eingabemaps</b>: direkte Kanäle, die in einem Textursatz hinzugefügt werden können. Über das Einstellungsbedienfeld TextureSet.
* <b> Mesh Maps</b>: Texturen, die in den zusätzlichen Kartenschlitzen eines Textursatzes vorhanden sind (gebackene Texturen).
* <b> konvertierte Karten:</b> virtuelle Texturen, diese werden während des Exports basierend auf den im Dokument vorhandenen Kanälen generiert.
  * <b>Normales OpenGL/DirectX</b> : Gibt eine Normale im dedizierten Raum aus, indem die Normale aus den zusätzlichen Karten, dem Height und dem Normalkanal kombiniert wird.
  * <b>Gemischte AO</b>: Kombinieren Sie die zusätzliche Umgebungskarte mit dem Kanal für die Verdeckung der Verdeckung.
  * <b>Diffus</b>: Diffuse Farbe, die aus den BaseColor- und Metallic-Kanälen generiert wird (metallische Teile werden durch eine schwarze Farbe ersetzt).
  * <b>Specular</b>: Specular-Farbe, die aus den BaseColor- und Metallic-Kanälen generiert wird.
  * <b>Glossarität</b>: Umgekehrt der Raueitskanal.
  * <b>Unity4 Diffuse</b>: Diffuse Farbe, die von der BaseColor generiert wurde, um Unity4-Shadern zu entsprechen.
  * <b>Unity4 Gloss</b>: Glanzlichtschärfe, die aus dem Kanal &quot;Raueit&quot; und &quot;Metallisch&quot; generiert wird, um Unity4-Shadern zu entsprechen.
  * <b>Reflexion</b>: Exportieren einer Karte, bei der Weiß auf ein dielektrisches Material und andere Farben für metallische Materialien hinweist
  * <b>1/ior</b>: 1 dividiert durch den älteren Wert, der aus der metallischen Karte generiert wird: 1.4 für Dielektrika, 100 für Metalle (schwarze Farbe)
  * <b>Glossarität<sup>2</sup></b>: Quadratische Version des Glanzkanals (Glanzgrad \* Glanzgrad)
  * <b>f0</b>: Reflexionswert bei Fresnel 0 (0,04 für Dielektrika, 1,0 für Metallic)
