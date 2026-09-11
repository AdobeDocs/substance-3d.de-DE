---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/maya/substance-output-node.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Substance-Ausgabeknoten in Maya funktionieren, um berechnete Texturen mit Shader-Netzwerken zu verbinden.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Maya > Substance Output Node
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Substance-Ausgabeknoten
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 0%

---


# Substance-Ausgabeknoten

Der Substance-Ausgabeknoten ist ein Verweis auf die berechnete Textur aus dem Substance Engine. Es ist mit dem Substance-Node verbunden. Wenn eine Ausgabe auf dem Substance-Node erstellt wird, berechnet das Substance-Engine die Textur und diese Daten werden im RAM gespeichert. Wenn Sie das GPU-Engine verwenden, werden die Daten auf der GPU berechnet und mithilfe des Engine &quot;Substance-GPU-Überblendung&quot; zurück an den Speicher gesendet. Ausgaben auf dem Substance-Node, die nicht aktiviert sind, werden nicht berechnet.

![](../../../assets/outputnode.png)

Auf diesem Knoten können Sie Ausgabeinformationen wie Identifizierung, Bezeichnung und Verwendung sehen, die für die Ausgabe in Substance Designer festgelegt sind. Dieser Knoten ermöglicht es Ihnen auch, die Textur im Abschnitt Ausgabecache auf die Festplatte Baking führen.
