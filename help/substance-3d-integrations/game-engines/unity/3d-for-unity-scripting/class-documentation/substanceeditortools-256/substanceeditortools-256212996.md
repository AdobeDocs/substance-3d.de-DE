---
helpx_url: "https://helpx.adobe.com/de/substance-3d-integrations/game-engines/unity/substance-3d-for-unity-scripting/class-documentation/substanceeditortools-256212996.html"
breadcrumb-title: ''
description: Referenzdokumentation für die SubstanceEditorTools-Klasse zum Substance von Materialverwaltung in Unity.
helpx_creative_field: ""
helpx_description: Substance 3D Integrations
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: SubstanceEditorTools
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '104'
ht-degree: 0%

---


# SubstanceEditorTools

## Adobe.SubstanceEditor.SubstanceEditorTools-Klassenreferenz

Tools und Dienstprogramme für Benutzer, die auf Editorskripten verwendet werden können.

Vererbungsdiagramm für Adobe.SubstanceEditor.SubstanceEditorTools:

![](../../../../../assets/image2022-10-14-17-53-23.png)

### Statische Funktionen für öffentliche Mitglieder

```
• static void SetGraphFloatInput (SubstanceGraphSO graph, int inputId, float value)
```


Diagrammeingabe für Gleitkommawerte festlegen.

```
• static void SetGraphFloat2Input (SubstanceGraphSO graph, int inputId, Vector2 value)
```


Stellen Sie den Diagrammeingang &quot;float2&quot; ein.

```
• static void SetGraphFloat3Input (SubstanceGraphSO graph, int inputId, Vector3 value)
```


Stellen Sie den Diagrammeingang &quot;float3&quot; ein.

```
• static void SetGraphFloat4Input (SubstanceGraphSO graph, int inputId, Vector3 value)
```


Stellen Sie den Diagrammeingang &quot;float4&quot; ein.

```
• static void SetGraphIntInput (SubstanceGraphSO graph, int inputId, int value)
```


Setzen Sie den Graph auf die Eingabe.

```
• static void SetGraphInt2Input (SubstanceGraphSO graph, int inputId, Vector2Int value)
```


Setzen Sie den Graphen int2-Eingang.

```
• static void SetGraphInt3Input (SubstanceGraphSO graph, int inputId, Vector3Int value)
```


Setzen Sie den Graphen int3-Eingang.

```
• static void SetGraphInt4Input (SubstanceGraphSO graph, int inputId, int value0, int value1, int value2, int value3)
```


Setzen Sie den Graphen int4-Eingang.

```
• static void SetGraphInputString (SubstanceGraphSO graph, int inputId, string value)
```


Stellen Sie die Zeichenfolgeneingabe für das Diagramm ein.

```
• static void SetGraphInputTexture (SubstanceGraphSO graph, int inputId, Texture2D value)
```


Festlegen der Eingabe für die Diagrammtextur.

```
• static void RenderGraph (SubstanceGraphSO graph)
```


Rendert das Zieldiagramm und aktualisiert seine Elemente.

```
• static string CreatePresetFromCurrentState (SubstanceGraphSO graph)
```


Erstellt eine voreingestellte XML-Datei aus dem aktuellen Status des Diagrammobjekts.

```
• static List< SubstanceGraphSO > GetGraphs (this SubstanceFileSO fileSO)
```


Gibt die Liste der SubstanceGraphSOs zurück, die einer SubstanceFileSO zugeordnet sind.
