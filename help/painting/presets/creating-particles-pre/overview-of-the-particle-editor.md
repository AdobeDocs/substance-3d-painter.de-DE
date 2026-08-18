---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/painting/presets/creating-particles-presets/overview-of-the-particle-editor.html"
breadcrumb-title: ''
description: Erfahren Sie mehr über den Partikel-Editor in Substance 3D Painter, um benutzerdefinierte Partikelpinselvorgaben für die Texturbearbeitung zu erstellen.
helpx_creative_field: ""
helpx_description: Painter > Painting > Presets > Creating particles presets > Overview of the particle editor
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Überblick über den Partikel-Editor
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '1677'
ht-degree: 0%

---


# Überblick über den Partikel-Editor

Diese Seite behandelt verschiedene Aspekte des PopcornFX-Partikel-Editors. Einige Fenstertitel und Parameter können sich je nach verwendeter Editorversion ändern.

## Viewport-Einrichtung

### Eigenes Gitter importieren

Kopieren Sie das Mesh und fügen Sie es in den Ordner &quot;Meshes&quot; Ihres Pakets ein. Öffnen Sie dann im Editor Ihr Mesh und klicken Sie auf &quot;Build&quot;.

Wählen Sie nun in Ihrem Partikelsystem in der Baumstruktur &quot;Hintergrund&quot; aus, klicken Sie mit der rechten Maustaste auf &quot;3D-Ebenen&quot;, &quot;Neuer Hintergrund&quot;, &quot;CNEdEditorBackdrop\_Model3D&quot;, und wählen Sie Ihr Mesh in &quot;Ressourcenmodell&quot; aus.

In Substance 3D Painter wird das Gitter so skaliert, dass es sich innerhalb eines Kastens mit der Größe [-1;1] auf jeder Achse befindet. Um mit Substance 3D Painter im Editor die richtige Skalierung zu erhalten, sollten Sie entweder ein Gitter importieren, das bereits so skaliert ist, dass es in dieses Feld passt (einfache Möglichkeit), oder mit Skalierungen im Editor spielen.

Hinweis: Nur das FBX-Gitterformat wird unterstützt.

#### Raster anzeigen

Strg+G. Sie können die Farbe des Rasters in den &quot;Editor-Eigenschaften&quot; unter &quot;GridColor&quot; anpassen.

## Emitter

### Erstellen von OnCollide-Ereignissen

Der Physik-Evolver behandelt Kollisionen mit Hintergrundmaschen in der Szene. In Substance 3D Painter wird die Szene zum Gitter.

Legen Sie zuerst im Physik-Evolver &quot;WorldInteractionMode&quot; auf &quot;OneWay&quot; fest, um die Partikelkollision zu aktivieren. Erstellen Sie dann ein Ereignis namens &quot;OnCollide&quot;, der Physik-Evolver löst es bei einer Kollision mit der Szene aus.

In Substance 3D Painter ist die Szene das Modell, an dem Sie arbeiten, und alle Ereignisse namens &quot;OnCollide&quot; werden vom Emitter-Partikelsystem des aktuellen Pinsels überschrieben.

#### Partikel aus der Kamera abfeuern

Aktivieren Sie oben im Viewport die 4. Schaltfläche &quot;Laien auf Kameraebene beschränken&quot;.

Substance 3D Painter löst standardmäßig Emitter aus der Kamera aus.

#### Partikel wie Regen von oben emittieren

Deaktivieren Sie &quot;Laich-Einstellungen auf Kameraebene beschränken&quot;, wenn diese Option aktiviert ist.

Erstelle ein Partikelattribut mit dem Namen &quot;Global&quot;. Substance 3D Painter erzeugt nun deine Partikel an der Quelle.

Um auf dem oberen Teil des Gitters zu laichen, füge eine Form-Sampler-BOX oder einen ZYLINDER hinzu. Platziere sie auf der oberen Seite des Gitters, und nimm sie in deinem Spawner-Skript auf.

