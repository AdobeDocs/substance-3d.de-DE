---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/renderers/vray/vray-next-substance-painter.html"
breadcrumb-title: ''
description: Exportieren Sie Substance Painter-Texturen für den V-Ray Next-Renderer mit Ausgabevorlagen und den richtigen Workflow-Einstellungen.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Vray > Vray Next - Substance Painter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Nächste variieren - Substance Painter
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 3%

---


# Nächste variieren - Substance Painter

Substance Painter 2020.1 (6.1.0) wird mit [VrayMtl](https://docs.chaosgroup.com/display/VRAY4MAYA/VRayMtl) Shadern für Metallic- und Specular-Arbeitsabläufe ausgeliefert. Sie können [Ihr Substance Painter-Projekt ](https://docs.substance3d.com/display/SPDOC/Project+Creation) mithilfe der **VrayMtl-Vorlage** einrichten, die Ihren Viewport-Shader konfiguriert.

![](../../../assets/template-16.jpg)

Unter den Shader-Einstellungen können Sie den Vray Shader für die Arbeit mit VrayMtl konfigurieren.

>[!NOTE]
>
> Wenn Ihr Projekt für die Verwendung von [UV-Kachel UDIM Legacy](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/uv-tile-udim-legacy-144310352.html) eingerichtet wurde. Verwenden Sie die Ausgabevorlage Nächste UDIM variieren.

![](../../../assets/vray-mtl-shader.png){width="800px"}

Um Texturen zum Rendern in Vray Next zu exportieren, wählen Sie die Vray Mtl-Ausgabevorlage aus.

![](../../../assets/template-project.jpg){width="800px"}

## Material variieren (Nächstes variieren - Metallic/Rauheit)

| Substance Painter Export | VRayMtl |
| --- | --- |
| Grundfarbe | (**Maya**) Diffuse Farbe (Stärke = 1,0) (**3ds Max**) Diffuse |
| Rauheit | (**Mai**) Reflexion/Raueit (BRDF = GGX) + (Raueit verwenden aktiviert) (**3ds Max**) Raueit → BRDF/GGX verwenden und Raueit verwenden aktivieren |
| Metallisch | (**Maya**) Reflektion/Metalität (**3ds Max**) Metalität |
| Normal | (**Maya**) Bump- und Normalzuordnung / Karte (Zuordnungstyp = Normal im Tangentenraum)(**3ds** **Max**) Bitmap → Normal |
| Höhe | (**Maya**) Versatz Shader / Versatz (**3ds** **Max**) Object-Modifizierer → VrayDisplacementMod → Textzuordnung |
| Ausstrahlend | Selbstbeleuchtung |
| Übertragbar | (**Maya**) Volumenstreuung/Translucency-Farbe (**3ds Max**) Translucency → Rückseitenfarbe |
| AnisotropyAngle | (**Maya**) Anisotropie/Anisotropie-Drehung (**3ds** **Max**) BRDF/Drehung |
| AnisotropyLevel | (**Maya**) Anisotropie/Anisotropie (**3ds Max**) BRDF/Angle |

## Vray Material (Vray Next - Specular/Glanz)

| Substance Painter Export | VRayMtl |
| --- | --- |
| Diffus | (**Maya**) Diffuse Farbe (Stärke = 1,0) (**3ds Max**) Diffuse |
| Glanz | (**Maya**) Reflexion/Reflexionsfarbe (Stärke = 1,0) (**3ds Max**) Reflexion |
| Glanz | (**Maya**) Reflexion/Raueit (BRDF = GGX) + (Raueit verwenden aktiviert) (**3ds Max**) Glanzgrad → BRDF/GGX verwenden und Glanzgrad verwenden aktivieren |
| Normal | (**Maya**) Bump- und Normalzuordnung / Karte (Zuordnungstyp = Normal im Tangentenraum)(**3ds** **Max**) Bitmap → Normal |
| Höhe | (**Maya**) Versatz Shader / Versatz (**3ds** **Max**) Object-Modifizierer → VrayDisplacementMod → Textzuordnung |
| Ausstrahlend | Selbstbeleuchtung |
| Übertragbar | (**Maya**) Volumenstreuung/Translucency-Farbe (**3ds Max**) Translucency → Rückseitenfarbe |
| AnisotropyAngle | (**Maya**) Anisotropie/Anisotropie-Drehung (**3ds** **Max**) BRDF/Drehung |
| AnisotropyLevel | (**Maya**) Anisotropie/Anisotropie (**3ds Max**) BRDF/Angle |

>[!NOTE]
>
> Karten, die Daten darstellen, müssen korrekt interpretiert werden. Weitere Informationen finden Sie auf der Seite [Farbmanagement](../../../renderers/color-management/color-management.md).

In diesem Beispiel wird der Substance Painter-Viewport mit dem Vray-Shader Metallic/Rauheit und der Vray-Render mit Maya gezeigt.

![](../../../assets/vray-maya.jpg){width="800px"}
