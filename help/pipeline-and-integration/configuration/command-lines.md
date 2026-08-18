---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/pipeline-and-integration/configuration/command-lines.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie Befehlszeilenargumente mit Substance 3D Painter für Automatisierung, Skripterstellung und Pipelineintegration verwenden.
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Configuration > Command lines
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Befehlszeilen
user-guide-description: ''
user-guide-title: ''
source-git-commit: 22871eab2f25d09bd82f1292d8b3e5f8c4f1c2cf
workflow-type: tm+mt
source-wordcount: '204'
ht-degree: 3%

---


# Befehlszeilen

Auf dieser Seite werden mehrere Befehlszeilen aufgeführt, die beim Starten der Anwendung zum Erstellen oder Öffnen von Projekten verwendet werden können.\
Diese Befehlszeilen können wie folgt verwendet werden:

```
"Adobe Substance 3D Painter.exe" --command [option] 
```


## Liste der Befehle

| Befehl | Beschreibung |
| --- | --- |
| **—help** **-?** **-h** | Zeigt Informationen über die verfügbaren Befehlszeilen und deren Verwendung an. |
| **- Version** **- Version** | Zeigt die aktuelle Version von Substance 3D Painter an. |
| **—mesh** | Gitter, das in einem Projekt geladen werden soll.Beispiel:  `// Create a new project with a specific mesh   "Adobe Substance 3D Painter.exe" --mesh "E:/MymeshFolder/MyMesh.obj"       // Update a mesh inside an existing project   "Adobe Substance 3D Painter.exe" --mesh "E:/MymeshFolder/MyMesh.obj" "E:/MyMeshFolder/Project.spp"` |
| **—mesh-map** | Mit dem Gitter verknüpfte durch Baking erzeugte Map (AO, Normal, Krümmung). Kann mehrfach angegeben werden. Nomenklatur: TextureSetName\_AdditionalMapSlot<ul data-preserve-html="true"> <li data-preserve-html="true">Umgebende Verdeckung = <strong> <em> ambient_Verdeckung </em> </strong></li> <li data-preserve-html="true">Krümmung = <strong> <em> Krümmung </em> </strong></li> <li data-preserve-html="true">Normal = <strong> <em> normal_base </em> </strong></li> <li data-preserve-html="true">Normaler Weltraum = <strong> <em> world_space_normals </em> </strong></li> <li data-preserve-html="true">Position = <strong> <em> Position </em> </strong></li> <li data-preserve-html="true">Thickness = <strong> <em> Thickness </em> </strong></li> <li data-preserve-html="true">ID = <em> <strong> ID </strong> </em></li> </ul>Beispiel:  `"Adobe Substance 3D Painter.exe" --mesh "E:/MyMeshFolder/MyMesh.obj" --mesh-map " E:/MyMeshFolder/DefaultMaterial_ambient_occlusion.png"` |
| **—split-by-udim** | Ein Textur-Set pro UDIM-Kachel erstellen. |
| **—export-path** | Standardexportpfad, unter dem die Ausgaben des Projekts exportiert werden. |
| **—vram-budget** | Überschreiben Sie das durch die Substance 3D Painter-Engine definierte Budget für den Videospeicher (VRAM). &quot;Menge&quot; wird in Megabyte angegeben.    Beispiel:  `// Set the VRam budget to 2GB   "Adobe Substance 3D Painter.exe" --vram-budget 2048` |
| **—disable-version-check** | Überprüfen Sie nicht, ob beim Starten eine neue Version der Anwendung verfügbar ist |
| **—enable-remote-scripting** | Lassen Sie zu, dass Skriptbefehle von außerhalb der Anwendung ausgeführt werden. Weitere Informationen finden Sie unter [Remotesteuerung mit Skripterstellung](../../scripting-and-development/scripts-and-plugins/remote-control-with-scripting.md). |
