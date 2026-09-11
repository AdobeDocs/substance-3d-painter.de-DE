---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/painting/presets/creating-particles-presets/overview-of-the-particle-editor.html"
breadcrumb-title: ''
description: Erfahren Sie mehr über den Partikel-Editor in Substance 3D Painter, um benutzerdefinierte Pinselvorgaben für die Partikel von Texturen zu erstellen.
helpx_creative_field: ""
helpx_description: Painter > Painting > Presets > Creating particles presets > Overview of the particle editor
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Überblick über den Partikeln-Editor
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '1677'
ht-degree: 0%

---


# Überblick über den Partikeln-Editor

Diese Seite behandelt verschiedene Aspekte des PopcornFX Partikel Editors. Einige Fenstertitel und Parameter können sich je nach verwendeter Editorversion ändern.

## Einrichtung des Viewports

### Importieren eigener Mesh

Fügen Sie Ihren Mesh kopiert und in den Ordner &quot;Mesh&quot; Ihres Pakets ein. Öffnen Sie dann im Editor Ihren Mesh und klicken Sie auf &quot;Build&quot;.

Gehen Sie nun in Ihrem Partikel-System in der Baumstruktur zu &quot;Hintergrund&quot;, klicken Sie mit der rechten Maustaste auf &quot;3D-Ebenen&quot;, &quot;Neuer Hintergrund&quot;, &quot;CNEdEditorBackdrop\_Model3D&quot;, und wählen Sie Ihren Mesh in &quot;Ressourcenmodell&quot;.

In Substance 3D Painter wird der Mesh so skaliert, dass er sich innerhalb eines Kastens mit der Größe [-1;1] auf jeder Achse befindet. Um die richtige Skalierung mit Substance 3D Painter im Editor zu erhalten, sollten Sie entweder einen Mesh importieren, der bereits skaliert ist, damit er in dieses Feld passt (einfache Möglichkeit), oder mit Skalierungen im Editor spielen.

Hinweis: nur FBX Mesh-Format werden unterstützt.

#### Anzeigen des Rasters

Strg+G. Sie können die Farbe des Rasters in den &quot;Editoreigenschaften&quot; unter &quot;GridColor&quot; anpassen.

## Emitter

### Erstellen von OnCollide-Ereignissen

Der Physikentwickler behandelt Kollisionen mit Hintergrund-Meshs in der Szene. In Substance 3D Painter ist die Szene Ihr Mesh.

Legen Sie zuerst im Physik-Evolver &quot;WorldInteractionMode&quot; auf &quot;OneWay&quot; fest, um die Kollision mit der Partikel zu aktivieren. Erstellen Sie dann ein Ereignis namens &quot;OnCollide&quot;, der Physik-Evolver löst es bei einer Kollision mit der Szene aus.

In Substance 3D Painter ist die Szene das Modell, an dem Sie arbeiten, und alle Emitter mit dem Namen &quot;OnCollide&quot; werden vom Pinselsystem des aktuellen Partikel überschrieben.

#### Partikeln aus der Kamera abfeuern

Aktivieren Sie oben im Viewport die 4. Schaltfläche &quot;Laien auf Kamera beschränken&quot;.

Substance 3D Painter löst standardmäßig Emitter aus der Kamera aus.

#### Partikeln wie Regen von oben aussenden

Deaktivieren Sie &quot;Laichen auf Kamera-Ebene beschränken&quot;, wenn diese Option aktiviert ist.

Erstelle ein Partikelattribut mit dem Namen &quot;Global&quot;. Substance 3D Painter erzeugt nun deine Partikel an der Quelle.

Um auf dem oberen Teil des Meshs zu laichen, füge eine Form Sampler BOX oder CYLINDER hinzu, platziere sie oben und nimm sie in deinem Spawner Script auf.

Fügen Sie z. B. mit der Shape Sampler BOX namens &quot;Spawn&quot; Folgendes zu Ihrem Spawner-Skript hinzu:

*Position = Spawn.samplePosition();*

## Empfänger

### Emitter beim Erstellen/Bearbeiten eines Receivers erstellen

Um beim Bearbeiten Ihres Receivers noch näher an den Substance 3D Painter-Arbeitsablauf heranzukommen, können Sie den Editor so einrichten, dass das erstellte Partikel-System überschrieben wird.

Wählen Sie in der Baumansicht Ihres Receivers &quot;Editor Properties&quot; aus, aktivieren Sie &quot;UserOverSpawn&quot; und wählen Sie Ihren Emitter in &quot;OverSpawnEffect&quot; aus.

