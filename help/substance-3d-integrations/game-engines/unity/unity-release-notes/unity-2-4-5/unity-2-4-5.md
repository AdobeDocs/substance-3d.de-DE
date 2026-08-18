---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-2-4-5.html"
breadcrumb-title: ''
description: Lesen Sie die Versionshinweise für Unity-Plug-in Version 2.4.5 , um mehr über neue Funktionen, Verbesserungen und Fehlerbehebungen zu erfahren.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 2.4.5
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Einheit 2.4.5
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 0%

---


# Einheit 2.4.5

Veröffentlicht am 6. April 2020

* Hinzugefügt: HDRP Asset Check mit der API 2019.3
* Hinzugefügt: Substance Engine 7.2-Update - Behebt einige Substance-Materialien von Source nicht
* Hinzugefügt: Zieleinstellungen an die CPU-Auflösung anpassen
* Hinzugefügt: Einstellung der maximalen Auflösung des CPU-Moduls (4K- oder 2K-Einstellung)
* Hinzugefügt: Konvertieren von Nicht-HDRP-Substance(s) in ein HDRP-Projekt
* Fest: Absturz beim Importieren einer großen Anzahl von Substance
* Fest: Ausnahme beim Klicken auf den erneuten Import im Wiedergabemodus nach dem Ändern der Substance-Parameter
* Fest: Auflösung der Ausgabe (Textur) überprüfen ( API zur Begrenzung der CPU-Engine auf 2K) Benutzervoreinstellung auf 4K
* Fest: Wenn Sie im Wiedergabemodus auf &quot;Mip-Maps generieren&quot; in einem Substance-Diagramm klicken und dann die Parameter ändern, entsteht ein unendlicher Hänger
* Fest: Bei Verwendung des Substance-Plug-ins in einem HDRP-Projekt werden Graustufen-Texturen bei Verwendung der Raw-Komprimierung auf Alpha8 gesetzt.
* Fest: GameObject im Wiedergabemodus deaktiviert
* Fest: Rauigkeitskarte wird nicht mit Parameteränderung aktualisiert
* Fest: Die Maskenausgabe wird für einige Substance-Dateien in HDRP nicht korrekt generiert
* Fest: Absturz beim Wechseln der gepackten Alpha-Map-Dropdown-Liste zwischen zwei Optionen
* Fest: Das Kontrollkästchen für die GPU-Instanz wird zurückgesetzt, wenn Sie auf einen Bereich außerhalb des Substance klicken.
* Fest: Wenn Sie die Funktion Duplicate() verwenden, wird die Smoothness des duplizierten Substance-Graphen nicht korrekt in das Alpha des Metallic-Graphen gepackt.
* Fest: Wenn Sie das Buildziel auf Android umstellen, werden Texturen so lange im falschen Format angezeigt, bis sie manuell erneut importiert werden.
* Fest: Das Löschen einer Substance-Datei in Unity führt zu einer NullReferenceException.
* Fest: Deaktivieren der Verwendung der Unity 2019.3 HDRP-API für frühere Versionen

Bekannte Probleme:

* Das Kontrollkästchen &quot;Emission&quot; ist standardmäßig nicht aktiviert und der HDR-Wert wird beim Importieren einer Substance auf Schwarz gesetzt.
* Materialeigenschaften von Verpackungen mit Standardsubstanzmaterialien werden beim Import nicht übernommen.
* Das Update von 2017-2019/2020 funktioniert nicht in HDRP
* Wenn Sie auf die 2048-Klemmoption im Einstellungsmenü klicken, während 4096 in den Zieleinstellungen ausgewählt ist (ohne Klicken auf Anwenden), wird ein Fehler im Konsolenprotokoll angezeigt
