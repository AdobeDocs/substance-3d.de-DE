---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-2-3-4.html"
breadcrumb-title: ''
description: Lesen Sie die Versionshinweise für Unity-Plug-in Version 2.3.4 , um mehr über neue Funktionen, Verbesserungen und Fehlerbehebungen zu erfahren.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 2.3.4
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Einheit 2.3.4
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '409'
ht-degree: 0%

---


# Einheit 2.3.4

>[!WARNING]
>
> **Bei Verwendung des Plug-ins mit Unity 2019.2 tritt der folgende Fehler auf:**
> 
> InspectorSubstanceImporter.OnInspectorGUI muss ApplyRevertGUI aufrufen, um unerwartetes Verhalten zu vermeiden.\
> UnityEditor.Experimental.AssetImporters.AssetImporterEditor:OnDisable()\
> Substance.Editor.InspectorSubstanceImporter:OnDisable()
> 
> Dieser Fehler kann gelöscht werden und wirkt sich nicht auf die Funktionalität des Plug-ins aus.

>[!WARNING]
>
> **Bitte lesen: Substance Materialbeschädigung:**\
> Beim Substance von Materialien, die eine benutzerdefinierte Ausgabe mit einer leeren Verwendung enthalten, wird der Import unterbrochen. Auch beim Substance von Materialien, die doppelte Verwendungen enthalten, wird der Inhalt beschädigt.\
> Ältere SBSAR-Dateien von GameTextures.com sind derzeit nicht mit dem Substance in Unity-Plug-in kompatibel. Diese Materialien, die nicht unterstützte Verwendungs-Ausgaben enthalten, werden beschädigt. Bevor Sie das Plug-in verwenden, stellen Sie sicher, dass Sie ein Backup Ihres Projekts erstellen.

## Neue Funktionen:

* Zusätzliche Unterstützung für Substance Engine v7
* Unterstützung für Linux hinzugefügt

### Fehlerbehebungen:

* Probleme beim Importieren einer Substance ohne Texturmaps wurden behoben
* Es wurde ein Problem behoben, bei dem der Reflexionsprozess in Unity 2019.x nicht korrekt funktionierte
* Probleme beim Umgang mit Prefabs beim Importieren eines Pakets, das Prefabs mit Substance-Materialien enthält, wurden behoben.
* Feste Material-/Texturzuweisungen werden nach dem Reflexionsprozess nicht übertragen
* Es wurde ein Problem behoben, durch das beim Ändern von Shadern Materialien beschädigt wurden.
* Es wurde ein Problem behoben, durch das die Raueit nicht in den metallischen Alphakanal verpackt wurde.
* Es wurde ein Problem behoben, bei dem bei der Installation des Substance-Plug-ins durch das Ändern der Importeinstellungen für Nicht-Substance-Texturen bestimmte Optionen zurückgesetzt wurden.
* Es wurde ein Problem behoben, bei dem die Substance Source unter Mac nicht geöffnet werden konnte.

## Bekannte Probleme:

**Core Substance-Plug-in**

* Der Benutzer muss &quot;Bitcode aktivieren&quot; im Menü &quot;Buildeinstellungen&quot; in Xcode deaktivieren, um für iOS zu erstellen.
* Substance funktionieren nicht mit Asset Bundles
* Substance-Vorschausymbole im Asset-Browser werden nach einem erneuten Import alle zum Substance S-Symbol
* Bei benutzerdefinierten Substance-Materialien, bei denen die Ausgabe auf &quot;leer&quot; gesetzt ist, wird das Material beschädigt.
* Bei benutzerdefinierten Substance-Materialien mit doppelter Nutzung wird das Material beschädigt.
* Der Editor muss neu gestartet werden, nachdem das Plugin unter Linux importiert wurde

**Skripterstellung**

* Skripterstellung funktioniert nicht zur Laufzeit, wenn das Projekt in den Buildeinstellungen auf x86 festgelegt ist
* Probleme bei der Verwendung von il2cpp-Skript-Backend mit bestimmten Build-Plattformen

**Substance Painter Live Link**

* Beim Erstellen eines Projekts nach dem Malen mit Substance Live Link wird das gemalte Gitter wieder auf ein Standardmaterial zurückgesetzt
* AO-Kanal wird nicht mit Painter-Live-Link gesendet
* Gitter mit mehreren Materialien funktionieren in Unity Live Link nicht
* Die Art und Weise, wie Unity LiveLink SimpleJson verwendet, kollidiert mit anderen Instanzen von SimpleJson in einem Projekt