Sie müssen noch Ihren Emitter öffnen, um die &quot;OnCollide&quot;-Ereignisse festzulegen, um den Receiver zu starten, den Sie gerade bearbeiten.

#### Felder für die Partikel einrichten

Hier ist die Beschreibung des Partikeln-Felds, das Sie in Ihrem Empfänger haben müssen:

*&quot;Size&quot; float*

Der Multiplikator der Pinselgröße in Substance 3D Painter.

*&quot;Deckkraft&quot; float*

Der Multiplikator der Pinseldeckkraft in Substance 3D Painter.

*&quot;UV&quot; float3*

Die Koordinate der Textur auf dem Mesh der Partikeln.

Nimm in einem Evolver-Skript den &quot;Mesh&quot; aus Shape Sampler mit der parametrischen Koordinate auf, die vom Projektion-Evolver angegeben wird:

UV = Mesh.sampleTexcoord(pCoords);

*&quot;Normal&quot; float3*

Die Normale der Mesh-Oberfläche unter den Partikeln.

Nimm in einem Evolver-Skript den &quot;Mesh&quot; des Shape Sampler mit der parametrischen Koordinate auf, die vom Projektion-Evolver angegeben wird:

Normal = normalize(Mesh.sampleNormal(pCoords));

*&quot;Seed&quot; int*

Nur ein zufällig generierter Wert für Substance 3D Painter:

In einem Evolver Script fügen Sie hinzu:

Seed = int(rand(0,20000000));

*&quot;Coords&quot; int3*

Wird nicht von Substance 3D Painter verwendet, ist aber für die Projektion der Partikel auf dem Mesh und das Ausprobieren anderer Felder unerlässlich.

#### Partikel auf den Mesh projizieren

Fügen Sie einen Projektion-Evolver im &quot;Zustand\_0&quot; Ihres Receivers hinzu.

Jeder Rahmen projiziert der Projektion-Evolver Partikeln auf die nächstgelegene Fläche eines Shape-Sampler.

Der Projektion-Evolver kann die parametrische Koordinate der Projektion in dem durch &quot;OutputParametricCoordsField&quot; angegebenen Feld &quot;Partikel&quot; ausfüllen (siehe &quot;Partikel&quot;-Feld &quot;Farben&quot;).

Und er kann einen Vektor auf die Oberfläche des Meshs projizieren mit &quot;ReprojectedField&quot;.

Hier wollen wir Partikeln auf den Sampler Shape &quot;Mesh&quot; projizieren, parametrische Koordinaten in das Feld int3 Partikel &quot;PCOORDS&quot; ausfüllen und die &quot;Velocity&quot; auch auf die Oberfläche projizieren:

#### Probe des Meshs

In Substance 3D Painter werden alle Shape Sampler mit dem Namen &quot;Mesh&quot; und &quot;ShapeType&quot; mit dem Namen &quot;MESH&quot; mit dem in Substance 3D Painter verwendeten Mesh überschrieben.<b>\
</b>

Legen Sie im Editor den Mesh fest, der dem Hintergrund entspricht.

Um ein Skript als Beispiel zu verwenden, schreiben Sie einfach &quot;Mesh.sample~Etwas~(Coords)&quot; in ein Skript. Hier finden Sie die Dokumentation:

<https://wiki.popcornfx.com/index.php/CParticleSamplerShape#Script_bindings>

Einige nützliche Codefragmente, die Sie benötigen:

```
// UV is the texture coordinate of the particle on the mesh

// Must be after CParticleEvolver_Projection

UV = Mesh.sampleTexcoord(pCoords);

// Normal is the Normal of the surface on the mesh just below the particle

// Must be after CParticleEvolver_Projection

Normal = normalize(Mesh.sampleNormal(pCoords));
```


## Allgemeine Tipps

### Importieren von Emitter/Empfänger in Substance 3D Painter

Wähle in Substance 3D Painter &quot;Datei > Partikeln importieren&quot;, oder drücke Strg+Alt+R. Wähle dann die Datei Emitter.pkfx oder Receiver.pkfx in deinem Paket aus.

Substance 3D Painter erkennt automatisch die Anforderungen (Partikel-Felder, OnCollide-Ereignisse), um zu entscheiden, ob Ihre pkfx-Datei ein Emitter, Receiver oder nicht kompatibel ist.

Jetzt sollten Sie Ihren Emitter/Empfänger im Regal sehen.

#### So debuggen Sie Partikeln mit einer akzeptablen Partikel

