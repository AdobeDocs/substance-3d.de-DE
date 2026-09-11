---
helpx_url: "https://helpx.adobe.com/de/substance-3d-bake/common-questions/should-i-enable-compute-tangent-space-per-fragment.html"
breadcrumb-title: ''
description: Erfahren Sie, wann Sie den Speicherplatz für die Tangente pro Fragment berechnen aktivieren und wie sich dies auf die Ergebnisse des Bakings auswirkt.
helpx_creative_field: ""
helpx_description: bakers > Common Questions > Should I enable
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Sollte ich
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 1%

---


# Soll ich &quot;Tangentenraum pro Fragment berechnen&quot; aktivieren?

>[!WARNING]
>
> **Frage**
> 
> Was bedeutet die Einstellung &quot;Tangente-Speicherplatz pro Fragment berechnen&quot; und wie wird sie verwendet?

>[!NOTE]
>
> **Erklärung**
> 
> Wenn diese Einstellung aktiviert ist, wird der Baker angewiesen, die Tangentialraum-Berechnung im Fragment-Shader (auch Pixel-Shader genannt) anstelle des Scheitelpunkt-Shader durchzuführen. Das bedeutet, dass die Berechnung pro Pixel erfolgt, anstatt von Scheitelpunkt zu Scheitelpunkt interpoliert zu werden. Diese Einstellungen werden vom Normalen-Map-Baker verwendet, um zu erfahren, wie die Textur codiert wird. Früher war es auch bekannt, wie die Textur von den Shadern gelesen wird.
> 
> Wenn Sie diesen Parameter aktivieren oder deaktivieren, müssen Sie in der Regel die Texturen neu erstellen, um sie mit den 3D-Viewporten und -Render-Engine (z. B. Iray) zu synchronisieren.

>[!NOTE]
>
> **Lösung**
> 
> Abhängig von der Software oder dem Game-Engine, die bzw. das zum Rendern der Textur vorgesehen ist, kann diese Einstellung deaktiviert oder aktiviert sein:
> 
> | *Software* | *Tangente-Speicherplatz pro Fragment berechnen* |
> | --- | --- |
> | **Unreales Engine 4** | Aktiviert |
> | **Einheit** | Deaktiviert |
