---
helpx_url: "https://helpx.adobe.com/de/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-2-6-0.html"
breadcrumb-title: ''
description: Lesen Sie die Versionshinweise für Unity-Plug-in Version 2.6.0 , um mehr über neue Funktionen, Verbesserungen und Fehlerbehebungen zu erfahren.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 2.6.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Unity 2.6.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 0%

---


# Unity 2.6.0

Veröffentlicht am 7. Juni 2021

Aktualisiert/hinzugefügt:

* Neuer Arbeitsablauf für den Zugriff auf die Substance Source! Die Substance Source-Aktion greift jetzt auf die Registerkarte &quot;Quelle&quot; im Substance Launcher zu, sodass Assets direkt an Unity gesendet werden können
* Versionsinformationen für Plug-ins können in die Zwischenablage kopiert werden
* &quot;Beim Laden generieren&quot; aus den Zieleinstellungen entfernt

Problembehebungen:

* In HDRP-Projekten wird der Versatz-Modus auf den Standardwert (Tessallation) zurückgesetzt, wenn die Materialeinstellung geändert wird
* Die Auflösungsgröße wird im Inspektorfenster nicht angezeigt
* Plug-in zu Unity-Versionen 2020.2 und höher kann nicht installiert werden

Bekannte Probleme:

* Fehler &quot;Zugriff verweigert&quot; und/oder Absturz tritt auf, wenn das Plug-in von früheren Versionen 2.5.4 und früher aktualisiert wird
  * Problemumgehung: Frühere Plug-in-Versionen 2.5.4 und niedriger müssen aus den Unity-Projektversionen 2020.2 und höher deinstalliert werden, bevor die Plug-in-Version 2.6.0 installiert wird
* Texturvorschauen für Bilddateien werden im Inspektor nicht angezeigt, wenn das Substance-Plugin installiert ist
  * Die Ursache dieses Problems existiert in Unity und soll von Unity in ihren Versionen von 2021.2 (derzeit in der Beta-Version) behoben werden.