Da das Feld &quot;Partikel&quot; zwischen 0 und 1 liegen muss, um die Pinselgröße in Substance 3D Painter zu multiplizieren, sind die Partikeln im Editor viel zu groß. Füge also einen benutzerdefinierten &quot;BBSize&quot;-Feldwert hinzu, der im Spawner-Skript auf 0,01 festgelegt ist und im Renderer für Billboard-Partikeln als &quot;SizeField&quot; verwendet wird, um die Partikel besser sehen zu können.

#### Wie man sich nicht mit der Reihenfolge der Entwickler anlegt

Die Reihenfolge der Evolution kann sehr wichtig sein.

Angenommen, Sie möchten immer Ihre 2 letzten Evolver haben, um der Projektions-Evolver zu sein, dann der Script-Evolver, der die UV- und Normal-Proben mit den vom Projektions-Evolver generierten Pfaden nimmt.

Beachte, dass die Reihenfolge der Evolutionäre buchstäblich die Reihenfolge der Ausführung innerhalb eines Rahmens ist und dass Substance 3D Painter Feldwerte für die Partikel und das Ende jedes Rahmens sammelt.

#### Normalen-Map des Meshs als Beispiel

Substance 3D Painter ersetzt alle Textur Samplers namens &quot;NormalMap&quot; durch die Normalen-Map des Meshs (falls importiert).

Dies ist die einzige Textur, die Sie derzeit haben können. Auf alle anderen Texturen kann Substance 3D Painter nicht zugreifen.

Nachdem Sie Ihre Textur Sampler mit dem Namen &quot;NormalMap&quot; hinzugefügt haben, können Sie sie in einem Skript testen :

<http://www.popcornfx.com/wiki/index.php/CParticleSamplerTexture>

Einige nützliche Codefragmente:

```
// In Evolver Script convert the NormalMap texture in tangent space to world space normal

// /!\ the "Normal" particle field must always be the normal of the mesh not influenced by the normal map

// /!\ dont forget to initialize your particle fields in your Spawn Script

// otherwise pCoords and Normal will be invalid at the first update

float normalFactor = 1.0; // change the intensity of the normal map

float3 meshnormal = Normal;

float4 rawtangent = Mesh.sampleTangent(pCoords);

float3 binormal = normalize(cross(meshnormal, rawtangent.xyz) * rawtangent.w);

float3 tangent = normalize(cross(meshnormal, binormal));

float3 tsNormal = normalize(((NormalMap.sample(UV).xyz * 2.0 - 1.0).xyz) * float3(-normalFactor, normalFactor, 1));

float3 normal = normalize(tsNormal.x * tangent + tsNormal.y * binormal + tsNormal.z * meshnormal);
```


#### Turbulenzen erzeugen

Erstellen Sie im Editor einen Turbulence Sampler.

<http://www.popcornfx.com/wiki/index.php/CParticleSamplerProceduralTurbulence>

Dann haben Sie zwei Möglichkeiten, die Turbulenz zu testen und Partikeln zu beeinflussen:

##### Der einfache Weg

Setze &quot;VelocityFieldSampler&quot; auf der Registerkarte &quot;Physics Evolver&quot; der Ebene auf den Namen des Turbulence Sampler. Setze &quot;Drag&quot; auf einen Wert > 0.

##### Die parametrisierte Art

Sie passen Turbulenzen mit Attributen an, indem Sie das Geschwindigkeitsfeld, das von Ihrem Turbulence Sampler generiert wurde, in einem Evolver Script abtasten:

2 Partikel-Attribute erstellen:

* float &quot;TurbulencePower&quot; minmax: [0;5]
* float &quot;TurbulenceScale&quot; minmax: [0,001; 5] (muss > 0 sein)

Erstellen Sie dann drei Partikel-Felder:

float &quot;TurbPower&quot; und float &quot;TurbScale&quot;

So speichern Sie Attribute im Spawner Script:

* TurbScale = 1,0 / TurbulenceScale;
* TurbPower = TurbulencePower;

float3 &quot;VelocityField&quot; im Rotationsmodus.

Es wird als &quot;VelocityField&quot; im Physik-Evolver verwendet (bereits standardmäßig auf das Feld &quot;VelocityField&quot; eingestellt).

Bevor du den Physik-Evolver startest, probiere in einem Script-Evolver deinen Turbulence Sampler namens &quot;Turb&quot; aus:

VelocityField = Turb.sample(Position \* TurbScale) \* TurbPower;

