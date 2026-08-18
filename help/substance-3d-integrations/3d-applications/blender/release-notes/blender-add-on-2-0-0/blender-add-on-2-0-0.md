---
helpx_url: "https://helpx.adobe.com/de/substance-3d-integrations/3d-applications/blender/release-notes/blender-add-on-2-0-0.html"
breadcrumb-title: ''
description: Lesen Sie die Versionshinweise für das Blender-Add-on Version 2.0.0, um mehr über neue Funktionen, Verbesserungen und Fehlerbehebungen zu erfahren.
helpx_creative_field: ""
helpx_description: Substance 3D Integrations
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Add-on 2.0.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---


# Add-on 2.0.0

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
