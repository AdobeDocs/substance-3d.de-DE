---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/maya/maya-plugin-release-notes/maya-3-0-0-plus.html"
breadcrumb-title: ''
description: Lesen Sie die Versionshinweise für Maya-Plugin-Version 3.0.0 und höher , um mehr über neue Funktionen, Verbesserungen und Fehlerbehebungen zu erfahren.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > 3ds Max > 3ds Max Plugin Release Notes > Maya 3.0.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Maya 3.0.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 0%

---


# Maya 3.0.0+

## Maya 3.0.3

<b>hinzugefügt/aktualisiert:</b>

* Das Caching-System des Maya-Plugins wurde verbessert, sodass es nur einmal bei der ersten Netzwerkerstellung zwischengespeichert werden kann, wobei manuelles Recaching aktiviert ist.
* Es wurde eine Option zum Ändern des Speicherorts des Ordners &quot;substance&quot; im Maya-Plugin bereitgestellt.
* Das Workflow-Importsystem des Maya-Plug-ins wurde aktualisiert, um die Kompatibilität mit dem Update von Autodesk auf Python 3.12 sicherzustellen.
* Substance-Plug-in-Symbole wurden mit den neuesten Symbolen aktualisiert.
* Neue Unterstützung für das Senden und Empfangen von Vorgaben mithilfe von Verbindung im Plug-in.

<b>Fest:</b>

* Es wurde ein Problem behoben, bei dem das Laden/Entladen des Substance-Plug-ins für Maya einen Fehlerbildschirm und Absturz verursacht.
* Cache-Probleme wurden behoben, insbesondere indem sichergestellt wurde, dass .exr-Dateien richtig referenziert werden und das cachingbedingte Einfrieren in großen Szenen reduziert wurde.
* Es wurde ein Problem behoben, durch das die Vorschau des Materials im Beispielfenster nicht angezeigt wurde, wenn eine Sbsar-Datei im Maya-Plug-in geladen wurde.
* Es wurde ein Problem behoben, bei dem die Verbindung keine Sbsar-Dateien empfangen kann, wenn mindestens ein SBSAR bereits in Hypershade vorhanden ist.
