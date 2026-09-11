---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/renderers/toolbag.html"
breadcrumb-title: ''
description: Verwenden Sie Substance-Rauheit und metallic Ausgaben in Toolbag 2 für Echtzeit-Material-Vorschau und -Rendering.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Toolbag
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Werkzeugtasche
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 5%

---


# Werkzeugtasche

Diese Seite zeigt, wie die Rauheit / metallic Ausgaben für Toolbag 2 zu verwenden.

Toolbag unterstützt sowohl den Specular/Glanz als auch die metallic/Rauheit Workflows.

Substance 3D Painter verwendet den metallic PBR-Shader als Standard, Sie können ihn jedoch auch mit dem Specular/Glanz-Shader verwenden. Dieser Arbeitsablauf zeigt, wie die metallic Ausgaben für Toolbag 2 verwendet werden. Toolbag unterstützt den metallic Arbeitsablauf.

[Download-Beispiel-Szene](https://www.dropbox.com/s/qyed3un2zhtuibj/toolbag.zip?dl=0)

## Aus Painter exportieren

1. Wenn Sie den standardmäßigen metallic PBR-Shader verwenden, können Sie den Export mit den standardmäßigen Dokumentkanälen + Normal + AO-Exportvoreinstellungen durchführen.  ***\*Die Dokumentkanäle exportieren Normalen-Map basierend auf der Projektkonfiguration. Toolbag erfordert OGL-Normalen-Map. Sie können das normale Format in der Projektkonfiguration ändern.***
1. Alternativ können Sie eine benutzerdefinierte Exportkonfiguration erstellen, die Glanz verwendet.

   ![](../../assets/settings-export.png){width="600px"}
1. Sie können das Normalformat vor dem Export in OpenGL ändern.  **Bearbeiten>Projektkonfiguration**

   ![](../../assets/settings-normal-format.png)

## Material einrichten

1. Reflexionsgrad auf &quot;Metallität&quot; setzen
1. Spiegelung auf GGX festlegen
1. Fügen Sie die Texturen den entsprechenden Kanälen hinzu, wie in der folgenden Abbildung dargestellt:

   | Substance 3D Painter Textur | Farbraum | Toolbag-Material |
   | --- | --- | --- |
   | Grundfarbe | sRGB | Albedo |
   | Rauheit | sRGB Aus | Mikrooberfläche - Glanz - Klicken Sie auf Umkehren |
   | Metallisch | sRGB Aus | Reflexionsgrad - Metalitätskarte |
   | Normal | sRGB Aus | Normal |
   | Umgebungsverdeckung | sRGB Aus | Verdeckung |

![](../../assets/settings-toolbag.jpg){width="600px"}
