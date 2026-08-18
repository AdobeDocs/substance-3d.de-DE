---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/3ds-max/3ds-max-plugin-release-notes/3ds-max-2-3-1.html"
breadcrumb-title: ''
description: Lesen Sie die Versionshinweise für das 3ds Max-Plugin Version 2.3.1 , um mehr über neue Funktionen, Verbesserungen und Fehlerbehebungen zu erfahren.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > 3ds Max > 3ds Max Plugin Release Notes > 3ds Max 2.3.1
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 3ds Max 2.3.1
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 0%

---


# 3ds Max 2.3.1

Veröffentlicht am 13. Februar 2020

Das Plug-in wird jetzt außerhalb des 3ds Max-Verzeichnisses unter C:\ProgramData\Autodesk\ApplicationPlugins\SubstanceIn3dsMax installiert. Es sollte jetzt überall funktionieren, wo 3ds Max aufgefordert wird, nach Plug-ins zu suchen, also sollte es jetzt auf einem Netzlaufwerk installiert funktionieren, usw.\
Beachten Sie, dass der Wechsel zum Applikations-Plug-in und die Änderung des Installationsverzeichnisses dazu führen, dass ein Upgrade von Version 2.1.1 und früher nicht ordnungsgemäß funktioniert. Diese sollten für 3ds Max 2018 und 2019 manuell entfernt werden. Die Version 2.2.0 sollte korrekt aktualisiert werden.\
Für einige der Probleme, die in dieser Version nicht behoben werden, ist in Kürze ein weiteres Problem geplant, um diese und andere Probleme, die auftreten können, zu beheben.

Diese Version wird derzeit für 3ds Max 2018, 2019, 2020 und 2021 veröffentlicht.

* &quot;Sbsar laden&quot; sucht jetzt zuerst im Ordner &quot;Projektbilder&quot;
* Das Dialogfeld &quot;Renderer-Kompatibilität&quot; wird jetzt nur für den Renderer &quot;VRay RT&quot; und &quot;VUE File&quot; angezeigt
* Drag &amp; Drop für den Slate Material Editor deaktiviert, um Probleme mit Max. Stapel zu entfernen
* Das Dialogfeld &quot;Rendern&quot; wird nicht mehr im Modus &quot;3ds Max, stumm&quot; angezeigt
* Kleinere Python-Skripte sind jetzt mit Python 3 kompatibel
* Unterstützung für den Substance Launcher hinzugefügt, um Substance Source-Assets an 3ds Max zu senden. Dies erfordert Änderungen am Launcher, aber die Unterstützung für das Plug-in wird vorhanden sein, da die Funktion hinzugefügt wird.
* Das Skript für den Redshift-Renderer verwendet jetzt die in Redshift 2.6.24 festgelegten neuen Knotennamen
* Max stürzt nicht mehr ab, wenn dem Substance2 SubstanceFilePath ein leerer Pfad zugewiesen wird
* Namenskollision des SubstanceOutput-Typs mit dem alten Plug-in entfernen
* SubstanceOutput-Klasse in Substance2Output umbenannt
* Substance Menu Manager-Klasse wurde in Substance2MenuManager umbenannt
* Paramblock-IDs werden jetzt beim Öffnen einer Szene gewaltsam gelöscht, sodass Kollisionen zwischen Szenendateien entfernt werden. Dadurch sollten Probleme mit ungültigen Parameterblöcken beim Laden behoben werden, wenn zwischen Szenen gewechselt wird. Beim Importieren können weiterhin Probleme auftreten, da dies komplexere Änderungen erfordert
* Das Plug-in wird jetzt außerhalb von 3ds Max installiert. Alle Pfade wurden von der Ladeposition aus in relative Pfade geändert.
* Das Plug-in verwendet jetzt das Autodesk Application Plug-in-System.