#### Wie wird dt richtig verwendet, die Delta-Zeit

Die Delta-Zeit ist die Simulationszeit in Sekunden zwischen den einzelnen Rahmen-Updates. Im Editor wird die Delta-Zeit mit der tatsächlich verstrichenen Zeit aktualisiert. In Substance 3D Painter ist die Delta-Zeit festgelegt und jede Aktualisierung wird gestartet, sobald die letzte abgeschlossen ist.

Ein Spiel mit 60 fps hat eine Delta-Zeit von 1/60 = 0,016 Sekunden, also versuche, deine Pinsel um 0,016 Sekunden Delta-Zeit laufen zu lassen.

* Große Delta-Zeit > 0,016s
* PRO - schnelles Update

Da der Zeitraum zwischen den Updates groß ist, werden Partikeln stärker verschoben, sodass der Pinsel in Substance 3D Painter schneller ausgeführt wird.

* CON-Näherung

PopcornFX ist eine Art großes Diskretisierungssystem, also größer der dt ist, größer die Ungenauigkeiten werden. Große Auswirkungen der Delta-Zeit auf Turbulenzen: <http://www.popcornfx.com/wiki/index.php/CParticleEvolver_Physics#Dealing_with_turbulences_at_low_framerates>

* CON-Flecken

Wenn die Delta-Zeit groß ist, ist auch die Partikel zwischen den Rahmen groß. In Substance 3D Painter können daher statt gerader Linien kleine Flecken erscheinen.

Der Grund hierfür ist, dass Substance 3D Painter für jede Partikel am Ende jedes Rahmens einen Konturpunkt und nicht für jede Partikel zwischen dem letzten und dem aktuellen Rahmen eine Linie zeichnet.

* Kleine Delta-Zeit &lt; 0,016s
* PRO-Genauigkeit

Je kleiner der Abstand zwischen den Pinselstrichen, desto geringer der Abstand zwischen den Pinselstrichen. Die Zeichnung wird also schärfer. Und die Diskretisierung der Simulation wird auch besser sein.

* CON langsam

Je kleiner die Deltazeit ist, desto mehr Aktualisierungen sind erforderlich, um dieselbe Entfernung zu zeichnen.

Abschließende Tipps zu den Delta-Zeiten : Eine gute Möglichkeit, um die richtige dt könnte sein, mit einem großen (0,1s) zu beginnen und dann Schritt für Schritt zu verringern, um das gewünschte Ergebnis zu erzielen.

#### So legt du die Parameter deiner Partikel

Substance 3D Painter erfasst die Partikel-Attribute von Partikel-Systemen und legt sie in den Parametern für Physische Pinsel bei:

<http://www.popcornfx.com/wiki/index.php/Particle_effect_attributes>

In PopcornFX haben Sie die Funktion &quot;Attribute in Evolve&quot;, die Ihnen den Zugriff auf Attribute in Evolve-Skripten ermöglicht: tu das nicht. Erstellen Sie stattdessen das Feld &quot;Partikel&quot;, und speichern Sie die Attribute im Spawner-Skript. Verwenden Sie dann das Feld &quot;Partikel&quot; in Evovler Scripts. (Dieses Problem könnte in Zukunft behoben werden.)

#### Problematische Partikeln erkennen

Partikel mit seltsamen Partikelfeldwerten sollten nie vorhanden sein. Stellen Sie daher sicher, dass Sie von Zeit zu Zeit mit problematischen Elementen arbeiten:

<http://www.popcornfx.com/wiki/index.php/Particle_tips_BreakOnProblematicParticle>

#### Beheben von Problemen mit Partikel-Systemen in Substance 3D Painter

Im Substance 3D Painter-Installationsverzeichnis sollte sich die Datei &quot;popcorn.htm&quot; befinden. Diese Datei enthält alle Protokolle von PopcornFX, werfen Sie einen Blick hinein, um zu sehen, was falsch passieren könnte.

#### Partikel-Felder richtig initialisieren

Um gültige Werte für UV und Normal ab dem ersten Frame zu erhalten, fügen Sie dies zu Ihrem Spawner-Skript hinzu:

<b>  
</b>

```
// PostEval() will be called after particles have been translated to their respective spawn locations

// so, PostEval() is executed in world space

function void PostEval()

{

// we need to initialize correctly the values needed by Substance 3D Painter:

pCoords = Mesh.projectParametricCoords(Position);

UV = Mesh.sampleTexcoord(pCoords);

Normal = normalize(Mesh.sampleNormal(pCoords));

}
```
