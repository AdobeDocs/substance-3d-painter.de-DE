---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/gpu-issues/gpu-drivers-crash-with-long-computations-tdr-crash.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie Abstürze von GPU-Treibern während langer Berechnungen in Substance 3D Painter beheben können, um TDR-Zeitüberschreitungsfehler zu vermeiden.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > GPU Issues > GPU drivers crash with long computations (TDR crash)
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: GPU-Treiber stürzen mit langen Berechnungen ab (TDR-Absturz)
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '859'
ht-degree: 0%

---


# GPU-Treiber stürzen mit langen Berechnungen ab (TDR-Absturz)

![TDR-Warnung in Substance 3D Painter](../../../assets/tdr-window-v2.png "TDR-Warnung in Substance 3D Painter"){zoomable="yes"}

Unter Windows wird dieses Fenster angezeigt, wenn Substance 3D Painter erkennt, dass der aktuelle TDR-Wert unter einem bestimmten Grenzwert liegt (10 Sekunden).

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

## Warum stürzt der GPU-Treiber ab?

</td>
<td style="border: 0;" valign="top">

### Bearbeiten der TDR-Werte

</td>
<td style="border: 0;" valign="top">

### TDR-Werte auf Standardwerte zurücksetzen

</td>
</tr>
</table>

## Warum stürzt der GPU-Treiber ab?

Um zu verhindern, dass das System **durch Rendering oder GPU-Berechnung** blockiert wird, beendet das Windows-Betriebssystem **den GPU-Treiber**, wenn das Rendern mehr als einige Sekunden dauert. Wenn der Treiber beendet wird, stürzt die Anwendung, die ihn verwendet, automatisch ab. Es ist nicht möglich zu wissen, wie lange eine Rendering-Aufgabe oder eine Berechnung dauern kann (es hängt von der GPU, den Treibern, dem Betriebssystem, der Maschengröße, der Texturgröße usw. ab), daher ist es nicht möglich, die Verarbeitungsdauer des Computers zu begrenzen und den Absturz von der Anwendungsebene aus zu vermeiden.

Unter Windows gibt es eine **Registrierung** **Schlüssel**, die angibt, wie lange das Betriebssystem warten soll, bevor der GPU-Treiber beendet wird. Anwendungen sind nicht berechtigt, diese Einstellung direkt zu ändern, dieses Verfahren muss manuell durchgeführt werden (siehe unten).

Weitere Informationen finden Sie in der offiziellen Dokumentation: <https://docs.microsoft.com/en-us/windows-hardware/drivers/display/tdr-registry-keys>

### Liste der Schlüssel, die geändert werden müssen

Um den TDR anzupassen, erhöhen Sie einfach die TDR-Verzögerung: ändern Sie sowohl **TdrDelay** als auch **TdrDdiDelay** in einen höheren Wert (z. B. 60 Sekunden).

![TDR-Schlüssel im Windows-Registrierungs-Editor](../../../assets/registry-example.png "TDR-Schlüssel im Windows-Registrierungs-Editor"){zoomable="yes"}

>[!NOTE]
>
> Beachten Sie, dass diese Tasten durch Windows-Updates oder Updates von GPU-Treibern auf ihren Standardwert zurückgesetzt werden können.

## Bearbeiten der TDR-Werte

Gehen Sie wie folgt vor, um den TDR-Wert zu ändern.

***Beachten Sie, dass zwei verschiedene Schlüssel erstellt/bearbeitet werden müssen.***

>[!WARNING]
>
> Bitte beachten Sie, dass die Bearbeitung der Registrierung schwerwiegende, unerwartete Folgen haben kann, die den Systemstart verhindern können, und möglicherweise eine Neuinstallation des gesamten Betriebssystems erforderlich machen kann, wenn Sie sich nicht sicher sind, wie Sie es ändern können. Die auf dieser Seite erwähnten Registrierungsschlüssel sollten solche Probleme jedoch nicht verursachen.
> 
> Adobe übernimmt keine Verantwortung für Schäden an Ihrem System durch Ändern der Systemregistrierung.

### 1 - Öffnen Sie das Fenster Ausführen.

Klicken Sie auf **Start** und anschließend auf **Ausführen** (oder drücken Sie die Tasten **Windows** und **R**). Das Fenster &quot;**Ausführen**&quot; wird geöffnet.

![Windows-Dialogfeld &quot;Ausführen&quot;](../../../assets/run-window.png "Windows-Dialogfeld &quot;Ausführen&quot;"){zoomable="yes"}

### 2 - Starten Sie den Registrierungseditor

Geben Sie **regedit** in das Textfeld ein, und drücken Sie **OK**.

