---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-2-4-4.html"
breadcrumb-title: ''
description: Lesen Sie die Versionshinweise für Unity-Plug-in Version 2.4.4 , um mehr über neue Funktionen, Verbesserungen und Fehlerbehebungen zu erfahren.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 2.4.4
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Einheit 2.4.4
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 0%

---


# Einheit 2.4.4

Veröffentlicht im Februar 2020

* Hinzugefügt: Geeignete Unterstützung für 2019.3: Unity API-Änderungen wurden behoben, die das skriptfähige Objekt des Substance-Plugins beschädigten. Objekte wurden überarbeitet, um mit API-Updates für 2019.3 zu arbeiten. Fest - Bei Verwendung von benutzerdefiniertem Material wird das Material beim Beenden des Spiels schwarz
* Fest - Absturz, wenn die Funktion Duplicate() in einem Skript verwendet wird, dann die Wiedergabe startet und beendet wird.
* Fest - Materialkachelung, Einstellungen und Shader-Zurücksetzung in 2019.3
* Fest - HDRP Material Shader aktualisiert keine Parameteränderungen
* Fest - HDRP-Maskenzuordnung wird nicht aktualisiert
* Fest - Zeichenfolgenparameter für Duplicate-Funktion hinzufügen
* Fest - Behebung der Linux-Unterstützung in der neuesten Unity Stable
* Behoben - Problem, dass Bitcode für iOS deaktiviert werden muss

Bekannte Probleme:

* Durch das Umbenennen des HDRP-Elements generiert das Plug-in keine Maskenzuordnung.
* Bei Verwendung des Substance-Plug-ins in einem HDRP-Projekt werden Graustufen-Texturen bei Verwendung der Raw-Komprimierung auf Alpha8 festgelegt.
* GameObjects wird im Wiedergabemodus deaktiviert.
* Wenn Sie im Wiedergabemodus auf &quot;Mip-Maps generieren&quot; in einem Substance-Diagramm klicken und dann die Parameter ändern, entsteht ein unendlicher Hänger.
