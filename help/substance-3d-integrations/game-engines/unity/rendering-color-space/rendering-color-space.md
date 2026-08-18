---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/rendering-color-space.html"
breadcrumb-title: ''
description: Konfigurieren Sie die Farbraumeinstellungen von Unity, um ein ordnungsgemäßes Rendering von Substance-Materialien mit physikalisch basierten Shadern sicherzustellen.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Rendering Color Space
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Rendering-Farbraum
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '102'
ht-degree: 0%

---


# Rendering-Farbraum

Substance-Texturen wurden für die Verwendung mit einem physikalisch basierten Shader entwickelt. Um optimale Ergebnisse zu erzielen, sollten Sie den Farbraum in den Unity Player-Einstellungen auf linear einstellen.

1. Gehen Sie zu Bearbeiten > Projekteinstellungen > Player.
1. Ändern Sie im Abschnitt Rendering den Farbraum in Linear. (Unity verwendet standardmäßig den Gammaraum, der falsch ist und dazu führt, dass die Texturfarbe falsch aussieht.)

   >[!NOTE]
   >
   > **Info**
   > 
   > sRGB-Optionen für Texturen sind deaktiviert, wenn die Farbraumeinstellung in Unity auf Gamma festgelegt ist

   ![](../../../assets/rendering-4.png){width="600px"}
