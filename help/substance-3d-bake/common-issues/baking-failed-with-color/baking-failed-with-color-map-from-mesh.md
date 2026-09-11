---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-issues/baking-failed-with-color-map-from-mesh.html"
breadcrumb-title: ''
description: Beheben Sie Fehler beim Farb-Map aus Mesh-Baking, indem Sie die Farbeigenschaften des Meshs und die UV-Zuordnung überprüfen.
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Baking failed with Color Map from Mesh
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Baking mit Farb-Map aus Mesh fehlgeschlagen
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '140'
ht-degree: 0%

---


# Baking mit Farb-Map aus Mesh fehlgeschlagen

>[!WARNING]
>
> **Problem**
> 
> Mögliche Fehlermeldung:
> 
> > > > 
> 
> [ Baking ] Baking fehlgeschlagen (Farb-Map aus Mesh)\
> Die Farben des Scheitelpunkts wurden nicht gefunden

>[!NOTE]
>
> **Erklärung**
> 
> Die Standardeinstellungen für [Farb-Map aus Mesh](../../bakers-settings/color-map-from-mesh/color-map-from-mesh.md) bestehen darin, die Scheitelpunkt-Farben mit hohem Poly-Mesh in eine Textur Baking führen, die auf den Mesh-UVs basiert. Es ist jedoch oft der Fall, dass der hochpolare Mesh keine Informationen über Scheitelpunkt-Farben hat. Daher kann der Baker keine Informationen schreiben, die nicht existieren.

>[!NOTE]
>
> **Lösung**
> 
> Es sind verschiedene Lösungen verfügbar, um diese Fehlermeldung zu vermeiden:
> 
> * Verwenden eines Meshs mit hohem Poly, der Scheitelpunkt enthält
> * Legen Sie den Farb-Map aus Mesh-Baker mit unterschiedlichen Einstellungen fest.
> * Verwenden Sie den Farb-Map aus Mesh-Baker nicht, wenn Sie ihn nicht benötigen.
