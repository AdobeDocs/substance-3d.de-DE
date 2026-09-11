---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-2-5-2.html"
breadcrumb-title: ''
description: Lesen Sie die Versionshinweise für Unity-Plug-in Version 2.5.2 , um mehr über neue Funktionen, Verbesserungen und Fehlerbehebungen zu erfahren.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 2.5.2
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Einheit 2.5.2
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '147'
ht-degree: 0%

---


# Einheit 2.5.2

Veröffentlicht am 23. Juli 2020

Hinzugefügt:

* &quot;IsProcessing()&quot;-Funktion, die angibt, ob der Renderer ausgelastet ist, oder Idle (nicht ausgelastet)

Fest:

* Beim Einstellen der Zieleinstellungen 2048 Clamp und 4096 wird kein Fehler mehr angezeigt
* Material-Eigenschaften werden beim Upgrade auf HDRP und/oder URP von Standard übernommen.
* Skripte, die Substance-Material ändern, funktionieren bei der Bereitstellung auf Mobilgeräten wie erwartet
* Der rote Kanal wird nicht mehr in das Alpha kopiert und das standardmäßige Alpha wird in Weiß geändert.
* Absturz beim Ändern der Zieleinstellungen in Mac
* NullReferenceException-Fehler beim Erstellen eines Unity-Materials entfernt
* Fehler beim Beenden des Wiedergabemodus nach dem Bearbeiten der Eigenschaften der Kachelung entfernt
* Aktivierung der GPU-Instanz möglich
* Materials, die &quot;Transparenz&quot; verwenden, verschwinden nicht oder werden falsch schwarz, wenn der vorhandene Wiedergabemodus vorhanden ist
* Substance-Material werden beim Aktualisieren des Plug-ins nicht im HDRP-Projekt zerstört
