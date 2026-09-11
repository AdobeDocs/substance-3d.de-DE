---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/guides/triangulating-before-baking.html"
breadcrumb-title: ''
description: Erfahren Sie, wie sich die Gittertriangulation auf die Backergebnisse auswirkt, und lernen Sie Best Practices für die Vorbereitung Ihrer Geometrie kennen.
helpx_creative_field: ""
helpx_description: bakers > Guides > Triangulating before baking
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Triangulation vor dem Backen
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 0%

---


# Triangulation vor dem Backen

3D-Meshes können mit Polygonen mit mehreren Rahmenkanten pro Fläche definiert werden. Normalerweise über Quads (4 Kanten), manchmal mehr (n-gons).\
Die Software wandelt diese Polygone jedoch später in Dreiecke um, da es einfacher ist, die Berechnung mit (insbesondere auf der GPU) zu verwalten und durchzuführen.

## Wie kann sich die Triangulation auf ein Mesh auswirken?

![](../../assets/triangulation.jpg)

Es gibt **keine Standardlösungen**, um Quad/N-Gons in Dreiecke umzuwandeln. Wie in der Abbildung oben gezeigt, sind mehrere Auswahlmöglichkeiten gültig.\
Es ist unwahrscheinlich, dass die Bäcker Gitter wie eine Game-Engine triangulieren, weil wir einen bestimmten Algorithmus gegenüber einem anderen wählen.

## Warum Triangulation vor dem Backen?

Der Backprozess liest die Geometrie und kodiert die Informationen dann in Texturen.\
Da diese Informationen auf UVs und manchmal auf der Gittertopologie basieren, kann andere Software die Informationen falsch dekodieren, wenn sie die Geometrie nicht auf die gleiche Weise lesen wie beim Anwenden der Textur.

Auf der Abbildung unten sehen Sie das Gitter mit niedriger Poly-Intensität oben links und das Gitter mit hoher Poly-Intensität oben rechts.\
Am unteren Ende befindet sich das Low-Poly mit der normalen Karte, die aus dem High-Poly gebacken wird. Das Gitter auf der linken Seite verwendet eine Triangulation, die mit der Triangulation identisch ist, die Substance Painter beim Backen verwendet. Das Gitter auf der rechten Seite weist keine schwarzen Artefakte auf. Das liegt daran, dass zwischen der Art und Weise, wie die normale Karte gebacken wurde, und der Art und Weise, wie das Gitter derzeit trianguliert wird, ein Missverhältnis besteht. Dieser Fehler kann behoben werden, indem **das Gitter und/oder die Wiederherstellung aktualisiert wird**.

![](../../assets/example-triangulation-artifact.jpg)
