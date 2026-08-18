---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-4/working-with-displacement-ue4.html"
breadcrumb-title: ''
description: Aktivieren Sie die Tesselierung und verwenden Sie Versatz-Maps von Substance-Materialien in Unreal Engine 4, um Oberflächendetails anzuzeigen.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 4 > Working with Displacement - UE4
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Arbeiten mit Versatz - UE4
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 0%

---


# Arbeiten mit Versatz - UE4

Um mit Versatz arbeiten zu können, müssen Sie die Tesselierung für Ihr Material aktivieren.

![](../../../../assets/tess.png){width="600px"}

Um die Height-Ausgabe zu verwenden, müssen Sie auf die Ausgabe in der Substance Factory Instance doppelklicken, um Height zu erstellen. Height ist standardmäßig nicht aktiviert. Sie können diese Materialausgabe dann in Ihr Height ziehen.

![](../../../../assets/height-1.png){width="800px"}

Nachdem du die Height-Ausgabe zu deinem Material hinzugefügt hast, musst du einige Knoten erstellen, um den World Versatz und den Tesselierungsmodifizierer zu steuern.

1. Erstellen Sie zwei skalare Parameter. Das eine ist die Distanz und das andere der Multiplikator für die Tesselierung.
1. Multiplizieren des Rotkanals vom Height mit dem Parameter &quot;Abstand&quot;
1. Fügen Sie einen VertexNormalWS -Knoten hinzu und multiplizieren Sie diesen mit der Ausgabe der Multiplikation in Schritt 2.
1. Geben Sie die Multiplikation von &quot;VertexNormal&quot; in den Versatz &quot;Welt&quot; auf dem Material ein.
1. Nehmen Sie den Parameter des Tesselierungsmultiplikators und geben Sie ihn an den Tesselierungsmultiplikator für das Material ein.

![](../../../../assets/setup-3.png){width="800px"}

>[!NOTE]
>
> Die anderen Texturausgaben wurden in diesem Bild weggelassen, um das Diagramm zu vereinfachen. Hier sind nur die Versatz- und Multiplikatorknoten zur Verdeutlichung dargestellt.
