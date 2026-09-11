---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/blueprints-ue5/blueprintue5-node-reference.html"
breadcrumb-title: ''
description: Referenzhandbuch für alle in Unreal Engine 5 verfügbaren Substance Blueprint-Knoten für Material-Vorgänge.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 5 > Blueprints - UE5 > Blueprint(UE5) Node Reference
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Blueprint(UE5)-Knotenreferenz
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '947'
ht-degree: 0%

---


# Blueprint(UE5): Knotenreferenz

## Allgemeine Substance-Nodes:

| Name | Eingaben | Beschreibung |
| --- | --- | --- |
| **GetSubstances** | Eingabe: **Material** | Gibt ein Array von Materialinstanzen zurück, die von einem Substance-Grafen verwendet werden. Wenn Sie ein Material erstellen, das Texturausgaben von zwei verschiedenen Grafikinstanzen verwendet, gibt diese Funktion diese beiden Grafikinstanzen zurück. |
| **GetSubstanceTextures** | Eingabe: **SubstanceGraphInstance** | Gibt ein Array aller aktivierten und aktuell berechneten Texturen aus dem Eingabeparameter für die Substance-Grafen-Instanz zurück. |
| **GetGraphName** | Eingabe: **SubstanceGraphInstance** | Gibt den in Designer festgelegten Diagrammnamen zurück. |
| **GetFactoryName** | Eingabe: **SubstanceGraphInstance** | Gibt den Namen der **GraphInstanceFactory** zurück, die zum Erstellen der **SubstanceGraphInstance** verwendet wurde, die an diesen Knoten übergeben wird. |
| **GetSubstanceLoadingProgress** | KEINE | Gibt einen Gleitkommawert zwischen 0 und 1 zurück, der angibt, wie viele Substanzen vollständig geladen wurden. |
| **CreateGraphInstance** | Eingabe: **SubstanceInstanceFactory** - Die Factory, aus der Sie eine Diagramminstanz erstellen möchten.Input: **GraphIndex** (int) - Der Index des Diagramms, den Sie erstellen möchten. Eingabe: **InstanceName** (FString): Der Name, den Sie für Ihre neue Instanz verwenden möchten. | Gibt eine neue eigenständige Grafikinstanz zurück, die beibehalten wird, bis die Anwendung geschlossen wird. |
| **DuplicateGraphInstance** | **SubstanceGraphInstance** - Die Grapheninstanz, von der Sie eine Kopie erstellen möchten. | Gibt eine neue eigenständige Grapheninstanz zurück, die beibehalten wird, bis die Anwendung geschlossen wird. |
| **EnableInstanceOutputs** | Eingabe: **SubstanceGraphInstance** - Die Grapheninstanz, die die Ausgabe enthält, um die Eingabe zu aktivieren: **OutputIndices** (int32 Array): Die Indizes der Ausgaben, die Sie aktivieren möchten. | Wenn diese Option zuvor deaktiviert wurde, werden die Textur-Ausgabe(en) von übergeben in **SubstanceGraphInstance** erstellt. Dies weist die gleiche Funktionalität auf wie das Aktivieren der Ausgabe vom **SubstanceGraphInstance**-Editor. *HINWEIS: Dadurch wird Ihr Material nicht mit der neu erstellten Textur aktualisiert. Dies muss durch Festlegen eines Samplerparameters zur Laufzeit mithilfe der neuen Ausgabe behandelt werden.* |
| **DisableInstanceOutputs** | Eingabe: **SubstanceGraphInstance** - Die Grapheninstanz, die die Ausgabe zum Deaktivieren der Eingabe enthält: **OutputIndices** (int32 Array) - Die Indizes der Ausgaben, die Sie deaktivieren möchten | Wenn diese Option aktiviert ist, wird die Textur-Ausgabe für die im Graf-Objekt übergebenen Elemente deaktiviert und gelöscht. |
| **CopyInputParameters** | Eingabe: **SubstanceGraphInstance** - Die Grapheninstanz, auf die Sie Werte anwenden möchten: **SubstanceGraphInstance** - Die Grapheninstanz, von der Sie die Werte abrufen möchten | Stellt alle geänderten Eingabewerte des Substance-Grafen Instance Eingabeparameters wieder her. |
| **ResetInputParameters** | Eingabe: SubstanceGraphInstance | Setzen Sie die Eingabewerte einer Substance-Grafen-Instanz auf ihre Standardwerte zurück. |
| **SetGraphInstanceOutputSize** | Eingabe: **SubstanceGraphInstance** Eingabe: Breite - Textur Auflösung der X-KoordinateEingabe: Height - Textur Auflösung der Y-Koordinate | Legt die Größenauflösung aller Ausgaben fest, die aus dieser Grapheninstanz generiert werden, wobei die Texturen aus den Parametern übergeben werden. Hinweis: Max. 2048 auf CPU-EngineHinweis: Max. 4096 auf GPU-Engine |
| **AsyncRendering** | **SubstanceGraphInstance** | Berechnet die Texturen der Substance-Grafen-Instanz neu. (Nicht blockieren) |
| **SyncRendering** | **SubstanceGraphInstance** | Berechnet Ausgabetexturen der Eingabe der Substance-Grafen-Instanz neu. (Sperren) |

