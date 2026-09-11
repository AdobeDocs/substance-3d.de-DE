---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/renderers.html"
breadcrumb-title: ''
description: Verwende Substance-Materialien mit führenden Renderern wie Arnold, V-Ray, Redshift und anderen in deinem 3D-Workflow.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Renderer
user-guide-description: ''
user-guide-title: ''
source-git-commit: 4a060ee1aaa1731c04e70d5512e3271cd63d0381
workflow-type: tm+mt
source-wordcount: '226'
ht-degree: 1%

---


# Renderer

In [Substance Source](https://source.substance3d.com/) bereitgestellte Substance-Materialien enthalten Ausgaben für physikalisch basierte Shader und unterstützen sowohl die Workflows [Metallisch/Raueit (Standardarbeitsablauf) als auch Specular/Glossiness](https://academy.substance3d.com/courses/pbrguides). Es ist wichtig, den Arbeitsablauf zu verstehen, den Ihr Renderermaterial unterstützt. Je nach Renderer können Sie die Substance-Materialausgaben möglicherweise direkt verwenden oder Sie müssen die Ausgabetexturen möglicherweise konvertieren. Benutzerdefinierte Substance-Materialien oder Materialien, die Sie von Substance share herunterladen, enthalten möglicherweise nicht die entsprechenden Ausgaben, die für einen bestimmten Renderer erforderlich sind.

![](../assets/outputs.png){width="200px"}

Bei &quot;Arnold&quot; oder &quot;Variieren als Nächstes&quot; können Sie direkt Metallic-/Raueit-Ausgaben verwenden. Mit pxrSurface von Renderman müssen jedoch die Ausgangsfarben/Metallic-Ausgaben in diffuse und Specular-Gesichtsfarben konvertiert werden. Ein Substance-Integrations-Plug-in verarbeitet diese Konvertierungen automatisch, wenn der Renderer unterstützt wird.

Mit Substance Painter können Sie eine [Ausgabevorlage](https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/getting-started/export/export-window/export-window) auswählen, die die entsprechenden Zuordnungstypen erstellt, die für einen bestimmten Renderer erforderlich sind. Wenn Ihr Renderer nicht standardmäßig unterstützt wird, können Sie auch benutzerdefinierte Ausgabevorlagen erstellen.

**Substance Painter Ausgabevorlage**

![](../assets/output-template.png){width="500px"}

## Rendererhandbücher

* [Konvertieren von Substance-Ausgaben](../renderers/converting-outputs/converting-substance-outputs.md)
* [Farbmanagement](../renderers/color-management/color-management.md)
* [Arnold](../renderers/arnold/arnold.md)
* [variieren](../renderers/vray/vray.md)
* [Renderman](../renderers/renderman/renderman.md)
* [Redshift](../renderers/redshift/redshift.md)
* [Maxwell](../renderers/maxwell/maxwell.md)
* [Corona](../renderers/corona/corona.md)
* [Oktan](../renderers/octane/octane.md)
* [Keyshot](../renderers/keyshot/keyshot.md)
* [Thea](../renderers/thea/thea.md)
* [eigenwillig](../renderers/maverick/maverick.md)
* [Werkzeugtasche](../renderers/toolbag/toolbag.md)
* [Zyklen und Evee](../renderers/cycles-and-eevee/cycles-and-eevee.md)
