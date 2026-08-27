---
helpx_url: "https://helpx.adobe.com/de/substance-3d-integrations/renderers/renderman/renderman-substance-painter.html"
breadcrumb-title: ''
description: Exportieren Sie Substance Painter-Texturen für Renderman mit pxrSurface-Material und korrekten Ausgabekonvertierungen.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Renderman > Renderman - Substance Painter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Renderman - Substance Painter
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '116'
ht-degree: 1%

---


# Renderman - Substance Painter

Substance Painter 2020.1 (6.1.0) unterstützt [**pxrSurface**](https://rmanwiki.pixar.com/display/REN/PxrSurface) und pxrDisney [Ausgabevorlagen](https://docs.substance3d.com/display/SPDOC/Export).

![](../../../assets/renderman.png)

Es wird empfohlen, **pxrSurface** für die Ausgabe zu verwenden.

![](../../../assets/pxrsurface.png)

## Renderman Shader (Maya - RM 23.1)

| Substance Painter Export | PxrSurface |
| --- | --- |
| DiffuseColor | Diffus/Farbe |
| SpecularRoughness | Primärer Specular/Raueit |
| SpecularFaceColor | Primärer Specular/Gesichtsfarbe |
| Normal | Globals / Bump / PxrNormalMap → Ausrichtung (Open GL) |
| Verschiebung | (roter Kanal) PxrDispTransform (Ergebnis F) → (disp-Skalar) PxrDisplace (Ausgangsfarbe) → (Versatz Shader) PxrSurfaceSG |
| GlowColor | Leuchten / Farbe (Verstärkung = 1,0) |
| Präsenz | Globals/Präsenz |

>[!NOTE]
>
> Karten, die Daten darstellen, müssen korrekt interpretiert werden. Weitere Informationen finden Sie auf der Seite [Farbmanagement](../../../renderers/color-management/color-management.md).