Fügen Sie z. B. mit der Shape Sampler BOX namens &quot;Spawn&quot; Folgendes zu Ihrem Spawner-Skript hinzu:

*Position = Spawn.samplePosition();*

## Empfänger

### Emitter beim Erstellen/Bearbeiten eines Empfängers erstellen

Um dem Substance 3D Painter-Workflow beim Bearbeiten Ihres Receivers noch näher zu kommen, können Sie den Editor so einrichten, dass das erstellte Partikelsystem überschrieben wird.

Wählen Sie in der Baumansicht Ihres Receivers &quot;Editor Properties&quot; aus, aktivieren Sie &quot;UserOverSpawn&quot; und wählen Sie Ihren Emitter in &quot;OverSpawnEffect&quot; aus.

Sie müssen noch Ihren Emitter öffnen, um die &quot;OnCollide&quot;-Ereignisse festzulegen, um den Empfänger zu starten, den Sie gerade bearbeiten.

#### Partikelfelder einrichten

Hier ist die Beschreibung des Partikelfelds, das Sie in Ihrem Empfänger haben müssen:

*&quot;Size&quot; float*

Der Multiplikator der Pinselgröße in Substance 3D Painter.

*&quot;Deckkraft&quot; float*

Der Multiplikator der Pinseldeckkraft in Substance 3D Painter.

*&quot;UV&quot; float3*

Die Strukturkoordinate auf dem Gitter der Partikel.

Nimm in einem Evolver-Skript die Form &quot;Sampler Mesh&quot; mit der parametrischen Koordinate des Projektions-Evolvers auf:

UV = Mesh.sampleTexcoord(pCoords);

*&quot;Normal&quot; float3*

Die Normale der Netzoberfläche unter den Partikeln.

Nimm in einem Evolver-Skript die Form Sampler &quot;Mesh&quot; mit der parametrischen Koordinate auf, die vom Projektions-Evolver angegeben wird:

Normal = normalize(Mesh.sampleNormal(pCoords));

*&quot;Seed&quot; int*

Nur ein zufällig generierter Wert für Substance 3D Painter:

In einem Evolver Script fügen Sie hinzu:

Seed = int(rand(0,20000000));

*&quot;Coords&quot; int3*

Nicht von Substance 3D Painter verwendet, aber unverzichtbar, um die Partikelprojektion auf das Gitter und Probe anderen Bereichen.

#### Partikel auf das Mesh projizieren

Fügen Sie einen Projektionsevolver im &quot;Status\_0&quot; Ihres Empfängers hinzu.

Bei jedem Frame projiziert der Projektionsentwickler Partikel auf die nächstgelegene Fläche eines Shape-Sampler.

Der Projektionsevolver kann die parametrische Koordinate der Projektion im Partikelfeld ausfüllen, das durch &quot;OutputParametricCoordsField&quot; angegeben wird (siehe &quot;pCoords&quot;-Partikelfeld).

Und er kann einen Vektor auf die Oberfläche des Gitters projizieren, indem er &quot;ReprojectionField&quot; verwendet.

Hier wollen wir auf die Sampler Shape &quot;Mesh&quot; Partikel projizieren, parametrische Koordinaten im int3 Partikelfeld &quot;PCOORDS&quot; ausfüllen und die &quot;Velocity&quot; auch auf die Oberfläche projizieren:

#### Mesh aufnehmen

In Substance 3D Painter werden alle Shape Sampler mit dem Namen &quot;Mesh&quot; und &quot;ShapeType&quot; mit dem Namen &quot;MESH&quot; mit dem in Substance 3D Painter verwendeten Gitter überschrieben.<b>\
</b>

Legen Sie es im Editor auf das gleiche Gitter wie Ihren Hintergrund fest.

Zum Aufnehmen von Dingen in einem Skript schreiben Sie einfach &quot;Mesh.sample~Etwas~(Coords)&quot; in ein Skript. Hier finden Sie die Dokumentation:

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

