---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/pipeline-and-integration/resource-management/adding-resource-paths-by-editing-preferences-manually/editing-the-shelf-preferences-with-python.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie Voreinstellungen für Regal mithilfe von Python-Skripten in Substance 3D Painter für die automatisierte Verwaltung von Ressourcenpfaden bearbeiten.
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Resource management > Adding resource paths by editing preferences manually > Edit Shelf Preferences with Python
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Bearbeitungseinstellungen mit Python
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '241'
ht-degree: 2%

---


# Bearbeiten der Regal-Voreinstellungen mit Python

Im Folgenden finden Sie Beispiele für Python-Skripte zum Ändern der Windows-Registrierung zum Bearbeiten von Ressourcenpfaden.

## Registrierungsschlüsselpfad

In der folgenden Tabelle finden Sie Informationen zum Verwenden des entsprechenden Registrierungsschlüsselpfads:

<table data-preserve-html="true"> <colgroup> <col/> <col/> <col/> </colgroup> <tbody> <tr> <th>System</th> <th>Version</th> <th>Pfad</th> </tr> <tr> <td rowspan="2"><p><strong>Windows</strong></p><p>(Registrierung)</p></td> <td><strong>7.2</strong> oder höher</td> <td>HKEY_CURRENT_USER\Software\Adobe\Adobe Substance 3D Painter</td> </tr> <tr> <td>Alte Version</td> <td>HKEY_CURRENT_USER\Software\Allegorithmic\Substance Painter</td> </tr> <tr> <td rowspan="2"><p><strong>Mac</strong></p><p>(Bibliothek)</p></td> <td><strong>7.2</strong> oder höher</td> <td>/Users/[Benutzername]/Library/Preferences/com.adobe.Adobe Substance 3D Painter.plist</td> </tr> <tr> <td>Alte Version</td> <td>/Users/[Benutzername]/Library/Preferences/com.substance3d.Substance Painter.plist</td> </tr> <tr> <td rowspan="2"><strong>Linux</strong></td> <td><strong>7.2</strong> oder höher</td> <td>/home/[Benutzername]/.config/Adobe/Adobe Substance 3D Painter.conf</td> </tr> <tr> <td>Alte Version</td> <td>/home/[Benutzername]/.config/Allegorithmic/Substance Painter.conf</td> </tr> </tbody> </table>

## Hinzufügen eines neuen Pfads

Zum Hinzufügen eines Ressourcenpfads muss überprüft werden, welcher bereits vorhanden ist, um die Liste mit einem neuen zu inkrementieren.

Mit dem folgenden Code wird dem Registrierungsschlüssel ein neuer Regal-Pfad hinzugefügt, nachdem überprüft wurde, wie viele Pfade bereits definiert sind.

>[!NOTE]
>
> Der Unterschlüssel **Regal** (neben **pathInfos**) ist möglicherweise nicht in der Registrierung vorhanden. Um den Text in der Anwendung zu starten, öffnen Sie die Voreinstellungen (&quot;Bearbeiten&quot; > &quot;Einstellungen&quot;), klicken Sie auf &quot;OK&quot; und schließen Sie die Anwendung.

```
import winreg 

 

RegistryKeyName = "SOFTWARE\Adobe\Adobe Substance 3D Painter\Shelf\pathInfos" 

 

ShelfName = "myshelf" #Needs to be lowercase 

ShelfPath = "C:/Temp" 

ShelfStatus = "false" #false = not disabled 

 

RegConnection = winreg.ConnectRegistry( None, winreg.HKEY_CURRENT_USER ) 

  

## Open parent registry key

Key = winreg.OpenKey( RegConnection, RegistryKeyName, winreg.KEY_READ  ) 

 

## Iterate over each sub-key to retrieve the biggest Shelf number

SubKeyCount = winreg.QueryInfoKey( Key )[0] 

ShelfNumber = 0 

 

for x in range(SubKeyCount) : 

 SubKeyName = winreg.EnumKey(Key, x) 

 ShelfNumber = max( ShelfNumber, int(SubKeyName) ) 

 

ShelfNumber += 1 

 

## Create the new Key and add its values

NewKey = winreg.CreateKey( Key, str( ShelfNumber ) ) 

 

winreg.SetValueEx( NewKey, "disabled", 0, winreg.REG_SZ, ShelfStatus) 

winreg.SetValueEx( NewKey, "name", 0, winreg.REG_SZ, ShelfName) 

winreg.SetValueEx( NewKey, "path", 0, winreg.REG_SZ, ShelfPath) 

 

NewKey.Close() 

 

## Increment the Shelf path counter

Count = winreg.QueryValueEx( Key, "size" ) 

Key.Close() 

 

Key = winreg.OpenKeyEx( RegConnection, RegistryKeyName, 0, winreg.KEY_SET_VALUE  ) 

winreg.SetValueEx( Key, "size", 0, winreg.REG_DWORD, Count[0] + 1 ) 

Key.Close()
```


## Deaktivieren oder Aktivieren eines Ressourcenpfads

Jeder erstellte Pfad kann entfernt werden, wenn er nicht mehr benötigt wird, aber auch deaktiviert werden für den Standardpfad, der nicht vollständig entfernt werden kann.

Mit dem folgenden Code wird die Windows-Registrierung analysiert und das Standard-Regal (mit dem Namen &quot;starter\_assets&quot;) deaktiviert.

```
import winreg 

 

RegistryKeyName = "SOFTWARE\Adobe\Adobe Substance 3D Painter\Shelf\pathInfos" 

RegConnection = winreg.ConnectRegistry( None, winreg.HKEY_CURRENT_USER ) 

 

## Open registry key

Key    = winreg.OpenKey( RegConnection, RegistryKeyName, winreg.KEY_READ ) 

SubKeyCount  = winreg.QueryInfoKey( Key )[0] 

 

## Iterate over each sub-key

for x in range(SubKeyCount) : 

 SubKeyName = winreg.EnumKey(Key, x) 

 SubKey = winreg.OpenKey( 

  RegConnection, 

  RegistryKeyName + "\" + SubKeyName, 

  winreg.KEY_READ ) 

 SubKeyValueCount = winreg.QueryInfoKey( SubKey )[1] 

 

## Read subkey values

 Values = [] 

 for i in range( SubKeyValueCount ) : 

  Values.append( winreg.EnumValue( SubKey, i ) ) 

 

## Note : Values is a table of tuples

 FoundKey = False 

 for Value in Values : 

  if Value[0] == "name" : 

   if Value[1] == "starter_assets" : 

    FoundKey = True 

 

 SubKey.Close() 

 

## Found the path ? Then we edit the Key

 if FoundKey : 

  print( " - Editing Windows Registry" ) 

 

## Re-Open key in edition mode

  SubKey  = winreg.OpenKey(   

   winreg.HKEY_CURRENT_USER, 

   RegistryKeyName + "\" + SubKeyName, 

   0, 

   winreg.KEY_SET_VALUE ) 

 

## Assign new value

  winreg.SetValueEx(SubKey, "disabled", 0, 1, "true" ) #use "false" to Enable that shelf path 

 

  SubKey.Close() 

 

## Finish

Key.Close()
```
