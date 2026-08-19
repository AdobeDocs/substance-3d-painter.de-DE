---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/pipeline-and-integration/resource-management/adding-resource-paths-by-editing-preferences-manually/editing-resource-paths-manually.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie Ressourcenpfade in den Substance 3D Painter-Voreinstellungen manuell bearbeiten, um Ihre Ablageressourcenspeicherorte anzupassen.
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Resource management > Adding resource paths by editing preferences manually > Editing resource paths manually
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Manuelles Bearbeiten von Ressourcenpfaden
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 1%

---


# Manuelles Bearbeiten von Ressourcenpfaden

Diese Seite enthält einen Leitfaden zum Bearbeiten der Voreinstellungen zum Hinzufügen oder Entfernen von Ressourcenpfaden, ohne die Anwendung zu starten.

## Speicherort der Voreinstellungen

Die Ressourcenstandorte werden mit den Anwendungsvoreinstellungen verwaltet, die sich je nach Plattform ändern können:

<table data-preserve-html="true"> <colgroup> <col/> <col/> <col/> </colgroup> <tbody> <tr> <th>System</th> <th>Version</th> <th>Pfad</th> </tr> <tr> <td rowspan="2"><p><strong>Windows</strong></p><p>(Registrierung)</p></td> <td><strong>7.2</strong> oder höher</td> <td>HKEY_CURRENT_USER\Software\Adobe\Adobe Substance 3D Painter</td> </tr> <tr> <td>Alte Version</td> <td>HKEY_CURRENT_USER\Software\Allegorithmic\Substance Painter</td> </tr> <tr> <td rowspan="2"><p><strong>Mac</strong></p><p>(Bibliothek)</p></td> <td><strong>7.2</strong> oder höher</td> <td>/Users/[Benutzername]/Library/Preferences/com.adobe.Adobe Substance 3D Painter.plist</td> </tr> <tr> <td>Alte Version</td> <td>/Users/[Benutzername]/Library/Preferences/com.substance3d.Substance Painter.plist</td> </tr> <tr> <td rowspan="2"><strong>Linux</strong></td> <td><strong>7.2</strong> oder höher</td> <td>/home/[Benutzername]/.config/Adobe/Adobe Substance 3D Painter.conf</td> </tr> <tr> <td>Alte Version</td> <td>/home/[Benutzername]/.config/Allegorithmic/Substance Painter.conf</td> </tr> </tbody> </table>

## Hinzufügen eines Pfads unter Windows

Unter Windows können Pfade über die Windows-Registrierung verwaltet werden:

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../../assets/reg-shelf-pathinfos.png)

</td>
<td style="border: 0;" valign="top">

![](../../../assets/reg-content.png)

</td>
</tr>
</table>

1. Klicken Sie auf **Start > Ausführen** oder drücken Sie **Windows + R** .
1. Geben Sie &quot;**regedit**&quot; (ohne Anführungszeichen) in das Dialogfeld ein und drücken Sie **OK**.
1. Navigieren Sie in der Strukturansicht auf der linken Seite des Fensters **Registrierungs-Editor** und navigieren Sie zu dem oben genannten Registrierungsschlüssel.
1. **Fügen Sie einen Schlüssel** unter **pathInfos** mit einer **number** als Namen hinzu. Erhöhen Sie die Anzahl basierend auf den bereits vorhandenen Schlüsseln (beginnend bei 1).
1. Führen Sie im rechten Teil des Fensters einen **Rechtsklick** > **Neu** > **Zeichenfolgenwert** aus. Benennen Sie ihn &quot;**disabled**&quot;, und legen Sie den Wert auf &quot;**false**&quot; fest.
1. Führen Sie im rechten Teil des Fensters einen **Rechtsklick** > **Neu** > **Zeichenfolgenwert** aus. Benennen Sie ihn **Name**, und geben Sie den Namen der benutzerdefinierten Ablage ein.
1. Führen Sie im rechten Teil des Fensters einen **Rechtsklick** > **Neu** > **Zeichenfolgenwert** aus. Benennen Sie ihn **Pfad**, und legen Sie den Wert auf den Pfad fest, in dem sich die Ablage befindet.
1. Vergessen Sie nicht, den Schlüssel &quot;**size** &quot; innerhalb von &quot;**pathInfos** &quot; um 1 zu erhöhen.
1. Schließen Sie das Fenster.
1. Starten Sie die Anwendung.

Es ist möglich, den neuen Pfad als Standardpfad zu definieren (wenn neue Ressourcen erstellt werden, z. B. Vorgaben), indem der Wert des Eintrags **writableShelf** in den Namen des neuen Speicherorts geändert wird.

![](../../../assets/default-shelf.png)

## Hinzufügen eines Pfads unter Linux

Auf **Linux** können zusätzliche Pfade über die Konfigurationsdatei der Benutzeranwendungsvoreinstellung erstellt werden, die im Stammverzeichnis gespeichert ist (siehe.

1. Navigieren Sie zu dem oben genannten Pfad.
1. Öffnen Sie die Datei **Substance 3D Painter.config**.
1. Scrollen Sie nach unten zum Abschnitt **[Shelf]**

Fügen Sie einen neuen Regalpfad hinzu, indem Sie die zuletzt angezeigte Zahl erhöhen. Beispiel:

```
pathInfos2disabled=false  

pathInfos2name=custom_resources 

pathInfos2path=/home/Username/Documents/custom_path 

writableShelf=custom_resources
```


Verwenden Sie die Variable **writableShelf**, um anzugeben, welcher Pfad der Standardpfad sein soll (wenn neue Ressourcen erstellt werden, z. B. Vorgaben).

Speichern Sie die Änderungen und starten Sie die Anwendung neu.
