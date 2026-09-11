---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/scripting-in-unity-deprecated/api-overview.html"
breadcrumb-title: ''
description: Referenzübersicht über die veraltete Substance Unity API für ältere Projekte und Skripterstellungsanforderungen.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Scripting in Unity (Deprecated) > API Overview
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: API-Übersicht
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '155'
ht-degree: 0%

---


# API-Übersicht

## Substance.Game

```
Using Substance.Game
```


Substance.Game ist die Assembly, die die für die Skripterstellung verwendeten Klassen enthält. Diese Klassen lauten wie folgt:

**Substance.Game.**&#x200B;**Substance**: Verweist auf den Unterstrich

**Substance.Game.SubstanceGraph**: Einzelner Graf im Unterabschnitt *(war früher ProceduralMaterial in Unity 2017)*

## Skripterstellung

1. Instanz von SubstanceGraph erstellen
1. Stellen Sie die Parameter auf der Grapheninstanz ein.
1. Rendering-Substance in die Warteschlange stellen: QueueForRender() fügt den Substance-Graf einer Warteschlange hinzu. Diese Liste wird beim nächsten Aufruf von RenderAsync oder RenderSync verarbeitet.

### Parameter für die Grapheninstanz

```
// panel color 

mySubstance.SetInputColor("paint_color", color); 

 

// panel size 

mySubstance.SetInputVector2("square_open", panelSize); 

 

// wear level 

mySubstance.SetInputFloat("wear_level", wearLevel);
```


Der Wert in Anführungszeichen ist die in Substance Designer festgelegte Identifizierung des Parameters.

Im Unity Inspector können Sie den Mauszeiger über einen Parameter bewegen, um eine QuickInfo anzuzeigen, die den Namen der in Substance Designer festgelegten Identifizierung anzeigt.

![](../../../../assets/tooltip-6.png)

### Substanz zum Rendern in die Warteschlange stellen

```
// queue the substance to render 

mySubstance.QueueForRender(); 

 

//render all substances async 

Substance.Game.Substance.RenderAsync();
```


![](../../../../assets/unityscript.gif)

>[!NOTE]
>
> Derzeit unterstützen wir nur die x86\_64-Architektur. Sie müssen x86\_64 in den Buildeinstellungen festlegen.

![](../../../../assets/arch.png)
