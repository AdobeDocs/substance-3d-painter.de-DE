---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/painting/presets/creating-particles-presets/creating-a-new-particle-script.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie in Substance 3D Painter ein neues Partikelskript erstellen, um das Verhalten und die Effekte von benutzerdefinierten Partikelpinseln zu definieren.
helpx_creative_field: ""
helpx_description: Painter > Painting > Presets > Creating particles presets > Creating A New Particle Script
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Erstellen eines neuen Partikelskripts
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '728'
ht-degree: 0%

---


# Erstellen eines neuen Partikelskripts

Laden Sie das vorkonfigurierte PopcornFX-Paket herunter: [Templates\_EmitterReceiver.pkkg](https://helpx.adobe.com/content/dam/help/en/substance-3d/documentation/spdoc/files/67403778/68419585/1/1411557944000/templates-emitterreceiver.pkkg)

Dieses Paket ist ein &quot;Start-Kit&quot;, das einen Sender und einen Empfänger enthält, die wir in Substance 3D Painter bearbeiten und importieren werden.

## Popcorn-FX-Setup

Starten Sie den PopcornFX-Editor, erstellen Sie ein neues Projekt und öffnen Sie es.

Klicken Sie in Ihrem Projekt mit der rechten Maustaste auf einen leeren Bereich und wählen Sie &quot;Popcorn-Paket importieren&quot;. Wählen Sie dann &quot;Templates\_EmitterReceiver.pkkg&quot;.

Jetzt sollten Sie Folgendes haben:

* Ein Partikelsystem &quot;\_Emitter&quot;, das eine Basisvorlage eines Emitters ist.
* Ein Partikelsystem &quot;\_Receiver&quot;, das eine Basisvorlage eines Receivers ist.
* Ein Kugelgitter, das als Standardhintergrund der Szene verwendet wird

&quot;\_Emitter&quot; und &quot;\_Receiver&quot; sind bereits &quot;Painter ready&quot;. Sie wurden bereits mit den notwendigen Evolvern, Feldern, Hintergründen usw. konfiguriert.

## Ein Gitter importieren.

PopcornFX unterstützt nur **FBX** . Stellen Sie sicher, dass Sie das Gitter in diesem Format exportieren. Überprüfe während des Exportschritts die Größe deines Gitters, um es an die richtigen Einheiten in der &quot;realen Welt&quot; anzupassen.

Kopieren Sie es und fügen Sie es in den &quot;Meshes&quot;-Ordner Ihres Projekts ein (in PopcornFX können Sie mit der rechten Maustaste auf den &quot;Meshes&quot;-Ordner klicken und &quot;Dateispeicherort öffnen&quot; auswählen).

Kehren Sie zum Editor zurück, öffnen Sie das Gitter (doppelklicken Sie darauf) und klicken Sie auf &quot;**Build** &quot;. Schließen Sie das Fenster und speichern Sie die Änderung.

## Emitter/Receiver-Bearbeitung

Wir werden bestehende Partikelsysteme duplizieren und an die neuen Netze anpassen.

Klicken Sie mit der rechten Maustaste auf das Partikelsystem &quot;\_Emitter&quot; (im Ordner &quot;Partikel&quot;) und wählen Sie &quot;Klonen&quot; (oder &quot;Duplizieren&quot;), um Ihren eigenen Emitter zu erstellen.

Öffnen Sie sie und wählen Sie im Fenster &quot;Particle Treeview&quot; (unten links) &quot;**Layer\_Model** &quot; aus, das sich befinden soll in: &quot;Editor-Eigenschaften => Hintergrund => 3D-Ebenen&quot;.

Ersetzen Sie dann im Fenster &quot;Node Properties&quot; (Knoteneigenschaften) die Datei &quot;dummymesh.fbx&quot; durch Ihr Modell. Speichern Sie die Änderung (Datei => Speichern) und schließen Sie das Emitterfenster.

**Klonen Sie nun &quot;\_Receiver** **&quot;** (im Ordner &quot;Particle&quot;), um Ihren eigenen Receiver aus diesem zu erstellen.

Öffne die Maske. Ersetze das Dummy-Gitter wie der Emitter durch dein Modell in &quot;Layer\_Model&quot;. Wir **haben das auf dem Bildschirm** angezeigte Gitter **&#x200B;**&#x200B;geändert, aber wir müssen auch **das von den Partikeln** verwendete Gitter **&#x200B;**&#x200B;ändern.

Klicken Sie dazu im Fenster &quot;Particle Treeview&quot; auf &quot;**Shape** &quot;, das sich in folgendem Verzeichnis befinden sollte: &quot;Partikeleffekt => Spawner => Ebene\_1 => Sampler => Gitter&quot;.

Ersetzen Sie dann die &quot;MeshResource&quot; durch Ihr Modell.

Und dann ist da noch eine letzte Sache: Wir müssen den Sender und den Empfänger mit dem verbinden, den wir gerade erstellt haben.

Wählen Sie in der Baumansicht Ihres Receivers &quot;Editor Properties&quot; aus, und wählen Sie dann Ihren Emitter in &quot;OverSpawnEffect&quot; aus. Speichern Sie den Empfänger.

Öffne deinen Emitter (den wir zuvor dupliziert haben) und klicke im Fenster &quot;Particle Treeview&quot; auf &quot;Events&quot;, das du im Ordner findest: &quot;Partikeleffekt => Spawner&quot;. Ersetze dann den Empfänger durch Deinen Empfänger, indem Du auf &quot;Extern&quot; klickst.\
Fertig! Wenn Sie jetzt die 3D-Ansicht (Ihres Emitters oder Empfängers) auswählen, können Sie Partikel erstellen, indem Sie auf die Schaltfläche &quot;Raum&quot; klicken.

## Optional: das Empfängerverhalten ändern

Öffnen Sie Ihren Empfänger und wählen Sie im Fenster &quot;Particle Treeview&quot; die Option &quot; CParticleEvolver\_Script &quot; (die oberste, die Ihnen gewidmet ist :)) aus, die sich in befinden soll: &quot;Partikeleffekt => Ebene\_1 => Status\_0&quot;.

