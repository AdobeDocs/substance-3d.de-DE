---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/maya/maya-plugin-release-notes/maya-2-1-0.html"
breadcrumb-title: ''
description: Lesen Sie die Versionshinweise für Maya-Plugin Version 2.1.0 , um mehr über neue Funktionen, Verbesserungen und Fehlerbehebungen zu erfahren.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Maya > Maya Plugin Release Notes > Maya 2.1.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Mai 2.1.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '357'
ht-degree: 0%

---


# Mai 2.1.0

Substance in Maya 2.1.0 Changelog

* Gesicherte Kompatibilität mit Python 3
* Substance Engine aktualisiert auf Version 7.2.9
* Fehler mit in Konflikt stehenden Namen globaler Mel-Variablen beim Anwenden eines Workflows behoben
* Redshift-Arbeitsablauf setzt Fresnel jetzt auf Metallität
* Neue Plugin-Datei hinzugefügt, substanceLink, die Interoperabilität mit anderen Substance-Programmen und dem Substance Launcher behandelt
* Beim Öffnen der Substance Source wird jetzt der Substance Launcher zur Registerkarte Source (Quelle) geöffnet, wenn das substanzielle Link-Plugin geladen wird.
* Das substancelink-Plugin ermöglicht es dem Launcher, beim Hinzufügen der Benutzeroberfläche Substance Source-Materials an die Maya-Integration zu senden
* Skriptbefehle wurden hinzugefügt, um interne Bibliotheksversionen abzurufen und den Substance Launcher auf der Quellseite zu öffnen
* Website-Links sind jetzt für [substance3d.com](http://substance3d.com) anstelle von [allegorithmic.com](http://allegorithmic.com) geöffnet.
* Beim Öffnen einer Webseite öffnen Dokumentations- und Quelllinks jetzt den vom Benutzer festgelegten Standardbrowser
* Unter Windows wird der Internet Explorer nicht mehr geöffnet
* Neuer Link im Regal und Menü zum Substance share hinzugefügt
* Neue Befehle zum Abfragen der Substance Linker-Version und des Hashs hinzugefügt
* In Maya LT wurde die Version aus dem Menü &quot;Einstellungen&quot; entfernt
* Das Menü &quot;Info&quot; wird nicht mehr in PySide2 und Python geschrieben, sondern in nativem Code, der stattdessen Qt verwendet. Es ist jetzt in Maya LT verfügbar, wo es vorher nicht war.
* Das Info-Menü enthält unterschiedliche Diagnoseinformationen. Es zeigt jetzt den Git-Hash an, der der Änderung in der Quellcodeverwaltung entspricht.
* Das Info-Menü, das in die Zwischenablage kopiert wird, enthält jetzt auch diesen Git-Hash, zusammen mit der Version von Maya, für die das Plug-In erstellt wurde.
* Die Lizenzen im Info-Fenster werden jetzt als Textdatei geöffnet
* Neue Unterstützung für Mai 2017
* Der Workflowskriptgenerator gibt keine Zeichenfolgen mehr für das Element &quot;ordering&quot; aus. Alle vorhandenen Arbeitsabläufe werden ordnungsgemäß verarbeitet.

Hinzugefügte Skriptbefehle:\
substcemaya:\
\* substanceUtilityGetLinkerVersion\
\* substanceUtilityGetLinkerHash\
\* substanceUiOpenAboutWindow\
\* substanceUiOpenSourceWebsite\
\* substanceUiOpenDocumentation\
\* substanceUiOpenShareWebsite

matericelink:\
\* substanceLinkGetLinkVersion\
\* substanceLinkGetPortalCliVersion\
\* substanceLinkOpenLauncher

Diese Version wird für Mai 2017, 2018, 2019 und 2020 unter Windows veröffentlicht,\
Linux und Mac OS. Es wird auch für Maya LT 2018, 2019 und 2020 veröffentlicht am\
Windows und MacOS.
