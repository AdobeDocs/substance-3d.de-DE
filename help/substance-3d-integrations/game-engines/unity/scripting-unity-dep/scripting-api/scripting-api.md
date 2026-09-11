---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/scripting-in-unity-deprecated/scripting-api.html"
breadcrumb-title: ''
description: Referenzdokumentation für die veraltete Substance Unity-Scripting-API für die Unterstützung älterer Projekte.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Scripting in Unity (Deprecated) > Scripting API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Scripting-API
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '1074'
ht-degree: 1%

---


# Scripting-API

## Substance in Unity API - 2.2.0

## Substance-Materialparameter

| Public-Methode | Beschreibung | Parameter |
| --- | --- | --- |
| public **float** *GetInputFloat*(**string** inputName) | Substance **Float**-Eingabe abrufen | **Zeichenfolge** *Eingabename* Name der Eingabe in der SBSAR |
| public **int** *SetInputFloat*(**string** inputName, **float** value) | Substance **Float**-Eingabe aktualisieren | **String** i *InputName* Name der Eingabe im SBSAR **Float** *value*-Wert, der zum Aktualisieren des Parameters verwendet wird |
| public **void** *SetInputVector2*(**string** inputName, **Vector2** value) | Substance **Vector2**-Eingabe aktualisieren | **String** *inputName* Name der Eingabe im SBSAR **Vector2** *input* Werte, die zum Aktualisieren des Parameters verwendet werden |
| public **vector2** *GetInputVector2*(**string** inputName) | Substance **Vector2**-Eingabe abrufen | **String** &quot;inputName&quot; Name der Eingabe in der SBSAR |
| public **void** *SetInputVector3*(**string** inputName, **Vector3** value) | Substance **Vector3**-Eingabe aktualisieren | **String** *inputName* Name der Eingabe im SBSAR **Vector3** *value* Werte, die zum Aktualisieren des Parameters verwendet werden |
| public **vector3** *GetInputVector3*(**string** inputName) | Substance **Vector3**-Eingabe abrufen | **Zeichenfolge** *Eingabename* Name der Eingabe in der SBSAR |
| public **void** *SetInputVector4*(**string** inputName, **Vector4** value) | Substance **Vector4**-Eingabe aktualisieren | **String** *inputName* Name der Eingabe im SBSAR **Vector4** *value* Werte, die zum Aktualisieren des Parameters verwendet werden |
| public **vector4** *GetInputVector4*(**string** inputName) | Substance **Vector4**-Eingabe abrufen | **Zeichenfolge** inputName Name der Eingabe in der SBSAR |
| public **void** *SetInputColor*(**string** inputName, **Color** value) | Substance **Color**-Eingabe aktualisieren | **Zeichenfolge** inputName Name der Eingabe im SBSAR **Color**-Wert, der zum Aktualisieren des Parameters verwendet wird |
| public **color** *GetInputColor*(**string** inputName, **int** dataType) | Substance **Color** abrufen | **String** *inputName* Name der Eingabe im SBSAR **Int** *dataType* |
| public **void** *SetInputBool*(**string** inputName, **bool** value) | Substance **Boolesche Wert**-Eingabe aktualisieren | **String** *inputName* Name der Eingabe im SBSAR **Bool** *value*-Wert, der zum Aktualisieren des Parameters verwendet wird |
| public **bool** *GetInputBool*(**string** inputName) | Substance **Boolesche Wert**-Eingabe abrufen | **Zeichenfolge** *Eingabename* Name der Eingabe in der SBSAR |
| public **void** *SetInputInt*(**string** inputName, **int** value) | Substance **Int**-Eingabe aktualisieren | **Zeichenfolge** *Eingabename* Name der Eingabe im SBSAR **Int** *Wert*, der zum Aktualisieren des Parameters verwendet wird |
| public **int** *GetInputInt*(**string** inputName) | Substance **Int**-Eingabe abrufen | **Zeichenfolge** *Eingabename* Name der Eingabe in der SBSAR |
| public **void** *SetInputVector2Int*(**string** inputName, **int** x, **int** y) | Substance **Vector2Int**-Eingabe aktualisieren | **String** *inputName* Name der Eingabe im SBSAR **Int** *x* Wert, der zum Aktualisieren des Parameters **Int** y Wert verwendet wird, der zum Aktualisieren des Parameters verwendet wird |
| **int[] Substance.Game.SubstanceGraph**.*GetInputVector2Int*( string inputName) | Array von 2 int (x/y-Werte von Vector2Int) | **String** *inputName* Name der Eingabe im SBSAR **Int** *x* Wert, der zum Aktualisieren des Parameters **Int** y Wert verwendet wird, der zum Aktualisieren des Parameters verwendet wird |
| **void Substance.Game.SubstanceGraph**.*SetInputVector3Int*( string inputName, int x, int y, int z) | Substance Vector3Int-Eingabe aktualisieren | **Zeichenfolge** *Eingabename* Name der Eingabe im SBSAR **Int** *x* Wert, der zum Aktualisieren des Parameters **Int** y Wert verwendet wird, der zum Aktualisieren des Parameters **Int** z Wert verwendet wird, der zum Aktualisieren des Parameters verwendet wird |
| **int[] Substance.Game.SubstanceGraph**.*GetInputVector3Int*( string inputName) | Array mit 3 int (x-, y- und z-Werte von Vector3Int) | **Zeichenfolge** *Eingabename* Name der Eingabe im SBSAR **Int** *x* Wert, der zum Aktualisieren des Parameters **Int** y Wert verwendet wird, der zum Aktualisieren des Parameters **Int** z Wert verwendet wird, der zum Aktualisieren des Parameters verwendet wird |
| **void Substance.Game.SubstanceGraph**.*SetInputVector4Int*( string inputName, int x, int y, int z, int w) | Substance Vector4Int-Eingabe aktualisieren | **Zeichenfolge** *Eingabename* Name der Eingabe im SBSAR **Int** *x* Wert, der zum Aktualisieren des Parameters **Int** y Wert verwendet wird, der zum Aktualisieren des Parameters **Int** z Wert verwendet wird, der zum Aktualisieren des Parameters **Int** w Wert verwendet wird, der zum Aktualisieren des Parameters verwendet wird |
| **int[] Substance.Game.SubstanceGraph**.*GetInputVector4Int*( string inputName) | Array mit 4 int (x-, y-, z- und w-Werte von Vector4Int) | **Zeichenfolge** *Eingabename* Name der Eingabe im SBSAR **Int** *x* Wert, der zum Aktualisieren des Parameters **Int** y Wert verwendet wird, der zum Aktualisieren des Parameters **Int** z Wert verwendet wird, der zum Aktualisieren des Parameters **Int** w Wert verwendet wird, der zum Aktualisieren des Parameters verwendet wird |
| **void Substance.Game.SubstanceGraph**.*SetInputString*( string inputName, string value) | Substance-Zeichenfolgeneingabe aktualisieren | **Zeichenfolge** *Eingabename* Name der Eingabe in SBSAR **Zeichenfolge** *Wert*, die zum Aktualisieren des Parameters verwendet wird |
| **Zeichenfolge Substance.Game.SubstanceGraph**.*GetInputString*(Zeichenfolge inputName) | Substance-Zeichenfolgeneingabe abrufen | **Zeichenfolge** *Eingabename* Name der Eingabe in der SBSAR |
| **void Substance.Game.SubstanceGraph**.*SetInputTexture*( string inputName, Textur2D value) | Substance Textur2D-Eingabe aktualisieren | **String** *inputName* Name der Eingabe im SBSAR **Textur2D** *value*, der zum Aktualisieren des Parameters verwendet wird |
| **Textur2D Substance.Game.SubstanceGraph**.*GetInputTexture*( string inputName) | Substance Textur2D-Eingabe abrufen | **Zeichenfolge** *Eingabename* Name der Eingabe in der SBSAR |
| **VectorInt Substance.Game.SubstanceGraph**.*GetTexturesResolution*() | Auflösung der Zieleinstellungen des Grafen abrufen (Texturen von Vector4Int: x = width, y = Height, Werte können 32, 64, 128, 256, 512, 1024, 2048 und 4096 sein) | Keine |
| **int Substance.Game.SubstanceGraph**.*SetTexturesResolution*( Vector2Int size) | Auflösung der Texturen für die Zieleinstellungen des Grafen festlegen (Vector2Int x = width, y = Height, Werte können 32, 64, 128, 256, 512, 1024, 2048 &amp; 4096 sein) Gibt 0 zurück, wenn der Vorgang erfolgreich war, andernfalls: -1. | **Vector2Int** *size* zum Aktualisieren des Parameters verwendet&#x200B;**.** |
| **Liste Substance.Game.SubstanceGraph**.*GetGeneratedTextures*() | Gibt alle Substance Textur2D-Objekte zurück, die vom Material-Shader des Grafen verwendet werden. | Keine |
| **int Substance.Game.SubstanceGraph**.*Baking*( Textur2D-Textur, Zeichenfolge absolutePath) | Generieren Sie .png-Dateien für alle Substance Textur2D-Objekte, die vom Material-Shader des Grafen verwendet werden. | Keine |
| **&#x200B;**&#x200B;Substance.Game.**&#x200B; SubstanceGraph**.*Duplicate*() | Duplizieren eines Substance-Grafen | Keine |
| **Substance.Game.SubstanceGraph**.*Duplicate*(string newGraphName) | Duplizieren Sie einen Substance-Grafen und geben Sie ihm einen Namen (das zugehörige Material hat ebenfalls denselben Namen). | **String newGraphName** |
| **&#x200B;**&#x200B;Substance.Game.**&#x200B; SubstanceGraph**.*GetInputProperties*() | Abfrage prozeduraler Eingabeinformationen, gibt ein Array von &quot;InputProperties&quot; zurück, mit :public Struktur InputProperties { public string name; // inputName public string label; // widget’s label in GUI public string group; // widget’s group in GUIpublic string[] componentLabels; // für Schieberegler (bis zu 4 Beschriftungen) public string[] enumOptions; // for optionMenuPublic InputPropertiesType type;public Vector4 maximum; // für Regler public Vector4 minimum; // für Regler public float step; // für Regler }public enum InputPropertiesType { Boolesche Wert = 0,// 0 Fließkommazahl, // 1 Vector2, // 2 Vector3, // 3 Vector4, // 4 Color, // 5 Enum, // 6 Textur, // 7 String, // 8 Invalid = -1// -1 }; | Keine |
| **bool** **Substance.Game.SubstanceGraph**.*HasInput*(**string** inputName) | Überprüfen Sie, ob eine Eingabe in einem Graf vorhanden ist, gibt true/false zurück: | **Zeichenfolge** *Eingabename* Name der Eingabe in der SBSAR |
| **bool** **Substance.Game.SubstanceGraph**.*IsInputVisible*(**string** inputName) | Überprüfen, ob eine sichtbare Eingabe sichtbar ist, gibt true/false zurück. | **Zeichenfolge** *Eingabename* Name der Eingabe in der SBSAR |

