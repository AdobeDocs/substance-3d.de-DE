---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-2-3-2.html"
breadcrumb-title: ''
description: Lesen Sie die Versionshinweise für Unity-Plug-in Version 2.3.2 , um mehr über neue Funktionen, Verbesserungen und Fehlerbehebungen zu erfahren.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 2.3.2
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Einheit 2.3.2
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---


# Einheit 2.3.2

## Neue Funktionen:

* Materialserialisierung
* Reflexion: Das Plug-in ermöglicht jetzt das Importieren alter Substance-Dateien in Paketen (automatisch aktualisiert auf neue Substance-Daten beim Importieren)
* Materialeigenschaften werden beim Import von Paketen mit Substance-Daten übertragen
  * Hinweis: Dies gilt nur für Pakete, die mit dem Update 2.3.0 oder höher erstellt wurden
* Schaltfläche &quot;Struktur backen&quot; zum Substance des Diagrammmenüs hinzugefügt

### Fehlerbehebungen:

* Es wurde ein Problem behoben, bei dem die Substance-Materialaufteilung zurückgesetzt wurde, wenn der Bibliotheksordner entfernt wurde.
* Verbesserte Geschwindigkeit beim Verlassen des Wiedergabemodus
* Es wurde ein Absturz beim Aktualisieren des Plug-ins behoben, während die Substance-DLL verwendet wurde.
* Der Ordner Allegorithmic kann jetzt nicht in Unity gelöscht werden.
  * Hinweis: Der Inhalt des Ordners &quot;Allegorithmic&quot; kann nicht geändert werden. Das Löschen in Unity kann mehrere Probleme verursachen, sodass der Ordner Allegorithmic wie von Zauberhand wieder angezeigt wird, wenn Unity geschlossen und erneut geöffnet wird. Es gibt jetzt eine Warnung, die den Benutzer auffordert, sie zu löschen, wenn Unity manuell aus dem Ordner &quot;Assets&quot; des Projekts geschlossen wird.
* Verbesserte Geschwindigkeit beim Verlassen des Wiedergabemodus
* Es wurde ein Fehler behoben, durch den die Substance-Materialeigenschaften zurückgesetzt wurden, wenn der Bibliotheksordner entfernt wurde.

## Bekannte Probleme:

**Core Substance-Plug-in**

* Der Benutzer muss &quot;Bitcode aktivieren&quot; im Menü &quot;Buildeinstellungen&quot; in Xcode deaktivieren, um für iOS zu erstellen.
* Substance funktionieren nicht mit Asset Bundles
* Substance-Vorschausymbole im Asset-Browser werden nach einem erneuten Import alle zum Substance S-Symbol

**Skripterstellung**

* Skripterstellung funktioniert nicht zur Laufzeit, wenn das Projekt in den Buildeinstellungen auf x86 festgelegt ist
* Probleme bei der Verwendung von il2cpp-Skript-Backend mit bestimmten Build-Plattformen

**Substance Painter Live Link**

* Beim Erstellen eines Projekts nach dem Malen mit Substance Live Link wird das gemalte Gitter wieder auf ein Standardmaterial zurückgesetzt
* AO-Kanal wird nicht mit Painter-Live-Link gesendet
* Gitter mit mehreren Materialien funktionieren in Unity Live Link nicht
* Die Art und Weise, wie Unity LiveLink SimpleJson verwendet, kollidiert mit anderen Instanzen von SimpleJson in einem Projekt
