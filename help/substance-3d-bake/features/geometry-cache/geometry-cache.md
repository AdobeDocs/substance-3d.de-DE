---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/features/geometry-cache.html"
breadcrumb-title: ''
description: Verwenden Sie Geometrie-Caching, um vorverarbeitete Mesh-Daten beizubehalten und nachfolgende Bakings erheblich zu beschleunigen.
helpx_creative_field: ""
helpx_description: bakers > Features > Geometry Cache
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Geometrie-Cache
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '148'
ht-degree: 0%

---


# Geometrie-Cache

Beim Baking werden die Mesh vorverarbeitet, um sie zu bereinigen, und in ein Format konvertiert, das mit dem Baking kompatibel ist. Der Geometriecache ist eine Möglichkeit, diese vorverarbeitete Geometrie so beizubehalten, dass sie schnell neu geladen werden kann, um eine spätere Wiederholung dieses Vorgangs zu vermeiden (es sei denn, der Quell-Mesh ändert sich).

* In **Substance Designer** wird der Geometriecache erstellt, nachdem ein erstes Baking ausgeführt wurde. Der Baker wird dann im Speicher gespeichert, bis das Cachefenster geschlossen wird.
* In **Substance Painter** wird der Geometriecache als Datei mit der Erweiterung **assbin** neben der Quelldatei nach dem ersten Baking gespeichert.

Durch die Wiederverwendung des Geometrie-Caches wird das Baking erheblich beschleunigt, insbesondere wenn Sie die Baker-Einstellungen anpassen, um ein perfektes Ergebnis zu erzielen.
