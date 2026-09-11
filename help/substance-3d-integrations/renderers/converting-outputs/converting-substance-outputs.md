---
helpx_url: "https://helpx.adobe.com/de/substance-3d-integrations/renderers/converting-substance-outputs.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie Substance Material-Ausgaben konvertieren, um verschiedene Rendereranforderungen und Arbeitsabläufe zu erfüllen.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Converting Substance outputs
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Konvertieren von Substance-Ausgaben
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 1%

---


# Konvertieren von Substance-Ausgaben

## Substance Painter

Sie können die konvertierten Karten aus dem Substance Painter exportieren. Eine Vielzahl von Render-Vorgaben wird unterstützt und durch einfaches Auswählen einer Vorgabe werden die Maps-Typen konvertiert. (Die Konvertierung basiert auf dem Metall-Rau-Workflow).

![](../../assets/convertpainter.png){width="800px"}

## Substance-Plug-in

Das Substance-Plug-in generiert Ausgaben und erstellt automatisch Material für bestimmte Workflows. Bei DCC-Anwendungen und Renderern von Drittanbietern müssen Sie die metallic/groben Ausgaben jedoch möglicherweise manuell konvertieren. Die folgenden Integrationen unterstützen automatische Rendering-Workflows und konvertieren bei Bedarf alle Map-Typen entsprechend:

* [Substance in Spanien](../../3d-applications/maya/using-workflows/using-workflows.md)
* [Substance in 3ds Max](../../3d-applications/3ds-max/3ds-max.md)

## Benutzerdefinierte Substance

Wenn Sie eine benutzerdefinierte Substance erstellen, können Sie die spezifischen Ausgaben erstellen, die Sie für Renderer wie Vray und Corona benötigen. Mit dem Konvertierungsknoten &quot;metallic/Rauheit&quot; (Library > PBR Utilities) können Sie die Grundfarbe, die Rauheit und die metallic Maps ganz einfach in den jeweiligen Renderer konvertieren.

![](../../assets/convert-designer.png){width="600px"}
