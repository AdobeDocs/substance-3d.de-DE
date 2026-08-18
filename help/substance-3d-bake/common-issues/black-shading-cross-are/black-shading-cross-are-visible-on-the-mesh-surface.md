---
helpx_url: "https://helpx.adobe.com/de/substance-3d-bake/common-issues/black-shading-cross-are-visible-on-the-mesh-surface.html"
breadcrumb-title: ''
description: Korrigieren Sie Artefakte in der schwarzen Schattierung, die auf Gitteroberflächen sichtbar sind, indem Sie den Tangentenraum und die Normalberechnungen korrigieren.
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Black shading cross are visible on the mesh surface
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Schwarze Schattierungen auf der Gitteroberfläche.
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 0%

---


# Schwarzes Schattierung-Kreuz auf der Gitteroberfläche.

Wenn die Schattierung unterbelichtet ist, werden in mehreren Bereichen des Gitters schwarze Artefakte angezeigt.

![](../../assets/black-shading-cross.jpg)


## Erläuterung

Ein schwarz schattiertes Kreuz bedeutet in der Regel, dass die normale Karte nicht mit dem Gitter übereinstimmt, normalerweise, weil sich die Gittergeometrie geändert hat oder auf eine Weise berechnet wurde, die sich von der vom Bäcker durchgeführten Berechnung unterscheidet. Beispiel: Die Triangulation des Gitters unterscheidet sich zwischen dem Baker und dem Viewport, der das Gitter und seine Normalmap rendert.

## Lösung

Stellen Sie sicher, dass die Anwendung, die das Gitter und seine Normalmap zeigt, mit der Art und Weise synchronisiert ist, wie die Textur gebacken wurde. Dies bedeutet:

* Stellen Sie sicher, dass der Tangentenraum zwischen Betrachter und Bäcker identisch ist.
* Stellen Sie sicher, dass das Format &quot;Normal&quot; zwischen der Ansicht und dem Bäcker identisch ist.
* Stellen Sie sicher, dass die Triangulation zwischen Betrachter und Bäcker identisch ist. Weitere Informationen finden Sie unter [dieser Seite](../../guides/triangulating-before-bak/triangulating-before-baking.md).
