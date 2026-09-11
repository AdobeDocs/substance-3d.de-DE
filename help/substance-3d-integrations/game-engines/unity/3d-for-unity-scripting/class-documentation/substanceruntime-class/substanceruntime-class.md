---
helpx_url: "https://helpx.adobe.com/de/substance-3d-integrations/game-engines/unity/substance-3d-for-unity-scripting/class-documentation/substanceruntime-class.html"
breadcrumb-title: ''
description: Referenzdokumentation für die SubstanceRuntime-Klasse, die für Substance-Material-Vorgänge zur Laufzeit in Unity verwendet wird.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Substance 3D for Unity Scripting > Class Documentation > SubstanceRuntime Class
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: SubstanceRuntime-Klasse
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '134'
ht-degree: 1%

---


# SubstanceRuntime-Klasse

## Adobe.Substance.Runtime.SubstanceRuntime-Klassenreferenz

Singleton-Klasse, die die Substance-Engine-Initialisierung behandelt, und sie wird verwendet, um systemeigene Handler für Substance-Instanzen zu erhalten.\
Vererbung-Diagramm für Adobe.Substance.Runtime.SubstanceRuntime:

![](../../../../../assets/image2022-6-22-14-35-28.png)

### Öffentliche Mitgliederfunktionen

```
• SubstanceNativeGraph InitializeInstance (SubstanceGraphSO substanceInstance)
```


Erstellt ein Substance SDK-Handle für eine bestimmte SubstanceGraphSO.

### Eigenschaften

```
• static SubstanceRuntime Instance [get]
```


Singleton-Instanz.

### Ausführliche Beschreibung

Singleton-Klasse, die die Substance-Engine-Initialisierung behandelt, und sie wird verwendet, um systemeigene Handler für Substance-Instanzen zu erhalten.

### Dokumentation der Mitgliederfunktion

#### InitializeInstance()

```
SubstanceNativeGraph Adobe.Substance.Runtime.SubstanceRuntime.InitializeInstance  

( SubstanceGraphSO substanceInstance ) [inline]
```


Erstellt ein Substance SDK-Handle für eine bestimmte SubstanceGraphSO.

**Parameter**

|  |  |
| --- | --- |
| substanceInstance | Target SubstanceGraphSO |


**Rückgaben**

Handle, das mit dem Substance SDK kommuniziert

### Eigenschaftendokumentation

#### Instanz

```
SubstanceRuntime Adobe.Substance.Runtime.SubstanceRuntime.Instance [static], [get]
```


Singleton-Instanz.

Globale Singletoninstanz.

>[!NOTE]
>
> NativeGraph.InRenderWork ist nur für die interne Verwendung zur Kommunikation mit dem Substance Engine vorgesehen und sollte nicht für benutzerdefinierte Workflows verwendet werden.
