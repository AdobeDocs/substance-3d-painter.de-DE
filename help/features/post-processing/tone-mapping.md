---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/features/post-processing/tone-mapping.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie die Tonzuordnungs-Nachbearbeitung in Substance 3D Painter verwenden, um Belichtung und Farbkorrektur im Viewport anzupassen.
helpx_creative_field: ""
helpx_description: Painter > Features > Post Processing > Tone Mapping
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Tone Mapping
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '690'
ht-degree: 0%

---


# Tone Mapping

![](../../assets/tone-mapping.png)

Mit den Parametern der Farbtonzuordnung können Sie steuern, wie die Farben skaliert werden, damit sie auf dem Bildschirm angezeigt werden. Diese Einstellungen können nützlich sein, um Farben aufgrund ihres breiten Wertebereichs (der über den Bereich hinausgehen kann, der auf dem aktuellen Bildschirm angezeigt werden kann) neu zu verteilen.

>[!NOTE]
>
> Substance 3D Painter gibt **HDR.** (High Dynamic Range) Farben (im linearen Gamma-Bereich) aus, aber die meisten Bildschirme ermöglichen nur die Darstellung von **LDR** (Low Dynamic Range) Farben. Um den HDR-Bereich dem LDR-Bereich zuzuordnen, muss eine Konvertierung durchgeführt werden. Dies ist das Prinzip der Tonkartierung.

| *Einstellung* | *Beschreibung* |
| --- | --- |
| **Belichtung** | Skaliert die Ergebnisse der HDR-Renderings, bevor Blendeffekt-Effekte angewendet oder eine Farbtonzuordnung durchgeführt werden. |
| **Gamma** | Dies ist der Gamma-Wert für die Gamma-Korrektur. |
| **Funktion** | Funktion zur Zuordnung des HDR zum LDR-Bereich.  Verfügbare Funktionen sind:<ul data-preserve-html="true"><li data-preserve-html="true"><strong> Auto </strong> : Die Farbtonzuordnungsfunktion wird automatisch ausgewählt. Der Standardwert ist <strong> Sensitometrisch </strong> . </li><li data-preserve-html="true"><strong> Linear </strong> : Die Ausgabefarbe ist nur für diesen Typ nicht auf 0 bis 1 festgeklemmt. Dies ist optimal für die Implementierung eines Effekts im HDR.-Bereich auf der Anwendungsseite nach dem Anwenden der Effekte. <br/>Wir empfehlen dies nur, wenn Sie einen bestimmten Grund für die Verwendung haben, da die Komponenten mit hoher Luminanz vollständig verloren gehen und ausgebrannte Lichter auftreten, wenn eine lineare Zuordnung als endgültige Bildschirmausgabe verwendet wird.</li><li data-preserve-html="true"><strong> LinearSat </strong> : Dies ist fast dasselbe wie <strong> Linear </strong> , mit dem Unterschied, dass die Ausgabefarbe eingeklemmt ist. Außerdem ist die Blendeffekt-Synthese etwas glatter als <strong> linear </strong> .</li><li data-preserve-html="true"><strong> sensitometrisch </strong> : Standardfunktion, wenn das Rendern von Szenen im HDR-Raum ausgeführt wird.</li><li data-preserve-html="true"><strong> Reinhard </strong>: Dies führt zu einer Zuordnung, die gradueller als <strong> Sensitometrisch </strong> ist, und zu einem leicht niedrigen Kontrast. Dadurch wird die Auflösung der Komponenten mit hoher Luminanz erhöht und die Wiedergabe der Luminanz ändert sich in den hellen Bereichen stärker.</li><li data-preserve-html="true"><strong> ReinhardLum </strong> : Typ für die Implementierung der <strong> Reinhard </strong>-Farbtonzuordnung mit der Luminanz als Referenz und unter Beibehaltung der Originalsättigung (Lebhaftigkeit: RGB-Verhältnis). Ordnet nur die Luminanz-Informationen dem LDR-Raum zu und gibt dann die ursprüngliche Sättigung wieder. Die Sättigung im HDR wird auch nach der Tonzuordnung beibehalten.</li><li data-preserve-html="true"><strong> Protokoll </strong> : Dies führt zu einer Zuordnung, die noch gradueller als <strong> ist Reinhard </strong> , und zu einem geringen Kontrast. Sie bewirkt, dass die Auflösungen der Komponenten mit hoher Luminanz hoch werden und die stärkste Reproduktion der Luminanz in den hellen Bereichen variiert.</li><li data-preserve-html="true"><strong> LogLum </strong> : Typ zum Implementieren der Gradationskurve des logarithmischen Raums mit der Luminanz als Referenz und unter Beibehaltung der Originalsättigung (Leuchtkraft: RGB-Verhältnis). Dadurch werden nur die Luminanz-Informationen dem logarithmischen Raum zugeordnet und anschließend die ursprüngliche Sättigung wiedergegeben. Die Sättigung im HDR wird auch nach der Tonzuordnung beibehalten.</li></ul> |
| **Zuordnungsfaktor** | Dadurch wird die maximale Stufe der Luminanz (Helligkeit) im HDR-Raum gesteuert, der dem endgültigen LDR-Raum im Tonzuordnungsprozess zugeordnet wird. Farben, die heller als die angegebene HDR sind, können nicht im LDR-Raum dargestellt werden, was zu überbelichteten Glanzlichtern führt. Konkret ist dieser Wert die Luminanz (nach Belichtungsskalierung) im HDR, die dem Maximalwert der Luminanz (1,0) im LDR-Raum entspricht. Im HDR-Rendering-Modus gilt: Je niedriger dieser Wert ist, desto höher ist der Kontrast und desto größer ist die Wahrscheinlichkeit ausgeblasener Glanzlichter. Umgekehrt führt die Angabe höherer Werte zu einem niedrigeren Kontrast und verringert die Wahrscheinlichkeit, dass Glanzlichter ausgeblendet werden. Wenn im LDR-Rendering-Modus eine Neuzuordnung zum HDR. Leerzeichen erfolgt, um einen Effekt anzuwenden, wird der Bereich der Luminanz bis zu dem in **Zuordnungsfaktor** angegebenen Wert erweitert. Umgekehrt wird die **Zuordnungsfaktor**-Luminanz während der Tonzuordnung der maximalen LDR-Luminanz zugeordnet.Mit anderen Worten, dies gibt den dynamischen Bereichsskalierungsfaktor an, der auf die LDR-Renderingergebnisse für die Anwendung von Effekten angewendet wird. Wenn Sie diesen Wert auf einen hohen Wert setzen, werden helle Bereiche in Effekten hervorgehoben.  **Hinweis:** Diese Einstellung hat keine Auswirkungen (sie wird ignoriert), wenn die **Funktion** im HDR-Rendermodus auf einen der folgenden Werte eingestellt ist:  **Linear** , **LinearSat** oder **Sensitometrisch** . |
