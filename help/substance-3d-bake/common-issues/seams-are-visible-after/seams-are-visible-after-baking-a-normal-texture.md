---
helpx_url: "https://helpx.adobe.com/de/substance-3d-bake/common-issues/seams-are-visible-after-baking-a-normal-texture.html"
breadcrumb-title: ''
description: Entfernen Sie sichtbare Nähte in gebackenen normalen Texturen, indem Sie die Auffüllung, das Anti-Aliasing und das UV-Layout anpassen.
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
> Normale Kartennähte sind auch nach einem sauberen Backen an den UV-Rändern des Gitters sichtbar.

>[!NOTE]
>
> **Erklärung**
> 
> Auch nach einem perfekten Backen können Nähte noch sichtbar sein. Der Hauptgrund dafür ist, dass eine normale Näherungsflächeninformation in eine Textur übergeht. Manchmal fehlt es der Textur an Präzision oder sie muss zu viel zwischen der niedrigen und der hohen Poly-Geometrie ausgleichen, um genau genug zu sein. In einer anderen Situation kann die Art und Weise, wie die Geometrie mit ihrer normalen Karte ausgeschrieben wird, beeinflussen, wie gut sie aussieht.

>[!NOTE]
>
> **Lösung**
> 
> Es gibt einige Möglichkeiten, die Intensität der Nähte mit normalen Karten zu reduzieren:
> 
> * Oft sind UVs nicht an Pixeln ausgerichtet, was zu Aliasing führt und Nähte erzeugt. Weitere Informationen finden Sie unter [dieser Seite](../../common-issues/aliasing-on-uv-seams/aliasing-on-uv-seams.md).
>   * Eine Erhöhung der Strukturauflösung kann diesen Effekt reduzieren.
>   * Eine andere Möglichkeit, diesen Effekt zu reduzieren, ist die Ausrichtung der UV-Ränder an Pixeln.
> * Erhöhen Sie die Einstellung für Shader **quality**. Die Shader-Qualität kann die Art und Weise beeinflussen, wie Specular-Reflexionen berechnet werden. Wenn einige UV-Inseln gedreht werden und dieser Parameter zu niedrig ist, kann es zu sichtbaren Nahtstellen kommen. Weitere Informationen finden Sie unter [dieser Seite](https://helpx.adobe.com/de/substance-3d/unlisted/documentation/spdoc/pbr-metal-rough-172818827.html).
