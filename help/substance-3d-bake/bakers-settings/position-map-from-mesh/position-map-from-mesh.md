---
helpx_url: "https://helpx.adobe.com/de/substance-3d-bake/bakers-settings/position-map-from-mesh.html"
breadcrumb-title: ''
description: Berechnen Sie genaue Positionsabbildungen aus hochpolaren Netzen, um präzise Geometriedaten zur Positionsbestimmung zu erfassen.
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Position map from Mesh
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Positionsmap aus Mesh
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 0%

---


# Positionsmap aus Mesh

Die Positionsmap des Gitterbäckers berechnet die Position der Gittergeometrie mit hoher Poly-Struktur und speichert sie in einer Textur. Es ähnelt dem Basispositionsbacker, kann aber genauere Ergebnisse erzielen.

**Verfügbar in:**

* Substance Designer
* Substance Automation Toolkit

## Parameter

| *Parameter* | *Beschreibung* |
| --- | --- |
| **Modus** | Steuert, welche Informationen in der Positionstextur berechnet werden.Mögliche Werte:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Alle Achsen:</strong> Die Position der X-, Y- und Z-Achsen wird in den RGB-Kanälen der Ausgabetextur gebacken.</li><li data-preserve-html="true"><strong>Eine Achse:</strong> Die Ausgabetextur wird als Graustufenbild mit einer einzelnen Achse gebacken.</li></ul> |
| **Achse** | Definiert, welche Achse berechnet werden soll, wenn der Parameter **Modus** auf **Eine Achse** festgelegt ist. |
| **Normalisierungstyp** | Legt fest, wie die Positionswerte pro Achse skaliert werden.Mögliche Werte:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Box:</strong> normalisiert jede Achse entsprechend dem Netzvolumen (Länge des Begrenzungsrahmens).</li><li data-preserve-html="true"><strong>BSphere:</strong> normalisiert alle Achsen entsprechend dem Gittervolumenradius (Begrenzungskugel).</li></ul> |
| **Normalisierungsskala** | Legt fest, wie die Positionswerte auf der Grundlage des Gitters skaliert werden.Mögliche Werte:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Pro Material</strong>: Werte werden so skaliert, dass sie für jedes Material (Texture Set) zwischen 0 und 1 liegen.</li><li data-preserve-html="true"><strong>Vollständige Szene</strong> (Standard): werden skaliert, um das gesamte Gitter zu berücksichtigen. Dies ermöglicht fortlaufende Positionswerte über Objekte und Materialien hinweg (Textursätze).</li></ul> |
