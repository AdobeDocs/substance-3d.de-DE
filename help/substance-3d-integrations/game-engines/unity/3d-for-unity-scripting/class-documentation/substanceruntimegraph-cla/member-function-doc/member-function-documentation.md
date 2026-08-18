---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/substance-3d-for-unity-scripting/class-documentation/substanceruntimegraph-class/member-function-documentation.html"
breadcrumb-title: ''
description: Detaillierte Dokumentation für alle Memberfunktionen der SubstanceRuntimeGraph-Klasse in Unity-Skripterstellung.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Substance 3D for Unity Scripting > Class Documentation > SubstanceRuntimeGraph Class > Member Function Documentation
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Dokumentation der Mitgliederfunktion
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '662'
ht-degree: 2%

---


# Dokumentation der Mitgliederfunktion

## AttachGraph()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.AttachGraph  

( SubstanceGraphSO graph ) [inline]
```


Fügt diesem Laufzeithandler ein neues Diagrammobjekt hinzu.

**Parameter**

|  |  |
| --- | --- |
| Graph | Diagramm der Zielsubstanz. |

### CreatePresetFromCurrentState()

```
string Adobe.Substance.Runtime.SubstanceRuntimeGraph.CreatePresetFromCurrentState ( ) [inline]
```


Speichert den aktuellen Diagrammstatus in einer voreingestellten XML-Datei.

**Rückgaben**

Vorgabe, die mit dem aktuellen Status der Diagrammeingaben erstellt wird.

### GetGeneratedTextures()

```
List< Texture2D > Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetGeneratedTextures ( ) [inline]
```


Gibt eine Liste mit allen Ausgabetexturen für die Substance-Instanz zurück.

**Rückgaben**

Ausgabetextur.

### GetInputBool()

```
bool Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputBool ( string inputName ) [inline]
```


Abrufen der booleschen Substance-Eingabe.

**Parameter**

|  |  |
| --- | --- |
| inputName | Name der Eingabe im SBSAR. |


**Rückgaben**

Aktueller Eingabewert.

### GetInputColor()

```
Color Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputColor ( string inputName ) [inline]
```


Substance Color herunterladen

**Parameter**

|  |  |
| --- | --- |
| inputName | Name der Eingabe im SBSAR |


**Rückgaben**

Aktueller Eingabewert.

### GetInputDescription()

```
SubstanceInputDescription Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputDescription ( string inputName ) [inline]
```


Gibt die vollständige Eingabebeschreibung für den Zieleingabenamen zurück.

**Parameter**

|  |  |
| --- | --- |
| inputName | Name der Zieleingabe. |


**Rückgaben**

Vollständige Eingabebeschreibung für die Zieleingabe.

### GetInputFloat()

```
float Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputFloat ( string inputName ) [inline]
```


Substance Float-Eingang abrufen

**Parameter**

|  |  |
| --- | --- |
| inputName | Name der Eingabe im SBSAR |


**Rückgaben**

Aktueller Eingabewert.

### GetInputInt()

```
int Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputInt ( string inputName ) [inline]
```


Substance-Eingabe abrufen

**Parameter**

|  |  |
| --- | --- |
| inputName | Name der Eingabe im SBSAR |


**Rückgaben**

Aktueller Eingabewert.

### GetInputString()

```
string Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputString ( string inputName ) [inline]
```


Substance-Zeichenfolgeneingabe abrufen.

**Parameter**

|  |  |
| --- | --- |
| inputName | Name der Eingabe im SBSAR |


**Rückgaben**

Aktuellen Wert eingeben.

### GetInputVector2()

```
Vector2 Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputVector2 ( string inputName ) [inline]
```


Substance Vector2-Eingang abrufen

**Parameter**

|  |  |
| --- | --- |
| inputName | Name der Eingabe im SBSAR |


**Rückgaben**

Aktueller Eingabewert.

### GetInputVector2Int()

```
Vector2Int Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputVector2Int ( string inputName ) [inline]
```


Array mit 2 int abrufen

**Parameter**

|  |  |
| --- | --- |
| inputName | Name der Eingabe im SBSAR |


**Rückgaben**

Aktueller Eingabewert.

### GetInputVector3()

```
Vector3 Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputVector3 ( string inputName ) [inline]
```


Substance Vector3-Input.

**Parameter**

|  |  |
| --- | --- |
| inputName | Name der Eingabe im SBSAR |


**Rückgaben**

Aktueller Eingabewert.

### GetInputVector3Int()

```
Vector3Int Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputVector3Int ( string inputName ) [inline]
```


Array mit 3 int (x-, y- und z-Werte von Vector3Int)

**Parameter**

|  |  |
| --- | --- |
| inputName | Name der Eingabe im SBSAR |


**Rückgaben**

Aktueller Eingabewert.

### GetInputVector4()

```
Vector4 Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputVector4 ( string inputName ) [inline]
```


Substance Vector4-Eingabe abrufen

**Parameter**

|  |  |
| --- | --- |
| inputName | Name der Eingabe im SBSAR |


**Rückgaben**

Aktueller Eingabewert.

### GetInputVector4Int()

```
int[] Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputVector4Int ( string inputName ) [inline]
```


Array mit 4 int (x-, y-, z- und w-Werte von Vector4Int)

**Parameter**

|  |  |
| --- | --- |
| inputName | Name der Eingabe im SBSAR |


**Rückgaben**

Aktueller Eingabewert.

### GetOutputTexture()

```
Texture2D Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetOutputTexture ( string outputName ) [inline]
```


Gibt die Ausgabetextur für einen bestimmten Ausgabenamen zurück.

**Parameter**

|  |  |
| --- | --- |
| outputName | Ausgabename. |


**Rückgaben**

Ausgabetextur.

### GetTexturesResolution()

```
Vector2Int Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetTexturesResolution ( ) [inline]
```


Gibt die Auflösung der Ausgabeinstanz-Textur zurück.

**Rückgaben**

Aktuelle Ausgabeauflösung.

### HasInput()

```
bool Adobe.Substance.Runtime.SubstanceRuntimeGraph.HasInput ( string inputName ) [inline]
```


Gibt &quot;true&quot; zurück, wenn diese Substance-Instanz eine Eingabe mit einem bestimmten Namen hat.

**Parameter**

|  |  |
| --- | --- |
| inputName | Eingabename. |


**Rückgaben**

TRUE, wenn die Substance-Instanz Eingaben mit dem angegebenen Namen enthält.

### LoadPreset()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.LoadPreset ( string presetXML ) [inline]
```


