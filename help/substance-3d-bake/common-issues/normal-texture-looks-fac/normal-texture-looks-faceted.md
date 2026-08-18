---
helpx_url: "https://helpx.adobe.com/de/substance-3d-bake/common-issues/normal-texture-looks-faceted.html"
breadcrumb-title: ''
description: Korrigieren Sie das Erscheinungsbild von Facetten in normalen Texturen, indem Sie Gitternormalen glätten und die Einstellungen der Glättungsgruppe anpassen.
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Normal texture looks faceted
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Normale Textur sieht facettenreich aus
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '201'
ht-degree: 0%

---


# Normale Textur sieht facettenreich aus

>[!WARNING]
>
> **Problem**
> 
> Die Struktur &quot;Normal&quot; sieht facettiert aus. Andernfalls ist nach dem Backen jedes Gesicht des Gitters sichtbar.
> 
> ![](../../assets/normal-faceted.jpg)

>[!NOTE]
>
> **Erklärung**
> 
> Der Hauptgrund, warum das Backen eines Normalwertes zu diesem Ergebnis führen würde, ist, dass die niedrigen Polygitter-Normalen nicht richtig eingestellt sind. Jede Kante jeder Seite ist eine harte Kante, sodass die Strahlprojektion während der Anpassung an das High-Poly-Gitter benachbarte Informationen ignoriert und Nähte oder unbewusste Informationen erzeugt. Auch wenn das Ergebnis im Gitter möglicherweise gut aussieht, kann dies zu späteren Problemen mit der Schattierung führen und sollte behoben werden.

>[!NOTE]
>
> **Lösung**
> 
> Die Hauptlösung besteht darin, die Scheitelpunktnormale oder das niedrige Polygitter zu überarbeiten, wobei die genaue Benennung des Prozesses von der 3D-Modellierungssoftware abhängt:
> 
> * Verwenden Sie **durchschnittliche Normale** in Maya, Houdini.
> * Verwenden Sie **eine Glättungsgruppe** im 3DS Max.
> * Verwenden Sie **Smooth Shade** in Blender.
> * Aus zBrush exportierte Gitter werden immer facettiert und sollten in einer anderen Software bereinigt werden.
> 
> Beachten Sie, dass dies möglicherweise nicht ausreicht: Stellen Sie sicher, dass die Einstellungen auch die Informationen zur Scheitelpunktnormale oder -Schattierung speichern/generieren, wenn Sie ein Gitter exportieren.
