---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/blender/release-notes/add-on-0-9-3/add-on-2-0-0-plus.html"
breadcrumb-title: ''
description: Lesen Sie die Versionshinweise für das Blender-Add-on Version 2.0.0 und höher , um mehr über die neuen Funktionen und Verbesserungen zu erfahren.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Blender > Release Notes > Add-on 2.0.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Add-on 2.0.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '738'
ht-degree: 0%

---


# Add-on 2.0.0+

## Add-on 2.2

<b>Hinzugefügt:</b>

* Unterstützung für Octane-Renderer
* Erste Unterstützung für Redshift
* Erste Unterstützung für Renderman

<b>Aktualisiert:</b>

* Upgrade auf die neueste Version von Connector
* Es wurde eine Funktion zum Empfangen von Vorgaben über den Connector hinzugefügt.
* Verbesserte Funktion für die Importvorgabe: Jetzt fügen alle Instanzen eines SBSAR, die das Material enthalten, die Vorgabe hinzu
* Standardisierte Connector-Funktionen

<b>Fest:</b>

* Beharrungsfehler, bei dem das Eingabebild nach dem Speichern der Mischdatei nicht funktionierte
* Problem mit Shader-Netzwerk funktioniert beim Aktualisieren der Shader-Vorgabe nicht
* Falsche URL in der Schaltfläche &quot;Plug-in herunterladen&quot;
* Umgekehrte Kachelung in Octane
* Nicht funktionierende Eingabewerte mit Renderern von Drittanbietern
* Problem, bei dem der Parameter für den Gleitkommaeingabewert nicht erstellt wurde
* Renderman-Farbräume funktionieren nicht richtig
* Shader-Vorgaben werden nicht nach verfügbarem Renderer gefiltert

## Add-on 2.1.1

Dieses Update enthält Unterstützung für Blender 4.0+ und mehrere neue Funktionen in den Add-on-Voreinstellungen. Wir haben auch Unterstützung für Substance Connector hinzugefügt, um Daten nahtlos zwischen Substance 3D Sampler und Blender (Senden an) zu übertragen, und einige Fehler behoben. Die detaillierten Versionshinweise finden Sie weiter unten.

<b>hinzugefügt/aktualisiert:</b>

* Substance Connector-Funktionalität hinzugefügt (unterstützt SBSAR-Dateien und USD-Dateien).
* Unterstützung für Blender 4.0 und höher.
* Unterstützung für SRE Version 2.1.0.
* In den Add-on-Voreinstellungen:
  * Möglichkeit, den Installationspfad für Substance-Integrationstools auszuwählen.
  * Schaltfläche zum Zurücksetzen der Integrationstools auf den Standardpfad.
  * Schaltfläche zum Öffnen des Ordners Integrationstools.
  * Hinzugefügter Typ zum Zuweisen von Material (Einfügen: als Hauptmaterial festlegen, Anfügen: am Ende der Liste).
  * Es wurde ein Kontrollkästchen hinzugefügt, um das Standardverhalten der Eingabegruppen (reduziert/erweitert) auszuwählen.
  * Es wurde ein Kontrollkästchen hinzugefügt, um das Standardverhalten der einzigen Eigenschaft zum Aktualisieren von Texturen auszuwählen.
  * Starten Sie die Substance Remote Engine automatisch, wenn Sie Blender öffnen (wichtig, dass Sie diese Option aktivieren, wenn Sie Connector verwenden).
* In Addon:
  * Hinzugefügt Nur Texturen aktualisieren (ermöglicht das Ändern der Parameter, ohne das Knotendiagramm neu zu erstellen).
  * Es wurden Schaltflächen zum Erweitern aller Gruppen und zum Reduzieren aller Gruppen hinzugefügt.
  * Eingabebildgruppe hinzugefügt, um alle Eingabebilder zu gruppieren, wenn sie in einem SBSAR benötigt werden.
  * Parametereingaben werden jetzt in derselben Reihenfolge wie in Designer angezeigt.
  * Eine Miniaturvorschau für jedes Substance-Material wurde hinzugefügt.

