---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/project-resources.html"
breadcrumb-title: ''
description: Greifen Sie auf Projektressourcen und technische Dokumentation für Substance 3D Painter zu, um Ihren Workflow und die Fehlerbehebung zu verbessern.
helpx_creative_field: ""
helpx_description: Substance 3D Painter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Projektressourcen
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 0%

---


# Projektressourcen und -einstellungen

Die Verwaltung von Projektressourcen kann Ihnen dabei helfen, eine gute Grundlage für die Leistung Ihres Projekts in Painter zu schaffen.

+++Durch Baking erzeugte Map herunterskalieren
Manchmal müssen nicht alle durch Baking erzeugte Map eine Auflösung von 2k oder 4k haben. Zögern Sie nicht, einen Stapel bei 2k zu backen, dann mit einer niedrigeren Auflösung erneut zu backen, um zu sehen, ob ein visueller Unterschied besteht.

+++

+++Verwalten von importierten Bitmaps
Importierte Bilder können die Leistung erheblich beeinträchtigen. Daher ist es wichtig, den Importvorgang genau zu verfolgen. Wenn deine Textursets auf 2k eingestellt sind und sowieso nicht mit einer höheren Auflösung exportiert werden, hat die Verwendung eines 8k-Bildes keine positiven Auswirkungen - seine Qualität wird auf 2k begrenzt, da dies die Auflösung des Textursets ist.

Auch das Format spielt eine Rolle - EXR, HDR und sogar PNG sind viel umfangreicher als eine JPG, und nicht alle Heights benötigen möglicherweise den Qualitätsgrad einer EXR (z. B. Grundfarbe oder Bilddetails).

+++

+++Shader-Einstellungen anpassen
Specular-Qualität bei Ultra wird ein präziseres Ergebnis liefern, aber die Einstellung ist kostspielig. Je mehr Effekte gleichzeitig im Shader aktiviert werden, desto schwerer ist die Berechnung. Teile komplexe Materialien nach Möglichkeit mit einem separaten Shader in ein anderes Texturset auf. Wenn Versatz aktiviert ist, achten Sie auf den Parameter &quot;Tessellation&quot;.

+++

+++Dateioptionen anpassen
Verwenden von <b>Datei > Speichern > Speichern und Reduzieren von Datei</b> <b>Größe </b>, um nicht benötigte Daten zu leeren, und <b>Nicht verwendete Ressourcen entfernen</b>, um in das Projekt importierte Dateien zu entfernen, die nirgendwo im Projekt verwendet werden.

+++