Verwendet eine voreingestellte XML-Datei, um Parameter für die Diagrammeingabe festzulegen.

**Parameter**

|  |  |
| --- | --- |
| presetXML | XML-Vorgabendaten. |

### RenderAsync()

```
Task Adobe.Substance.Runtime.SubstanceRuntimeGraph.RenderAsync ( ) [inline]
```


Die Substance-Instanz wird asynchron gerendert.

**Rückgaben**

Vorgang, der nach Abschluss des Renderns abgeschlossen wird.

### SetInputBool()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputBool ( string inputName, 

bool value ) [inline]
```


Aktualisieren der booleschen Substance-Eingabe

**Parameter**

|  |  |
| --- | --- |
| inputName | Name der Eingabe im SBSAR |
| Wert | Zum Aktualisieren des Parameters verwendeter Wert |

### SetInputColor()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputColor ( string inputName, 

Color value ) [inline]
```


Aktualisieren der Substance-Farbeingabe

**Parameter**

|  |  |
| --- | --- |
| inputName | Name der Eingabe im SBSAR |
| Wert | Zum Aktualisieren des Parameters verwendeter Wert |

### SetInputFloat()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputFloat ( string inputName, 

float value ) [inline]
```


Aktualisieren des Substance-Float-Eingangs

**Parameter**

|  |  |
| --- | --- |
| inputName | Name der Eingabe im SBSAR |
| Wert | Zum Aktualisieren des Parameters verwendeter Wert |

### SetInputInt()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputInt ( string inputName, 

int value ) [inline]
```


Substance-Int-Eingabe aktualisieren

**Parameter**

|  |  |
| --- | --- |
| inputName | Name der Eingabe im SBSAR |
| Wert | Zum Aktualisieren des Parameters verwendeter Wert |

### SetInputString()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputString ( string inputName, 

string value ) [inline]
```


Substance-Zeichenfolgeneingabe aktualisieren.

**Parameter**

|  |  |
| --- | --- |
| inputName | Name der Eingabe im SBSAR |
| Wert | Zum Aktualisieren des Parameters verwendeter Wert |

### SetInputTexture()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputTexture (string inputName, 

Texture2D value ) [inline]
```


Substance Texture2D-Eingabe aktualisieren.

**Parameter**

|  |  |
| --- | --- |
| inputName | Name der Eingabe im SBSAR |
| Wert | Zum Aktualisieren des Parameters verwendeter Wert |

### SetInputVector2()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputVector2 ( string inputName, 

Vector2 value ) [inline]
```


Substance Vector2-Eingabe aktualisieren

**Parameter**

|  |  |
| --- | --- |
| inputName | Name der Eingabe im SBSAR |
| Wert | Zum Aktualisieren des Parameters verwendeter Wert |

### SetInputVector2Int()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputVector2Int ( string inputName, 

Vector2Int value ) [inline]
```


Aktualisieren Sie die Substance Vector2Int-Eingabe.

**Parameter**

|  |  |
| --- | --- |
| inputName | Name der Eingabe im SBSAR |
| Wert | Zum Aktualisieren des Parameters verwendeter Wert |

### SetInputVector3()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputVector3 ( string inputName, 

Vector3 value ) [inline]
```


Substance Vector3-Eingabe aktualisieren

**Parameter**

|  |  |
| --- | --- |
| inputName | Name der Eingabe im SBSAR |
| Wert | Zum Aktualisieren des Parameters verwendeter Wert |

### SetInputVector3Int()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputVector3Int ( string inputName, 

Vector3Int value ) [inline]
```


Aktualisieren Sie die Substance Vector3Int-Eingabe.

**Parameter**

|  |  |
| --- | --- |
| inputName | Name der Eingabe im SBSAR |
| Wert | Zum Aktualisieren des Parameters verwendeter Wert |

### SetInputVector4()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputVector4 ( string inputName, 

Vector4 value ) [inline]
```


Substance Vector4-Eingabe aktualisieren

**Parameter**

|  |  |
| --- | --- |
| inputName | Name der Eingabe im SBSAR |
| Wert | Zum Aktualisieren des Parameters verwendeter Wert |

### SetInputVector4Int()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputVector4Int ( string inputName, 

int x, 

int y, 

int z, 

int w ) [inline]
```


Substance Vector4Int-Eingabe aktualisieren

**Parameter**

|  |  |
| --- | --- |
| inputName | Name der Eingabe im SBSAR |
| x | Wert, der zum Aktualisieren des Parameters verwendet wird |
| y | Wert, der zum Aktualisieren des Parameters verwendet wird |
| z | Wert, der zum Aktualisieren des Parameters verwendet wird |
| w | Wert, der zum Aktualisieren des Parameters verwendet wird |

### SetTexturesResolution()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetTexturesResolution ( Vector2Int size ) [inline]
```


Legt die Auflösung der Ausgabeinstanz-Textur fest.

**Parameter**

|  |  |
| --- | --- |
| Umfang |  |
