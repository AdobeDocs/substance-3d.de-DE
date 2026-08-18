---
helpx_url: "https://helpx.adobe.com/de/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-2-5-1.html"
breadcrumb-title: ''
description: Lesen Sie die Versionshinweise für Unity-Plug-in Version 2.5.1, um mehr über neue Funktionen, Verbesserungen und Fehlerbehebungen zu erfahren.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 2.5.1
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Unity 2.5.1
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 0%

---


# Unity 2.5.1

Veröffentlicht am 21. Mai 2020

Hinzugefügt

* Unterstützung für universelle Render-Pipeline: Substance-Texturen verwenden automatisch URP-Shader und -Materialien.

Fest

* Einstellung für die maximale Auflösung des Substance-CPU-Moduls:
  * Feldname im Menü &quot;Substance-Einstellungen&quot; von &quot;Texturklemme \*\*&quot; auf &quot;Substance CPU Engine Max Resolution&quot; aktualisiert
  * Es wird eine Warnmeldung angezeigt, die darauf hinweist, dass alle Substanzmaterialien wieder importiert werden, wenn die Einstellung geändert wird.
* Unnötige Debugmeldung, die bei der Installation angezeigt wurde, wurde entfernt (&quot;TextureClamp = 4096 Unity.Engine.Debug:Log(Object)&quot;).
* HDRP-Projekt: Materialeigenschaften, die sowohl in Standard- als auch in HDRP-Materialien vorliegen, werden übertragen, wenn Pakete importiert werden, die Substance enthalten.
* Reflexions- und DRP-Masken werden erstellt und funktionieren wie erwartet, wenn ein Substance-Material aus einem Substance-Paket importiert wird, das sich in der vorherigen Unity-Version befand
* Dupliziertes Substance-Material hat die gewünschte Farbe und ist bei Verwendung der Duplikatfunktion nicht mehr gelb.
* Die Substance-Quelle wird nach dem Schließen und erneuten Öffnen von Unity wie erwartet geladen
* Absturz beim Importieren eines Pakets in ein HDRP-Projekt (zeitweise)
* Der Schieberegler funktioniert wie erwartet für das Substance von Materialien mit einem angezeigten Parameter, dessen Editor auf Color(Grayscale) festgelegt ist
* Absturz beim Klicken auf &quot;Vorgabe auf Standard zurücksetzen&quot; mit Substance-Graphen ohne Standardauflösung
* Absturz beim Ändern der Ausgabegröße eines Substance-Materials, wenn der Parameter für die Ausgabegröße nicht angezeigt wird
* Das Erstellen für iOS wird nicht fehlschlagen
* Skripte, die Substance-Materialien verwenden, werden beim Erstellen für Windows Standalone ausgeführt
