---
helpx_url: "https://helpx.adobe.com/de/substance-3d-bake/common-issues/seam-visible-on-every-face.html"
breadcrumb-title: ''
description: Korrigieren Sie die auf allen Gesichtern sichtbaren Nähte, indem Sie das UV-Auspacken, die Glättungsgruppen und die Gittertopologie überprüfen.
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Seam visible on every face
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Naht auf jedem Gesicht sichtbar
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '195'
ht-degree: 0%

---


# Naht auf jedem Gesicht sichtbar

>[!WARNING]
>
> **Problem**
> 
> An einigen Kanten der Geometrie ist eine Naht sichtbar, auch wenn keine UV-Naht vorhanden ist:
> 
> ![](../../assets/seam-every-face.jpg)

>[!NOTE]
>
> **Erklärung**
> 
> Wenn kein [Käfig](https://helpx.adobe.com/de/substance-3d/unlisted/documentation/bake/cage-projection-172822982.html) verwendet wird, startet der Backvorgang Strahlen in Richtung der Scheitelpunktnormalen des Gitters mit geringer Poly-Polung. Wenn jede Scheitelpunktnormale geteilt ist (d. h., dass jede Fläche nicht dieselbe Scheitelpunktnormale wie die benachbarte Fläche hat), werden die Strahlen an den Kanten nicht in dieselbe Richtung gesendet. Dies führt zu einer Teilung, da die Informationen auf jeder Seite der Kanten unterschiedlich sind.
> 
> Dieses Problem wird auch durch Aliasing verstärkt, wie in [dieser Seite](../../common-issues/aliasing-on-uv-seams/aliasing-on-uv-seams.md) erläutert.

>[!NOTE]
>
> **Lösung**
> 
> Hier sind nur zwei Lösungen möglich:
> 
> * Verwenden Sie einen [Käfig](https://helpx.adobe.com/de/substance-3d/unlisted/documentation/bake/cage-projection-172822982.html), um die Strahlrichtung zu steuern, anstatt den Bäcker sie aus der Geometrie mit niedriger Poly berechnen zu lassen.
> * Fügen Sie die Scheitelpunktnormalen des Polygonnetzes zusammen (erweichen Sie sie/wenden Sie eine gemeinsame Glättungsgruppe an).