## Spezifische Funktionen für Grapheninstanzen:

Kann nur von einer Diagramminstanz aufgerufen werden

| Name | Eingabe | Beschreibung |
| --- | --- | --- |
| GetDynamicMaterialInstance | Eingabe: Name (Zeichenfolge) | Gibt die Common Language Runtime Dynamic Material Instance einer Substanz zurück oder erstellt eine Instanz, falls keine vorhanden ist. Dynamische Material-Instanzen sind für die meisten Laufzeitwertänderungen von Substance-Wertausgaben erforderlich. |
| **GetInputNames** | KEINE | Gibt ein Array von Strings zurück, das alle Namen der Eingabeparameter enthält. |
| **GetInputType** | KEINE | Gibt den Datentyp zurück, der mit dieser Eingabe verknüpft ist. |
| **SetInputInt** | Eingabe: **Bezeichner** (Zeichenfolge)Eingabe: **InputValues** (int array) | Ändern Sie den Wert einer Eingabe, die vom Bezeichner gefunden wird. Innerhalb eines Spiels muss die Substanz mit **AyncRender** oder **SyncRender** gerendert werden, damit die Änderungen angewendet werden. |
| **SetInputFloat** | Eingabe: **Bezeichner** (Zeichenfolge)Eingabe: **InputValues** (schwebendes Array) | Ändern Sie den Wert einer Eingabe, die vom Bezeichner gefunden wird. Innerhalb eines Spiels muss die Substanz mit **AyncRender** oder **SyncRender** gerendert werden, damit die Änderungen angewendet werden. |
| **GetInputInt** | Eingabe: **Identifizierung** (Zeichenfolge) | Gibt ein Array von int-Werten mit den aktuellen Werten eines Eingabeparameters zurück. |
| **GetInputFloat** | Identifizierung (Zeichenfolge) | Gibt ein Array von Gleitkommazahlen mit den aktuellen Werten eines Eingabeparameters zurück. |
| **SetInputBool** | Eingabe: **Bool** (Boolesche Wert)Eingabe: **Identifizierung** (Zeichenfolge) | Verwendet einen booleschen Wert, um einen umschaltbaren Eingabewerttyp zuzuweisen. Bisher konnte dies nur erreicht werden, indem ein int-Wert von entweder einer 1 oder einer 0 Geworfen zu einem bool gesetzt wurde. |
| **GetInputBool** | Eingabe: **Identifizierung** (Zeichenfolge) | Gibt den aktuellen booleschen Wert einer Eingabe zurück. |
| **SetIputColor** | Eingabe: **Color** (LinearColor)Eingabe: **Identifizierung** (FString) | Verwendet einen FLinearColor-Wert, dem ein Farbeingabewerttyp zugewiesen werden soll. Bisher konnte dies nur durch Festlegen eines Floatwerts und Übergeben eines Arrays von Floats erreicht werden. |
| **GetInputColor** | Eingabe: Identifizierung (FString) | Gibt den aktuellen Farbwert im UE4-Format zurück. |
| **CreateAggregateSubstanceFactory** | Eingabe: **Output Factory** (SubstanceInstanceFactory)*Die Factory, die die Ausgaben erstellt, die als Eingabe für die Input Factory verwendet werden.* Eingabe: **Output Factory Graf Index** (Ganzzahl)*Welcher Graf innerhalb des Stoffes, den Sie kombinieren möchten.* Eingabe: **Input Factory** (SubstanceInputFactory)*Die Factory, die die Ausgaben als Eingabebild aus der Output Factory verwendet.*Input:**Verbindungen**(Array of SubstanceConnections)*Diese Verbindung kann mit dem Blueprint-Knoten Make Array erstellt werden. Mit einer Substance-Verbindung können Sie den Aggregatknoten bestimmen, der in die Verknüpfung mit den jeweiligen Ausgaben eingibt.* ** Return (SubstanceInstanceFactory)***Kann zum Erstellen einer Grapheninstanz der neuen kombinierten Instanz verwendet werden.* | Mit dem neuen Aggregatsubstanzknoten können Sie zwei Substanzinstanzfactorys verwenden und zur Laufzeit eine neue Instanzfactory erstellen, mit der eine neue Grapheninstanz erstellt werden kann. Das Besondere daran ist, dass Sie Texturen von einer der kombinierten Grapheninstanzen mit Eingabebildern der anderen kombinierten Grapheninstanz verbinden können. Informationen zum Erstellen einer Substance-Grapheninstanz von diesem neuen Werk finden Sie in unserer Dokumentation zu Grapheninstanzen der Laufzeit. |
| **SubstanceConnectionStruct** | Eingabe: **Identifizierung der Ausgabe** (FString)*Die Identifizierung der Textur, die in eine Eingabe verkettet werden soll.* Eingabe: **Eingabe-Identifizierung** (FString) | Wird von Create Aggregate Substance Factory verwendet, um anzugeben, wie jede Ausgabe-Textur mit neuen Eingabe-Texturen verkettet werden soll. |
