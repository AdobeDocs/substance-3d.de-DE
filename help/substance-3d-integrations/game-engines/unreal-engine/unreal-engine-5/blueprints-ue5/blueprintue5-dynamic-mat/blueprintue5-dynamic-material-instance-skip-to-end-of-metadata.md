---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/blueprints-ue5/blueprintue5-dynamic-material-instance-skip-to-end-of-metadata.html"
breadcrumb-title: ''
description: Erstellen Sie mithilfe von Blueprints dynamische Materialinstanzen aus Substance-Materialien zur Laufzeit in der Unreal Engine 5.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 5 > Blueprints - UE5 > Blueprint(UE5) Dynamic Material Instance Skip to end of metadata
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Blueprint(UE5) Dynamic Material Instance Zum Ende der Metadaten springen
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 0%

---


# Blueprint(UE5): Dynamische Materialinstanz Zum Ende der Metadaten springen

1. Erstellen Sie eine Variable vom Typ Substance Instance Factory und setzen Sie den Standardwert auf Imported Substance Factory.
1. Fügen Sie einen Knoten &quot;Graph-Instanz erstellen&quot; hinzu und schließen Sie die Substance Instance Factory zusammen mit einem übergeordneten Material an die Factory-Eingabe an, um als Vorlage zu fungieren (dies kann eines der standardmäßigen\_Substance-Materialien sein, die im Plug-in enthalten sind).
1. Erstellen Sie eine weitere Variable, um das im vorherigen Substance-Grafen erstellte Schrittinstanzobjekt zu speichern.
1. Verwenden Sie die Funktion &quot;Dynamische Materialinstanz abrufen&quot; in der Grafikinstanz, um eine vorhandene Materialinstanz zu erstellen oder abzurufen. Wenn &quot;Name&quot; und &quot;Übergeordnetes Material&quot; leer bleiben, werden die Parameter verwendet, die beim Generieren der Instanz in Schritt 2 verwendet werden.
1. Erstellen Sie eine Variable des Typs &quot;Material&quot;. Dies ist die Materialinstanz-Dynamik (MID). Legen Sie den Rückgabewert von &quot;Dynamische Materialinstanz abrufen&quot; auf die Variable fest.

   ![](../../../../../assets/dynamic-material-annotated-1.png)
1. Fügen Sie einen Materialknoten-Wert hinzu und legen Sie den Wert der Variablen &quot;MID&quot; als Materialeingabe fest. Legen Sie das Ziel auf das Objekt fest, auf das Sie das Material anwenden möchten.
1. Optional: Legen Sie alle gewünschten Substance-Parameter fest (in diesem Beispiel wird eine bereits vorhandene Substance-Graph-Instanz verwendet und die Werte werden in die neue Instanz kopiert).
1. Erstellen Sie einen asynchronen oder synchronen Renderingknoten und verbinden Sie die zu rendernden Instanzen mit der Variablen für die Substance-Grafen-Instanz.
