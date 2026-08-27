---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-4/blueprints-ue4/blueprintue4-node-reference.html"
breadcrumb-title: ''
description: Referenzhandbuch für alle in Unreal Engine 4 verfügbaren Substance Blueprint-Knoten für Material-Vorgänge.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 4 > Blueprints - UE4 > Blueprint(UE4) Node Reference
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Blueprint(UE4)-Knotenreferenz
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '856'
ht-degree: 0%

---


# Blueprint(UE4): Knotenreferenz

## Allgemeine Substance-Nodes:

| Name | Eingaben | Beschreibung |
| --- | --- | --- |
| **GetSubstances** | Material | Gibt ein Array von Materialinstanzen zurück, die von einem Substance-Grafen verwendet werden. Wenn Sie ein Material erstellen, das Texturausgaben von zwei verschiedenen Grafikinstanzen verwendet, gibt diese Funktion diese beiden Grafikinstanzen zurück. |
| **GetSubstanceTextures** | **SubstanceGraphInstance** | Gibt ein Array aller aktivierten und aktuell berechneten Texturen aus dem Eingabeparameter für die Substance-Grafen-Instanz zurück. |
| **GetGraphName** | **SubstanceGraphInstance** | Gibt den in Designer festgelegten Diagrammnamen zurück. |
| **GetFactoryName** | **SubstanceGraphInstance** | Gibt den Namen der **GraphInstanceFactory** zurück, die zum Erstellen der **SubstanceGraphInstance** verwendet wurde, die an diesen Knoten übergeben wird. |
| **GetSubstanceLoadingProgress** | KEINE | Gibt einen Gleitkommawert zwischen 0 und 1 zurück, der angibt, wie viele Substanzen vollständig geladen wurden. |
| **CreateGraphInstance** | Eingabe: **SubstanceInstanceFactory** - Die Factory, aus der Sie eine Diagramminstanz erstellen möchten.Input: **GraphIndex** (int) - Der Index des Diagramms, den Sie erstellen möchten. Eingabe: **InstanceName** (FString): Der Name, den Sie für Ihre neue Instanz verwenden möchten. | Gibt eine neue eigenständige Grafikinstanz zurück, die beibehalten wird, bis die Anwendung geschlossen wird. |
| **DuplicateGraphInstance** | **SubstanceGraphInstance** - Die Grapheninstanz, von der Sie eine Kopie erstellen möchten. | Gibt eine neue eigenständige Grafikinstanz zurück, die beibehalten wird, bis die Anwendung geschlossen wird. |
| **EnableInstanceOutputs** | Eingabe: **SubstanceGraphInstance** - Die Diagramminstanz, die die Ausgabe enthält, um die Eingabe zu aktivieren: **OutputIndices** (int32 Array): Die Indizes der Ausgaben, die Sie aktivieren möchten. (Änderungen vorbehalten) | Wenn zuvor deaktiviert, wird/werden die Texturausgabe(en) von übergeben in **SubstanceGraphInstance** erstellt. Dies weist die gleiche Funktionalität auf wie das Aktivieren einer Ausgabe aus dem **SubstanceGraphInstance**-Editor. *HINWEIS: Dadurch wird dein Material nicht mit der neu erstellten Textur aktualisiert. Dies muss durch Festlegen eines Samplerparameters zur Laufzeit mithilfe der neuen Ausgabe behandelt werden.* |
| **DisableInstanceOutputs** | Eingabe: **SubstanceGraphInstance** - Die Diagramminstanz, auf die Sie Werte anwenden möchten.Input: **SubstanceGraphInstance** - Die Diagramminstanz, von der Sie die Werte abrufen möchten. | Stellt alle geänderten Eingabewerte des Eingabeparameters &quot;Substance-Grafen-Instanz&quot; wieder her. |
| **SetGraphInstanceOutputSize** | Eingabe: **SubstanceGraphInstance** Eingabe: Breite - Texturauflösung der X-KoordinateEingabe: Height - Texturauflösung der Y-Koordinate | Legt die Strukturauflösung aller Ausgaben fest, die von dieser Diagramminstanz mit den Größen generiert werden, die von den Parametern übergeben werden. Hinweis: Max. 2048 auf CPU-EngineHinweis: Max. 4096 auf GPU-Engine |
| **AsyncRendering** | **SubstanceGraphInstance** | Berechnet Ausgabetexturen der Eingabe der Substance-Grafen-Instanz neu. (Nicht blockieren) |
| **SyncRendering** | **SubstanceGraphInstance** | Berechnet Ausgabetexturen der Eingabe der Substance-Grafen-Instanz neu. (Sperren) |