<b>Fest:</b>

* Fehler in einer leeren allgemeinen Eingabegruppe behoben.

<b>Bekannte Probleme:</b>

* Die Funktion zur automatischen Auswahl von SBSAR bei der Auswahl eines Objekts funktioniert derzeit nicht, daher ist sie deaktiviert.

## Add-on 2.0.0

Das Substance 3D Add-on 2.0 markiert ein transformatives Update für Blender-Benutzer mit einer komplett überarbeiteten Plug-in-Architektur. Dieses neue Design konzentriert sich auf nahtlose Integration, verbesserte Leistung und ein flexibles Fundament für zukünftige Erweiterungen. Es handelt sich nicht nur um ein Upgrade, sondern um eine Neuinterpretation der Handhabung von Substance-Materialien in Blender, die den wachsenden Anforderungen von 3D-Profis gerecht wird.

<b>Highlights von Version 2.0:</b>

* Umgestaltete Architektur - verbesserte Plug-in-Struktur für verbesserte Leistung und Integration
* Unterstützung zukünftiger Erweiterungen - das Update legt die Grundlage für das einfache Hinzufügen zukünftiger Funktionen
* Größere Kompatibilität - vollständig kompatibel mit den Blender-Versionen 3.0 und höher, einschließlich Unterstützung für Mac-Anwender

<b>hinzugefügt/aktualisiert:</b>

* [SRE] Unterstützung der Substance Engine-Auswahl (GPU ist der Standard)
* [SRE] Neue Bildformate zum Exportieren der Texturen
* [SRE] Auswahl der Bittiefe für jeden Kartentyp
* [BLD] Unterstützung für Wertausgaben
* [BLD] Unterstützung für Zeichenfolgeneingabe
* [SRE] Option zur Auswahl des temporären Standardordners für das Bildexportziel hinzugefügt

<b>Fest:</b>

* [SRE] Gesamtleistungssteigerung
* [BLD] Kommunikationsprobleme zwischen den Integrationstools und Blender wurden behoben
* [BLD] Integration Tools können nicht installiert/gestartet werden
* [BLD] Integrationstools können beim Schließen von Blender nicht beendet werden
* [BLD] Material wird nicht aktualisiert, wenn der Dateityp einer Karte geändert wird
* [SRE] Alle Karten der Materialien werden ständig exportiert.
* [SRE] Integrationstools exportieren Normalmaps mit Treppenstufen
* [SRE] Das Laden des Substance wird nie abgeschlossen.
* [SRE] Szeneneinheiten werden nicht an die Physische Größe angepasst.
* [BLD] In Blender generierte Vorgaben funktionieren nicht mit anderen Integrationen
* [BLD] Material wird in Zyklen nicht aktualisiert
* [BLD] Weiche und harte Grenzen der Eingaben werden ignoriert
* [BLD] Farbintensität wird beim Anpassen eines Parameters nicht korrekt aktualisiert
* [SRE] Deinstallation der Integrationstools schlägt fehl
* [SRE] Wir haben das Problem behoben, dass das mehrmalige Duplizieren von Materialien einen Fehler verursacht hat.
* [SRE] Der Farbraum der Bildknoten stimmt jetzt mit den Benutzereinstellungen überein.

<b>Bekannte Probleme:</b>

* Bei Verwendung von Blender 4.0 und höher sind die Sockel nach mehrfacher Aktivierung und Deaktivierung nicht in der richtigen Reihenfolge
* Strg+Z zum Rückgängigmachen von Änderungen kann zu Fehlern führen
* Das Laden einer leeren Datei oder eines Ordners anstelle einer .sbsar-Datei kann das Plug-in beschädigen
* Unterstützung für den Headless-Modus von Blender
