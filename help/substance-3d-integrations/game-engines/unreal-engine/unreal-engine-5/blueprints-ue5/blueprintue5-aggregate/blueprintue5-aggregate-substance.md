---
helpx_url: "https://helpx.adobe.com/de/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/blueprints-ue5/blueprintue5-aggregate-substance.html"
breadcrumb-title: ''
description: Kombinieren Sie mehrere Substance-Material zur Laufzeit in Unreal Engine 5 mithilfe von Blueprint-Aggregatknoten für erweiterte Workflows.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 5 > Blueprints - UE5 > Blueprint(UE5) Aggregate Substance
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Blueprint(UE5) Aggregate-Substance
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 0%

---


# Blueprint(UE5): Aggregate-Substance

1. Verwenden Sie den Knoten &quot;Aggregate Substance Factory erstellen&quot;, und legen Sie die Output- und die Input-Factory fest. Die Output-Factory sollte über eine Textur-Map verfügen, die als Eingabebild in den Input-Factory-Parametern verwendet wird.
1. Erstellen Sie SubstanceConnection-Objekte für jede als Eingabe verwendete Ausgabe-Textur mit den Namen der entsprechenden Werte (dem Ausgabenamen des Ausgabe-Grafen und dem Namen des Eingabeparameters des Eingabe-Grafen).
1. Fügen Sie einen Knoten Grapheninstanz erstellen hinzu, und schließen Sie das Ergebnis des Knotens &quot;Aggregate Substance Factory erstellen&quot; zusammen mit einem übergeordneten Material an die Factory-Eingabe an, um als Vorlage zu fungieren (dies kann eines der standardmäßigen\_substance-Material sein, die im Plug-in enthalten sind).
1. Erstellen Sie eine Knoteninstanzvariable und speichern Sie das Ergebnis des vorherigen Substance-Grafen.
1. Optional: Stellen Sie die gewünschten Substanzparameter ein (in diesem Beispiel wird eine neue Auflösung für die Graphausgaben festgelegt).
1. Erstellen Sie einen asynchronen oder synchronen Renderingknoten und verbinden Sie die zu rendernden Instanzen mit der Variablen für die Substance-Grafen-Instanz.
1. Verwenden Sie die Funktion &quot;Dynamische Material-Instanz abrufen&quot; in der Grapheninstanz, um eine vorhandene Material-Instanz zu erstellen oder abzurufen. Wenn Sie &quot;Name&quot; und &quot;Übergeordnetes Material&quot; leer lassen, werden die Parameter verwendet, die beim Generieren der Instanz in Schritt 3 verwendet werden.
1. Fügen Sie einen Materialknoten-Wert hinzu und legen Sie den Wert der Variablen &quot;MID&quot; als Materialeingabe fest. Legen Sie das Ziel auf das Objekt fest, auf das Sie das Material anwenden möchten.
