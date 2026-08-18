---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/maya/maya-plugin-release-notes/maya-2-2-1.html"
breadcrumb-title: ''
description: Lesen Sie die Versionshinweise für Maya-Plugin-Version 2.2.1, um mehr über neue Funktionen, Verbesserungen und Fehlerbehebungen zu erfahren.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Maya > Maya Plugin Release Notes > Maya 2.2.1
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Mai 2.2.1
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '226'
ht-degree: 0%

---


# Mai 2.2.1

Version Mai 2.2.1:

* Substance Engine auf 8.3.0 aktualisieren
* Native Unterstützung für Arnold hinzufügen, sodass kein Cache auf der Festplatte erforderlich ist
* Dies kann verwendet werden, nachdem Sie Rendering-Erweiterungen in den Einstellungen aktiviert und Maya neu gestartet haben.
* Die unterstützten Versionen sind:
* Mai 2017 - MtoA 3.1.0/Arnold 5.2.0
* Maya 2018 - MtoA 4.0.0/Arnold 6.0.0, MtoA 4.2.0/Arnold 6.2.0
* Maya 2019 - MtoA 4.0.0/Arnold 6.0.0, MtoA 4.2.0/Arnold 6.2.0, MtoA 5.0.0/Arnold 7.0.0
* Maya 2020 - MtoA 4.0.0/Arnold 6.0.0, MtoA 4.2.0/Arnold 6.2.0, MtoA 5.0.0/Arnold 7.0.0
* Maya 2022 - MtoA 4.2.1/Arnold 6.2.0, MtoA 5.0.0/Arnold 7.0.0
* Installationsverzeichnis unter Windows und MacOS aktualisiert
* Binärdateien unter MacOS/Windows werden jetzt mit Adobe-Zertifikaten signiert
* Kanalschalter sind jetzt ausgeblendet, wenn der Autor des SBSAR entweder Allegorithmic oder Adobe ist, anstelle von Allegorithmic
* Neue Workflow-Benutzeroberfläche mit zusätzlichen Funktionen zum Duplizieren, Überschreiben, Umbenennen und Löschen von Workflows hinzugefügt

Die folgenden neuen Skriptbefehle wurden hinzugefügt:

Substcemaya

substanceGetEnableRenderingExtensions

substanceSetEnableRenderingExtensions

substance.workflow.py

substanceWorkflowIsReadOnly

substanceWorkflowRenameWorkflow

substanceWorkflowDuplicateWorkflow

substanceWorkflowOverwriteWorkflow

substanceWorkflowRemoveWorkflow

Fehlerbehebungen:

* Fehler beim Öffnen des Dialogfelds &quot;Einstellungen&quot; beheben
* Workflow-Funktionen schlagen nicht mehr fehl, wenn ein pyc generiert wurde

Diese Version wird für Maya 2017, 2018, 2019, 2020 und 2022 unter Linux, MacOS und Windows und Maya LT 2018, 2019 und 2020 unter MacOS und Windows veröffentlicht.
