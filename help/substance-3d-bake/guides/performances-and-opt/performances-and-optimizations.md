---
helpx_url: "https://helpx.adobe.com/de/substance-3d-bake/guides/performances-and-optimizations.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie Ihre Hardware-Einrichtung und die Netzvorbereitung optimieren, um eine schnellere Backleistung zu erzielen.
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

* Eine gute CPU bietet geringere Rechenzeiten (mehrere Kerne beschleunigen die Berechnung von **aus Mesh**-Bäcker, die Raytracing verwenden).
* Eine ordentliche Menge an Arbeitsspeicher (RAM) wird es ermöglichen, Maschen mit vielen Details (Polygonen) zu laden.
* Mit einem guten Grafikprozessor lassen sich Strukturen mit hoher Auflösung (z. B. 8K) erzeugen.

## Triangulation

Die Bäcker arbeiten intern mit dreieckigen Maschen. Wenn die 3D-Modelle (niedrige und hohe Poly-Werte) nicht trianguliert werden, werden die Maschen selbst trianguliert. Dieser Vorgang kann viel Zeit in Anspruch nehmen und wird linear im Verhältnis zur Menge der im Modell enthaltenen Polygone zunehmen. Es wird im Allgemeinen empfohlen, die Maschen (insbesondere das hohe Poly-Mesh) zu triangulieren, um diesen Vorgang beim Backen zu vermeiden.

Wenn Ihr Workflow auf FBX basiert, können Sie das Gitter zur Exportzeit mithilfe einer Option in der DCC-Anwendung triangulieren.

## Geometrie-Cache

Weitere Informationen finden Sie auf der folgenden Seite : [Geometrie-Cache](../../features/geometry-cache/geometry-cache.md)

## Glätten

Die Bäcker können Supersampling verwenden, um Anti-Aliasing durchzuführen. Neuberechnung bedeutet, dass die Bäcker mehr Strahlen pro Pixel werfen, um das Ergebnis zu glätten. Die Backzeit kann durch diese Einstellung erheblich beeinflusst werden. Dies gilt insbesondere für Bäcker, bei denen viel Strahlen benötigt werden, wie z.B. die umgebende Verdeckung vom Mesh-Bäcker.

Beispiel:

* Bei einer AA-Einstellung von 2x2 wird der Bäcker viermal so viel Strahlen gießen wie zuvor. Bei einer Textur mit 2048\*2048 px entspricht die resultierende Berechnung dem Backen einer Textur mit 4096\*4096 px und sollte etwa viermal so viel Zeit in Anspruch nehmen.
* Wenn die AA-Einstellung &quot;8x8&quot; lautet, wird der Bäcker das 64-fache der ursprünglichen Strahlen gießen. Bei einer Textur mit 2048\*2048 px entspricht die resultierende Berechnungszeit dem Backen einer 16384\*16384px-Textur und sollte etwa 64-mal mehr Zeit für die Berechnung in Anspruch nehmen.

**Unter Berücksichtigung dieser Zahlen sollte die Einstellung 8x8 mit Vorsicht verwendet werden**.

Um das Rauschen zu reduzieren, wird im Allgemeinen empfohlen, die Anzahl der Sekundärstrahlen zu erhöhen (für Bäcker mit Umgebungsgeräuschen, Thickness und gebogenen Normalen) und eine 2x2- oder 4x4 AA-Verdeckung einzuhalten, anstatt eine geringe Anzahl von Sekundärstrahlen und eine hohe AA-Einstellung zu verwenden.

>[!NOTE]
>
> Eine gute Leistungs-/Qualitätseinstellung für die Verdeckung aus Mesh bei Umgebungsbedingungen ist die Verwendung von AA 2x2 und mindestens 128 Sekundärstrahlen.

## Dateiformat

Das Exportieren von Dateien auf die Festplatte kann je nach Dateiformat, Auflösung, Bittiefe und Komprimierungseinstellungen eine beträchtliche Zeit in Anspruch nehmen. Komprimierungseinstellungen können in den Optionen Voreinstellungen / Projekte / Allgemein / Dateiformat geändert werden. Wenn Sie die Komprimierung deaktivieren, kann sich die Exportzeit beim Erweitern größerer Dateien verringern.

## Abstürze und TDR

Abstürze können durch mehrere Faktoren verursacht werden, von denen einer der TDR (Timeout Detection Recovery) ist. Der TDR ist ein Windows-Mechanismus, der darauf ausgelegt ist, Situationen zu erkennen und wiederherzustellen, in denen die GPU nicht zu reagieren scheint. Aufgrund eines niedrigen Standardwerts für die TDR-Verzögerungs-Erkennung können in einigen Situationen Abstürze beim Einsatz bestimmter Bäcker auftreten:

* beim Backen dichter Maschen mit dem Bäcker &quot;Ambient Verdeckung&quot;
* bei Verwendung der DXR-beschleunigten Bäcker mit sehr dichten, hohen Poly-Maschen (mehr als 60 Millionen Dreiecke)

Weitere Informationen zum TDR und eine Anleitung zum Ändern der zugehörigen Einstellungen finden Sie hier: [GPU-Treiber stürzen mit langen Berechnungen ab (TDR-Absturz)](https://helpx.adobe.com/de/substance-3d/unlisted/documentation/spdoc/gpu-drivers-crash-with-long-computations-128745489.html)
