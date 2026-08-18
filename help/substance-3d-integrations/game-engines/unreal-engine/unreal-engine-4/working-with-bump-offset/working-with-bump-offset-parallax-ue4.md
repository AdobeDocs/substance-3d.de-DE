---
helpx_url: "https://helpx.adobe.com/de/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-4/working-with-bump-offset-parallax-ue4.html"
breadcrumb-title: ''
description: Verwenden Sie die Bump Offset-Zuordnung mit Substance-Materialien in Unreal Engine 4, um Tiefen-Illusionen und Oberflächendetails zu erstellen.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 4 > Working with Bump Offset (Parallax) - UE4
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Arbeiten mit Bump Offset (Parallax) - UE4
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 0%

---


# Arbeiten mit Bump Offset (Parallax) - UE4

**Bump Offset**-Zuordnung verleiht einer Oberfläche die Illusion von Tiefe, indem die UV-Koordinaten auf kreative Weise geändert werden, um die Texel weiter von der Oberfläche des Objekts zu verschieben, sodass die Illusion entsteht, dass die Oberfläche mehr Details aufweist als sie tatsächlich tut. In diesem Beispiel wird beschrieben, wie Sie nicht nur den Ausdruck &quot;Bump-Offset-Material&quot; finden, sondern auch, wie Sie den Knoten &quot;Bump-Offset&quot; in Ihren Materialien verwenden können.

<https://docs.unrealengine.com/latest/INT/Engine/Rendering/Materials/HowTo/BumpOffset/>

Um die Height-Ausgabe zu verwenden, müssen Sie auf die Ausgabe in der Substance Factory Instance doppelklicken, um Height zu erstellen. Height ist standardmäßig nicht aktiviert. Sie können diese Materialausgabe dann in Ihr Height ziehen.

![](../../../../assets/height-1.png){width="600px"}

Erstellen Sie einen Bump-Offset-Knoten und schließen Sie dann den Rot-Kanal des Heights an das Height an. Sie können dann einen TexCoord in den Koordinateneingang des Bumpoffset eingeben. Der Ausgang des Bump-Offsets wird an den UV-Eingang für alle Substance-Texturen angeschlossen.

![](../../../../assets/bump.png){width="800px"}
