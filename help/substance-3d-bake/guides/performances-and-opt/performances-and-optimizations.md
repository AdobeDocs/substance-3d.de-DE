---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/guides/performances-and-optimizations.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie Ihre Hardwarekonfiguration und die Vorbereitung Ihres Meshs optimieren, um eine schnellere Baking führ-Performance zu erzielen.
helpx_creative_field: ""
helpx_description: bakers > Guides > Performances and optimizations
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Performance und Optimierung
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 0%

---


# Performance und Optimierung

## Mindest-Hardwareanforderungen

Es gibt keine Mindestanforderungen für den Einsatz von Substance Bakers, es ist jedoch wichtig, Folgendes zu beachten:

* Eine gute CPU bietet eine kürzere Berechnung (mehrere Prozessorkerne beschleunigen die Berechnung von **von Mesh**-Bakern, die Raytracing verwenden).
* Ein ordentlicher Arbeitsspeicher (RAM) wird es ermöglichen, Mesh mit vielen Details (Polygonen) zu laden.
* Mit einem guten Grafikprozessor lassen sich Texturen mit hoher Auflösung (z. B. 8K) erzeugen.

## Triangulation

Die Baker arbeiten intern mit triangulierten Meshs. Wenn die 3D-Modelle (niedrige und hohe Poly-Werte) nicht trianguliert werden, triangulieren die Baker die Mesh selbst. Dieser Vorgang kann viel Zeit in Anspruch nehmen und wird linear im Verhältnis zur Menge der im Modell enthaltenen Polygone zunehmen. Es wird im Allgemeinen empfohlen, die Meshs (insbesondere die High-Poly-Mesh) zu triangulieren, um zu vermeiden, dass dieser Vorgang beim Baking auftritt.

Wenn Ihr Workflow auf FBX basiert, können Sie den Mesh zur Exportzeit mithilfe einer Option in der DCC-Anwendung triangulieren.

## Geometrie-Cache

Weitere Informationen finden Sie auf der folgenden Seite : [Geometrie-Cache](../../features/geometry-cache/geometry-cache.md)

## Glätten

Die Baker können das Anti-Aliasing mit Supersampling durchführen. Neuberechnung bedeutet, dass die Baker mehr Strahlen pro Pixel Geworfen haben, um das Ergebnis zu glätten. Die Dauer des Bakings kann durch diese Einstellung erheblich beeinflusst werden. Dies gilt insbesondere für Baker, bei denen viel Strahlen benötigt werden, wie z.B. das ambient occlusion von Mesh Baker.

Beispiel:

* Wenn die AA-Einstellung &quot;2x2&quot; lautet, Wirft der Baker das Vierfache der ursprünglichen Strahlenmenge. Bei einer Textur von 2048\*2048 px entspricht die resultierende Berechnung dem Baking führ einer Textur von 4096\*4096 px und sollte etwa das Vierfache der Berechnungszeit in Anspruch nehmen.
* Wenn die AA-Einstellung &quot;8x8&quot; lautet, Wirft der Baker das 64-fache der ursprünglichen Strahlenmenge. Bei einer Textur von 2048\*2048 px entspricht die resultierende Berechnung dem Baking führ einer 16384\*16384px-Textur und sollte etwa 64-mal mehr Zeit für die Berechnung in Anspruch nehmen.

**Unter Berücksichtigung dieser Zahlen sollte die Einstellung 8x8 mit Vorsicht verwendet werden**.

Um die Rauschen-Präsenz zu reduzieren, wird im Allgemeinen empfohlen, die Anzahl der Sekundärstrahlen (für ambient occlusion-, Thickness- und bent normals-Baker) zu erhöhen und eine 2x2- oder 4x4 AA-Einstellung beizubehalten, anstatt eine geringe Anzahl von Sekundärstrahlen und eine hohe AA-Einstellung zu verwenden.

>[!NOTE]
>
> Eine gute Einstellung für die Leistung/Qualität beim ambient occlusion von Mesh ist die Verwendung von AA 2x2 und mindestens 128 Sekundärstrahlen.

## Dateiformat

Das Exportieren von Dateien auf die Festplatte kann je nach Dateiformat, Auflösung, Bittiefe und Komprimierungseinstellungen eine beträchtliche Zeit in Anspruch nehmen. Komprimierungseinstellungen können in den Optionen Voreinstellungen / Projekte / Allgemein / Dateiformat geändert werden. Wenn Sie die Komprimierung deaktivieren, kann sich die Exportzeit beim Erweitern größerer Dateien verringern.

## Absturz und TDR

Absturz können durch mehrere Faktoren verursacht werden, von denen einer der TDR (Timeout Detection Recovery) ist. Der TDR ist ein Windows-Mechanismus, der darauf ausgelegt ist, Situationen zu erkennen und wiederherzustellen, in denen die GPU nicht zu reagieren scheint. Aufgrund des niedrigen Standardwerts für die TDR-Verzögerungs-Erkennung können in einigen Situationen Absturz auftreten, wenn bestimmte Baker verwendet werden:

* beim Baking führ von dichten Meshs mit dem Ambient occlusion-Baker
* bei Verwendung der DXR beschleunigten Baker mit sehr dichten, hohen Poly-Meshs (mehr als 60 Millionen Dreiecke)

Weitere Informationen zum TDR und eine Anleitung zum Ändern der zugehörigen Einstellungen finden Sie hier: [Absturz mit langen Berechnungen für GPU-Treiber (TDR-Absturz)](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/gpu-drivers-crash-with-long-computations-128745489.html)
