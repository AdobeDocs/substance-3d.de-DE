---
helpx_url: "https://helpx.adobe.com/de/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-3-0-0-plus.html"
breadcrumb-title: ''
description: Lesen Sie die Versionshinweise für Unity-Plug-ins ab Version 3.0.0, um mehr über neue Funktionen und Verbesserungen zu erfahren.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 3.0.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Unity 3.0.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 4a060ee1aaa1731c04e70d5512e3271cd63d0381
workflow-type: tm+mt
source-wordcount: '1384'
ht-degree: 0%

---


# Unity 3.0.0+

## Einheit 3.12.0

<b>hinzugefügt/aktualisiert:</b>

* Unterstützung für den Substance 3D Connector in Unity, der die SendTo-Funktion zum Senden von Elementen zwischen Substance 3D Sampler und Unity aktiviert.
* Unterstützung für das Umbenennen und erneute Veröffentlichen von .sbsar-Grafen aus Designer in Unity, um sicherzustellen, dass in Designer vorgenommene Änderungen beibehalten werden, wenn der aktualisierte Graf erneut in das Unity-Plug-in importiert wird.
* Dokumentation zum Freigeben von .sbsar-Dateien zwischen Unity-Projekten.
* Community-Beitragseite zur Unity-Plug-in-Dokumentation: https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/community-contributions.html

<b>Fest:</b>

* Ein Problem, bei dem die Miniaturansicht des Materials im Unity-Projektelementordner nach der erneuten Veröffentlichung einer sbsar-Datei nicht aktualisiert wird und das vorherige Material anstelle des aktuellen angezeigt wird.

## Unity 3.11.0

<b>hinzugefügt/aktualisiert:</b>

* Verbesserte Leistung für Projekte mit mehr als 1.000 Substance-Grafen, wodurch die Reaktionszeiten der Benutzeroberfläche beim Überprüfen von SBSAR-Dateien im Ordner &quot;Assets&quot; erheblich reduziert wurden.
* Es wurde eine Schaltfläche zum Zurücksetzen hinzugefügt, um SBSAR-Dateien auf ihren ursprünglichen Zustand zurückzusetzen, wodurch die Effizienz des Arbeitsablaufs verbessert wurde.
* Aktualisierte Dokumentation mit einer Problemumgehung für das Problem &quot;Bildeingaben gesperrt auf 8-Bit&quot;, verfügbar unter: [Substance 3D-Integrationen in Unity - Aktualisieren von Projekten und bekannten Problemen](../../../../game-engines/unity/upgrading-projects-known/upgrading-projects-known-issues.md).
* Die Dokumentation wurde aktualisiert, um den Fehler &quot;Assertion bei Ausdruck fehlgeschlagen&quot; zu beheben, der beim Navigieren zu Bedienfeldordnern in Unity aufgetreten ist: [Substance 3D-Integrationen in Unity - Aktualisieren von Projekten und bekannten Problemen](../../../../game-engines/unity/upgrading-projects-known/upgrading-projects-known-issues.md).

<b>Fest:</b>

* Es wurde ein Problem behoben, das dazu führte, dass das Plug-in auf Linux-Plattformen nicht funktionierte.
* Kompatibilitätsprobleme mit dem Unity-Plug-in in Version 2023 wurden behoben.

## Einheit 3.10.1

<b>Fest:</b>

* Es wurde ein Problem behoben, bei dem das Substance Engine aufgrund eines Problems mit sbsario.dll im Substance 3D for Unity-Plug-in nicht geladen werden konnte.

## Unity 3.10.0

<b>hinzugefügt/aktualisiert:</b>

* Der Kommentarabschnitt für die RenderInstanceAsync-API im Plug-in wurde aktualisiert.

<b>Fest:</b>

