---
helpx_url: "https://helpx.adobe.com/de/substance-3d-bake/common-issues/mesh-parts-bleed-between-each-other.html"
breadcrumb-title: ''
description: Verhindern Sie, dass während des Backens Gitterteile ineinander übergehen, indem Sie "Anpassung durch Name" verwenden oder die Abstände anpassen.
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Mesh parts bleed between each other
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Gitterteile ineinander verlaufen
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '131'
ht-degree: 0%

---


# Gitterteile ineinander verlaufen

>[!WARNING]
>
> **Problem**
> 
> Mit Gittergeometrien lassen sich Anschnitte an anderen Teilen erzeugen und Artefakte erzeugen.
> 
> ![](../../assets/bleed-example.png)

>[!NOTE]
>
> **Erklärung**
> 
> Beim Backen werden Strahlen von der Oberfläche des Gitters mit niedrigem Polyeffekt auf das Gitter mit hohem Polyeffekt übertragen, um eine Übereinstimmung zu erzielen. Manchmal gehen die Strahlen zu weit und treffen auf die falsche Geometrie, was zu Blutungen und Artefakten führt.

>[!NOTE]
>
> **Lösung**
> 
> Es gibt einige Lösungen, um dieses Problem zu vermeiden:
> 
> * Verwenden Sie die Funktion [Zuordnung nach Name](../../features/matching-by-name/matching-by-name.md), um die Gitter zu isolieren.
> * Verwenden Sie einen [Käfig](https://helpx.adobe.com/de/substance-3d/unlisted/documentation/bake/cage-projection-172822982.html), um den Strahlenabstand zu begrenzen.
> * Legen Sie in den allgemeinen Bäcker-Einstellungen einen niedrigeren Standardwert für den Strahlenabstand fest.
