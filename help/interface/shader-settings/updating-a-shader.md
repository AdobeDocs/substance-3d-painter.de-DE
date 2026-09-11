---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/interface/shader-settings/updating-a-shader.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie benutzerdefinierte Shader in Substance 3D Painter aktualisieren, um Shader-Änderungen anzuwenden und Shader-Dateien neu zu laden.
helpx_creative_field: ""
helpx_description: Painter > Interface > Shader settings > Updating a shader
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Aktualisieren eines Shaders
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 0%

---


# Aktualisieren eines Shaders

Manchmal muss der von einem Projekt verwendete Shader aktualisiert werden, um Probleme zu beheben oder die neuesten Funktionen zu nutzen. Auf dieser Seite wird beschrieben, wie Sie dies tun können.

Im Folgenden finden Sie zwei schrittweise Methoden, wie Sie den Shader eines Projekts aktualisieren können:

* **Aktualisieren eines Shaders über das Shader-Fenster**
* **Aktualisieren eines Shader über das Resource Updater-Plug-in**

Wenn ein Projekt einen **benutzerdefinierten Shader** verwendet (nicht standardmäßig mit Substance 3D Painter ausgeliefert), finden Sie auf der Seite [Benutzerdefinierter Shader](https://substance3d.adobe.com/display/DRAFTPAINTER/Shader+API) eine Anleitung zum Aktualisieren des Projekts.

## Shader über das Shader-Fenster aktualisieren

### 1 - Öffnen Sie das Fenster Shader-Einstellungen.

Das Fenster **Shader-Einstellungen** ist in der Dock-Symbolleiste standardmäßig auf der rechten Seite verfügbar.

![](../../assets/shader-settings-window.png)

### 2 - Klicken Sie auf den Shader-Button und wählen Sie den aktualisierten Shader aus

Klicken Sie auf den Shader-Button (unter der Schaltfläche &quot;Rückgängig/Wiederholen&quot;) und suchen Sie nach dem Shader, der mit dem bereits verwendeten übereinstimmt.

![](../../assets/shader-mini-shelf.png)

### 3 - Shader wird aktualisiert

Sobald der neue Shader geladen ist, sollte der Hinweis **veraltet** entfernt werden und das 3D-Modell sollte normal im Viewport angezeigt werden.

![](../../assets/updated-shader.png)

## Aktualisieren eines Shader über das Resource Updater-Plug-in

### 1 - Öffnen Sie das Ressourcenaktualisierungsprogramm.

Gehen Sie auf der linken Seite der Benutzeroberfläche zur Symbolleiste &quot;**Plug-ins**&quot; und klicken Sie auf das Symbol &quot;**Resource Updater**&quot;.

![](../../assets/resource-icon.png)

### 2 - Wechseln zur Registerkarte Shader

Klicken Sie in dem neu erschienenen Fenster auf die Registerkarte &quot;Shader&quot;, um den im aktuellen Projekt vorhandenen Shader anzuzeigen.

![](../../assets/shader-tab.png)

### 3 - Finden Sie den Shader und aktualisieren Sie ihn

Auf der Registerkarte Shader sollte eine Liste aller Shader-Ressourcen angezeigt werden, die vom aktuellen Projekt verwendet werden. **Veraltete** Shader sind mit **rotem Hintergrund** sichtbar. Klicken Sie auf die Schaltfläche &quot;Aktualisieren&quot; neben einer Ressource, um sie zu aktualisieren.

![](../../assets/update-shader-click.gif)
