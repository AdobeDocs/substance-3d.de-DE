---
helpx_url: "https://helpx.adobe.com/de/substance-3d-bake/common-questions/is-dithering-applied-to-baked-textures.html"
breadcrumb-title: ''
description: Erfahre, ob Dithering auf Texturen angewendet wird und wie sich dies auf die Texturqualität auswirkt.
helpx_creative_field: ""
helpx_description: "bakers > Common Questions > Is dithering applied to baked textures "
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 'Wird Dithering auf Texturen angewendet, die bereits bearbeitet wurden '
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '140'
ht-degree: 0%

---


# Wird bei gebackenen Texturen Dithering angewendet?

>[!WARNING]
>
> **Frage**
> 
> Unterstützt der Baker die Textur [Dithering](https://en.wikipedia.org/wiki/Dither) und wenn ja, wann wird sie angewendet?

>[!NOTE]
>
> **Erklärung**
> 
> Dithering wird angewendet, um Streifenbildung in normalen 8-Bit-Maps zu vermeiden, z. B. :
> 
> ![](../../assets/dither.jpg)

>[!NOTE]
>
> **Lösung : Substance Designer**
> 
> In den folgenden Situationen wird das Dithering automatisch angewendet:
> 
> * Wenn eine Baker-Ausgabe in einer 8-Bit-Texturdatei gespeichert wird
> * Wenn eine Baker-Ausgabe in einem Bitmapknoten mit einem auf 8 Bit gesetzten Diagramm verwendet wird.

>[!NOTE]
>
> **Lösung : Substance Painter**
> 
> Dithering ist eine Option, die während des Exportvorgangs aktiviert oder deaktiviert werden kann. Es wird nur beim Export in das 8-Bit-Dateiformat für Normal, Versatz und Height angewendet.

>[!NOTE]
>
> **Lösung : Substance Automation Toolkit**
> 
> Dithering wird derzeit nicht unterstützt.
