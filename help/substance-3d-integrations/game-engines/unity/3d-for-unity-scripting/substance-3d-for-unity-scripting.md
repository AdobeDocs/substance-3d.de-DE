---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/substance-3d-for-unity-scripting.html"
breadcrumb-title: ''
description: Verwenden Sie die Substance 3D API in Unity, um Skripte zu schreiben, die Substance-Parameter zur Laufzeit aktualisieren und ändern.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Substance 3D for Unity Scripting
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Substance 3D für Unity Scripting
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---


# Substance 3D für Unity Scripting

Dieser Abschnitt der Dokumentation enthält Details zur Substance 3D API, die wir über das Substance 3D-Plug-in für Unity bereitstellen. Mithilfe der Substance-APIs können Sie Skripte schreiben, um Substance-Parameter zur Laufzeit zu aktualisieren und zu ändern.

## API-Übersicht

Das Plugin ist in 3 verschiedene Baugruppen unterteilt.

* Adobe.Substance
* Adobe.Substance.Editor
* Adobe.Substance.Runtime

### Adobe.Substance

Enthält freigegebene Komponenten für die Interaktion mit dem Substance SDK und zum Generieren entsprechender Unity-Objekte. Außerdem verfügt es über Marshallingdatenstrukturen für die Kommunikation zwischen C# und der Substance SDK C++-API.

#### Adobe.Substance.Editor

Enthält editorspezifische Klassen zum Behandeln der Anzeige von Informationen über die Unity-Substance-Objekte sowie zum Behandeln der Importpipeline, wenn dem Projekt SBSAR-Dateien hinzugefügt werden. Die SubstanceEditorEngine-Klasse ist ein Singleton, der die Lebensdauer des Substance-Moduls und aller seiner verwalteten Instanzen behandelt.

#### Adobe.Substance.Runtime

Diese Klasse verfügt über Komponenten, die die Erstellung und Verwaltung von Substance-Objekten während der Laufzeit verarbeiten. Die SubstanceRuntime entspricht der SubstanceEditorEngine-Klasse für die Laufzeit. Es wird die Initialisierung der Substance-Engine sowie die Instanziierung jeder Substance-Instanz verarbeiten, mit der Benutzerskripte interagieren.

## Laufzeitnutzung

Damit die Substance-Instanzeingaben zur Laufzeit geändert werden können, müssen Sie Ihrer Szene ein SubstanceRuntime←-Material hinzufügen (idealerweise zu demselben GameObject wie das Substance-Material). Diese Klasse unterstützt Sie beim Einrichten des Materials mit dem Singleton Adobe.Substance.Runtime.SubstanceRuntime, der die Instanziierung von Substance SDK-Objekten zur Laufzeit verwaltet.

## Codebeispiele

Das folgende Beispiel zeigt, wie Eingabeparameter zur Laufzeit mithilfe von SubstanceRuntimeGraph geändert werden.

### Parameter ändern

```
using System.Collections; 

using System.Collections.Generic; 

using UnityEngine; 

using Adobe.Substance.Runtime; 

public class scifiScript: MonoBehaviour { 

  public Adobe.Substance.Runtime.SubstanceRuntimeGraph mySubstance; 

  // Use this for initialization 

  void Start() { 

    UpdateSubstance(); 

  } 

  public void UpdateSubstance() { 

    // panel color 

    mySubstance.SetInputColor("paint_color", new Color(0.237 f, 0.834 f, 0.045 f, 1.0 f)); 

    // panel size 

    mySubstance.SetInputVector2("square_open", new Vector2(0.101 f, 0.209 f)); 

    // wear level 

    mySubstance.SetInputFloat("wear_level", 0.977 f); 

    // Submit async render. 

    mySubstance.RenderAsync(); 

  } 

}
```


Sie können SubstanceRuntimeGraph auch verwenden, um auf Eingabe- und Ausgabeinformationen zu Ihrem Substance-Material zuzugreifen.

#### Eingabeinformationen abrufen

```
using System.Collections; 

using System.Collections.Generic; 

using UnityEngine; 

using Adobe.Substance.Runtime; 

public class scifiScript: MonoBehaviour { 

  public Adobe.Substance.Runtime.SubstanceRuntimeGraph mySubstance; 

  // Use this for initialization 

  void Start() { 

    UpdateSubstance(); 

  } 

  public void UpdateSubstance() { 

    SubstanceInputDescription desc = mySubstance.GetInputDescription("paint_color"); 

    Debug.Log($ "Input: {desc.Identifier}"); 

    Debug.Log($ "Index: {desc.Index}"); 

    Debug.Log($ "Type: {desc.Type}"); 

    Debug.Log($ "Label: {desc.Label}"); 

  } 

}
```


Das folgende Beispiel zeigt, wie Sie ein benutzerdefiniertes Vorgabenmenü im Editor mit SubstanceEditorTools erstellen.

##### Erstellen von Vorgaben.

```
using System.Collections; 

using System.Collections.Generic; 

using UnityEngine; 

using Adobe.Substance.Runtime; 

public class scifiScript: MonoBehaviour { 

  public Adobe.Substance.Runtime.SubstanceRuntimeGraph mySubstance; 

  // Use this for initialization 

  void Start() { 

    UpdateSubstance(); 

  } 

  public void UpdateSubstance() { 

    SubstanceInputDescription desc = mySubstance.GetInputDescription("paint_color"); 

    Debug.Log($ "Input: {desc.Identifier}"); 

    Debug.Log($ "Index: {desc.Index}"); 

    Debug.Log($ "Type: {desc.Type}"); 

    Debug.Log($ "Label: {desc.Label}"); 

  } 

}
```
