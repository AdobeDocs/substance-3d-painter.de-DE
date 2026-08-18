---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/pipeline-and-integration/configuration/environment-variables.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie in Substance 3D Painter das Anwendungsverhalten und die Pipelineintegration mithilfe von Umgebungsvariablen konfigurieren.
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Configuration > Environment variables
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Umgebungsvariablen
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '513'
ht-degree: 3%

---


# Umgebungsvariablen

Auf dieser Seite werden Umgebungsvariablen aufgelistet, die verwendet werden können, um das Standardverhalten der Anwendung zu überschreiben.

| Variable | Beschreibung | Version |
| --- | --- | --- |
| **SUBSTANCE\_PAINTER\_LICENSE** | Wert: Direkter Pfad zu einer Lizenzdatei.Überschreiben des Standardspeicherorts der Lizenzdatei zulassen. Beispiel : Wenn sich die Lizenzdatei auf **H:/allegorithmic/licenses/substance\_painter.key** befindet, sollten die Variablendaten **&quot;H:/allegorithmic/licenses/substance\_painter.key&quot;** lauten.  **Hinweis:** Verwenden Sie SUBSTANCE\_PAINTER\_2\_LICENSE stattdessen für Version vor 3.x (2017.x). | <ol data-preserve-html="true"><li data-preserve-html="true">1</li></ol> |
| **ALLEGO\_LICENSE\_IDLE\_DELAY** | Wert: 7200Geben Sie an, wie lange (in Sekunden) vor dem Freigeben einer Lizenzlizenz bei einer Konfiguration mit mehreren Benutzern gewartet werden soll. Der Standardwert beträgt 2 Stunden (7200s). | <ol data-preserve-html="true"><li data-preserve-html="true">1</li></ol> |
| **ALG\_PAINTER\_SKIP\_CHECK\_FOR\_UPDATES** | Wert : 0 oder 1 (1 = Update-Prüfung deaktivieren)Ermöglicht das Überspringen der Update-Prüfung beim Start der Anwendung. Deaktivieren Sie den Bereich &quot;Neue Funktionen&quot;. | <ol data-preserve-html="true"><li data-preserve-html="true">2.2</li></ol> |
| **SUBSTANCE\_PAINTER\_SVT\_HARDWARE\_ACCELERATION** | Wert: 0 oder 1 (1 = Aktiviert)Verwenden Sie die Funktion &quot;Selten&quot; auf der GPU. Wenn sie von der GPU oder dem Betriebssystem nicht unterstützt wird, wird die Einstellung ignoriert. Informationen zu kompatiblen Hardwarekonfigurationen finden Sie in der Dokumentation: [Virtuelle Strukturen mit geringer Dichte](../../features/sparse-virtual-textures.md)Diese Variable überschreibt den im Fenster [Einstellungen](../../interface/settings/settings.md) verfügbaren Parameter. | <ol data-preserve-html="true"><li data-preserve-html="true">3</li></ol> |
| **SUBSTANCE\_PAINTER\_TEMP\_LOCATION** | Wert: Direkter Pfad zu einem OrdnerDefiniert, wo der Substance Painter seine temporären Dateien schreiben soll (einschließlich des SVT-Caches).Diese Variable überschreibt den im Fenster [Einstellungen](../../interface/settings/settings.md) verfügbaren Parameter. | <ol data-preserve-html="true"><li data-preserve-html="true">3</li></ol> |
| **SUBSTANCE\_PAINTER\_PREVIEWS\_MEMORY\_BUDGET** | Wert: 500Definiert den Arbeitsspeicher (RAM), den die Anwendung zum Laden und Zwischenspeichern von Vorschauen über das Fenster &quot;Elemente&quot; verwenden kann. Wenn die Grenze des Budgets erreicht ist, werden alte Vorschauen entladen. Dieser Wert steuert nur die Anzeige der Vorschauen im Fenster &quot;Elemente&quot;.Der Wert wird in Megabyte definiert. Der Standardwert ist 500 MB. | <ol data-preserve-html="true"><li data-preserve-html="true">2</li></ol> |
| **SUBSTANCE\_PAINTER\_PLUGINS\_PATH** | Speicherort zusätzlicher Python-Plug-ins. | 6.1 |
| **PYTHONPATH** | Zusätzliche Python-Module, die mit der Python-Integration der Anwendung geladen werden können. Weitere Informationen finden Sie unter [Laden von externen Python-Modulen](https://helpx.adobe.com/de/substance-3d/unlisted/documentation/spdoc/loading-external-python-modules-205363420.html). | <ol data-preserve-html="true"><li data-preserve-html="true">1</li></ol> |
| **OCIO** | Pfad zu einer **config.ocio**-Datei, die verwendet wird, um die [Farbmanagement](../../features/color-management/color-management.md)-Einstellungen mit OpenColorIO zu steuern.  **Hinweis:** Diese Umgebungsvariable hat Vorrang vor der Variablen **PAINTER\_ACE\_CONFIG**. | <ol data-preserve-html="true"><li data-preserve-html="true">4</li></ol> |
| **PAINTER\_ACE\_CONFIG** | Pfad zu einer JSON-Datei, die verwendet wird, um die [Farbmanagement](../../features/color-management/color-management.md)-Einstellungen mit Adobe ACE zu steuern. | <ol data-preserve-html="true"><li data-preserve-html="true">1</li></ol> |
| **SUBSTANCE\_DISABLE\_SPECIFIC\_FEATURES** | Deaktivieren Sie mehrere Funktionen innerhalb der Anwendungen:<ul data-preserve-html="true"><li data-preserve-html="true">Links zu externen Ressourcen (Hilfe, Webseiten, Beispiele usw.)</li><li data-preserve-html="true">Suche nach Updates deaktivieren</li><li data-preserve-html="true">Senden von Nutzungsstatistiken deaktivieren</li><li data-preserve-html="true">Export auf Substance share deaktivieren</li><li data-preserve-html="true">Deaktivieren der Begrüßungs- und Neuerungen-Bedienfelder</li></ul> | <ol data-preserve-html="true"><li data-preserve-html="true">1</li></ol> |
| **ALG\_PAINTER\_DEBUG\_FPS** | Zeigt im Viewport einen Zähler an, der angibt, wie viele Frames pro Sekunde vom Viewport gerendert werden. | <ol data-preserve-html="true"><li data-preserve-html="true">1</li></ol> |
| **SUBSTANCE\_PAINTER\_VRAM\_BUDGET** | Geben Sie an, wie viel GPU-Speicher Painter verwenden kann. Damit wird ein globales Budget in MB festgelegt. Wenn Sie beispielsweise einen Grenzwert von 4 GB definieren möchten, verwenden Sie den Wert 4000. Ein Befehlszeilenargument kann auch verwendet werden, um dieselbe Aktion auszuführen. Siehe [Befehlszeilen](command-lines.md). | <ol data-preserve-html="true"><li data-preserve-html="true">2.1</li></ol> |
