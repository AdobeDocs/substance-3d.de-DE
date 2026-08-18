---
helpx_url: "https://helpx.adobe.com/de/substance-3d-bake/common-questions/why-are-there-strange-stretches-in-my-textures-after-baking-or-exporting.html"
breadcrumb-title: ''
description: Identifizieren und beheben Sie seltsame Dehnungen in Ihren Texturen, die durch UV-Mapping- oder Gitterprobleme verursacht werden.
helpx_creative_field: ""
helpx_description: "bakers > Common Questions > Why are there strange stretches in my textures after baking or exporting "
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 'Warum gibt es seltsame Dehnungen in meinen Texturen nach dem Backen oder Exportieren? '
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '108'
ht-degree: 0%

---


# Warum gibt es seltsame Dehnungen in meinen Texturen nach dem Backen oder Exportieren?

>[!WARNING]
>
> **Frage**
> 
> Warum gibt es außerhalb der UV-Insel nach dem Backen oder Exportieren seltsame gestreckte Linien oder farbenfrohe Farbverläufe?

>[!NOTE]
>
> **Lösung**
> 
> Die Substance Baker verwenden sowohl Diffusion als auch Dilatation außerhalb der UV-Inseln, um die Lücke zu füllen und sicherzustellen, dass die Textur in Game-Engines gut funktioniert, wenn Mipmaps generiert werden. Weitere Informationen hierzu finden Sie unter: [Auffüllen](https://helpx.adobe.com/de/substance-3d/unlisted/documentation/spdoc/padding-134643719.html).
