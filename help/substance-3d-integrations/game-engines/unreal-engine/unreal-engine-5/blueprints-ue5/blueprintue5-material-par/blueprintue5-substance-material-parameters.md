---
helpx_url: "https://helpx.adobe.com/de/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/blueprints-ue5/blueprintue5-substance-material-parameters.html"
breadcrumb-title: ''
description: Ändern Sie die Parameter des Substance-Materials zur Laufzeit in Unreal Engine 5 mithilfe von Blueprint-Knoten für die dynamische Steuerung des Materials.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 5 > Blueprints - UE5 > Blueprint(UE5) Substance material parameters
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Blueprint(UE5) Substance Material-Parameter
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 0%

---


# Blueprint(UE5): Substance Material-Parameter

## Parameter &quot;float&quot; ändern:

Sie verwenden den Knoten [Set Input Fließkommazahl](https://helpx.adobe.com/de/substance-3d/unlisted/documentation/integrations/blueprint-node-reference-151584784.html), um die Parameter &quot;float&quot;, &quot;color(float4)&quot; und &quot;Boolesche Wert&quot; zu ändern.

1. Erstellen Sie eine Variable mit dem Typ &quot;Substance-Grafen Instance&quot; als Referenz.\
   \**Fügen Sie hierzu auf der Registerkarte &quot;Mein Blueprint&quot; eine Variable hinzu und geben Sie ihr einen Namen. Suchen Sie in der Dropdown-Liste nach Substance-Grafen-Instanz > Objektreferenz. Ziehen Sie die Variable in den Graf und wählen Sie Get (Variablenname). Legen Sie die Detailinstanz im Abschnitt &quot;Standardwert&quot; der Registerkarte &quot;Substance-Grafen&quot; fest.*
1. Erstellen Sie einen Knoten &quot;Fließkommazahl für Eingabe festlegen&quot; und legen Sie das Ziel als Variable für die Substance-Grafen-Instanz fest. Das Kontrollkästchen &quot;Kontextsensitiv&quot; im Suchfenster muss möglicherweise deaktiviert werden, um alle Ergebnisse anzuzeigen.
1. Legen Sie im Knoten Fließkommazahl festlegen die Identifizierung auf den Namen des zu ändernden Substance-Parameters fest.\
   *\* Sie können den Namen der Identifizierung finden, indem Sie die Substance INST öffnen und mit der Maus auf den Parameternamen zeigen. Der Name der Identifizierung wird im QuickInfo-Popup angezeigt.*
1. Ziehen Sie im Knoten &quot;Eingangsverbindung&quot; eine Fließkommazahl auf die Zeichenfläche und erstellen Sie einen Knoten &quot;Array erstellen&quot;. Der Make Array Node hat einen Index von 0. Der Index 0 entspricht dem float-Wert.
1. Erstellen Sie einen Renderknoten für Async oder Sync und verbinden Sie die Ausführungszeile von der Fließkommazahl &quot;Eingabe festlegen&quot; mit dem Renderknoten. Legen Sie die Instanzen auf Rendern fest und setzen Sie sie auf die Variable der Substance-Grafen-Instanz.\
   *\* Async ist nicht blockierend und Sync blockiert.*

![](../../../../../assets/steps.png){width="800px"}

## Boolesche Wert-Parameter

Die Boolesche Wert-Parameter werden mit &quot;Eingabewert festlegen&quot; geändert.

![](../../../../../assets/setbool.png){width="800px"}

## Farbparameter

Die Farbparameter werden mit &quot;Eingabefarbe festlegen&quot; geändert.

![](../../../../../assets/setcolor.png){width="800px"}

## Parameter &quot;Ganzzahl&quot; ändern:

Die Parameter für die Ganzzahl funktionieren genauso wie die Fließkommazahl &quot;Eingabe festlegen&quot;. Sie verwenden den Knoten &quot;Ganzzahl der Eingabe festlegen&quot;.

![](../../../../../assets/int.png)

## Identifizierungen

Sie finden die Identifizierung für einen Parameter in der Substanz INST. Bewegen Sie den Mauszeiger über den Parameter, und die QuickInfo zeigt den Namen der Identifizierung an. Dies ist der Name, der im Feld &quot;Identifizierung&quot; der Ausgabe in Substance Designer festgelegt wird.

![](../../../../../assets/screen-shot-2022-04-01-at-4-50-02-pm-copy.png)
