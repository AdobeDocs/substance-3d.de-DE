---
helpx_url: "https://helpx.adobe.com/de/substance-3d-bake/common-issues/normal-texture-looks-faceted.html"
breadcrumb-title: ''
description: Korrigieren Sie das facettierte Erscheinungsbild bei normalen Texturen, indem Sie Mesh-Normalen glätten und die Einstellungen der Glättungsgruppe anpassen.
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
> Die Textur &quot;Normal&quot; sieht facettiert aus oder jede Fläche des Meshs ist nach dem Baking sichtbar.
> 
> ![](../../assets/normal-faceted.jpg)

>[!NOTE]
>
> **Erklärung**
> 
> Der Hauptgrund, warum der Baking führ einer Normalität zu diesem Ergebnis führen würde, ist, dass die Low-Poly-Mesh-Normalwerte nicht richtig festgelegt sind. Jede Kante jeder Fläche ist eine harte Kante, sodass die Strahl-Projektion beim Abgleich mit dem hochgepolten Mesh benachbarte Informationen ignoriert und Nähte oder unbewusste Informationen erzeugt. Auch wenn das Ergebnis auf dem Mesh möglicherweise gut aussieht, kann dies zu späteren Problemen mit der Schattierung führen und sollte behoben werden.

>[!NOTE]
>
> **Lösung**
> 
> Die Hauptlösung besteht darin, den Scheitelpunkt normal oder die Low-Poly-Mesh zu überarbeiten, wobei die genaue Benennung des Prozesses von der 3D-Modellierungssoftware abhängt:
> 
> * Verwenden Sie **durchschnittliche Normale** in Maya, Houdini.
> * Verwenden Sie **eine Glättungsgruppe** im 3DS Max.
> * Verwenden Sie **Smooth Shade** in Blender.
> * Aus zBrush exportierte Meshs werden immer facettiert und sollten in einer anderen Software bereinigt werden.
> 
> Beachten Sie, dass dies möglicherweise nicht ausreicht: Stellen Sie sicher, dass die Einstellungen auch die Informationen zur normalen Schattierung des Scheitelpunkts oder zur Mesh speichern/generieren, wenn Sie einen  exportieren.
