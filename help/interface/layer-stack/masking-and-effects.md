---
helpx_url: "https://helpx.adobe.com/de/substance-3d-painter/interface/layer-stack/masking-and-effects.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie Masken und Effekte in Substance 3D Painter-Ebenenstapeln verwenden, um die Ebenensichtbarkeit zu steuern und Ebeneneffekte anzuwenden.
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

Ebenen können maskiert werden, um ihren Inhalt nur auf bestimmte Teile der Textur anzuwenden. Die Maske fungiert als Intensitätsparameter über dem Inhalt der Ebene. Eine Maske auf einer Ebene ist immer in Graustufen enthalten, unabhängig davon, mit welchem Inhalt Sie darüber malen (daher wird jede Farbe vor dem Malen in einen Graustufenwert konvertiert).

Sie können eine Maske hinzufügen, indem Sie das Kontextmenü verwenden oder die spezielle Schaltfläche verwenden:

![](../../assets/layer-mask.gif)

Mögliche Operationen an Masken :

* Sie können die Maske selbst anzeigen, indem Sie **ALT + Linksklick** auf die Miniaturansicht ausführen. Von dieser Ebene wird das Ansichtsfenster auf eine isolierte Ansicht der Maske umgeschaltet. Dieser Funktion ist auch über die Viewer-Einstellungen verfügbar.
* Sie können eine Maske vorübergehend deaktivieren, indem Sie **UMSCHALT + Linksklick** auf die Miniaturansicht ausführen. Wiederholen Sie diesen Vorgang, um ihn wieder zu aktivieren. Diese Funktion ist auch über das Kontextmenü verfügbar („Maske umschalten“).
* Sie können den Inhalt einer Maske in eine andere Maske kopieren, indem Sie **Rechtsklick > Maskeninhalt kopieren** über der Miniaturansicht und dann **Rechtsklick > In Maske einfügen** auf der Miniaturansicht der zweiten Maske ausführen.
* Sie können den Hintergrund der Maske umkehren, indem Sie **Rechtsklick > Maskenhintergrund umkehren** ausführen. Dies ist nützlich, wenn Sie verhindern möchten, dass die mit einer Maske verknüpften Effekte zerstört werden.

>[!WARNING]
>
> Wenn Sie eine Maske erneut hinzufügen oder entfernen, werden die Maske und alle damit verbundenen Effekte zerstört.

Es ist möglich, beim Erstellen einer Füllebene (per Drag &amp; Drop) sofort eine Maske zu erstellen, wenn die **STRG**-Taste gedrückt wird:

![](../../assets/mask-material-optimized.gif)

## Effekte

Effekte sind spezielle Vorgänge, die jederzeit bearbeitet werden können. Die Effekte können entweder auf einer Maske oder auf dem Inhalt einer Ebene platziert werden.\
Die Effekte sind jedoch besser für die jeweils andere geeignet. Beispielsweise sind die &quot;Generatoren&quot; für die Masken geeignet.

Die Linie unter jeder Miniaturansicht auf einer Ebene zeigt an, ob Effekte vorhanden sind. Grau = keine Effekte, Rot = mindestens ein Effekt. Es gibt einen Effektstapel pro Maske und pro Inhalt.

![](../../assets/effect.gif)

Weitere Informationen [finden Sie auf der dedizierten Seite &#x200B;](../../features/effects/effects.md).

## Intelligente Masken

Mithilfe der Smart-Masken können Sie eine Maske und ihren Effekt speichern, um sie auf einfache Weise für andere Ebenen oder andere Projekte wiederzuverwenden. Klicken Sie zum Erstellen einer Smartmaske einfach mit der rechten Maustaste auf eine Maske und wählen Sie &quot;**Smartmaske erstellen**&quot; aus.\
Wenn Sie eine Smart-Maske per Drag-and-Drop auf eine Ebene ziehen, wird eine schwarze Maske erstellt, sofern sie noch nicht vorhanden ist. Andernfalls wird die Effektliste mit der vorhandenen zusammengeführt. Es ist möglich, die Effektliste vollständig zu überschreiben, indem beim Ablegen der Smartmaske &quot;**CTRL**&quot; gedrückt gehalten wird.

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
