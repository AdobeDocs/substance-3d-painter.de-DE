---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/technical-support/technical-issues/stability-issues/crash-when-opening-or-saving-a-file.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie Substance 3D Painter-Absturz beim Öffnen oder Speichern von Dateien für eine zuverlässige Projektverwaltung beheben können.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Stability Issues > Crash when opening or saving a file
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Absturz beim Öffnen oder Speichern einer Datei
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '225'
ht-degree: 0%

---


# Absturz beim Öffnen oder Speichern einer Datei

Es gibt einige Gründe, warum Substance 3D Painter unter Windows beim Öffnen eines Dateidialogs einen Absturz auslöst. Auf dieser Seite werden die Gründe und Lösungen für dieses Problem zusammengefasst.

## Softwarekonflikte

Einige Programme können benutzerdefinierte Shell-Erweiterungen hinzufügen, die zu Instabilitäten oder Abstürzen führen können. Weitere Informationen finden Sie in der Liste [Softwarekonflikte](../startup-issues/software-conflicts.md).

## Shell-Erweiterungen/Benutzerdefinierte Designs

Benutzerdefinierte Designs werden von unserem GUI-Framework nicht unterstützt. Daher wird dringend empfohlen, das aktuelle Design vor der Verwendung von Substance 3D Painter zu deinstallieren.

**Alienware** / **Dell**-Computer integrieren standardmäßig einige Shellerweiterungen, von denen bekannt ist, dass sie nicht mit Substance 3D Painter kompatibel sind. Wir empfehlen, sie zu deinstallieren. Obwohl wir nicht genau alle Erweiterungen kennen, die inkompatibel sind, entsprechen sie meistens:

* DBROverlayIconBackuped.DBROverlayIconBackuped-Klasse
* DBROverlayIconNotBackuped.DBROverlayIconNotBackuped-Klasse

Mit dem folgenden Tool können Sie sehen, welche Erweiterungen auf Ihrem Computer installiert sind. Im Folgenden finden Sie eine grobe Anleitung für das weitere Vorgehen:

1. ShellExView von NirSoft herunterladen und installieren: <http://www.nirsoft.net/utils/shexview.html>
1. Programm ausführen
1. Klicken Sie auf **Option** und wählen Sie **Nach Erweiterungstyp filtern** aus.
1. **Symbolüberlagerungshandler auswählen**
1. Sie sollten die beiden Einträge für **Alien Respawn** sehen.
1. Wählen Sie **Beide** aus und klicken Sie auf die rote Schaltfläche, um sie zu deaktivieren.
