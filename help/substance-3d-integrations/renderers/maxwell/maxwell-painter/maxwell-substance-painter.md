---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/renderers/maxwell/maxwell-substance-painter.html"
breadcrumb-title: ''
description: Exportieren Sie Substance Painter-Texturen für den Maxwell-Renderer mit den richtigen Ausgabevorlagen und Material-Einstellungen.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Maxwell > Maxwell - Substance Painter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Maxwell - Substance Painter
user-guide-description: ''
user-guide-title: ''
source-git-commit: 4a060ee1aaa1731c04e70d5512e3271cd63d0381
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 0%

---


# Maxwell - Substance Painter

Substance Painter 2020.1 (6.1.0) unterstützt Maxwell [Ausgabevorlagen](https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/getting-started/export/export) für metallic/Rauheit und Specular/Glanz. Sie können den Export einfach mit der Maxwell-Ausgabevorlage** durchführen.\
Maxwell 5.1.0** verfügt über eine Integration mit Substance Painter, die es Ihnen ermöglicht, Texturen einfach zu importieren und automatisch ein Maxwell-Material einzurichten.

## Exportieren von Texturen

Sie können die Maxwell-Ausgabevorlage (Metallische Rauheit) oder Maxwell- (Specular-Glanz) auswählen, um Texturen zum Rendern in Maxwell zu exportieren.

![](../../../assets/maxwell-output.png){width="500px"}

## Anwenden von Texturen in Maxwell

Sie können die Substance Painter-Integration in Maxwell verwenden, um automatisch ein Material mit den exportierten Maps aus angewendetem Substance Painter zu erstellen.\
Klicken Sie zunächst mit der rechten Maustaste auf das Material und wählen Sie **Neu>Substance Painter** aus.

![](https://helpx-prod.scene7.com/is/image/HelpxProd/maxwell-painter?$png$&jpegSize=100&wid=413)

Navigieren Sie zu dem Speicherort, in den Sie die Texturen des Substance Painters exportiert haben, und wählen Sie eine der Zuordnungen aus, z. B. Grundfarbe. Wenn Sie auf &quot;Öffnen&quot; klicken, erstellt die Integration ein neues Maxwell-Material mit den zugewiesenen Maps.\
Wenn mehrere Textursatz aus dem Substance Painter exportiert wurden, verwendet die Integration die Namenskonvention für die Textur, um entsprechende Textur-Maps zuzuweisen.

![](https://helpx-prod.scene7.com/is/image/HelpxProd/image-material?$png$&jpegSize=100&wid=620){width="600px"}

Anschließend können Sie das Material dem Element in Ihrer Szene zuweisen.

![](../../../assets/assigned.png){width="500px"}

Alle Material, die mithilfe der Substance Painter-Integration angewendet wurden.

![](https://helpx-prod.scene7.com/is/image/HelpxProd/materials-assigned?$pjpeg$&jpegSize=300&wid=1511){width="800px"}
