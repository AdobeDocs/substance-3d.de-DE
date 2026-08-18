---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/physical-size-ue5.html"
breadcrumb-title: ''
description: Verwenden Sie die Physische Größe-Einstellungen, um Substance-Materialien basierend auf den realen Abmessungen in der Unreal Engine 5 zu skalieren.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 5 > Physical Size - UE5
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Physische Größe - UE5
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '163'
ht-degree: 0%

---


# Physische Größe - UE5

Physische Größe in Substance-Materialien ermöglicht die Skalierung von Materialien auf Basis ihrer Größe in der Welt. Dieser Wert wird in Substance Designer festgelegt und über das Materialvorlagensystem in Unreal eingelesen.\
Das Material [Substance\_Triplanar\_Template](../../../../game-engines/unreal-engine/unreal-engine-5/material-template-usage/out-the-box-material-tem/out-of-the-box-material-templates.md) im übergeordneten Element enthält ein Beispiel dafür, wie Physische Größe zum Skalieren von unrealen Materialien verwendet werden kann.



Unabhängig von den Upscaling-Werten auf dem Gitter werden die Materialien basierend auf der Größe, die sie in der Welt einnehmen, in Zentimetern kacheln. Bei dem Gesteinsmaterial (Bild 1) beträgt diese 1,8m (180cm) für jede Messung.

![](../../../../assets/rock-material-parameters.png)

Bei Substance-Materialien, die Physische Größen enthalten, werden die Werte in jeden vorhandenen Materialvektorparameterknoten mit dem Namen &quot;physicalsize&quot; kopiert.



Da in UE5 kein Materialwert vorhanden ist, kopiert die Kartenvorlage den Versatz als X, Y, X für die triplanare Physische Größe.
