---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/substance-3d-for-unity-scripting/class-documentation/substanceruntimegraph-class.html"
breadcrumb-title: ''
description: Referenzdokumentation für die SubstanceRuntimeGraph-Klasse, die für Laufzeitdiagrammvorgänge in Unity verwendet wird.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Substance 3D for Unity Scripting > Class Documentation > SubstanceRuntimeGraph Class
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: SubstanceRuntimeGraph-Klasse
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---


# SubstanceRuntimeGraph-Klasse

## Adobe.Substance.Runtime.SubstanceRuntimeGraph-Klassenreferenz

Klasse, die Laufzeitfunktionen zum Ändern von Eingaben bei Substanzdiagrammen und zum Rendern von Substanzdiagrammen bereitstellt, sodass Substance←GraphSO seine Assets zur Laufzeit generieren kann.

Vererbungsdiagramm für Adobe.Substance.Runtime.SubstanceRuntimeGraph:

![](../../../../../assets/image2022-10-14-17-53-23-1.png)

### Öffentliche Mitgliederfunktionen

```
• void AttachGraph (SubstanceGraphSO graph)
```


Fügt diesem Laufzeithandler ein neues Diagrammobjekt hinzu.

```
• void SetInputFloat (string inputName, float value)
```


Aktualisieren des Substance-Float-Eingangs

```
• float GetInputFloat (string inputName)
```


Substance Float-Eingang abrufen

```
• void SetInputVector2 (string inputName, Vector2 value)
```


Substance Vector2-Eingabe aktualisieren

```
• Vector2 GetInputVector2 (string inputName)
```


Substance Vector2-Eingang abrufen

```
• void SetInputVector3 (string inputName, Vector3 value)
```


Substance Vector3-Eingabe aktualisieren

```
• Vector3 GetInputVector3 (string inputName)
```


Substance Vector3-Input.

```
• void SetInputVector4 (string inputName, Vector4 value)
```


Substance Vector4-Eingabe aktualisieren

```
• Vector4 GetInputVector4 (string inputName)
```


Substance Vector4-Eingabe abrufen

```
• void SetInputColor (string inputName, Color value)
```


Aktualisieren der Substance-Farbeingabe

```
• Color GetInputColor (string inputName)
```


Substance Color herunterladen

```
• void SetInputBool (string inputName, bool value)
```


Aktualisieren der booleschen Substance-Eingabe

```
• bool GetInputBool (string inputName)
```


Abrufen der booleschen Substance-Eingabe.

```
• void SetInputInt (string inputName, int value)
```


Substance-Int-Eingabe aktualisieren

```
• int GetInputInt (string inputName)
```


Substance-Eingabe abrufen

```
• void SetInputVector2Int (string inputName, Vector2Int value)
```


Aktualisieren Sie die Substance Vector2Int-Eingabe.

```
• Vector2Int GetInputVector2Int (string inputName)
```


Array mit 2 int abrufen

```
• void SetInputVector3Int (string inputName, Vector3Int value)
```


Aktualisieren Sie die Substance Vector3Int-Eingabe.

```
• Vector3Int GetInputVector3Int (string inputName)
```


Array mit 3 int (x-, y- und z-Werte von Vector3Int)

```
• void SetInputVector4Int (string inputName, int x, int y, int z, int w)
```


Substance Vector4Int-Eingabe aktualisieren

```
• int[ ] GetInputVector4Int (string inputName)
```


Array mit 4 int (x-, y-, z- und w-Werte von Vector4Int)

```
• void SetInputString (string inputName, string value)
```


Substance-Zeichenfolgeneingabe aktualisieren.

```
• string GetInputString (string inputName)
```


Substance-Zeichenfolgeneingabe abrufen.

```
• SubstanceInputDescription GetInputDescription (string inputName)
```


Gibt die vollständige Eingabebeschreibung für den Zieleingabenamen zurück.

```
• void SetInputTexture (string inputName, Texture2D value)
```


Substance Texture2D-Eingabe aktualisieren.

```
• Vector2Int GetTexturesResolution ()
```


Gibt die Auflösung der Instanztexturausgabe zurück.

```
• void SetTexturesResolution (Vector2Int size)
```


Legt die Auflösung der Ausgabeinstanz-Textur fest.

```
• bool HasInput (string inputName)
```


Gibt &quot;true&quot; zurück, wenn diese Substance-Instanz eine Eingabe mit einem bestimmten Namen hat.

```
• List< Texture2D > GetGeneratedTextures ()
```


Gibt eine Liste mit allen Ausgabetexturen für die Substance-Instanz zurück.

```
•  Texture2D GetOutputTexture (string outputName)
```


Gibt die Ausgabetextur für einen bestimmten Ausgabenamen zurück.

```
• void Render ()
```


Rendert die Substance-Instanz synchron.

```
• Task RenderAsync ()
```


Die Substance-Instanz wird asynchron gerendert.

```
• void LoadPreset (string presetXML)
```


Verwendet eine voreingestellte XML-Datei, um Parameter für die Diagrammeingabe festzulegen.

```
• string CreatePresetFromCurrentState ()
```


Speichert den aktuellen Diagrammstatus in einer voreingestellten XML-Datei.

## Öffentliche Attribute

```
• SubstanceGraphSO GraphSO
```


Zielsubstanzinstanz.

## Geschützte Elementfunktionen

```
• void Awake ()
```


Bei Aktivierung wird SubstanceRuntime verwendet, um eine Instanz für die angehängte SubstanceGraphSO in der Substanz zu erstellen.

SDK

```
• void Update ()
```


Überprüfen Sie die Render-ConcurrentQueue auf Renderergebnisse.

```
• void OnDestroy ()
```


Stellt den Substance SDK-Handler bereit.

## Eigenschaften

```
• Material DefaulMaterial [get]
```


Hauptmaterial, das von der Substance-Instanz generiert wird.
