---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/sharing-sbsar-files-between-projects.html"
breadcrumb-title: ''
description: Teilen Sie Substance SBSAR-Dateien zwischen Unity-Projekten, während Sie Parameteranpassungen mithilfe von Vorgabedateien beibehalten.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity >Sharing sbsar Files Between Projects
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Freigeben von Unterfensterdateien zwischen Projekten
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 0%

---


# Freigeben von Unterfensterdateien zwischen Projekten

Es ist möglich, .sbsar-Dateien zwischen Projekten und Computern auszutauschen und dabei die gleichen Parameteranpassungen mit der Verwendung von .sbsprs-Dateien beizubehalten.

Nachdem das Material im ursprünglichen Projekt an die Einstellungen angepasst wurde, die freigegeben werden, navigieren Sie zu den Vorgabeeinstellungen im Bedienfeld &quot;Inspektor&quot;. Erstellen Sie in den Voreinstellungen eine neue Voreinstellung und benennen Sie sie. Diese neue benannte Vorgabe wird in der Liste der Vorgaben für dieses Material angezeigt. Exportieren Sie anschließend die Vorgabe, um sie lokal zu speichern.

Wenn Sie die .sbsar-Datei in einem anderen Projekt oder Computer verwenden, schließen Sie die exportierte Vorgabedatei ebenfalls ein. Nachdem der Untertitel in das Unity-Projekt importiert wurde, navigieren Sie zu den Vorgabeeinstellungen und wählen Sie die Importoption aus. Wählen Sie die Vorgabedatei aus dem vorherigen Schritt aus und importieren Sie sie. Eine Vorgabe mit den Einstellungen aus dem vorherigen Projekt sollte der Vorgabenliste hinzugefügt werden.

Wiederholen Sie diesen Vorgang für alle Materialien, die gemeinsam verwendet werden.