### Importieren von Emitter/Receiver in Substance 3D Painter

Wählen Sie in Substance 3D Painter &quot;Datei&quot; > &quot;Partikel importieren&quot; oder Strg-Alt-R und anschließend in Ihrer Verpackung die Datei &quot;Emitter.pkfx&quot; oder &quot;Receiver.pkfx&quot; aus.

Substance 3D Painter erkennt automatisch die Anforderungen (Partikelfelder, OnCollide-Ereignisse), um zu entscheiden, ob Ihr pkfx entweder ein Emitter, Receiver oder nichts kompatibel ist.

Jetzt sollten Sie Ihre Emitter/Receiver im Shelf sehen.

#### Partikel mit einer lebensfähigen Partikelgröße debuggen

Da das Partikelfeld &quot;Size&quot; zwischen 0 und 1 liegen muss, um die Pinselgröße in Substance 3D Painter zu multiplizieren, sind die Partikel im Editor viel zu groß. Füge also einen benutzerdefinierten &quot;BBSize&quot;-Feldwert von 0,01 im Spawner-Skript hinzu, der im Renderer für Billboard-Partikel als &quot;SizeField&quot; verwendet wird, um Partikel besser sehen zu können.

#### Wie man sich nicht mit der Reihenfolge der Entwickler anlegt

Die Reihenfolge der Evolution kann sehr wichtig sein.

Angenommen, Sie möchten immer Ihre 2 letzten Evolver haben, um der Projektions-Evolver zu sein, dann der Script-Evolver, der die UV- und Normal-Proben mit den vom Projektions-Evolver generierten Pfaden nimmt.

Beachte, dass die Reihenfolge der Evolutionäre buchstäblich die Reihenfolge der Ausführung innerhalb eines Frames ist und dass Substance 3D Painter die Partikelfeldwerte und das Ende jedes Frames erfasst.

#### So nehmen Sie die Normalmap des Gitters auf

Substance 3D Painter ersetzt alle Texturaufnehmer mit dem Namen &quot;NormalMap&quot; durch die Normalmap des Gitters (falls importiert).

Das ist die einzige Textur, die du vorerst haben kannst. Auf alle anderen Texturen kann Substance 3D Painter nicht zugreifen.

Nachdem Sie Texture Sampler mit dem Namen &quot;NormalMap&quot; hinzugefügt haben, können Sie es in einem Skript testen :

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

Dann haben Sie 2 Möglichkeiten, die Turbulenz zu testen und Partikel zu beeinflussen:

##### Der einfache Weg

Setze &quot;VelocityFieldSampler&quot; auf der Registerkarte &quot;Physics Evolver&quot; der Ebene auf den Namen des Turbulence Sampler. Setze &quot;Drag&quot; auf einen Wert > 0.

##### Die parametrisierte Art

Sie passen Turbulenzen mit Attributen an, indem Sie das Geschwindigkeitsfeld, das von Ihrem Turbulence Sampler generiert wurde, in einem Evolver Script abtasten:

2 Partikelattribute erstellen:

* float &quot;TurbulencePower&quot; minmax: [0;5]
* float &quot;TurbulenceScale&quot; minmax: [0,001; 5] (muss > 0 sein)

Erstellen Sie dann drei Partikelfelder:

float &quot;TurbPower&quot; und float &quot;TurbScale&quot;

So speichern Sie Attribute im Spawner Script:

* TurbScale = 1,0 / TurbulenceScale;
* TurbPower = TurbulencePower;

float3 &quot;VelocityField&quot; im Rotationsmodus.

Es wird als &quot;VelocityField&quot; im Physik-Evolver verwendet (bereits standardmäßig auf das Feld &quot;VelocityField&quot; eingestellt).

Bevor du den Physik-Evolver startest, probiere in einem Script-Evolver deinen Turbulence Sampler namens &quot;Turb&quot; aus:

VelocityField = Turb.sample(Position \* TurbScale) \* TurbPower;

