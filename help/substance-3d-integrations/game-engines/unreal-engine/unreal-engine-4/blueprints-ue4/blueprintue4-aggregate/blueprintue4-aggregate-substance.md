---
helpx_url: "https://helpx.adobe.com/de/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-4/blueprints-ue4/blueprintue4-aggregate-substance.html"
breadcrumb-title: ''
description: Kombinieren Sie mehrere Substance-Material zur Laufzeit in Unreal Engine 4 mithilfe von Blueprint-Aggregatknoten für erweiterte Workflows.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 4 > Blueprints - UE4 > Blueprint(UE4) Aggregate Substance
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Blueprint(UE4) Aggregate-Substance
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---


# Blueprint(UE4): Aggregate-Substance

Mit dem neuen Aggregatsubstanzknoten können Sie zwei Substanzinstanzfactorys verwenden und zur Laufzeit eine neue Instanzfactory erstellen, mit der eine neue Grapheninstanz erstellt werden kann. Das Besondere daran ist, dass Sie Texturen von einer der kombinierten Grapheninstanzen mit Eingabebildern der anderen kombinierten Grapheninstanz verbinden können. Informationen zum Erstellen einer Substance-Grapheninstanz von diesem neuen Werk finden Sie in unserer Dokumentation zu Grapheninstanzen der Laufzeit. [Material-Instanzdefinition - UE4](https://helpx.adobe.com/de/substance-3d/unlisted/documentation/integrations/material-instance-definition-157352129.html)

1. Importiere Substance, die du verwenden möchtest.
1. Erstellen Sie eine &quot;AggregateGraphInstance&quot;-Variable vom Typ &quot;**Substance-Grafen Instance**&quot;.
1. Erstellen einer Variablen vom Typ &quot;**Material**&quot; und &quot;**Material Instance Dynamic**&quot;
1. Erstellen Sie eine **Substance-Verbindung herstellen**, und legen Sie die Identifizierungen für Ausgabe und Eingabe fest.
1. Erstellen Sie **Aggregate Substance Instance Factory**, und legen Sie die Output- und Input Factory fest.
1. Erstellen Sie eine **Grapheninstanz**, und legen Sie einen Instanznamen fest.
1. Legen Sie die Variable **Aggregate Grapheninstanz** fest.
1. Rufen Sie Substance-Texturen aus der Aggregate-Grapheninstanz in Schritt 7 ab, indem Sie **Substance-Texturen abrufen**.
1. Erstellen Sie eine **Instanz des dynamischen Materials**, indem Sie die Material-Variable aus Schritt 3 als übergeordnete Instanz verwenden.
1. Legen Sie die MID-Variable aus Schritt 3 fest.
1. Legen Sie das Material für den Mesh mithilfe von **Set Material** mit der MID-Variablen fest.

   ![](../../../../../assets/a2-3.png){width="800px"}
1. Legen Sie die Kanäle für das Material fest, wie in den Dokumenten zu dynamischen Material-Instanzen gezeigt (Schritte 11-19)\
   [Blueprint(UE4): Instanz des dynamischen Materials &#x200B;](https://helpx.adobe.com/de/substance-3d/unlisted/documentation/integrations/blueprint-dynamic-material-instance-152535142.html)

   ![](../../../../../assets/a4-3.png){width="800px"}
