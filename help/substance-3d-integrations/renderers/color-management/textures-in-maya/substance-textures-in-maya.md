---
helpx_url: "https://helpx.adobe.com/de/substance-3d-integrations/renderers/color-management/substance-textures-in-maya.html"
breadcrumb-title: ''
description: Konfigurieren Sie die Farbraumeinstellungen für das Substance von Texturen in Maya, um ein präzises Farbmanagement und Rendering zu gewährleisten.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Color Management > Substance textures in Maya
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Substance von Texturen in Maya
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '134'
ht-degree: 0%

---


# Substance von Texturen in Maya

Der Farbraum, den Sie für Zuordnungen festlegen, hängt von den Einstellungen und Regeln ab, die in den [Maya-Farbmanagement-Einstellungen](https://help.autodesk.com/view/MAYAUL/2020/ENU/?guid=GUID-B260195C-A0FE-4F51-9EA2-099B61B7725A) festgelegt wurden.

Das Substance in Maya-Plugin ist auf &quot;Farbraum-Dateiregeln ignorieren&quot; im Dateiknoten eingestellt. Das Plug-in übernimmt die Farbraumeinstellung unabhängig vom Farbmanagement, indem es die folgenden Funktionen verwendet:

BaseColor, Diffuse, Emissive, Specular = sRGB\
Normal, Height, Versatz, Raueit, metallisch = RAW

In der Regel müssen Sie den Farbraum auf RAW festlegen, wenn es sich um Bilder handelt, die keine Farbdaten darstellen. Diese Einstellung kann jedoch von den Regeln beeinflusst werden, die Sie im Farbmanagement festgelegt haben.

![](../../../assets/raw.png)
