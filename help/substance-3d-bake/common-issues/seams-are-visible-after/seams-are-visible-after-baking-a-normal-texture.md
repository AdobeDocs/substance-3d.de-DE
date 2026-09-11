---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-issues/seams-are-visible-after-baking-a-normal-texture.html"
breadcrumb-title: ''
description: Entfernen Sie sichtbare Nähte in Baking geführt normalen Texturen, indem Sie die Auffüllung, das Anti-Aliasing und das UV-Layout anpassen.
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Seams are visible after baking a normal texture
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Nähte sind nach dem Backen einer normalen Textur sichtbar
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---


# Nähte sind nach dem Backen einer normalen Textur sichtbar

>[!WARNING]
>
> **Problem**
> 
> Normalen-Map-Nähte werden an den UV-Rändern des Meshs auch nach einem sauberen Baking führ angezeigt.

>[!NOTE]
>
> **Erklärung**
> 
> Auch nach einem perfekten Baking führ können Nähte noch sichtbar sein. Der Hauptgrund dafür ist, dass eine normale ungefähre Oberflächeninformation in eine Textur übergeht. Manchmal mangelt es der Textur an Präzision oder sie muss zu viel zwischen der niedrigen und der hohen Polygeometrie ausgleichen, um präzise genug zu sein. In einer anderen Situation kann sich die Art und Weise, wie die Geometrie mit dem Normalen-Map ausgeschrieben wird, darauf auswirken, wie gut sie aussieht.

>[!NOTE]
>
> **Lösung**
> 
> Es gibt einige Lösungsmöglichkeiten, um die Intensität der Nähte mit Normalen-Map zu verringern:
> 
> * Oft sind UVs nicht an Pixeln ausgerichtet, was zu Aliasing führt und Nähte erzeugt. Weitere Informationen finden Sie unter [dieser Seite](../../common-issues/aliasing-on-uv-seams/aliasing-on-uv-seams.md).
>   * Eine Erhöhung der Textur-Auflösung kann diesen Effekt reduzieren.
>   * Eine weitere Möglichkeit besteht darin, die UV-Ränder an Pixeln auszurichten.
> * Erhöhen Sie die Einstellung Shader **Qualität**. Die Shader-Qualität kann die Art und Weise beeinflussen, wie Specular-Reflexionen berechnet werden. Wenn einige UV-Inseln gedreht werden und dieser Parameter zu niedrig ist, kann dies zu sichtbaren Nähte führen. Weitere Informationen finden Sie unter [dieser Seite](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/pbr-metal-rough-172818827.html).
