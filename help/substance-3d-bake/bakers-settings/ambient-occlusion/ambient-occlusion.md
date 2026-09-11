---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/bakers-settings/ambient-occlusion.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie den Ambient occlusion-Baker verwenden, um mithilfe schneller GPU-beschleunigter Texturen Umgebungsschatten zu erzeugen.
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Ambient Occlusion
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Umgebungsverdeckung
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 4%

---


# Umgebungsverdeckung

Mit dem Ambient occlusion-Baker kann eine Textur für Umgebungsschatten Baking geführt werden. Dieser Baker verwendet einen schnellen Algorithmus, der auf der GPU ausgeführt wird.

**Verfügbar in:**

* Substance Designer
* Substance Automation Toolkit

>[!WARNING]
>
> * Dieser Baker wird möglicherweise auf alten GPUs nicht unterstützt.
> * Der Baking führ mit hoher Auflösung auf Low-End-/mobilen GPUs kann zu einem Absturz führen.

## Parameter

| *Name* | *Beschreibung* |
| --- | --- |
| **Normale Karte** | Normalen-Map-Eingabedatei, die verwendet werden kann, um zusätzliche Geometriedetails auf der Oberfläche des Meshs bereitzustellen, die bei der Berechnung des Bakers berücksichtigt werden sollen. Dieser Parameter ist optional. |
| **Weltraum** | Wenn diese Option aktiviert ist, geben Sie an, dass die Eingabe-Normalen-Map im Welt-Raum (anstelle des Tangentialraums) vorliegt. Wenn keine Eingabe-Normalen-Map angegeben wird, werden diese Parameter ignoriert/deaktiviert. |
| **Normal umkehren** | Berechnen Sie die ambient occlusion-Map mit invertierten Normalen (kann zum Generieren einer Dicken-Map verwendet werden). |
| **Nicht ausgewählte Mesh-Teile verwenden** | Verwenden Sie nicht ausgewählte Mesh-Teile des Meshs, um die ambient occlusion-Map Baking führen. |
| **Qualität** | Wählen Sie die Qualität der Ambient occlusion-Map aus. Eine höhere Qualität ist langsamer zu berechnen.Verfügbare Werte:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Niedrig</strong> (3 Durchgänge)</li><li data-preserve-html="true"><strong>Medium</strong> (Standard, 5 Durchgänge)</li><li data-preserve-html="true"><strong>Hoch</strong> (10 Durchgänge)</li><li data-preserve-html="true"><strong>Sehr hoch</strong> (16 Durchgänge)</li></ul> |
| **Precision-Bias** | Genauigkeit des ambient occlusion. Ein niedrigerer Wert sorgt für eine höhere Präzision, kann jedoch auch größere Artefakte erzeugen. |
| **Abstandsverblassung** | Ausdehnung der Umgebungsverdeckung. |
