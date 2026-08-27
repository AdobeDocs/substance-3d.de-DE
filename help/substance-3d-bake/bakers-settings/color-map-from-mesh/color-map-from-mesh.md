---
helpx_url: "https://helpx.adobe.com/de/substance-3d-bake/bakers-settings/color-map-from-mesh.html"
breadcrumb-title: ''
description: Projizieren Sie Farbeigenschaften aus Gittern mit hohem Poly-Anteil in Texturen, um Polypaint- oder Material-IDs für Auswahlmasken zu backen.
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Color Map from Mesh
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Farbmatrix aus Mesh
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 5%

---


# Farbmatrix aus Mesh

Diese Farbzuordnung aus dem Gitterbaker projiziert Farbeigenschaften aus einem HD-Gitter in eine Textur. Sie kann verwendet werden, um Polypaint- oder Material-IDs zu backen, um Auswahlmasken zu erstellen.

**Verfügbar in:**

* Substance Designer
* Substance Automation Toolkit
* Substance Painter

## Parameter

| *Parameter* | *Beschreibung* |
| --- | --- |
| **Farbquelle** | Steuert, auf welcher Eigenschaft des Gitters mit hoher Poly-Intensität die Farbgenerierung basieren soll.Mögliche Werte:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Eckpunktfarbe</strong>: liest die Scheitelpunktfarbe und speichert sie in der Textur. Die Farbe wird von Scheitelpunkt zu Scheitelpunkt interpoliert.</li><li data-preserve-html="true"><strong>Materialfarbe</strong>: liest die Materialfarbe, die einer Polygonfläche zugewiesen ist.</li><li data-preserve-html="true"><strong>Mesh-ID</strong>: weist eine Farbe pro gefundenem Objekt zu.</li><li data-preserve-html="true"><strong>Polygroup/Submesh ID</strong>: weisen Sie jedem Unterobjekt (auch als Element bezeichnet) eine Farbe zu.</li></ul> |
| **Farbgenerator** | Definiert, wie die Farbe generiert wird, wenn die **Farbquelle** auf **Mesh-ID** oder **Polygroup/Submesh-ID** festgelegt ist.Mögliche Werte:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Zufällig</strong>: Jedes Objekt oder Unterobjekt wird durch eine zufällig erzeugte Farbe eingefärbt.</li><li data-preserve-html="true"><strong>Farbtonverschiebung</strong>: Jedes Objekt oder Unterobjekt wird durch eine eindeutige Farbe basierend auf einem Farbton eingefärbt.</li><li data-preserve-html="true"><strong>Graustufen</strong>: Jedes Objekt oder Unterobjekt wird durch einen eindeutigen Graustufenwert eingefärbt.</li></ul> |
