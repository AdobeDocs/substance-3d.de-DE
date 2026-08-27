---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-4/blueprints-ue4/blueprintue4-substance-material-parameters.html"
breadcrumb-title: ''
description: Ändern Sie die Parameter des Substance-Materials zur Laufzeit in Unreal Engine 4 mithilfe von Blueprint-Knoten für die dynamische Steuerung des Materials.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 4 > Blueprints - UE4 > Blueprint(UE4) Substance material parameters
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Blueprint(UE4) Substance Material-Parameter
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 0%

---


# Blueprint(UE4): Substance-Materialparameter

## Parameter &quot;float&quot; ändern:

Sie verwenden den Knoten [Fließende Eingabefunktion festlegen](https://helpx.adobe.com/substance-3d/unlisted/documentation/integrations/blueprint-node-reference-151584784.html), um die Parameter &quot;float&quot;, &quot;color(float4)&quot; und &quot;Boolean&quot; zu ändern.

1. Erstellen Sie eine Variable mit dem Typ &quot;Substance-Grafen Instance&quot; als Referenz.
1. Erstellen Sie einen &quot;Unverankerten Eingabeknoten festlegen&quot; und legen Sie das Ziel als Variable der Substance-Grafen-Instanz fest.
1. Legen Sie im Knoten &quot;Fließkommaeingabe festlegen&quot; die Kennung auf den Namen des zu ändernden Substance-Parameters fest.\
   *\* Sie können den Bezeichnernamen finden, indem Sie die Substance INST öffnen und den Mauszeiger über den Parameternamen bewegen. Der Bezeichnername wird im QuickInfo-Popup angezeigt.*
1. Ziehen Sie am Eingangs-Float-Knoten eine Verbindung heraus, und erstellen Sie einen &quot;Make Array Node&quot; (Array-Knoten erstellen). Der Make Array Node hat einen Index von 0. Der Index 0 entspricht dem float-Wert.
1. Erstellen Sie einen asynchronen oder synchronen Rendering-Knoten und verbinden Sie die Ausführungszeile vom Set Input Float mit dem Rendering-Knoten. Legen Sie die Instanzen auf Rendern fest und setzen Sie sie auf die Variable der Substance-Grafen-Instanz.\
   *\* Async ist nicht blockierend und Sync blockiert.*

![](../../../../../assets/steps.png){width="800px"}

## Boolesche Parameter

Boolesche Parameter werden mithilfe von &quot;Eingabebool festlegen&quot; geändert.

![](../../../../../assets/setbool.png){width="800px"}

## Farbparameter

Die Farbparameter werden mit &quot;Eingabefarbe festlegen&quot; geändert.

![](../../../../../assets/setcolor.png){width="800px"}

## Parameter &quot;Ganzzahl&quot; ändern:

Die Parameter für die Ganzzahl funktionieren genauso wie die Fließkommazahl &quot;Eingabe festlegen&quot;. Sie verwenden den Knoten &quot;Ganzzahl der Eingabe festlegen&quot;.

![](../../../../../assets/int.png)

## Identifizierungen

Sie finden den Bezeichner für einen Parameter in der Substanz INST. Bewegen Sie den Mauszeiger über den Parameter, und die QuickInfo zeigt den Bezeichnernamen an. Dies ist der Name, der im ID-Feld der Ausgabe in Substance Designer festgelegt wird.

![](../../../../../assets/indent-1.png){width="800px"}
