---
helpx_url: "https://helpx.adobe.com/de/substance-3d-bake/guides/error-and-warning-messages.html"
breadcrumb-title: ''
description: Referenzhandbuch für alle Fehler- und Warnmeldungen, die beim Backen mit Substance-Software angezeigt werden können.
helpx_creative_field: ""
helpx_description: bakers > Guides > Error and Warning Messages
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Fehler- und Warnmeldungen
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 0%

---


# Fehler- und Warnmeldungen

Nachfolgend finden Sie eine Liste aller Fehlermeldungen, die beim Backen mit Substance-Software auftreten können.

## Beliebige Bäcker

| *Nachricht* | *Beschreibung* |
| --- | --- |
| Baker nicht verfügbar. | Auf diese Fehlermeldung folgen in der Regel zusätzliche Fehlermeldungen, die häufig auf GPU-Probleme zurückzuführen sind. Dies kann vorkommen, wenn die GPU zu alt ist und die [technischen Anforderungen](https://www.allegorithmic.com/products/tech-specs) der Software nicht erfüllt. |
| Der UV-Satz [X] ist nicht vorhanden. | Der Bäcker versuchte, mit einem gegebenen UV-Satz zu arbeiten, der nicht in dem Nieder-Poly-Gitter vorhanden ist. |
| Die Szene kann nicht von der URL geladen werden. | Diese Meldung bedeutet, dass der Bäcker nicht in der Lage war, die Gitterdatei zu laden, in der Regel das High-Poly-Gitter. Die Ursache für diese Meldung kann eine Reihe von Gründen sein:<ul data-preserve-html="true"><li data-preserve-html="true">Die referenzierte Gitterdatei existiert nicht mehr.</li><li data-preserve-html="true">Die Gitterdatei ist beschädigt oder beschädigt und kann nicht gelesen werden.</li><li data-preserve-html="true">Das Gitter wird derzeit von einer anderen Anwendung bearbeitet und kann nicht gelesen werden.</li></ul> |

## UV zu SVG Baker

| *Nachricht* | *Beschreibung* |
| --- | --- |
| UVs für Gitter [Gittername] konnten nicht gefunden werden. | Es wurden keine UVs für ein bestimmtes Gitter gefunden. Dies kann passieren, wenn mehrere Gitter importiert werden, aber nur einige von ihnen UVs haben. |
| Die Szene verfügt nicht über UVs. Abbrechen des Backens. | Wenn kein Gitter in der Szene UVs enthält, wird der Backvorgang abgebrochen. |

## Lagebacken

| *Nachricht* | *Beschreibung* |
| --- | --- |
| Das Gitter [Gittername] hat keine Positionen. | Bei einem niedrigen Polygitter sind die Scheitelpunkte nicht positioniert. |
| Für das Gitter [Gittername] sind keine UVs für den UV-Satz [X] vorhanden. | Der Bäcker versuchte, mit einem gegebenen UV-Satz zu arbeiten, der nicht in dem Nieder-Poly-Gitter vorhanden ist. |

## Jeder Bäcker &quot;aus Gitter&quot;

| *Nachricht* | *Beschreibung* |
| --- | --- |
| Es wurden keine Scheitelpunktnormalen im Gitter [Gittername] gefunden. | Im angegebenen Gitter wurden keine Scheitelpunktnormalen gefunden. Normalerweise geschieht dies nicht, weil Scheitelpunktnormalen neu berechnet werden, wenn sie im Gitter nicht vorhanden sind. Es könnte passieren, weil ein defektes benutzerdefiniertes Tangentenraum-Plugin. |
| Scheitelpunkttangenten im Gitter [Gittername] wurden nicht gefunden. | Wie oben. |
| Vertex-Binormalitäten im Gitter [Gittername] wurden nicht gefunden. | Wie oben. |
| Scheitelpunktfarben im Gitter [Gittername] wurden nicht gefunden. | Im angegebenen Gitter wurden keine Scheitelpunktfarben gefunden. Dies kann passieren, wenn für mindestens ein Teilgitter im High-Poly-Gitter keine Scheitelpunktfarben definiert sind. |
| Nicht genügend Daten im hohen Poly, um den ausgewählten Bäcker zu verwenden. Baking wird abgebrochen. | Zumindest einer der obigen Meldungen vorangestellt. Normalerweise, wenn nur wenige Daten in der Szene fehlen (Beispiel : nur ein Mesh in hoher Poly-Szene hat keine Scheitelpunkt-Farben), der Baking führ-Prozess füllt die fehlenden Daten mit Nullen und Baking führe weiter. Wenn zu viele Daten fehlen, wird diese Meldung ausgegeben und der Baking führ wird beendet. |

## Transferierte Textur aus Mesh

| *Nachricht* | *Beschreibung* |
| --- | --- |
| Laden der detaillierten Textur fehlgeschlagen. | Die in den Baker-Einstellungen definierte Textur konnte nicht geladen werden. Dies kann daran liegen, dass die Datei tatsächlich auf der Festplatte fehlt oder dass sie beschädigt und nicht lesbar ist. |