![&#39;regedit&#39; im Windows-Dialogfeld &quot;Ausführen&quot; ](../../../assets/run-regedit-2.png "&#39;regedit&#39; im Windows-Dialogfeld &quot;Ausführen&quot; "){zoomable="yes"}

### 3 - Navigieren Sie zum Registrierungsschlüssel GraphicsDrivers .

Das Registrierungsfenster wird geöffnet.\
Navigieren Sie im linken Bereich in der Struktur zum Schlüssel **GraphicsDrivers**, indem Sie wie folgt vorgehen:

```
Computer\HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\GraphicsDrivers
```


Vergewissern Sie sich, dass **auf** &quot;GraphicsDrivers&quot; (Grafiktreiber) und **auf** auf der Registrierung **Schlüssel unten** nicht klicken, bevor Sie die nächsten Schritte ausführen.

+++&#39;GraphicsDrivers&#39; in der Windows-Registrierungsstruktur
![ &quot;GraphicsDrivers&quot; in der Windows-Registrierungsstruktur ](../../../assets/reg-left-pane.png " &quot;GraphicsDrivers&quot; in der Windows-Registrierungsstruktur "){zoomable="yes"}



+++

### 4 - TdrDelay-Wert hinzufügen oder bearbeiten

>[!NOTE]
>
> Wenn der <b>TdrDelay</b>-Wert <b> noch nicht vorhanden ist</b>, klicken Sie mit der rechten Maustaste in den rechten Bereich und wählen Sie <b>Neu > DWORD(32bit)-Wert</b> . Nennen Sie ihn &quot;<b>TdrDelay</b>&quot;. Die Groß-/Kleinschreibung ist wichtig. Achten Sie darauf, ihr zu folgen (und stellen Sie sicher, dass keine weiteren Zeichen vorhanden sind, z. B. nachgestellte Leerzeichen).
> 
> ![](../../../assets/create-value.png)

Doppelklicken Sie im **rechten Fensterbereich** auf den Wert **TdrDelay**. Ändern Sie die **Base**-Einstellung in **Decimal** . Setzen Sie den Wert auf einen anderen Wert als den Standardwert **2** (wir empfehlen **60**).

Dieser Wert gibt in Sekunden an, wie lange das Betriebssystem warten wird, bevor es berücksichtigt, dass die GPU während einer Berechnung nicht reagiert.

![ &#39;TdrDelay&#39; DWORD-Wert im Windows-Registrierungs-Editor ](../../../assets/tdrdelay-edit.png " &#39;TdrDelay&#39; DWORD-Wert im Windows-Registrierungs-Editor "){zoomable="yes"}

### 5 - Hinzufügen oder Bearbeiten des TdrDdiDelay-Werts

>[!NOTE]
>
> Wenn der <b>TdrDdiDelay</b>-Wert <b> nicht vorhanden ist</b> , klicken Sie mit der rechten Maustaste in den rechten Bereich und wählen Sie <b>Neu > DWORD(32bit)-Wert</b> . nennen Sie ihn &quot;<b>TdrDdiDelay</b> &quot;. Falls wichtig, folgen Sie der Groß-/Kleinschreibung (und stellen Sie sicher, dass keine weiteren Zeichen wie Leerzeichen vorhanden sind).
> 
> ![](../../../assets/create-value.png)

Doppelklicken Sie im **rechten Fensterbereich** auf den Wert **TdrDdiDelay** . Ändern Sie die **Base**-Einstellung in **Decimal** . Setzen Sie den Wert auf einen anderen Wert als den Standardwert **5** (wir empfehlen **60** ).

Dieser Wert gibt in Sekunden an, wie lange das Betriebssystem warten wird, bevor es berücksichtigt, dass es zu lange gedauert hat, bis eine Software die GPU-Treiber verlassen hat.

**Hexadezimal** ist der Standardwert. Wechseln Sie einfach zu **Dezimal**, um den richtigen Wert anzuzeigen. Beachten Sie, dass **3C** (Hexadezimal) gleich **60** (Dezimal) ist.

### 6 - Fertigstellen und Neustarten

Der rechte Bereich sollte nun so aussehen:

![TDR-Schlüssel im Windows-Registrierungs-Editor - Final](../../../assets/registry-example.png "TDR-Schlüssel im Windows-Registrierungs-Editor - Final"){zoomable="yes"}

**Schließen Sie** den Registrierungseditor. **Starten Sie den Computer neu**, indem Sie **Start** und anschließend **Neu starten** verwenden.

Der TdrValue wird nur beim Starten des Computers überprüft, sodass ein Neustart erforderlich ist, um eine Aktualisierung zu erzwingen.

Wenn die Anwendung bei einer langen Berechnung immer noch abstürzt, versuchen Sie, die Verzögerung (in Sekunden) von 60 auf 120 zu erhöhen.

## TDR-Werte auf Standardwerte zurücksetzen

Es gibt zwei Möglichkeiten, den TDR auf die Standardwerte zurückzusetzen:

* Legen Sie die **TdrDelay** auf **2s** und die **TdrDdiDelay** auf **5s** fest, indem Sie die oben beschriebenen Schritte ausführen.
* Oder **Entfernen** Sie die Schlüssel **TdrDelay** und **TdrDdiDelay** aus dem Registrierungseintrag.
