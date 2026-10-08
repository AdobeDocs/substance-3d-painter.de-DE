---
breadcrumb-title: ""
description: Greifen Sie auf Projektressourcen und technische Dokumentation für Substance 3D Painter zu, um Ihren Workflow und die Fehlerbehebung zu verbessern.
title: Projektressourcen
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 0%
---

# Projektressourcen und -einstellungen

Die Verwaltung von Projektressourcen kann Ihnen dabei helfen, eine gute Grundlage für die Leistung Ihres Projekts in Painter zu schaffen.

+++Durch Baking erzeugte Map herunterskalieren
Manchmal müssen nicht alle durch Baking erzeugte Map eine Auflösung von 2k oder 4k haben. Zögern Sie nicht, einen Stapel mit 2k Baking führen und dann mit einer niedrigeren Auflösung erneut zu erstellen, um festzustellen, ob ein sichtbarer Unterschied besteht.

+++

+++Verwalten von importierten Bitmaps
Importierte Bilder können die Leistung erheblich beeinträchtigen. Daher ist es wichtig, den Importvorgang genau zu verfolgen. Wenn deine Textursatz auf 2k eingestellt sind und sowieso nicht mit einer höheren Auflösung exportiert werden, hat die Verwendung eines 8k-Bildes keine positiven Auswirkungen - seine Qualität wird auf 2k begrenzt, da dies die Auflösung des Textursatzes ist.

Auch das Format spielt eine Rolle - EXR, HDR und sogar PNG sind viel umfangreicher als eine JPG, und nicht alle Heights benötigen möglicherweise den Qualitätsgrad einer EXR (z. B. Grundfarbe oder Bilddetails).

+++

+++Shader-Einstellungen anpassen
Specular-Qualität bei Ultra wird ein präziseres Ergebnis liefern, aber die Einstellung ist kostspielig. Je mehr Effekte gleichzeitig im Shader aktiviert werden, desto schwerer ist die Berechnung. Wenn möglich, teilen Sie komplexe Material auf einen anderen Textursatz mit einem separaten Shader auf. Wenn Versatz aktiviert ist, achten Sie auf den Parameter &quot;Tessellation&quot;.

+++

+++Dateioptionen anpassen
Verwenden von <b>Datei > Speichern > Speichern und Reduzieren von Datei</b> <b>Größe </b>, um nicht benötigte Daten zu leeren, und <b>Nicht verwendete Ressourcen entfernen</b>, um in das Projekt importierte Dateien zu entfernen, die nirgendwo im Projekt verwendet werden.

+++
