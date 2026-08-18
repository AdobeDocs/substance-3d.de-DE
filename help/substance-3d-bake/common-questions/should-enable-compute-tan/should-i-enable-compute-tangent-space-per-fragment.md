---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-questions/should-i-enable-compute-tangent-space-per-fragment.html"
breadcrumb-title: ''
description: Erfahren Sie, wann der Tangentenraum pro Fragment berechnet werden soll und wie sich dies auf die Backergebnisse auswirkt.
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
> Was bedeutet die Einstellung &quot;Tangentenraum pro Fragment berechnen&quot; und wie wird sie verwendet?

>[!NOTE]
>
> **Erklärung**
> 
> Wenn diese Einstellung aktiviert ist, wird der Bäcker angewiesen, die Berechnung des Tangent-Leerzeichens im Fragment-Shader (auch Pixel-Shader genannt) anstelle des Scheitelpunkt-Shaders durchzuführen. Das bedeutet, dass die Berechnung pro Pixel erfolgt, anstatt von Scheitelpunkt zu Scheitelpunkt interpoliert zu werden. Diese Einstellungen werden vom normalen Map-Bäcker verwendet, um zu erfahren, wie die Textur codiert wird. Früher war es auch bekannt, wie man die Textur durch die Shader liest.
> 
> Wenn Sie diesen Parameter aktivieren oder deaktivieren, müssen die Texturen in der Regel neu erstellt werden, um sie mit den 3D-Viewports und Rendering-Engines (z. B. Iran) zu synchronisieren.

>[!NOTE]
>
> **Lösung**
> 
> Je nach Software oder Game-Engine, mit der die Textur gerendert werden soll, kann diese Einstellung deaktiviert oder aktiviert sein:
> 
> | *Software* | *Tangentenraum pro Fragment berechnen* |
> | --- | --- |
> | **Unreale Engine 4** | Aktiviert |
> | **Einheit** | Deaktiviert |
