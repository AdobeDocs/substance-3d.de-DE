---
description: Lesen Sie die Versionshinweise für 3ds Max-Plugin der Version 3.0.0 und höher , um mehr über neue Funktionen, Verbesserungen und Fehlerbehebungen zu erfahren.
title: 3Ds Max 3.1.0+
source-git-commit: 28a9d8cf7a4eed4163f99e8158c9cb8f9da88302
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 0%
---

# 3ds Max 3.1.0+

## 3ds Max 3.1.1

**Freigabedatum:** 18. November 2026

**Kompatibel mit:** 3ds Max 2025 und höher

### Hinzugefügt/aktualisiert

* Substance Engine-Update (9.6.1.) einschließlich Sicherheitskorrekturen
* OpenPBR-Unterstützung für 3ds Max 2025, 2026 und 2027 (Arnold und V-Ray)

### Bekannte Einschränkungen

* Emissionsgewicht: Der Parameter &quot;emission_weight&quot; ist nicht Teil der Spezifikation für OpenPBR 1.1 und wird nicht automatisch angeschlossen. Stellen Sie nach Anwenden des Workflows den Wert Emissionsgewicht im Knoten OpenPBR manuell ein, wenn Ihr Material Emissionen verwendet.
* Unterschiede zwischen den Renderern: Einige Variationen zwischen der Material-Vorschau in Substance 3D Designer und dem gerenderten Ergebnis in Arnold oder V-Ray sind auf Unterschiede in der Implementierung der OpenPBR-Spezifikation durch jeden Renderer zurückzuführen und werden durch die Konvergenz der Implementierungen verbessert.
* SBSAR-Dateien, die aus Substance 3D Painter 12.2.0 exportiert wurden. oder eine frühere Version stellt möglicherweise keine richtige Verbindung her, wenn ein OpenPBR-Arbeitsablauf verwendet wird

## 3ds Max 3.1.0

**Freigabedatum:** 18. November 2026

**Kompatibel mit:** 3ds Max 2024

### Hinzugefügt/aktualisiert

* Substance Engine-Update (9.6.1.) einschließlich Sicherheitskorrekturen
