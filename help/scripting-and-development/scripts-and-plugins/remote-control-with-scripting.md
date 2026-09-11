---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/scripting-and-development/scripts-and-plugins/remote-control-with-scripting.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie die Skripterstellung per Fernsteuerung in Substance 3D Painter verwenden können, um Workflows zu automatisieren und die Anwendung programmgesteuert zu steuern.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > Scripts and plugins > Remote control with scripting
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Fernsteuerung mit Scripting
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 0%

---


# Fernsteuerung mit Scripting

Auf dieser Seite wird beschrieben, wie Sie die Anwendung remote steuern, um JavaScript- oder Python-Befehle auszuführen.\
Dazu ist ein bestimmtes Befehlszeilenargument erforderlich. Anschließend kann ein einfaches Python-Skript alle Befehle ausführen, die über die vorhandenen JavaScript- und Python-APIs verfügbar sind.

## Starten der Anwendung

Um die Anwendung remote zu steuern, muss Substance 3D Painter mit der folgenden Befehlszeile gestartet werden:

```
"Adobe Substance 3D painter.exe" --enable-remote-scripting
```


>[!NOTE]
>
> Stellen Sie sicher, dass die Anwendung mit diesem Befehl läuft, bevor Sie Skripte ausführen. Skripte können fehlschlagen, wenn die Anwendung noch gestartet wird/noch nicht fertig ist.

## Fernsteuerungsskript

Das folgende Python-Skript kann als Bibliothek für die Kommunikation mit der Anwendung dienen.

Speichern Sie das folgende Skript in einer Datei mit dem Namen **lib\_remote.py**, damit die folgenden Beispiele ordnungsgemäß funktionieren.

```
import sys 

import json 

import base64 

import subprocess 

 

if sys.version_info >= (3, 0): 

 import http.client as http 

else: 

 import httplib as http 

 

class RemotePainter() : 

 def __init__(self, port=60041, host='localhost'): 

  self._host = host 

  self._port = port 

 

## Json server connection

  self._PAINTER_ROUTE = '/run.json' 

  self._HEADERS = {'Content-type': 'application/json', 'Accept': 'application/json'} 

 

## Execute a HTTP POST request to the Substance Painter server and send/receive JSON data

 def _jsonPostRequest( self, route, body, type ) : 

  connection = http.HTTPConnection(self._host, self._port, timeout=3600) 

  connection.request('POST', route, body, self._HEADERS) 

  response = connection.getresponse() 

 

  data = response.read() 

  connection.close() 

 

  if type == "js" : 

   data = json.loads( data.decode('utf-8') ) 

 

   if 'error' in data: 

    OutJson = json.loads( body.decode() ) 

    print( base64.b64decode( OutJson["js"] ) ) 

    raise ExecuteScriptError(data['error']) 

  else : 

## Python can return nothing, so decoding can fail

   try: 

    data = data.decode('utf-8').rstrip() 

   except: 

    pass 

 

  return data 

 

 def checkConnection(self): 

  connection = http.HTTPConnection(self._host, self._port) 

  connection.connect() 

 

## Execute a command

 def execScript( self, script, type ) : 

  Command = base64.b64encode( script.encode('utf-8') ) 

 

  if type == "js" : 

   Command = '{{"js":"{0}"}}'.format( Command.decode('utf-8') ) 

  else : 

   Command = '{{"python":"{0}"}}'.format( Command.decode('utf-8') ) 

 

  Command = Command.encode( "utf-8" ) 

 

  return self._jsonPostRequest( self._PAINTER_ROUTE, Command, type ) 

 

class PainterError(Exception): 

 def __init__(self, message): 

  super(PainterError, self).__init__(message) 

 

class ExecuteScriptError(PainterError): 

 def __init__(self, data): 

  super(PainterError, self).__init__('An error occured when executing script: {0}'.format(data)) 

 
```


## Beispiele

Im Folgenden finden Sie zwei einfache Beispiele, die zeigen, wie Sie Befehle in beiden APIs ausführen können, die von der Anwendung unterstützt werden:

### Ausführen von JavaScript-Befehlen

Die meisten Javascript-Funktionen in der API geben String- oder Json-Daten zurück, die eine einfache Bearbeitung innerhalb des Python-Skripts ermöglichen. Es sollte keine größeren Probleme beim Senden und Empfangen von Daten geben.

Erstellen Sie eine Python-Skriptdatei mit dem Namen **example\_js.py** und fügen Sie den folgenden Code hinzu:

```
import lib_remote 

 

Remote = lib_remote.RemotePainter() 

Remote.checkConnection() 

 

## Print the API version

Version = Remote.execScript( "alg.version.painter", "js" ) 

print( Version ) 

 

## Get a list of all the files in the default shelf/library:

Files = Remote.execScript( 'alg.resources.findResources("starter_assets", "*")', "js" ) 

 

for File in Files : 

 print( File )
```


Wenn die Anwendung mit der Befehlszeile ausgeführt wird, werden beim Ausführen dieses Skripts Befehle ausgeführt und die Ergebnisse abgerufen.

### Ausführen von Python-Befehlen

Die meisten Python-Funktionen geben möglicherweise Objekte zurück, die nicht in das Remoteskript übergeben werden können. Dies bedeutet, dass die Daten zum Empfangen explizit in Zeichenfolgen oder Json-Wörterbücher konvertiert werden müssen.

Um die Dinge zu erleichtern, ist es möglich, ein benutzerdefiniertes Python-Skript zu erstellen, das während des Starts der Anwendung geladen wird, und Funktionen aufzurufen, die diese Art der Konvertierung verarbeiten, ohne auf Inline-Konvertierungen angewiesen zu sein.

Erstellen Sie eine Python-Skriptdatei mit dem Namen **example\_py.py** und fügen Sie den folgenden Code hinzu:

```
import lib_remote 

 

Remote = lib_remote.RemotePainter() 

Remote.checkConnection() 

 

## import the substance_painter module to make

## its API available to us

Remote.execScript( "import substance_painter", "python" ) 

 

## Print the API version

Version = Remote.execScript( "substance_painter.__version__", "python" ) 

print( Version ) 

 

## Get a list of all the files in the default shelf/library

## Because the search function return objects, we have to convert

## the information into a string within the same command (inline)

Command = 'substance_painter.resource.search( "p:starter_assets/" )' 

Command = '"|||".join( [ x.identifier().url() for x in {0}] )'.format( Command ) 

 

Files = Remote.execScript( Command, "python" ) 

Files = Files.split( "|||" ) 

 

for File in Files : 

 print( File )
```


Wenn die Anwendung mit der Befehlszeile ausgeführt wird, werden beim Ausführen dieses Skripts Befehle ausgeführt und die Ergebnisse abgerufen.