#### Wie wird dt richtig verwendet, die Delta-Zeit

Die Delta-Zeit ist die Simulationszeit in Sekunden zwischen jeder Frame-Aktualisierung. Im Editor wird die Delta-Zeit mit der tatsächlich verstrichenen Zeit aktualisiert. In Substance 3D Painter ist die Delta-Zeit festgelegt und jede Aktualisierung wird gestartet, sobald die letzte abgeschlossen ist.

Ein Spiel mit 60 fps hat eine Delta-Zeit von 1/60 = 0,016 Sekunden, also versuche, deine Pinsel um 0,016 Sekunden Delta-Zeit laufen zu lassen.

* Große Delta-Zeit > 0,016s
* PRO - schnelles Update

Da der Zeitraum zwischen den Aktualisierungen groß ist, werden die Partikel stärker verschoben, sodass der Pinsel in Substance 3D Painter schneller ausgeführt wird.

* CON-Näherung

PopcornFX ist eine Art großes Diskretisierungssystem, also größer der dt ist, größer die Ungenauigkeiten werden. Große Auswirkungen der Delta-Zeit auf Turbulenzen: <http://www.popcornfx.com/wiki/index.php/CParticleEvolver_Physics#Dealing_with_turbulences_at_low_framerates>

* CON-Flecken

Wenn die Delta-Zeit groß ist, ist auch die Partikelbewegung zwischen Rahmen groß. In Substance 3D Painter können daher statt gerader Linien kleine Flecken erscheinen.

Der Grund hierfür ist, dass Substance 3D Painter für jedes Partikel am Ende jedes Frames einen Konturpunkt und zwischen dem letzten und dem aktuellen Frame nicht jeweils eine Linie zeichnet.

* Kleine Delta-Zeit &lt; 0,016s
* PRO-Genauigkeit

Je kleiner der Abstand zwischen den Pinselstrichen, desto geringer der Abstand zwischen den Pinselstrichen. Die Zeichnung wird also schärfer. Und die Diskretisierung der Simulation wird auch besser sein.

* CON langsam

Je kleiner die Deltazeit ist, desto mehr Aktualisierungen sind erforderlich, um dieselbe Entfernung zu zeichnen.

Abschließende Tipps zu den Delta-Zeiten : Eine gute Möglichkeit, um die richtige dt könnte sein, mit einem großen (0,1s) zu beginnen und dann Schritt für Schritt zu verringern, um das gewünschte Ergebnis zu erzielen.

#### So belichten Sie die Parameter Ihres Partikelsystems

Substance 3D Painter erfasst die Partikelattribute von Partikelsystemen und macht sie in den Parametern des Physic-Pinsels verfügbar:

<http://www.popcornfx.com/wiki/index.php/Particle_effect_attributes>

In PopcornFX haben Sie die Funktion &quot;Attribute in Evolve&quot;, die Ihnen den Zugriff auf Attribute in Evolve-Skripten ermöglicht: tu das nicht. Erstellen Sie stattdessen ein Partikelfeld, und speichern Sie Attribute in diesem Feld im Spawner-Skript. Verwenden Sie dann dieses Partikelfeld in den Evovler-Skripten. (Dieses Problem könnte in Zukunft behoben werden.)

#### Problematische Partikel erkennen

Partikel mit seltsamen Partikelfeldwerten sollten nie vorhanden sein. Stellen Sie daher sicher, dass Sie von Zeit zu Zeit mit problematischen Elementen arbeiten:

<http://www.popcornfx.com/wiki/index.php/Particle_tips_BreakOnProblematicParticle>

#### So beheben Sie Probleme mit Partikelsystemen in Substance 3D Painter

Im Substance 3D Painter-Installationsverzeichnis sollte sich die Datei &quot;popcorn.htm&quot; befinden. Diese Datei enthält alle Protokolle von PopcornFX, werfen Sie einen Blick hinein, um zu sehen, was falsch passieren könnte.

#### Wie man Partikelfelder richtig initialisiert

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