## Rendervorgang läuft

| Public-Methode | Beschreibung | Parameter |
| --- | --- | --- |
| public **void** *QueueForRender*() | Substance-Graf zur Warteschlange hinzufügen | Keine |
| ***mySubstance.**&#x200B;RenderAsync()* | Alle Substance-Graf in der Warteschlange asynchron rendern | Keine |
| ***mySubstance.**&#x200B;RenderSync()* | Alle Substance-Graf in der Warteschlange synchron rendern | Keine |

## Scripting im Editor-Modus:

Damit Graf-Modifikationen im Editor-Modus permanent übernommen werden können, muss ein erneuter Import der jeweiligen Substance durchgeführt werden. Dies geschieht mit der folgenden Funktion:

```
static void ReImportSubstance(Substance.Game.Substance pSubstance)

{



// Re-import Substance object:

SubstanceImporter importer = AssetImporter.GetAtPath(pSubstance.assetPath) as SubstanceImporter;

importer.CommitSubstanceToImporter(pSubstance); // plugin function

EditorUtility.SetDirty(importer);

importer.SaveAndReimport();



}
```


(mit &quot;CommitSubstanceToImporter&quot;, einer Substance-Plug-in-Funktion: Kopieren aller modifizierten Graf-Parameter und/oder Eingaben in das Substance-Importobjekt, das dann über den Importmechanismus von Unity auf die Festplatte serialisiert wird.)
