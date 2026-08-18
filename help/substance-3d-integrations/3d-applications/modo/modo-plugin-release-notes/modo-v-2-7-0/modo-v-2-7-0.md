---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/modo/modo-plugin-release-notes/modo-v-2-7-0.html"
breadcrumb-title: ''
description: Lesen Sie die Versionshinweise für MODO Plugin Version 2.7.0, um mehr über neue Funktionen, Verbesserungen und Fehlerbehebungen zu erfahren.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > MODO > Modo Plugin Release Notes > Modo v. 2.7.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Modo v. 2.7.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 0%

---


# Modo v. 2.7.0

* Zahlreiche Fehlerbehebungen für Abstürze
* 32-Bit-Gleitkommaunterstützung
* 4k Texturen in der CPU Engine und 8k Texturen in der GPU Engine
* neues LPK-Format für die Plugin-Version
* Neues Kit-Menü für das Substance-Plugin
* glTF / Principled shader Unterstützung für MODO 12.0
* Relativer Pfad für Substance-Dateien hinzugefügt
* Linux-Unterstützung
* Neue Benutzeroberfläche zum Laden und Speichern von Vorgaben
* Eingebettete Vorgaben werden aus Designer geladen
* Warnfeld zum Entfernen des GPU-Speichers
* Bearbeitete voreingestellte Lade-/Speicherbefehle

  Die neuen verfügbaren Befehle sind:

  **substance.getsbsname** Konvertieren des Bezeichners eines Substanzobjekts in seinen internen Namen

  Alle diese erwarten einen korrekten internen Namen, der von substance.getsbsname erworben wurde:

  **substance.setpreset** Legt eine aktuelle Vorgabe für den Substance fest **substance.getpresetindex** Ruft den aktuellen Vorgabeindex **substance.getpresetat** Gibt den Zeichenfolgennamen einer Vorgabe für eine gegebene **indexsubstanz zurück.getpresetcount** Gibt die Anzahl der Vorgaben zurück, die eine Substance hat **substance.savepresetfile** Speichert eine Vorgabe der aktuellen Konfiguration in dem angegebenen Dateipfad **substance.loadetfile** Lädt eine Vorgabe der Substance unter Angabe eines Dateipfads

  UI-Befehle:

  **substance.loadpresetui** UI-Befehl zum Laden einer Vorgabe **substance.savepresetui** UI-Befehl zum Speichern einer Vorgabe **substance.selectpresetui** UI-Befehl zum Festlegen der Vorgabe
