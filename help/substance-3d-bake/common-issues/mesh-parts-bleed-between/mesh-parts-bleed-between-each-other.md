---
helpx_url: "https://helpx.adobe.com/de/substance-3d-bake/common-issues/mesh-parts-bleed-between-each-other.html"
breadcrumb-title: ''
description: Verhindere, dass Mesh-Teile beim Baking ineinander übergehen, indem du die Funktion "Abgleich nach Name" verwendest oder den Abstand anpasst.
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Mesh parts bleed between each other
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Mesh-Teile ineinander verlaufen
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '131'
ht-degree: 0%

---


# Mesh-Teile ineinander verlaufen

>[!WARNING]
>
> **Problem**
> 
> Anschnitt mit Mesh an anderen Teilen, um Artefakte zu erzeugen.
> 
> ![](../../assets/bleed-example.png)

>[!NOTE]
>
> **Erklärung**
> 
> Beim Baking werden Strahlen von der Oberfläche des Meshs mit geringer Poly-Struktur auf den Mesh mit hoher Poly-Struktur gestrahlt, um eine Übereinstimmung zu erzielen. Manchmal gehen die Strahlen zu weit und treffen auf die falsche Geometrie, was zu Blutungen und Artefakten führt.

>[!NOTE]
>
> **Lösung**
> 
> Es gibt einige Lösungen, um dieses Problem zu vermeiden:
> 
> * Verwenden Sie die Funktion [Zuordnung nach Name](../../features/matching-by-name/matching-by-name.md), um die Mesh zu isolieren.
> * Verwenden Sie einen [Käfig](https://helpx.adobe.com/de/substance-3d/unlisted/documentation/bake/cage-projection-172822982.html), um den Strahlenabstand zu begrenzen.
> * Legen Sie in den allgemeinen Baker-Einstellungen einen niedrigeren Standardwert für den Strahlenabstand fest.
