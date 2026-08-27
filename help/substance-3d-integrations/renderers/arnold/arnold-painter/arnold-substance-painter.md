---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/renderers/arnold/arnold-substance-painter.html"
breadcrumb-title: ''
description: Verwenden Sie Substance Painter-Ausgabevorlagen für den Arnold-Renderer mit aiStandard-Material für das physikalisch basierte Rendering.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Arnold > Arnold - Substance Painter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Arnold - Substance Painter
user-guide-description: ''
user-guide-title: ''
source-git-commit: 4a060ee1aaa1731c04e70d5512e3271cd63d0381
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 3%

---


# Arnold - Substance Painter

Substance Painter 2020.1 (6.1.0) wird mit [Ausgabevorlagen](https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/getting-started/export/output-templates/export-presets) für Arnold geliefert, wobei das [aiStandard-Material](https://docs.arnoldrenderer.com/display/A5AFMUG/Standard+Surface) verwendet wird.

![](../../../assets/arnold-export.png){width="800px"}

## Arnold Standard Shader (Arnold 5 und höher)

| Substance Painter Export | Arnold AiStandardSurface |
| --- | --- |
| Grundfarbe | Basis/Farbe |
| Rauheit | Specular/Raueit |
| Metallik | Basis / Metallität |
| Normal | (**Maya**) Geometrie/Bump-Zuordnung/bump2d (als Tangent-Space-Normale verwenden) (**3ds** **Max**) Bitmap → Normal |
| Höhe | (**Maya**) Versatz Shader / Versatz (**3ds** **Max**) Object modifier → Arnold Properties → Versatz → Use Map |
| Ausstrahlend | Emission/Farbe (Emissionsgewicht = 1,0) |
| Anisotropie (nicht in der Standard-Arnold-Ausgabevorlage enthalten) | (**Maya**) Coat/Anisotropie (**3ds** **Max**) Coat/Anisotropie |
| Anisotropie (nicht in der Standard-Arnold-Ausgabevorlage enthalten) | (**Maya**) Coat/Rotation (**3ds** **Max**) Coat/Rotation |

>[!NOTE]
>
> Karten, die Daten darstellen, müssen korrekt interpretiert werden. Weitere Informationen finden Sie auf der Seite [Farbmanagement](../../../renderers/color-management/color-management.md).
