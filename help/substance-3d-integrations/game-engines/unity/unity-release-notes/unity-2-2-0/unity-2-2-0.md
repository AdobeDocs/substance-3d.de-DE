---
helpx_url: "https://helpx.adobe.com/de/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-2-2-0.html"
breadcrumb-title: ''
description: Lesen Sie die Versionshinweise für Unity-Plug-in Version 2.2.0 , um mehr über neue Funktionen, Verbesserungen und Fehlerbehebungen zu erfahren.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 2.2.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Unity 2.2.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '674'
ht-degree: 0%

---


# Unity 2.2.0

## 2.2.0 Versionshinweise

**Freigabedatum: 10.01.2019**

### Kern-Plug-in:

* Aktualisiertes Substance Engine
* Verbesserte Codestabilität
* **Unterstützung für Unity 2018.3**
* **.NET 4.x-Unterstützung**
* Unterstützung von Substance Sourcen im Jahr 2018.3
* Problem mit der Farbgebung für Substance Sourcen wurde behoben
* Das Diagramm und das entsprechende Material haben jetzt denselben Objektnamen
* Verbesserungen bei der Lesbarkeit der Unity Pro-Skin-GUI
* Zusätzliche Unterstützung für Materialausgabezuweisungen
* Fehler in der sRGB-Verarbeitung behoben
* Es wurde ein Fehler behoben, durch den ein Benutzer alle Instanzen eines Diagramms löschen konnte
* Es wurde ein Fehler behoben, durch den der Versuch, Substance zu rendern, während Parameter zur Laufzeit geändert wurden, dazu führte, dass nur zwei gleichzeitig gerendert werden konnten.
* Beim Importieren eines Pakets, das alte Substance-Dateien enthält, benachrichtigt das Plug-in den Anwender, dass es alte Substance-Daten enthält, und löscht die Paketdateien, wenn Unity versucht, sie zu importieren (d. h. der Anwender muss nicht alles manuell löschen, wenn es defekt geliefert wurde)
* Es wurde eine Schaltfläche &quot;Info&quot; im Substance-Menü hinzugefügt, um Informationen zum Substance-Plug-in anzuzeigen.
* Hinzugefügte QuickInfos zum Mouseover in der Substance-GUI zum Anzeigen der angezeigten Substance-Parameternamen
* Navigationsschaltflächen in der Substance-Benutzeroberfläche wurden hinzugefügt, um einen Link zu Substance-Grafiken und -Materialien zu erstellen.
* Neue Symbole für das Substance-Diagramm/Material/Texturen im Inhaltsbrowser hinzugefügt
* Substance-Miniaturansichten im Inhaltsbrowser aktualisiert
* Die .mat-Datei von der Vorderseite der Substance-Materialnamen entfernt
* Substance-Grafiken und -Materialien können jetzt umbenannt werden.
* Wenn Sie die Substance-Diagrammauflösung ändern, wird das Popupfenster &quot;Anwenden/Wiederherstellen&quot; nicht mehr angezeigt, sodass der Benutzer die Änderung in diesem Moment bestätigen muss
* Es wurde ein Fehler behoben, durch den beim Reflexionsprozess nur die vom Benutzer definierte Standardauflösung für den Substance verwendet wurde.
* Es wurde eine Warnung zum Mouseover zur Substance-GUI hinzugefügt, die den Benutzer informiert, wenn der Farbraum auf Gamma festgelegt ist.
* Die Funktionalität von Substance-Graph-Instanzen wurde geändert: Benutzer können jetzt Grafikinstanzen auf einem Substance erstellen, ohne zu jeder erstellten Instanz auf der grafischen Substance-Benutzeroberfläche aufgefordert zu werden

### Skripterstellung:

* Wir haben einige Funktionen ausgeblendet, die nicht für die Skriptunterstützung vorgesehen sind
* Funktion zum Duplizieren von Substance-Graphinstanzen über das Skript hinzugefügt: Duplicate()
* Funktion zum Abfragen prozeduraler Eingabeinformationen über C# hinzugefügt, gibt ein Array von &quot;InputProperties&quot;-Elementen zurück: GetInputProperties()
* Zusätzliche Funktion zum Überprüfen, ob eine Eingabe in einem Diagramm vorhanden ist, gibt true/false zurück: HasInput(string inputName)
* Funktion hinzugefügt, um zu überprüfen, ob eine visibleF-Eingabe sichtbar ist, gibt true/false zurück: IsInputVisible(string inputName)
* Das Rendering-Schema wurde neu gestaltet. RenderSubstancesAsync() als solche veraltet ist, wurde dies in graphName.RenderAsync() geändert.

## Bekannte Probleme:

**Core Substance-Plug-in**

* Der Benutzer muss &quot;Bitcode aktivieren&quot; im Menü &quot;Buildeinstellungen&quot; in Xcode deaktivieren, um für iOS zu erstellen.
* Substance-Objektvorschauen im Inhaltsbrowser werden schwarz angezeigt, wenn das Buildziel auf Android/iOS festgelegt ist
* Die Schaltfläche &quot;Alpha&quot; und der Schieberegler für die Vorschau der Mip-Map fehlen auf der nicht-Substance-Textur-GUI nach dem Importieren des Substance-Plugins
* Der Anwender muss zwei Möglichkeiten nutzen, um eine Substance-Diagrammauflösung durch Skript zu definieren
* Substance-Materialien sind nicht dauerhaft, wenn sie mit einem Unity-Paket exportiert/importiert werden
* Substance funktionieren nicht mit Asset Bundles
* Substance-Vorschausymbole im Asset-Browser werden nach einem erneuten Import alle zum Substance S-Symbol
* Durch das Umbenennen eines Substance-Diagramms, das ein Material in der Szene enthält, wird dieses Material von den Objekten entfernt, auf denen es platziert ist.
* (Nur Mac) Durch die Aktualisierung des Plug-ins auf Mac werden Substance-Materialien aus Vorschauen in der Szene entfernt|

**Skripterstellung**

* Skripterstellung funktioniert nicht zur Laufzeit, wenn das Projekt in den Buildeinstellungen auf x86 festgelegt ist
* Probleme bei der Verwendung von il2cpp-Skript-Backend mit bestimmten Build-Plattformen

**Substance Painter Live Link**

* Beim Erstellen eines Projekts nach dem Malen mit Substance Live Link wird das gemalte Gitter wieder auf ein Standardmaterial zurückgesetzt
* AO-Kanal wird nicht mit Painter-Live-Link gesendet
* Gitter mit mehreren Materialien funktionieren in Unity Live Link nicht
* Die Art und Weise, wie Unity LiveLink SimpleJson verwendet, kollidiert mit anderen Instanzen von SimpleJson in einem Projekt
