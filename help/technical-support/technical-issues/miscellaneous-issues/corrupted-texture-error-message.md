---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/technical-support/technical-issues/miscellaneous-issues/corrupted-texture-error-message.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie Fehlermeldungen zu beschädigten Texturen in Substance 3D Painter beheben, um die Funktionen zur Textur wiederherzustellen.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Miscellaneous Issues > Corrupted texture error message
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Fehlermeldung "Beschädigte Textur"
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 0%

---


# Fehlermeldung &quot;Beschädigte Textur&quot;

Beschädigte Texturen in einem Projekt verursachen beim Speichern Fehler und können dazu führen, dass Projekte vollständig beschädigt und nicht rückgängig gemacht werden können. Dies kann jedoch manuell behoben werden.\
Eine beschädigte Ressource wird im Protokoll angezeigt, wenn ein Projekt mit einer ähnlichen Fehlermeldung wie im Protokollfenster geöffnet wird:

![](../../../assets/corrupt1.png)

## Korrigieren eines beschädigten Ressourcenverweises

### 1 - Suchen der Ressource

Der erste Schritt, wenn ein Fehler angezeigt wird, ist das Suchen und Identifizieren der problematischen Ressource.\
In den meisten Fällen stammt der Schuldige aus den **Mesh-Map** (Baking geführt Texturen). Das lässt sich schnell überprüfen, indem man sich die Maskengenerator im Ebenenstapel ansieht.

Beschädigte Ressourcen werden wie folgt aussehen:

![](../../../assets/corrupt2.png)

>[!NOTE]
>
> Das könnte auch bedeuten, dass die Ressource einfach fehlt.\
> Versuchen Sie, den Steckplatz zu leeren und das Baking manuell erneut zu beeinflussen. Wenn das rote Kreuz weiterhin angezeigt wird, bedeutet dies, dass die Ressource beschädigt ist.

### 2 - Ersetzen der Ressource

Um eine beschädigte Ressource zu ersetzen, müssen zuerst alle Verweise darauf entfernt werden. Ist der Strom relativ klein, kann dies manuell erfolgen.\
Wenn sich das Projekt jedoch über mehrere Textursatz oder viele Ebenen erstreckt, kann der [Ressourcenaktualisierer](../../../features/plugins/resources-updater.md) hilfreich sein, um die beschädigte Ressource zu finden und sie vorübergehend durch eine andere zu ersetzen.

>[!NOTE]
>
> * Vergessen Sie bei den Baking geführt Texturen nicht, auch die Mesh-Map-Steckplätze im Fenster &quot;[Textursatz settings](../../../interface/texture-set/texture-set-settings.md)&quot; zu löschen.
> * Baking führte, die nur in den Textursatz-Einstellungen wie der Normalen-Map verwendet werden, können ebenfalls beschädigt werden. Versuchen Sie auch, sie zu entfernen, wenn weiterhin Fehler auftreten.

### 3 - Bereinigung

Sobald alle Verweise auf die beschädigten Ressourcen verschwunden sind, führen Sie eine Bereinigung des Projekts über das Hauptmenü durch (**Datei** > **Bereinigen**).\
Dadurch sollten alle jetzt nicht verwendeten beschädigten Ressourcen aus dem Projekt entfernt werden. Sie können dies überprüfen, indem Sie im Regal zur Registerkarte Projekt navigieren, um sicherzustellen, dass alle problematischen Ressourcen verschwunden sind.

### 4 - Speichern

Versuchen Sie nach der Bereinigung, das Projekt zu speichern :

* Wenn es fehlerfrei speichert, ist das Projekt jetzt frei von Beschädigungen (Mesh-Map können jetzt rückgängig gemacht und Ressourcen erneut importiert werden).
* Wenn weiterhin Fehler auftreten, bedeutet dies, dass im Projekt weiterhin auf eine beschädigte Ressource verwiesen wird.