Fügen Sie im Fenster &quot;Spezialisierter Node-Editor&quot; in der Funktion &quot;Life = 0,5;&quot; hinzu, um die Lebensdauer der Partikel zu ändern. Verwenden Sie dann die Tastenkombination &quot;Strg+s&quot;, um das Skript zu speichern. Der Unterschied in der 3D-Ansicht sollte dir auffallen.

Weitere Informationen zur Funktionsweise finden Sie unter dem folgenden Link:

<http://wiki.popcornfx.com/index.php/Main_Page>

## Emitter/Receiver in Substance 3D Painter importieren

Wähle in Substance 3D Painter &quot;Datei > Partikel importieren&quot;, oder drücke Strg+Alt+R. Wähle den Emitter und den Receiver (beide im Format .pkfx) in deinem Paket aus.

Substance 3D Painter erkennt automatisch die Anforderungen (Partikelfelder, OnCollide-Ereignisse), um zu entscheiden, ob Ihr pkfx entweder ein Emitter, Receiver oder nichts kompatibel ist.

Nun sollten Sie Ihre Emitter/Receiver im Shelf sehen (in den Registerkarten &quot;Emitter&quot; und &quot;Receiver&quot;).

Um sie zu verwenden, müssen Sie zuerst auf die Schaltfläche &quot;Partikel umschalten&quot; klicken.

Dann können Sie im Fenster &quot;Werkzeuge&quot; unter &quot;Physik&quot; Ihren Emitter (um &quot;default\_emitter&quot; zu ersetzen) und Ihren Empfänger (um &quot;default\_recipient&quot; zu ersetzen) auswählen.

Sie können jetzt mit der rechten Maustaste in das Fenster &quot;Werkzeug&quot; klicken und das Werkzeug speichern.