* Es wurde ein Speicherleck im C++-Code des Plug-ins behoben, wodurch eine vollständige Speicherwiederherstellung beim Löschen von Objekten sichergestellt wurde.
* Es wurde ein Problem unter Linux behoben, bei dem der Import des Unity-Plug-in-Pakets zu einer &quot;SubstanceException: Dem API-Fehler wurde ein ungültiges Argument zugewiesen, das jetzt den erfolgreichen Import von SBSAR-Dateien ermöglicht.
* Es wurde ein Problem behoben, bei dem SubstanceGraphSO.CurrentStatePreset zum Laden von Vorgaben mit einem benutzerdefinierten Editorfensterskript in Unity nicht ordnungsgemäß funktionierte. ein Korrekturskript ist jetzt auf unserer Substance-Dokumentationsseite (HelpX) verfügbar: https://experienceleague.adobe.com/de/docs/substance-3d/ecosystem/game-engines/unity/substance-3d-for-unity-scripting/substance-3d-for-unity-scripting
* Es wurde ein Fehler behoben, durch den Diagrammeigenschaften bei der Neuauswahl im Unity-Editor nicht mehr angezeigt wurden.
* Es wurde das Problem &quot;Unknown managed type referenced&quot; im Zusammenhang mit SubstanceGraphSO im Unity-Plug-in behoben, durch das die Kompatibilität und Funktionalität auf Android-Plattformen verbessert wurden, insbesondere für Unity 2022.1 und möglicherweise für alle Unity-Versionen.
* Es wurde ein Problem behoben, durch das die Auswahl &quot;NORMAL FORMAT&quot; im Abschnitt &quot;TECHNISCHE PARAMETER&quot; fälschlicherweise als Zahleneingabefeld angezeigt wurde, anstatt als erwartete Dropdown-Liste mit DirectX- und OpenGL-Optionen.

## Unity 3.9.0

<b>hinzugefügt/aktualisiert:</b>

* Sbsar-Dateien können jetzt per Drag &amp; Drop in das Projekt gezogen werden. Das .sbsar-Objekt kann wie in Unity 2022.3 erwartet auf ein Gitter angewendet werden.
* Verbesserte Dokumentation für das Plug-in.

<b>Fest:</b>

* Es wurde ein Problem behoben, bei dem das Unity-Plug-in unter Android nicht funktionierte.
* Benennungseinschränkungen im Unity-Plug-in behoben. Wenn ein Dateiname ein &quot;.&quot; enthielt, wurde die Datei vom Plug-in nicht korrekt geladen.
* Es wurde ein Problem behoben, bei dem durch Deaktivieren von &quot;Alle Ausgaben generieren&quot; die zusätzliche Textur nicht automatisch gelöscht wurde.
* Der falsche Import von SBSAR-Materialien in Unity 2021.3-Standardprojekten wurde behoben. Im Standardvorlagenprojekt können SBSAR-Materialien nun fehlerfrei in den Ordner &quot;Assets&quot; importiert und auf ein 3D-Gitter angewendet werden.
* Der falsche Import von SBSAR-Materialien in Unity 2021/2022 HDRP-Projekten wurde behoben. Im HDRP-Vorlagenprojekt können SBSAR-Materialien nun fehlerfrei in den Ordner &quot;assets&quot; importiert und auf ein 3D-Mesh angewendet werden.
* Es wurde ein Kompilierungsfehler bei der Generierung des Android-Builds zur Erstellung der APK behoben: &quot;Kompilierung fehlgeschlagen; Weitere Informationen finden Sie in der Compilerfehlerausgabe.&quot;
* Es wurde ein Problem behoben, das dazu führte, dass der Buildprojektprozess unter Windows mit Fehlern fehlschlug.
* Es wurde ein Problem behoben, das dazu führte, dass der Buildprojektprozess unter Android mit Fehlern fehlschlug: UnityEditor.BuildPlayerWindow+BuildMethodException.
* Behebung der UnityException, die beim Ändern von SubstanceGraph-Eingaben zur Laufzeit auftrat. Beim Aufrufen von SubstanceRuntimeGraph.SetTexturesResolution und SubstanceRuntimeGraph.Render() wurde SubstanceGraph zuvor veranlasst, falsche Ergebnisse zu rendern.
* Es wurde ein typografischer Fehler in SubstanceEditorTools.cs behoben.

