---
helpx_url: "https://helpx.adobe.com/de/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-4/live-link-in-ue4.html"
breadcrumb-title: ''
description: Verwenden Sie Live Link in Unreal Engine 4, um Substance-Materials in Echtzeit zwischen Painter und UE4 zu synchronisieren.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 4 > Live Link in UE4
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Live Link in UE4
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 0%

---


# Live Link in UE4

>[!WARNING]
>
> Live Link in Unreal Engine wird nicht mehr unterstützt. Benutzer mit einer älteren Version des Plug-ins, in der Live Link verwendet wird, können die Funktion weiterhin verwenden.

>[!WARNING]
>
> Live Link funktioniert nicht mit UE4 BSP-Meshs. Bei dem von Ihnen gesendeten Element muss es sich um eine in Ihr UE4-Projekt importierte Modelldatei handeln

## Herstellen einer Verknüpfung zum Substance Painter

1. Substance Painter öffnen
1. Klicken Sie im Inhaltsbrowser mit der rechten Maustaste auf das Element, das Sie an Painter senden möchten, und wählen Sie &quot;An Painter senden&quot;.

   ![](../../../../assets/link1-22.png){width="400px"}
1. Der Mesh erscheint im Substance Painter und du kannst mit der Texturierung beginnen. Während du arbeitest, werden die Texturen an UE4 gesendet und auf die Materialien angewendet. Der grüne Punkt auf dem UE4-Symbol in der Symbolleiste zeigt an, dass der Link live ist und Texturen sendet.

   ![](../../../../assets/icon-12.png)

   1. Sie können das Streamen von Daten in den Optionen zum Konfigurieren des Plug-ins anhalten. Gehen Sie zu Plug-ins > dcc-live-link und wählen Sie Konfigurieren. Deaktivieren Sie Streaming aktivieren, um das Senden von Daten an UE4 anzuhalten.

      ![](https://helpx-prod.scene7.com/is/image/HelpxProd/config-6?$png$&jpegSize=100&wid=393)
1. Texturen aus Painter werden im Inhaltsbrowser angezeigt und auf das Material in UE4 angewendet.

   ![](../../../../assets/link3-11.png){width="500px"}
1. Ein Substance Painter-Projekt (.spp) wird im Projektordner UE4 in einem Ordner mit der Bezeichnung &quot;.sp&quot; erstellt

   ![](../../../../assets/link4-5.png)

## Wiederherstellen einer Verknüpfung zum Substance Painter

Sie können dort weitermachen, wo Sie aufgehört haben, nachdem Sie Painter oder Unity geschlossen haben.

1. Öffnen Sie das Projekt .spp im Substance Painter unter Ihrem Unity-Projekt>assets>.sp-Ordner.
1. Klicken Sie im Inhaltsbrowser mit der rechten Maustaste auf den Mesh und wählen Sie &quot;An Painter senden&quot;, um die Verknüpfung wiederherzustellen.

   ![](../../../../assets/link5-3.png){width="600px"}
