---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/bakers-settings/ambient-occlusion.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie den Bäcker "Umgebungsschatten" verwenden, um mithilfe schneller GPU-beschleunigter Verdeckungen Umgebungs-Schattenstrukturen zu erzeugen.
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

Mit dem Bäcker &quot;Umgebung - Verdeckung&quot; kannst du eine Umgebungs-Schattenstruktur backen. Dieser Bäcker verwendet einen schnellen Algorithmus, der auf der GPU ausgeführt wird.

**Verfügbar in:**

* Substance Designer
* Substance Automation Toolkit

>[!WARNING]
>
> * Dieser Bäcker wird möglicherweise auf alten GPUs nicht unterstützt.
> * Backen mit hoher Auflösung auf Low-End-/mobilen GPUs kann zu einem Absturz führen.

## Parameter

| *Name* | *Beschreibung* |
| --- | --- |
| **Normale Karte** | Geben Sie eine normale Map-Datei ein, die verwendet werden kann, um zusätzliche Geometriedetails auf der Oberfläche des Gitters bereitzustellen, die bei der Bäckerberechnung berücksichtigt werden sollen. Dieser Parameter ist optional. |
| **Weltraum** | Wenn diese Option aktiviert ist, geben Sie an, dass sich die Eingabe-Normalmap im Weltraum (anstelle des Tangent-Raums) befindet. Wenn keine Eingabe-Normalmap angegeben wird, werden diese Parameter ignoriert/deaktiviert. |
| **Normal umkehren** | Berechnen Sie die Umgebungskarte mit invertierten Verdeckungen (kann zum Generieren einer Thicknessen-Map verwendet werden). |
| **Nicht ausgewählte Gitterteile verwenden** | Verwenden Sie nicht ausgewählte Gitterteile des Gitters, um die Umgebungskarte für die Verdeckung zu backen. |
| **Qualität** | Wählen Sie die Qualität der Umgebungskarte aus. Verdeckung Eine höhere Qualität ist langsamer zu berechnen.Verfügbare Werte:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Niedrig</strong> (3 Durchgänge)</li><li data-preserve-html="true"><strong>Medium</strong> (Standard, 5 Durchgänge)</li><li data-preserve-html="true"><strong>Hoch</strong> (10 Durchgänge)</li><li data-preserve-html="true"><strong>Sehr hoch</strong> (16 Durchgänge)</li></ul> |
| **Präzisionsvorspannung** | Präzision der Verdeckung. Ein niedrigerer Wert sorgt für eine höhere Präzision, kann jedoch auch größere Artefakte erzeugen. |
| **Abstandsübergang** | Ausdehnung der Umgebungsverdeckung. |