## Unity 3.8.0

<b>hinzugefügt/aktualisiert:</b>

* Neue Unterstützung für Parameter mit bedingter Sichtbarkeit (Sichtbar, wenn-Funktion).
* Substance-Engine auf Version 9 aktualisiert.
* Die Dokumentation wurde aktualisiert, um ein Problem zu beheben, bei dem NativeGraph.InRenderWork in einem Skript für ein benutzerdefiniertes Editorfenster nicht funktioniert. Weitere Informationen finden Sie hier: [Substance 3D für Unity Scripting - Klassendokumentation](../../../../game-engines/unity/3d-for-unity-scripting/class-documentation/substanceruntime-class/substanceruntime-class.md)

<b>Fest:</b>

* Es wurde ein Problem behoben, das Normalen-Map in Android-Projekten betraf.
* Es wurde ein Fehler behoben, durch den das Ziehen eines SBSAR-Objekts in die Szene-Ansicht versehentlich dazu führte, dass die Materials aller Mouseover-Objekte durch das SBSAR-Objekt-Material überschrieben wurden.
* Es wurde ein Fehler behoben, der beim Überprüfen eines Materials, das im Laufzeitmodus als &quot;Nur Laufzeitumgebung&quot; markiert war, und beim Öffnen der Zuordnung der Ausgabe-Textur auftrat.

## Unity 3.7.0

<b>hinzugefügt/aktualisiert:</b>

* Unterstützung für eingebettete und externe Vorgaben
* Kompatibilität mit Unity 2022.2

<b>Fest:</b>

* Fehler beim Erstellen eines neuen Grafen für eine sbsar-Datei mithilfe der Schaltfläche &quot;Graf kopieren&quot;: &quot;Unerwartete rekursive Übertragung der skriptbasierten Klasse&quot;
* Erstellung zusätzlicher Material-Ordner auf Mac nach dem erneuten Öffnen eines Projekts
* SubstanceFileSO-Array wird beim Erstellen/Löschen von Grapheninstanzen nicht aktualisiert
* Beim Duplizieren eines Substance werden falsche Eingabeoptionen angezeigt
* Leere Beschriftungsfelder beim Export von .sbsprs-Dateien
* Fehler beim Export/Import von Vorgaben im Editor: EndLayoutGroup: BeginLayoutGroup muss zuerst aufgerufen werden.

<b>Entfernt:</b>

* Abschnitt &quot;Kanäle&quot; von Unity-Plug-in aufgrund fehlender Benutzerwerte

## Unity 3.6.0

<b>hinzugefügt/aktualisiert:</b>

* Die Möglichkeit, einzelne Int 4-Werte unabhängig voneinander editierbar zu machen.

<b>Fest:</b>

* Problem, bei dem Materialien beim erneuten Öffnen eines Projekts auf einen früheren Status zurückgesetzt wurden
* Beim Versuch, den Material-Graf zu ändern, wurde die Meldung &quot;Keine Graf gefunden&quot; angezeigt
* Problem, bei dem sich die Eingabewerte für den Parameter &quot;Versatz bei Drehung&quot; in der Funktion &quot;Physische Größe&quot; nicht geändert haben
* Problem, bei dem duplizierte Grapheninstanzen falsche GraphID-Werte für Eingaben hatten
* Problem, bei dem der Substance-Generator im Editor nicht ordnungsgemäß initialisiert wurde, während ein Graf mit Editorskripten (benutzerdefiniertes Editorfenster) geändert wurde
* Ein Problem, bei dem beim Exportieren einer SubstanceGraphSO.CurrentStatePreset aus einem benutzerdefinierten Editorfensterskript eine zwischengespeicherte Version des Grafen exportiert wurde
* Problem, bei dem Parameteränderungen nicht gespeichert wurden, als das Inspektorfenster gesperrt war
* Ein Problem, bei dem die manuelle Tastatureingabe im Abschnitt &quot;Positionsversatz&quot; der Optionen für die Physische Größe keine Auswirkungen auf das Material im Editor hatte
* Fehler bei der manuellen Eingabe von Parameterwerten im SBSAR-Objekt

