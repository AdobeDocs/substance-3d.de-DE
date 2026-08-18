---
helpx_url: "https://helpx.adobe.com/de/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/tiling-substance-ue5.html"
breadcrumb-title: ''
description: Kacheln Sie Substance-Texturen in Unreal Engine 5, indem Sie Texturkoordinatenknoten und Skalarparameter zu Materialien hinzufügen.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 5 > Tiling Substance - UE5
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Kachel-Substance - UE5
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '78'
ht-degree: 0%

---


# Kachel-Substance - UE5

Um eine Substance-Textur zu kacheln, müssen Sie einen Texturkoordinatenknoten hinzufügen und diesen mit dem Skalarparameter multiplizieren.

<https://docs.unrealengine.com/latest/INT/Engine/Rendering/Materials/ExpressionReference/Coordinates/#texturecoordinate>

Um Parameter für die U- und die V-Kachel zu erstellen, können Sie einen Append Vector verwenden und diesen mit dem TextCode multiplizieren. Auf diese Weise können Sie die U- und V-Kachelbeträge unabhängig einstellen.

![](../../../../assets/tiling-3.png){width="800px"}
