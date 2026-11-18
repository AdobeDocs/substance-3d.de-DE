---
description: Lesen Sie die Versionshinweise für Maya-Plugin-Version 3.0.0 und höher , um mehr über neue Funktionen, Verbesserungen und Fehlerbehebungen zu erfahren.
title: Maya 3.0.0
source-git-commit: 28a9d8cf7a4eed4163f99e8158c9cb8f9da88302
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 0%
---

# Maya 3.1.0+

## Maya 3.1.1

**Freigabedatum:** 18. November 2026

**Kompatibel mit:** Mai 2025 und höher

### Hinzugefügt/aktualisiert

* Substance Engine-Update (9.6.1.) einschließlich Sicherheitskorrekturen
* OpenPBR-Unterstützung für Mai 2025, 2026 und 2027 (Arnold und V-Ray)

### Bekannte Einschränkungen

* Emissionsgewicht: Der Parameter &quot;emission_weight&quot; ist nicht Teil der Spezifikation für OpenPBR 1.1 und wird nicht automatisch angeschlossen. Stellen Sie nach Anwenden des Workflows den Wert Emissionsgewicht im Knoten OpenPBR manuell ein, wenn Ihr Material Emissionen verwendet.
* OpenPBR - V-Ray - Subsurface Radius Scale: Bei Verwendung des OpenPBR-V-Ray-Workflows gibt subsurface_radius_scale möglicherweise den Wert 0 zurück. Entfernen Sie in diesem Fall die Verbindung und legen Sie den Wert manuell im V-Ray-Knoten fest.
* Unterschiede zwischen den Renderern: Einige Variationen zwischen der Material-Vorschau in Substance 3D Designer und dem gerenderten Ergebnis in Arnold oder V-Ray sind auf Unterschiede in der Implementierung der OpenPBR-Spezifikation durch jeden Renderer zurückzuführen und werden durch die Konvergenz der Implementierungen verbessert.
* SBSAR-Dateien, die aus Substance 3D Painter 12.2.0 exportiert wurden. oder früher werden möglicherweise nicht ordnungsgemäß verbunden, wenn ein OpenPBR-Arbeitsablauf verwendet wird. Mai 3.1.0 Hinzugefügt/aktualisiert: Substance Engine-Update (9.6.1.) einschließlich Sicherheitskorrekturen.

## Maya 3.1.0

**Freigabedatum:** 18. November 2026

**Kompatibel mit:** Mai 2024

### Hinzugefügt/aktualisiert

* Substance Engine-Update (9.6.1.) einschließlich Sicherheitskorrekturen
