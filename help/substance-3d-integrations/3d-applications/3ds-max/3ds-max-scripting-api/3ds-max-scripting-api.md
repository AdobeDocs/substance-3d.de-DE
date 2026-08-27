---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/3ds-max/3ds-max-scripting-api.html"
breadcrumb-title: ''
description: Referenzdokumentation zur Substance 3ds Max-Scripting-API zur Automatisierung von Material-Vorgängen.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > 3ds Max > 3ds MAX Scripting API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 3ds MAX Scripting API
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '895'
ht-degree: 2%

---


# 3ds MAX Scripting API

Unten finden Sie die Liste der Befehle und Eigenschaften für den Knoten Substance 2.

## Eigenschaften:

| Eigenschaft | Beschreibung | Typ |
| --- | --- | --- |
| Name | Name des Substance2-Knotens. Der Standard ist &quot;Substance2&quot; | Zeichenfolge |

## Befehle:

| Befehl | Beschreibung | Zurückgeben | Rückgabetyp: | Parameter |
| --- | --- | --- | --- | --- |
| getCurrentPackageName | Rufen Sie den Basisdateinamen des geladenen Pakets ab (im Knoten &quot;Graf&quot; geladene sbsar-Dateien). | Der Dateiname (ohne das Präfixverzeichnis) des geladenen Pakets (sbsar-Datei) | Zeichenfolge |  |
| getCurrentGraphName | Den Namen des aktuellen Grafen abrufen | Identifizierung der aktuellen Grapheninstanz | Zeichenfolge |  |
| getOutputsNamesFromCurrentGraph | Liste der Ausgabenamen für aktivierte Ausgaben abrufen | Tabelle mit einer Liste von Kanalnamen für aktivierte Ausgaben | Liste |  |
| getPresetIdentifiers | Liste der Vorgaben vom Substance-Graf abrufen | Tabelle mit der Liste der Zeichenfolgen-Identifizierungen für alle Vorgaben | Liste |  |
| setPackageAndGraphNames | Laden einer sbsar-Datei vom Datenträger in den Graf-Knoten | Richtig bei Erfolg, Falsch bei Fehler | Boolescher Wert | ***Zeichenfolgenparameter***: **substancePackageFilePath** Der Pfad zum Parameter &quot;sbsar-Datei auf dem Datenträger ***String&quot;***: **graphInstanceNameToSelect** Die Zeichenfolgen-Identifizierung des Grafen |
| setInputInt | Festlegen einer Ganzzahl mit einem neuen Wert |  |  | ***Ganzzahl-Parameter***: **Wert** Ganzzahl zum Festlegen des Eingabeparameters auf ***String***: **inputIdentifier** Die eindeutige Zeichenfolgen-Identifizierung der Eingabe |
| setInputFloat | Festlegen eines gleitenden Eingangs mit einem neuen Wert |  |  | ***Fließkommazahl-Parameter***: **Wert** Fließkommazahl zum Festlegen des Eingabeparameters auf ***String***: **inputIdentifier** Die eindeutige Zeichenfolgen-Identifizierung der Eingabe |
| setInputString | Festlegen einer Zeichenfolgeneingabe mit einem neuen Wert |  |  | ***Zeichenfolgenparameter***: **Wert** String-Wert, um den Input auf den ***String-Parameter festzulegen***: **inputIdentifier** Die eindeutige Zeichenfolgen-Identifizierung der Eingabe |
| setInputBool | Festlegen einer booleschen Eingabe mit einem neuen Wert |  |  | ***Boolesche Wert-Parameter:* Wert **Boolesche Wert-Wert, um den Input auf***String-Parameter festzulegen ***: **inputIdentifier** Die eindeutige Zeichenfolgen-Identifizierung der Eingabe |
| setInputVec2 | Festlegen einer Vektoreingabe mit zwei Elementen |  |  | ***Point2-Parameter:*****Wert** Max. Point2-Wert zum Festlegen des Eingangs auf den ***String-Parameter ***: **inputIdentifier** Die eindeutige Zeichenfolgen-Identifizierung der Eingabe |
| setInputVec3 | Festlegen einer Vektoreingabe mit drei Elementen |  |  | ***Point3-Parameter:* Wert **Max. Point3-Wert, um den Input auf den***-String-Parameter festzulegen ***: **inputIdentifier** Die eindeutige Zeichenfolgen-Identifizierung der Eingabe |
| setInputVec4 | Festlegen einer Vektoreingabe mit vier Elementen |  |  | ***Point4-Parameter***: **Wert** Max. Point4-Wert zum Festlegen der Eingabe auf ***String-Parameter:* inputIdentifier **Die eindeutige Zeichenfolgen-Identifizierung der Eingabe |
| setInputColor | Festlegen einer Farbeingabe mit einem neuen Wert |  |  | ***Farbparameter***: **Wert** Max. Farbwert, um die Eingabe auf ***Zeichenfolgenparameter festzulegen:* inputIdentifier **Die eindeutige Zeichenfolgenkennung der Identifizierung |
| setInputComboSelection | Aktuell ausgewählten Wert in einer Kombinationsfeldeingabe festlegen |  |  | ***Ganzzahl-Parameter***: **Wert** Index des Kombinationsfeld-Widget ***String-Parameters***: **inputIdentifier** Die eindeutige Zeichenfolgen-Identifizierung der Eingabe |
| getInputInt | Abrufen des Eingabewerts für einen Ganzzahl-Eingabetyp | Die aktuelle Ganzzahl der Eingabe | Ganzzahl | ***Zeichenfolgenparameter:* inputIdentifier **Die eindeutige Zeichenfolgenversion der Identifizierung der Eingabe |
| getInputFloat | Abrufen des Eingabewerts für einen Gleitkommaeingabetyp | Der aktuelle Gleitkommawert der Eingabe | Float | ***Zeichenfolgenparameter:* inputIdentifier **Die eindeutige Zeichenfolgenversion der Identifizierung der Eingabe |
| getInputString | Abrufen des Eingabewerts für einen Zeichenfolgeneingabetyp | Der aktuelle Zeichenfolgenwert der Eingabe | Zeichenfolge | ***Zeichenfolgenparameter:* inputIdentifier **Die eindeutige Zeichenfolgenversion der Identifizierung der Eingabe |
| getInputBool | Abrufen des Eingabewerts für einen booleschen Eingabetyp | Der aktuelle boolesche Wert der Eingabe | Boolescher Wert | ***Zeichenfolgenparameter:* inputIdentifier **Die eindeutige Zeichenfolgenversion der Identifizierung der Eingabe |
| getInputVec2 | Abrufen des Eingabewerts für einen point2-Eingabetyp | Der aktuelle max point2-Wert der Eingabe | Punkt 2 | ***Zeichenfolgenparameter:* inputIdentifier **Die eindeutige Zeichenfolgenversion der Identifizierung der Eingabe |
| getInputVec3 | Abrufen des Eingabewerts für einen point3-Eingabetyp | Der aktuelle max point3-Wert der Eingabe | Punkt 3 | ***Zeichenfolgenparameter:* inputIdentifier **Die eindeutige Zeichenfolgenversion der Identifizierung der Eingabe |
| getInputVec4 | Abrufen des Eingabewerts für einen point4-Eingabetyp | Der aktuelle max point4-Wert der Eingabe | Punkt 4 | ***Zeichenfolgenparameter:* inputIdentifier **Die eindeutige Zeichenfolgenversion der Identifizierung der Eingabe |
| getInputColor | Abrufen des Eingabewerts für einen Farbeingabetyp | Der aktuelle Wert der Eingabe als Farbe | Color | ***Zeichenfolgenparameter:* inputIdentifier **Die eindeutige Zeichenfolgenversion der Identifizierung der Eingabe |
| getInputComboSelection | Index der Kombinationsfeldauswahl nach Identifizierung abrufen | Der Index des ausgewählten Kombinationsfeldelements | Ganzzahl | ***Zeichenfolgenparameter:* inputIdentifier **Die eindeutige Zeichenfolgenversion der Identifizierung der Eingabe |
| getMaterialDependentCount | Die Anzahl der Abhängigkeiten in einem Material abrufen | Die Anzahl der abhängigen Verweise eines Materials vom Typ | Ganzzahl |  |
| ApplyValuesToSelectedPreset | Überschreibt die aktuell ausgewählte Vorgabe mit den aktuellen Eingabewerten |  |  |  |
| RemoveAllPresets | Alle Vorgaben im aktuellen Graf entfernen |  |  |  |
| CreatePreset | Erstellen einer neuen Vorgabe aus den aktuellen Eingaben |  |  | ***Zeichenfolgenparameter:* newPresetName **Anzeigename für die neue Vorgabe |
| RemoveOnePreset | Vorgabe mit dem angegebenen Namen entfernen |  |  | ***Zeichenfolgenparameter:* selectedPresetName **Name der zu entfernenden Vorgabe |
| ImportPreset | Die SBSPS-Datei in die aktuellen Vorgaben importieren |  |  | ***String-Parameter:*****filePath** String, der den Dateipfad enthält, aus dem die Vorgabe importiert werden soll |
| ExportPreset**\*veraltet** In 2.5.0 entfernen\* | Exportieren der aktuell ausgewählten Vorgabe in eine SBSPRS-Datei |  |  | ***Zeichenfolgenparameter***: **filePath**-Zeichenfolge mit dem Dateipfad zum Exportieren der Vorgabe in |
| exportPresetList | Exportieren Sie die angegebenen Vorgaben in eine einzelne Voreinstellungsdatei |  |  | ***Zeichenfolgenparameter***: **filePath**-Zeichenfolge mit dem Dateipfad zum Exportieren der Vorgaben in den ***List-Parameter***: **Vorgaben** Liste mit den Namen der zu exportierenden Vorgaben |
| BakeOutputsOfSelectedGraph | Bitmaps der ausgewählten Diagramminstanz auf der Festplatte backen |  |  | ***String-Parameter:* filePath **Das Stammpfadverzeichnis zum Schreiben des Images in den***String-Parameter ***: **imageFormatExtension** Die Dateierweiterung/das Dateiformat zum Schreiben der Bilder als |
