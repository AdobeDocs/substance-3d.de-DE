---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/3ds-max/3ds-max-plugin-release-notes/3ds-max-3-0-0-plus.html"
breadcrumb-title: ''
description: Lesen Sie die Versionshinweise für 3ds Max-Plugin der Version 3.0.0 und höher , um mehr über neue Funktionen, Verbesserungen und Fehlerbehebungen zu erfahren.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > 3ds Max > 3ds Max Plugin Release Notes > 3ds Max 3.0.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 3Ds Max 3.0.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---


# 3ds Max 3.0.0+

## 3ds Max 3.0.4

<b>hinzugefügt/aktualisiert:</b>

* Substance-Plug-in-Symbole wurden mit den neuesten Symbolen aktualisiert.
* Neue Unterstützung für das Senden und Empfangen von Vorgaben mit Connector im Plug-in.
* Integrierter Menü-Manager aus dem Benachrichtigungsparameter, um die Verwendung der Kernschnittstelle zu ersetzen.

<b>Fest:</b>

* Es wurde ein Problem behoben, durch das Substance 2-Materialien möglicherweise nicht in der IR/Produktion mit Corona gerendert werden konnten, wenn der Slate Material Editor geöffnet ist und die Substance2-Texturmap ausgewählt ist.
* Es wurde ein Problem behoben, durch das Sampler Connector-Updates neue Substance2-Knoten erstellten, anstatt vorhandene Knoten zu aktualisieren.
* Es wurde ein Absturzproblem im 3ds Max-Plugin beim Hinzufügen eines Substance2-Knotens behoben und sichergestellt, dass bei der Verwendung von Batch Import zum Laden von .sbsar-Dateien der Skripteditor nicht mehr geöffnet wird.
* Es wurde ein Problem behoben, bei dem das 3DSMax 2025-Plug-in aufgrund einer inkompatiblen DLL-Datei nicht geladen werden konnte, wenn das MSI-Installationsprogramm verwendet wurde.

## 3ds Max 3.0.2

<b>hinzugefügt/aktualisiert:</b>

* Standardisierte Symbolverwaltung im Substance-Plugin durch Einbinden aller vorhandenen Symbole in qrc- und rcc-Dateien, Anpassung an die von Autodesk bevorzugten Methoden und Sicherstellung eines konsistenten Ladens im SBSAR-Grafikbedienfeld.
* Die Reaktionsfähigkeit des Substance-Einstellungsfensters im Plug-in wurde verbessert, um sicherzustellen, dass Eingabefelder und ihre Beschreibungen beim Anpassen der Fenstergröße korrekt passen.
* Das Substance-Plugin ist jetzt mit Corona 11 kompatibel.

<b>Fest:</b>

* Es wurde ein Problem behoben, bei dem die Glanzfarbe- und Glanzrauhigkeit in V-Ray-Materialien nicht automatisch verbunden wurde. Jetzt werden beide Eigenschaften automatisch verknüpft, wenn ein Workflow in V-Ray und Arnold erstellt wird.
* Es wurde ein Problem mit der Benutzeroberfläche im Plug-in behoben, bei dem beim Anpassen der Einstellung &quot;CPU-Kerngrenzwert&quot; fälschlicherweise zweistellige Werte angezeigt wurden, wenn der gespeicherte Wert eine einstellige Zahl war.
* Es wurde ein Rendering-Fehler in der Konsole für das 3ds Max-Plugin v3.0.0 im Zusammenhang mit der Substance-Kompatibilitätsfunktion behoben. Substance-Knoten, die mit dem Menü &quot;Substance-Batch-Import&quot; erstellt wurden, werden nun wie erwartet gerendert.
