---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-issues/baker-output-is-fully-black-or-empty.html"
breadcrumb-title: ''
description: Beheben Sie, warum Bäcker-Ausgaben vollständig schwarz oder leer sind, und erfahren Sie, wie Sie Gitter- und UV-Probleme beheben können.
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Baker output is fully black or empty
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Baker-Ausgabe ist vollständig schwarz oder leer
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 0%

---


# Baker-Ausgabe ist vollständig schwarz oder leer

>[!WARNING]
>
> **Problem**
> 
> Das Ergebnis eines Bäckers ist eine schwarze oder leere Textur:
> 
> ![](../../assets/black.png)

>[!NOTE]
>
> **Erklärung**
> 
> Eine schwarze Textur bedeutet, dass der Bäcker nicht in der Lage war, die Informationen zu finden, die für die Ausgabe eines Ergebnisses erforderlich sind. Zum Beispiel fand der Backprozess nicht das High-Poly-Gitter, das mit dem Low-Poly übereinstimmt, was zu nichts zum Vergleich führte.

>[!NOTE]
>
> **Lösung**
> 
> * Überprüfen Sie, ob das für den Bäcker erforderliche High-Poly-Mesh ordnungsgemäß geladen wurde (Fehler in der Protokolldatei/im Fenster).
> * Stellen Sie sicher, dass die Gitter mit niedrigem oder hohem Poly nicht zu groß (mehr als einen Kilometer) oder zu klein (weniger als einen Zentimeter) sind.
> * Überprüfen Sie, ob der Bäcker das Mesh lesen/verarbeiten konnte (Fehler finden Sie in der Protokolldatei/im Fenster).
> * Überprüfen Sie, ob die Funktion &quot;[ Matching by Name](../../features/matching-by-name/matching-by-name.md)&quot; nicht ordnungsgemäß eingerichtet wurde (einige Objekte schließen sich möglicherweise gegenseitig aus und überlappen sich nie).
> * Stellen Sie sicher, dass die UVs mit niedrigem Poly-Wert im Bereich von 0 bis 1 liegen.
