---
helpx_url: "https://helpx.adobe.com/de/substance-3d-integrations/game-engines/unity.html"
breadcrumb-title: ''
description: Importieren und verwenden Sie Substance-Materialien in Unity Game Engine mit nativer Plug-in-Unterstützung und Laufzeitparametersteuerung.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Einheit
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '743'
ht-degree: 0%

---


# Einheit

![](../../assets/unity.png)

>[!NOTE]
>
> **Von Unity unterstützte Versionen**
> 
> Das Adobe Substance 3D Plugin für Unity Version 3.0.0 unterstützt derzeit Unity 2020.3.27x und höher. Sie kann aus dem [Unity Asset Store](https://assetstore.unity.com/packages/tools/utilities/substance-3d-for-unity-beta-213208) heruntergeladen werden.

>[!WARNING]
>
> Überprüfen Sie vor dem Aktualisieren oder Verwenden des Plug-Ins die [-Aktualisierungsprojektseite](https://helpx.adobe.com/de/substance-3d/unlisted/documentation/integrations/upgrading-projects-182256244.html).

>[!WARNING]
>
> Überprüfen Sie die Seite [Optimierungsrichtlinien](../../game-engines/unity/optimization-guidelines/optimization-guidelines.md), bevor Sie benutzerdefinierte Substance-Material erstellen.

## Inhaltsverzeichnis

* [Unity-Versionshinweise](https://helpx.adobe.com/de/substance-3d/unlisted/documentation/integrations/beta-release-information-170460277.html) — Neue Funktionen auf der Substance in Unity-Plug-in nach Versionen
* [Herunterladen des Substance 3D-Plug-ins in Unity](../../game-engines/unity/downloading-plugin-unity/downloading-substance-3d-plugin-in-unity.md) — Die Adobe Substance 3D für Unity ist im Unity Asset Store unter https://assetstore.unity.com/packages/tools/utilities/substance-in-unity-110555 verfügbar.
* [Unity-Plug-in - Übersicht](../../game-engines/unity/unity-plugin-overview/unity-plugin-overview.md)
* [Unity Preferences](../../game-engines/unity/unity-preferences/unity-preferences.md) — Im Substance-Einstellungsfenster können Sie benutzerdefinierte Optionen für das Plug-in festlegen.
* [Optimierungsrichtlinien](../../game-engines/unity/optimization-guidelines/optimization-guidelines.md) — Wenn Sie eigene benutzerdefinierte Substance-Material erstellen, überprüfen Sie unbedingt die folgenden Optimierungsrichtlinien.
* [Aktualisieren von Projekten/Bekannte Probleme](https://helpx.adobe.com/de/substance-3d/unlisted/documentation/integrations/upgrading-projects-182256244.html) — Bekannte Probleme mit dem Substance in Unity-Plug-in
* [Verwalten von Substance-Grafen](https://helpx.adobe.com/de/substance-3d/unlisted/documentation/integrations/managing-and-navigating-substance-graphs-170459636.html) — Sie können neue Material auf der Grundlage des Substance-Materials mithilfe des Substance-Grafen-Managers (SGM) erstellen
* [Parameter ändern](../../game-engines/unity/changing-parameters/changing-parameters.md) — Auf Parameter für das Substance-Material kann über das Substance-Grafen-Objekt (SGO) zugegriffen werden.
* [Generierte Texturen (Packing)](../../game-engines/unity/generated-textures-pac/generated-textures-packing.md) — Die generierten Texturen zeigen die Ausgaben von der Substance an, die vom Substance Engine zum Erstellen von Texturen berechnet werden.
* [Farbraum wird gerendert](../../game-engines/unity/rendering-color-space/rendering-color-space.md) — Um die besten Ergebnisse zu erzielen, sollten Sie den Farbraum in den Unity Player-Einstellungen auf linear einstellen.
* [Verwenden von Bildeingaben](../../game-engines/unity/using-image-inputs/using-image-inputs.md)
* [Veröffentlichen für Mobilgeräte](../../game-engines/unity/publishing-for-mobile/publishing-for-mobile.md) — Richtlinien für die Veröffentlichung auf mobilen Plattformen
* [Substance 3D for Unity Scripting](../../game-engines/unity/3d-for-unity-scripting/substance-3d-for-unity-scripting.md) — Mithilfe der Substance-API können Sie Skripte schreiben, um Substance-Parameter zur Laufzeit zu aktualisieren und zu ändern.
* [Skripterstellung in Unity (veraltet)](https://helpx.adobe.com/de/substance-3d/unlisted/documentation/integrations/scripting-in-unity-170459644.html) — Mithilfe der Substance-API können Sie Skripte schreiben, um Substance-Parameter zur Laufzeit zu aktualisieren und zu ändern.
* [Nutzung der Substance 3D Assets-Bibliothek](https://helpx.adobe.com/de/substance-3d/unlisted/documentation/integrations/substance-3d-assets-library-225970070.html)
* [Entfernen des Substance-Zusatzmoduls](../../game-engines/unity/removing-plugin/removing-substance-plugin.md)
* [Substance 3D in Tutorials](../../game-engines/unity/3d-in-unity-tutorials/substance-3d-in-unity-tutorials.md)
* [Physische Größe in der Einheit](../../game-engines/unity/physical-size-in-unity/physical-size-in-unity.md)
* [Freigeben von Unterfensterdateien zwischen Projekten](https://helpx.adobe.com/sharing-sbsar-files-between-projects.html) [&#128279;](../../game-engines/unity/sharing-sbsar-files-bet/sharing-sbsar-files-between-projects.md)

**[FORMULAR GEFUNDEN - ERFORDERLICHE REGELN]**

>[!WARNING]
>
> Überprüfen Sie vor dem Aktualisieren oder Verwenden des Plug-Ins die [-Aktualisierungsprojektseite](https://helpx.adobe.com/de/substance-3d/unlisted/documentation/integrations/upgrading-projects-182256244.html).

>[!WARNING]
>
> Überprüfen Sie die Seite [Optimierungsrichtlinien](../../game-engines/unity/optimization-guidelines/optimization-guidelines.md), bevor Sie benutzerdefinierte Substance-Material erstellen.

### Inhaltsverzeichnis

* [Unity-Versionshinweise](https://helpx.adobe.com/de/substance-3d/unlisted/documentation/integrations/beta-release-information-170460277.html) — Neue Funktionen auf der Substance in Unity-Plug-in nach Versionen
* [Herunterladen des Substance 3D-Plug-ins in Unity](../../game-engines/unity/downloading-plugin-unity/downloading-substance-3d-plugin-in-unity.md) — Die Adobe Substance 3D für Unity ist im Unity Asset Store unter https://assetstore.unity.com/packages/tools/utilities/substance-in-unity-110555 verfügbar.
* [Unity-Plug-in - Übersicht](../../game-engines/unity/unity-plugin-overview/unity-plugin-overview.md)
* [Unity Preferences](../../game-engines/unity/unity-preferences/unity-preferences.md) — Im Substance-Einstellungsfenster können Sie benutzerdefinierte Optionen für das Plug-in festlegen.
* [Optimierungsrichtlinien](../../game-engines/unity/optimization-guidelines/optimization-guidelines.md) — Wenn Sie eigene benutzerdefinierte Substance-Material erstellen, überprüfen Sie unbedingt die folgenden Optimierungsrichtlinien.
* [Aktualisieren von Projekten/Bekannte Probleme](https://helpx.adobe.com/de/substance-3d/unlisted/documentation/integrations/upgrading-projects-182256244.html) — Bekannte Probleme mit dem Substance in Unity-Plug-in
* [Verwalten von Substance-Grafen](https://helpx.adobe.com/de/substance-3d/unlisted/documentation/integrations/managing-and-navigating-substance-graphs-170459636.html) — Sie können neue Material auf der Grundlage des Substance-Materials mithilfe des Substance-Grafen-Managers (SGM) erstellen
* [Parameter ändern](../../game-engines/unity/changing-parameters/changing-parameters.md) — Auf Parameter für das Substance-Material kann über das Substance-Grafen-Objekt (SGO) zugegriffen werden.
* [Generierte Texturen (Packing)](../../game-engines/unity/generated-textures-pac/generated-textures-packing.md) — Die generierten Texturen zeigen die Ausgaben von der Substance an, die vom Substance Engine zum Erstellen von Texturen berechnet werden.
* [Farbraum wird gerendert](../../game-engines/unity/rendering-color-space/rendering-color-space.md) — Um die besten Ergebnisse zu erzielen, sollten Sie den Farbraum in den Unity Player-Einstellungen auf linear einstellen.
* [Verwenden von Bildeingaben](../../game-engines/unity/using-image-inputs/using-image-inputs.md)
* [Veröffentlichen für Mobilgeräte](../../game-engines/unity/publishing-for-mobile/publishing-for-mobile.md) — Richtlinien für die Veröffentlichung auf mobilen Plattformen
* [Substance 3D for Unity Scripting](../../game-engines/unity/3d-for-unity-scripting/substance-3d-for-unity-scripting.md) — Mithilfe der Substance-API können Sie Skripte schreiben, um Substance-Parameter zur Laufzeit zu aktualisieren und zu ändern.
* [Skripterstellung in Unity (veraltet)](https://helpx.adobe.com/de/substance-3d/unlisted/documentation/integrations/scripting-in-unity-170459644.html) — Mithilfe der Substance-API können Sie Skripte schreiben, um Substance-Parameter zur Laufzeit zu aktualisieren und zu ändern.
* [Nutzung der Substance 3D Assets-Bibliothek](https://helpx.adobe.com/de/substance-3d/unlisted/documentation/integrations/substance-3d-assets-library-225970070.html)
* [Entfernen des Substance-Zusatzmoduls](../../game-engines/unity/removing-plugin/removing-substance-plugin.md)
* [Substance 3D in Tutorials](../../game-engines/unity/3d-in-unity-tutorials/substance-3d-in-unity-tutorials.md)
* [Physische Größe in der Einheit](../../game-engines/unity/physical-size-in-unity/physical-size-in-unity.md)
