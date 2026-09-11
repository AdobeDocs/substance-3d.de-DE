---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-questions/texture-baked-outside-of-substance-software-looks-incorrect.html"
breadcrumb-title: ''
description: Beheben Sie, warum außerhalb der Substance-Software Baking geführt Texturen falsch aussehen und erfahren Sie, wie Sie Farbraumprobleme beheben können.
helpx_creative_field: ""
helpx_description: bakers > Common Questions > Texture baked outside of Substance software looks incorrect
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Textur, die außerhalb der Substance-Software gebacken wurde, sieht falsch aus
user-guide-description: ''
user-guide-title: ''
source-git-commit: 4a060ee1aaa1731c04e70d5512e3271cd63d0381
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 0%

---


# Textur, die außerhalb der Substance-Software gebacken wurde, sieht falsch aus

>[!WARNING]
>
> **Frage**
> 
> Warum sieht die Textur, die ich mit einer externen Anwendung Baking geführt habe, und nicht die Substance Baker im Substance Painter falsch aus?

>[!NOTE]
>
> **Lösung**
> 
> Es gibt keine sofortige Lösung für dieses Problem, da viele Faktoren zu dem Problem beitragen können:
> 
> * Stellen Sie sicher, dass das Standardformat zwischen der Substance-Software und der externen Anwendung identisch ist. OpenGL ist [X+, Y+, Z+] und DirectX ist [X+, Y-, Z+]
>   * Im Substance Painter kann das Normalformat in der [Projektkonfiguration](https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/interface/project-configuration) geändert werden.
>   * Im Substance Designer kann das Normalformat in den [Projektvoreinstellungen](https://experienceleague.adobe.com/en/docs/substance-3d-designer/using/workspace/preferences/project-settings) geändert werden.
> * Überprüfen Sie, ob das Gitter trianguliert wurde, bevor Sie es in der Substance-Software backen und importieren. Weitere Informationen finden Sie unter [dieser Seite](../../guides/triangulating-before-bak/triangulating-before-baking.md).
