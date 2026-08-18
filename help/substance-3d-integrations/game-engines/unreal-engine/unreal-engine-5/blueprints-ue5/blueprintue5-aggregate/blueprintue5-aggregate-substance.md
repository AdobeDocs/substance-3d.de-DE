---
helpx_url: "https://helpx.adobe.com/de/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/blueprints-ue5/blueprintue5-aggregate-substance.html"
breadcrumb-title: ''
description: Kombinieren Sie mehrere Substance-Materialien zur Laufzeit in Unreal Engine 5 mithilfe von Blueprint-Aggregatknoten für erweiterte Workflows.
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

1. Verwenden Sie den Knoten &quot;Aggregate Substance Factory erstellen&quot;, und legen Sie die Output- und die Input-Factory fest. Die Output-Factory sollte über eine Texturmap verfügen, die als Eingabebild in den Input-Factory-Parametern verwendet wird.
1. Erstellen Sie SubstanceConnection-Objekte für jede Ausgabetextur, die als Eingabe verwendet wird, mit den Namen der entsprechenden Werte (dem Ausgabenamen aus dem Ausgabediagramm und dem Namen des Eingabeparameters aus dem Eingabediagramm).
1. Fügen Sie einen Knoten &quot;Graph-Instanz erstellen&quot; hinzu und fügen Sie das Ergebnis des Knotens &quot;Aggregate Substance Factory erstellen&quot; zusammen mit einem übergeordneten Material in die Factory-Eingabe ein, um als Vorlage zu fungieren (dies kann eines der standardmäßigen\_Substance-Materialien sein, die im Plug-in enthalten sind).
1. Erstellen Sie eine Knoteninstanzvariable und speichern Sie das Ergebnis des vorherigen Substance-Grafen.
1. Optional: Legen Sie die gewünschten Substance-Parameter fest (in diesem Beispiel wird eine neue Auflösung für die Graphausgaben festgelegt).
1. Erstellen Sie einen asynchronen oder synchronen Renderingknoten und verbinden Sie die zu rendernden Instanzen mit der Variablen für die Substance-Grafen-Instanz.
1. Verwenden Sie die Funktion &quot;Dynamische Materialinstanz abrufen&quot; in der Grafikinstanz, um eine vorhandene Materialinstanz zu erstellen oder abzurufen. Wenn &quot;Name&quot; und &quot;Übergeordnetes Material&quot; leer bleiben, werden die Parameter verwendet, die beim Generieren der Instanz in Schritt 3 verwendet werden.
1. Fügen Sie einen Materialknoten-Wert hinzu und legen Sie den Wert der Variablen &quot;MID&quot; als Materialeingabe fest. Legen Sie das Ziel auf das Objekt fest, auf das Sie das Material anwenden möchten.
