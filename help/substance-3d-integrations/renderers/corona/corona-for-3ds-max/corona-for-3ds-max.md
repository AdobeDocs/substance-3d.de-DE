---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/renderers/corona/corona-for-3ds-max.html"
breadcrumb-title: ''
description: Verwenden Sie Substance-Materialien mit dem Corona-Renderer in 3ds Max mithilfe des Specular/Glossiness-Workflows und der erforderlichen Karten.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Corona > Corona for 3ds Max
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Corona für 3ds Max
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 0%

---


# Corona für 3ds Max

## Substance in Maya-Plugin

![](../../../assets/scene-001v03.jpg)

## Corona 1,6-6

Mit dem [3ds Max-Plugin](../../../3d-applications/3ds-max/3ds-max.md) können Sie Corona im Substance-Menü auswählen, um das Corona-Material automatisch mit Substance-Textureingaben einzurichten.

![](../../../assets/corona.png){width="500px"}

## Corona 7-9

Bei Corona-Rendering 7 und höher wird durch Auswahl von &quot;Substance zu Corona&quot; mit dem ausgewählten Substance2-Knoten ein Netzwerk für das Corona-Physikalische Material erstellt.

![](https://helpx-prod.scene7.com/is/image/HelpxProd/corona-physical-material?$png$&jpegSize=200&wid=857)

* **LiftGamaGain** wird zwischen der Grundfarbenausgabe und der Grundfarbeneingabe erstellt. Ein Gamma-Wert von 0,455 wird zur Korrektur der Farbdifferenz verwendet.
* **CoronaNormal** wird zwischen der Standardausgabe und der Base-Bump-Eingabe sowie zwischen der Coat-Normal-Ausgabe und der Clearcoat-Bump-Eingabe erstellt. Es werden keine Einstellungen geändert, aber hier können Änderungen für den Normalzustand vorgenommen werden.
* **CoronaMix** wird zwischen der Glanzfarbe-Ausgabe und der Glanzfarbe-Eingabe erstellt. Ein Mischbetrag von 0 wird festgelegt, und ein Multiplikator von 2 wird für die Basisebene festgelegt. Benutzer können den Wert für die Mischmenge anpassen, um den Glanz zu steuern.
