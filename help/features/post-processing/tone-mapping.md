---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/post-processing/tone-mapping.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie die Tonzuordnungs-Nachbearbeitung in Substance 3D Painter verwenden, um die Belichtung und die Farbkorrektur im Viewport anzupassen.
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
> Substance 3D Painter gibt **HDR** (High Dynamic Range)-Farben (im linearen Gamma-Bereich) aus, aber die meisten Bildschirme ermöglichen nur die Darstellung von **LDR** (Low Dynamic Range)-Farben. Um den HDR-Bereich dem LDR-Bereich zuzuordnen, muss eine Konvertierung durchgeführt werden. Dies ist das Prinzip der Tonkartierung.

| *Einstellung* | *Beschreibung* |
| --- | --- |
| **Belichtung** | Skaliert die Renderingergebnisse des HDR-Raums, bevor Blendeffekte angewendet oder eine Farbtonzuordnung durchgeführt werden. |
| **Gamma** | Dies ist der Gamma-Wert für die Gamma-Korrektur. |
| **Funktion** | Funktion zum Zuordnen des HDR-Bereichs zum LDR-Bereich.  Verfügbare Funktionen sind:<ul data-preserve-html="true"><li data-preserve-html="true"><strong> Auto </strong> : Die Farbtonzuordnungsfunktion wird automatisch ausgewählt. Der Standardwert ist <strong> Sensitometrisch </strong> . </li><li data-preserve-html="true"><strong> Linear </strong> : Die Ausgabefarbe ist nur für diesen Typ nicht auf 0 bis 1 festgeklemmt. Dies ist optimal für die Implementierung von Effekten im HDR-Raum auf der Anwendungsseite nach dem Anwenden der Effekte. <br/>Wir empfehlen dies nur, wenn Sie einen bestimmten Grund für die Verwendung haben, da die Komponenten mit hoher Luminanz vollständig verloren gehen und überbelichtete Glanzlichter auftreten, wenn eine lineare Zuordnung als endgültige Bildschirmausgabe verwendet wird.</li><li data-preserve-html="true"><strong> LinearSat </strong> : Dies ist fast dasselbe wie <strong> Linear </strong> , mit dem Unterschied, dass die Ausgabefarbe eingeklemmt ist. Außerdem ist die Blendsynthese etwas glatter als <strong> linear </strong> .</li><li data-preserve-html="true"><strong> sensitometrisch </strong> : Standardfunktion, wenn das Rendern von Szenen im HDR-Raum ausgeführt wird.</li><li data-preserve-html="true"><strong> Reinhard </strong>: Dies führt zu einer Zuordnung, die gradueller als <strong> Sensitometrisch </strong> ist, und zu einem leicht niedrigen Kontrast. Dadurch wird die Auflösung der hohen Luminanzkomponenten erhöht und die Reproduktion der Luminanzschwankungen in den hellen Bereichen verstärkt.</li><li data-preserve-html="true"><strong> ReinhardLum </strong> : Typ für die Implementierung der <strong> Reinhard </strong>-Farbtonzuordnung mit der Luminanz als Referenz und unter Beibehaltung der ursprünglichen Sättigung (Leuchtkraft: RGB-Verhältnis). Weist dem LDR-Raum nur die Luminanzinformationen zu und gibt dann die ursprüngliche Sättigung wieder. Die Sättigung im HDR-Raum wird auch nach der Tonzuordnung beibehalten.</li><li data-preserve-html="true"><strong> Protokoll </strong> : Dies führt zu einer Zuordnung, die noch gradueller als <strong> ist Reinhard </strong> , und zu einem geringen Kontrast. Sie bewirkt, dass die Auflösung der Komponenten mit hoher Luminanz hoch wird und die stärkste Reproduktion der Luminanzschwankungen in den hellen Bereichen.</li><li data-preserve-html="true"><strong> LogLum </strong> : Typ zum Implementieren der Gradationskurve des logarithmischen Raums mit der Luminanz als Referenz und Beibehaltung der ursprünglichen Sättigung (Leuchtkraft: RGB-Verhältnis). Dies ordnet nur die Luminanzinformationen dem logarithmischen Raum zu und gibt dann die ursprüngliche Sättigung wieder. Die Sättigung im HDR-Raum wird auch nach der Tonzuordnung beibehalten.</li></ul> |
| **Zuordnungsfaktor** | Dadurch wird die maximale Luminanz (Helligkeit) im HDR-Raum gesteuert, die dem endgültigen LDR-Raum im Tonzuordnungsprozess zugeordnet wird. Farben, die heller als die angegebene HDR-Raumluminanz sind, können im LDR-Raum nicht dargestellt werden, was zu überbelichteten Glanzlichtern führt. Konkret ist dieser Wert die Luminanz (nach Belichtungsskalierung) im HDR-Raum, die dem maximalen Luminanzwert (1,0) im LDR-Raum entspricht. Im HDR-Rendering-Modus gilt: Je niedriger dieser Wert ist, desto höher ist der Kontrast und desto größer ist die Wahrscheinlichkeit ausgeblasener Glanzlichter. Umgekehrt führt die Angabe höherer Werte zu einem niedrigeren Kontrast und verringert die Wahrscheinlichkeit, dass Glanzlichter ausgeblendet werden. Wenn im LDR-Rendering-Modus eine Neuzuordnung zum HDR-Raum erfolgt, um einen Effekt anzuwenden, wird der Luminanzbereich bis zu dem in **Zuordnungsfaktor** angegebenen Wert erweitert. Umgekehrt wird die Luminanz des **Zuordnungsfaktors** während der Tonzuordnung der maximalen LDR-Luminanz zugeordnet.Mit anderen Worten, dies gibt den dynamischen Bereichsskalierungsfaktor an, der auf die LDR-Renderingergebnisse für die Anwendung von Effekten angewendet wird. Wenn Sie diesen Wert auf einen hohen Wert setzen, werden helle Bereiche in Effekten hervorgehoben.  **Hinweis:** Diese Einstellung hat keine Auswirkungen (sie wird ignoriert), wenn die **Funktion** im HDR-Rendering-Modus auf einen der folgenden Werte eingestellt ist:  **Linear** , **LinearSat** oder **Sensitometrisch** . |
