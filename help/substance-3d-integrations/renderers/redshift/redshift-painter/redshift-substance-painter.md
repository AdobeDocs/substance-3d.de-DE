---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/renderers/redshift/redshift-substance-painter.html"
breadcrumb-title: ''
description: Exportieren Sie Substance Painter-Texturen für den Redshift-Renderer mit Ausgabevorlagen und den richtigen Materialeinstellungen.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Redshift > Redshift - Substance Painter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Redshift - Substance Painter
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '142'
ht-degree: 2%

---


# Redshift - Substance Painter

Substance Painter 2020.1 (6.1.0) unterstützt Redshift [Ausgabevorlagen](https://docs.substance3d.com/display/SPDOC/Export) für Metall/Raueit (rsMaterial). Sie können die Redshift-Vorlage einfach exportieren, um Texturen zu erzeugen, die mit den Redshift-Materialien kompatibel sind.

![](../../../assets/rs-export.png)

## Werkstoffeinrichtung für Umschichtung

| Substance Painter Export | Redshift-Material |
| --- | --- |
| Color | Diffus/Farbe |
| Rauheit | Reflexion/Raueit (BRDF = GGX) |
| Metallik | Reflexion/Metallität (Fresnellinie = Metallität) |
| Normal | Allgemein/Bumpmap/rsBumpMap (Eingabemapartyp = Tangent-Leerzeichen Normal - Height-Skalierung = 1,0) |
| DisplaceHeightField | Versatz Shader / rsDisplacement TextMap (Kartencodierung = Height-Feld) |
| EmissionColor | Gesamt / Emission (Emissionsgewicht = 1,0) |

>[!NOTE]
>
> Karten, die Daten darstellen, müssen korrekt interpretiert werden. Weitere Informationen finden Sie auf der Seite [Farbmanagement](../../../renderers/color-management/color-management.md).

## Beispiel für Maya/Redshift

![](https://helpx-prod.scene7.com/is/image/HelpxProd/maya-example?$pjpeg$&jpegSize=300&wid=1583){width="800px"}
