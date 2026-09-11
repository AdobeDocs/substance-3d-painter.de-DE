---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/interface/layer-stack/masking-and-effects.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie Masken und Effekte in Substance 3D Painter Ebenenstapel verwenden, um die Ebenensichtbarkeit zu steuern und Ebeneneffekte anzuwenden.
helpx_creative_field: ""
helpx_description: Painter > Interface > Layer stack > Masking and effects
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Maskierung und Effekte
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '473'
ht-degree: 5%

---


# Maskierung und Effekte

## Maskierung

Ebenen können maskiert werden, um ihren Inhalt nur auf bestimmte Teile der Textur anzuwenden. Die Maske fungiert als Intensitätsparameter über dem Inhalt der Ebene. Eine Maske auf einer Ebene ist immer in Graustufen enthalten, unabhängig davon, welchen Inhalt Sie darüber Malen. (Daher wird jede Farbe vor dem Malen in einen Graustufenwert konvertiert.)

Sie können eine Maske hinzufügen, indem Sie das Kontextmenü verwenden oder die spezielle Schaltfläche verwenden:

![](../../assets/layer-mask.gif)

Mögliche Operationen an Masken :

* Sie können die Maske selbst anzeigen, indem Sie **ALT + Linksklick** auf die Miniaturansicht ausführen. Von dieser Ebene wird der Viewport auf eine isolierte Maskenansicht umgeschaltet. Dieser Funktion ist auch über die Viewer-Einstellungen verfügbar.
* Sie können eine Maske vorübergehend deaktivieren, indem Sie **UMSCHALT + Linksklick** auf die Miniaturansicht ausführen. Wiederholen Sie diesen Vorgang, um ihn wieder zu aktivieren. Diese Funktion ist auch über das Kontextmenü verfügbar („Maske umschalten“).
* Sie können den Inhalt einer Maske in eine andere Maske kopieren, indem Sie **Rechtsklick > Maskeninhalt kopieren** über der Miniaturansicht und dann **Rechtsklick > In Maske einfügen** auf der Miniaturansicht der zweiten Maske ausführen.
* Sie können den Hintergrund der Maske umkehren, indem Sie **Rechtsklick > Maskenhintergrund umkehren** ausführen. Dies ist nützlich, wenn Sie verhindern möchten, dass die mit einer Maske verknüpften Effekte zerstört werden.

>[!WARNING]
>
> Wenn Sie eine Maske erneut hinzufügen oder entfernen, werden die Maske und alle damit verbundenen Effekte zerstört.

Es ist möglich, beim Erstellen einer Füllebene sofort eine Maske zu erstellen (per Drag &amp; Drop), wenn die **STRG**-Taste gedrückt wird:

![](../../assets/mask-material-optimized.gif)

## Effekte

Effekte sind spezielle Vorgänge, die jederzeit bearbeitet werden können. Die Effekte können entweder auf einer Maske oder auf dem Inhalt einer Ebene platziert werden.\
Die Effekte sind jedoch besser für die jeweils andere geeignet. Beispielsweise sind die &quot;Generatoren&quot; für die Masken geeignet.

Die Linie unter jeder Miniaturansicht auf einer Ebene zeigt an, ob Effekte vorhanden sind. Grau = keine Effekte, Rot = mindestens ein Effekt. Es gibt einen Effekt-Stapel pro Maske und pro Inhalt.

![](../../assets/effect.gif)

Weitere Informationen [finden Sie auf der dedizierten Seite &#x200B;](../../features/effects/effects.md).

## Intelligente Masken

Mit den intelligente Masken können Sie eine Maske speichern und ihren Effekt so einsetzen, dass sie in anderen Ebenen oder anderen Projekten wiederverwendet werden kann. Zum Erstellen einer intelligente Maske klicken Sie einfach mit der rechten Maustaste auf eine Maske und wählen Sie &quot;**intelligente Maske erstellen**&quot; aus.\
Wenn Sie eine intelligente Maske per Drag &amp; Drop auf eine Ebene ziehen und ablegen, wird eine schwarze Maske erstellt, sofern sie noch nicht vorhanden ist. Andernfalls wird die Effektliste mit der bestehenden Ebene zusammengeführt. Es ist möglich, die Effektliste vollständig zu überschreiben, indem &quot;**CTRL**&quot; beim Ablegen der intelligente Maske gedrückt gehalten wird.

![](../../assets/smart-mask-new-optimized.gif)

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../assets/smart-mask-add-optimized.gif)

</td>
<td style="border: 0;" valign="top">

![](../../assets/smart-mask-overwrite-optimized.gif)

</td>
</tr>
</table>