## Unity 3.5.0

<b>hinzugefügt/aktualisiert:</b>

* Unterstützung für Benutzer, die ändern können, wie Ausgabe-Texturen dem Unity-Material zugewiesen werden
* Plug-in-Kompatibilität mit der neuesten Unity 2022.2-Version

<b>Fest:</b>

* Null-Referenzfehler, wenn Material einen Int4-Eingang haben
* Fehler bei Int4-Eingängen, der W-Wert wird Data2 anstelle von Data3 zugewiesen
* Typo im Funktionsnamen &quot;\_OcclusionStrength&quot;

## Unity 3.4.0

<b>hinzugefügt/aktualisiert:</b>

* Mit den Steuerungen unter &quot;Position&quot; wird die Textur über die Fläche im Bedienfeld &quot;Physische Größe&quot; Kamera bewogen.
* Links zum Herunterladen von Adobe Substance 3D Assets- und Substance Community-Assets in den Projekteinstellungen

## Unity 3.3.0

<b>hinzugefügt/aktualisiert:</b>

* Die Physische Größe-Funktion für HDR-Bilder, die das Anwenden und Skalieren von Materialien auf Basis ihrer realen Abmessungen ermöglicht
* Benutzeroberfläche für die GPU-Aktivierung in den Projekteinstellungen

<b>Entfernt:</b>

* GraphIDs der meisten API-Aufrufe

## Einheit 3.2.1

<b>Fest:</b>

* Das Problem beim Aktualisieren des Plug-ins von 3.0.0 und 3.1.0 auf die neueste Version.

## Unity 3.2.0

<b>hinzugefügt/aktualisiert:</b>

* Leistungsverbesserung bei der Neukompilierung von Skripten

<b>Fest:</b>

* Fehler beim Importieren von Elementen im Unity-Plug-in beim Importieren von benutzerdefinierten SBSAR-Materialien
* &quot;ArgumentException: Der Wert liegt nicht innerhalb des erwarteten Bereichs.&quot;
* &quot;ArgumentOutOfRangeException: Der Index lag außerhalb des zulässigen Bereichs.&quot;

## Unity 3.1.0

<b>hinzugefügt/aktualisiert:</b>

* 1,38-fache Leistungsverbesserung für Mac
* Das GPU-Engine auf dem Mac verwendet Metal anstelle von OpenGL

<b>Fest:</b>

* Mac-Problem, bei dem die R- und B-Kanäle der ausgegebenen Texturen gespiegelt werden

## Unity 3.0.0

<b>hinzugefügt/aktualisiert:</b>

* Unterstützung für Apple Silicon
* Neues YouTube-Tutorial zur Verwendung des Plug-ins
* Neue Skriptdokumentation

<b>Fest:</b>

* Fehler im Inspektor-Display, wenn der Zufallsgenerator-Button immer wieder gedrückt wird
* Null-Textur-Eingaben brechen Substance-Updates
* &quot;Alle Ausgaben generieren&quot;, &quot;Mip-Maps generieren&quot; und &quot;Nur Laufzeitumgebung&quot; funktionieren nicht
* Probleme mit Namespaces
* Null-Referenzfehler beim Aufrufen des Wiedergabemodus mit ausgewähltem Grafikelement
* Problem mit HDRP und URP für die neueste LTS-Version 2021.3 von Unity, wenn nur Laufzeitmaterialien verwendet werden
