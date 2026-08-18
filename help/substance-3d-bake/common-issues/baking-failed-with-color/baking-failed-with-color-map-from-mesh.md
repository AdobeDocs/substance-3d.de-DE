---
helpx_url: "https://helpx.adobe.com/de/substance-3d-bake/common-issues/baking-failed-with-color-map-from-mesh.html"
breadcrumb-title: ''
description: Beheben Sie Farbzuordnungen aus Gitterbackfehlern, indem Sie die Gitterfarbeneigenschaften und die UV-Zuordnung überprüfen.
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Baking failed with Color Map from Mesh
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Fehler beim Backen mit der Farbzuordnung aus dem Gitter
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '140'
ht-degree: 0%

---


# Fehler beim Backen mit der Farbzuordnung aus dem Gitter

>[!WARNING]
>
> **Problem**
> 
> Mögliche Fehlermeldung:
> 
> &#x200B;> > > 
> 
> [ Backen ] Fehler beim Backen (Farbzuordnung aus Gitter)\
> Scheitelpunktfarben konnten nicht gefunden werden

>[!NOTE]
>
> **Erklärung**
> 
> Die Standardeinstellungen für die [Farbzuordnung aus Gitter](../../bakers-settings/color-map-from-mesh/color-map-from-mesh.md) bestehen darin, die Scheitelpunktfarben mit hohem Poly-Gitter in einer Textur auf der Grundlage der Gitter-UVs zu backen. Es ist jedoch oft der Fall, dass das High-Poly-Gitter keine Informationen zu Scheitelpunktfarben enthält. Deshalb kann der Bäcker keine Informationen schreiben, die nicht existieren.

>[!NOTE]
>
> **Lösung**
> 
> Es sind verschiedene Lösungen verfügbar, um diese Fehlermeldung zu vermeiden:
> 
> * Verwenden eines Gitters mit hoher Poly-Intensität, das Scheitelpunktfarben aufweist
> * Einstellen der Farbzuordnung über den Gitterbaker mit unterschiedlichen Einstellungen
> * Verwenden Sie die Farbzuordnung in Mesh Baker nicht, wenn Sie sie nicht benötigen.