## Diagramminstanzspezifische Funktionen:

Kann nur von einer Diagramminstanz aufgerufen werden

| Name | Eingabe | Beschreibung |
| --- | --- | --- |
| **GetInputNames** | KEINE | Gibt ein Array von Strings zurück, das alle Namen der Eingabeparameter enthält. |
| **GetInputType** | KEINE | Gibt den Datentyp zurück, der mit dieser Eingabe verknüpft ist. |
| **SetInputInt** | Eingabe: **Bezeichner** (Zeichenfolge)Eingabe: **InputValues** (int array) | Ändern Sie den Wert einer Eingabe, die vom Bezeichner gefunden wird. Innerhalb eines Spiels muss die Substanz mit **AyncRender** oder **SyncRender** gerendert werden, damit die Änderungen angewendet werden. |
| **SetInputFloat** | Eingabe: **Bezeichner** (Zeichenfolge)Eingabe: **InputValues** (schwebendes Array) | Ändern Sie den Wert einer Eingabe, die vom Bezeichner gefunden wird. Innerhalb eines Spiels muss die Substanz mit **AyncRender** oder **SyncRender** gerendert werden, damit die Änderungen angewendet werden. |
| **GetInputInt** | Eingabe: **Bezeichner** (Zeichenfolge) | Gibt ein Array von int-Werten mit den aktuellen Werten eines Eingabeparameters zurück. |
| **GetInputFloat** | Bezeichner (Zeichenfolge) | Gibt ein Array von Gleitkommazahlen mit den aktuellen Werten eines Eingabeparameters zurück. |
| **SetInputBool** | Eingabe: **Bool** (Boolean)Eingabe: **Bezeichner** (Zeichenfolge) | Verwendet einen booleschen Wert, um einen umschaltbaren Eingabewerttyp zuzuweisen. Bisher konnte dies nur durch Einstellen eines in einen bool-Wert gegossenen int-Wertes von entweder 1 oder 0 erreicht werden. |
| **GetInputBool** | Eingabe: **Bezeichner** (Zeichenfolge) | Gibt den aktuellen booleschen Wert einer Eingabe zurück. |
| **SetIputColor** | Eingabe: **Color** (LinearColor)Eingabe: **Identifizierung** (FString) | Verwendet einen FLinearColor-Wert, dem ein Farbeingabewerttyp zugewiesen werden soll. Bisher konnte dies nur durch Festlegen eines Floatwerts und Übergeben eines Arrays von Floats erreicht werden. |
| **GetInputColor** | Eingabe: Identifizierung (FString) | Gibt den aktuellen Farbwert im UE4-Format zurück. |
| **CreateAggregateSubstanceFactory** | Eingabe: **Output Factory** (SubstanceInstanceFactory)*Die Factory, die die Ausgaben erstellt, die als Eingabe für die Input Factory verwendet werden.* Eingabe: **Output Factory Graf Index** (Ganzzahl)*Welcher Graf innerhalb des Stoffes, den Sie kombinieren möchten.* Eingabe: **Input Factory** (SubstanceInputFactory)*Die Factory, die die Ausgaben als Eingabebild aus der Output Factory verwendet.*Input:**Verbindungen**(Array of SubstanceConnections)*Diese Verbindung kann mit dem Blueprint-Knoten Make Array erstellt werden. Mit einer Substance-Verbindung können Sie den Aggregatknoten bestimmen, der in die Verknüpfung mit den jeweiligen Ausgaben eingibt.* ** Return (SubstanceInstanceFactory)***Kann zum Erstellen einer Grapheninstanz der neuen kombinierten Instanz verwendet werden.* | Mit dem neuen Aggregatsubstanzknoten können Sie zwei Substanzinstanzfactorys verwenden und zur Laufzeit eine neue Instanzfactory erstellen, mit der eine neue Grapheninstanz erstellt werden kann. Das Besondere daran ist, dass Sie Texturen von einer der kombinierten Grapheninstanzen mit Eingabebildern der anderen kombinierten Grapheninstanz verbinden können. Informationen zum Erstellen einer Substance-Grapheninstanz von diesem neuen Werk finden Sie in unserer Dokumentation zu Grapheninstanzen der Laufzeit. |
| **SubstanceConnectionStruct** | Eingabe: **Identifizierung der Ausgabe** (FString)*Die Identifizierung der Textur, die in eine Eingabe verkettet werden soll.* Eingabe: **Eingabe-Identifizierung** (FString) | Wird von Create Aggregate Substance Factory verwendet, um anzugeben, wie jede Ausgabe-Textur mit neuen Eingabe-Texturen verkettet werden soll. |
