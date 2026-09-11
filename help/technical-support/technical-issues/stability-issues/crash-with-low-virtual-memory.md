---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/stability-issues/crash-with-low-virtual-memory.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie Substance 3D Painter-Absturz beheben, die durch zu wenig virtuellen Speicher verursacht werden, um eine stabile Anwendungsleistung zu gewährleisten.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Stability Issues > Crash with low virtual memory
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Absturz mit wenig virtuellem Arbeitsspeicher
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 0%

---


# Absturz mit wenig virtuellem Arbeitsspeicher

Substance 3D Painter kann instabil sein, wenn die Datei **paging** ( **swap** Speicher/ **virtueller** Speicher) mit einem Wert **zu niedrig** festgelegt ist.\
Es wird empfohlen, diese Einstellungen vom Betriebssystem behandeln zu lassen (was in der Regel standardmäßig der Fall ist). Substance 3D Painter benötigt mindestens **** **16 GB** virtuellen Speicher, damit es ordnungsgemäß funktioniert.

## Wie kann ich die Größe des virtuellen Arbeitsspeichers unter Windows ändern?

>[!NOTE]
>
> Wenn Sie die Größe des virtuellen Arbeitsspeichers unter Windows ändern, muss der Computer neu gestartet werden.

Zugriff auf die Einstellungen für den virtuellen Arbeitsspeicher mit den folgenden Schritten

1. Klicken Sie mit der rechten Maustaste auf das Symbol **Computer/This PC** und wählen Sie **Eigenschaften** aus.
1. &quot;**Erweiterte Systemeinstellungen**&quot; auswählen
1. Klicken Sie im Abschnitt **Leistung** auf die Schaltfläche **Einstellungen**.
1. Klicken Sie auf die Registerkarte **Erweitert**.
1. Klicken Sie im Abschnitt **Virtueller Speicher** auf **Ändern**.

Jetzt ist es möglich:

* Aktivieren Sie das Kontrollkästchen **Paging-Dateigröße für alle Laufwerke automatisch verwalten**

**oder**

* Wählen Sie die Festplatte aus, auf der Sie die Größe des virtuellen Arbeitsspeichers ändern möchten, wählen Sie **Vom System verwaltete Größe** aus, und klicken Sie auf die Schaltfläche **Festlegen**.

**Automatisch:**

![](../../../assets/virtual-memory-default.png)

**Manuell:**

![](../../../assets/virtual-memory-settings.png)
