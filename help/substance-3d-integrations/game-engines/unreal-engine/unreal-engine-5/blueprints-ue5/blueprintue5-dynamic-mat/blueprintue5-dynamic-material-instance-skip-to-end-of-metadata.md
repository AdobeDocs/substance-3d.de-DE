---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/blueprints-ue5/blueprintue5-dynamic-material-instance-skip-to-end-of-metadata.html"
breadcrumb-title: ''
description: Erstellen Sie mithilfe von Blueprints dynamische Material-Instanzen aus Substance-Materialien zur Laufzeit in Unreal Engine 5.
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
1. Fügen Sie einen Knoten Grapheninstanz erstellen hinzu und schließen Sie die Substance Instance Factory zusammen mit einem übergeordneten Material an die Factory-Eingabe an, um als Vorlage zu fungieren (dies kann eines der standardmäßigen\_substance-Material sein, die im Plug-in enthalten sind).
1. Erstellen Sie eine weitere Variable, um das im vorherigen Substance-Grafen erstellte Schrittinstanzobjekt zu speichern.
1. Verwenden Sie die Funktion &quot;Dynamische Material-Instanz abrufen&quot; in der Grapheninstanz, um eine vorhandene Material-Instanz zu erstellen oder abzurufen. Wenn Sie &quot;Name&quot; und &quot;Übergeordnetes Material&quot; leer lassen, werden die Parameter verwendet, die beim Generieren der Instanz in Schritt 2 verwendet werden.
1. Erstellen Sie eine Variable des Typs &quot;Material&quot;. Dies ist die Materialinstanz-Dynamik (MID). Legen Sie den Rückgabewert von &quot;Get Dynamic Material Instance&quot; auf die Variable fest.

   ![](../../../../../assets/dynamic-material-annotated-1.png)
1. Fügen Sie einen Materialknoten-Wert hinzu und legen Sie den Wert der Variablen &quot;MID&quot; als Materialeingabe fest. Legen Sie das Ziel auf das Objekt fest, auf das Sie das Material anwenden möchten.
1. Optional: Stellen Sie die gewünschten Substanzparameter ein (in diesem Beispiel wird eine bereits vorhandene Substance-Grapheninstanz verwendet und die Werte in die neue Substance kopiert).
1. Erstellen Sie einen asynchronen oder synchronen Renderingknoten und verbinden Sie die zu rendernden Instanzen mit der Variablen für die Substance-Grafen-Instanz.
