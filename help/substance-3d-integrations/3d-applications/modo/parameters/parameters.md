---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/modo/parameters.html"
breadcrumb-title: ''
description: Ändern Sie die Parameter von Substance-Materialien in MODO über das Bedienfeld "Substance-Eigenschaften", um Material anzupassen.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > MODO > Parameters
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Parameter
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 1%

---


# Parameter

Eine Substance verfügt über eine Reihe von Kernparametern. Diese Parameter sind in Substance, Ausgaben und Tweak unterteilt. Sie finden sie im Bedienfeld &quot;Substance-Eigenschaften&quot;.\
Substance aus Substance Source enthält die technischen Parameter und Kanäle. Die Kanaloptionen haben keine Auswirkungen auf MODO. Ausgaben werden über den Abschnitt &quot;Ausgaben&quot; aktiviert/deaktiviert.

![](../../../assets/parameters-4.png){width="300px"}

## Substance

Eine Substance verfügt über eine Reihe von Kernparametern, die Sie in der Kategorie &quot;Substance&quot; des Bedienfelds &quot;Substance-Eigenschaften&quot; finden.

* **Substance neu laden:** Mit diesem Parameter können Sie eine Substance neu laden. Es wurde für die Verwendung mit Substance Designer entwickelt. Wenn Sie auf einer benutzerdefinierten Substance arbeiten und ein neues Tweak oder eine Ausgabe hinzugefügt haben, können Sie die neu veröffentlichte Substance wieder in MODO laden. Die neuen Änderungen und Ausgaben werden hinzugefügt und die vorherigen Änderungen werden beibehalten.
* **Schattierung-Modus:** Mit diesem Parameter können Sie den Schattierung-Modus festlegen, der für den Substance verwendet werden soll. Principled (Standard), Unreal, Unity oder glTF.
* **Substance zurücksetzen:** Mit diesem Parameter werden die Änderungen auf die Standardeinstellungen zurückgesetzt.
* **Graf auswählen:** Sie können in der Substance-Datei auswählen, von welchem Graf ein Material erstellt werden soll.
* **Vorgabe laden:** Sie können eine Vorgabe laden, die die Substance-Tweak-Parameter konfiguriert. Vorgaben können mit Substance Player erstellt werden. Die Vorgabedatei ist ein SBSPRS-Dateityp. Nachdem Sie eine Vorgabe geladen haben, müssen Sie auf die Dropdown-Liste Vorgabe klicken und die Vorgabe auswählen, da eine SBSPR-Datei mehrere Vorgaben enthalten kann.
* **Vorgabe speichern:** Ermöglicht das Speichern einer Vorgabe.
* **Vorgabe auswählen:** Ermöglicht Ihnen die Auswahl einer eingebetteten Vorgabe in der Substance-Datei oder aus Vorgaben, die in MODO gespeichert sind.
* **Baking auf Datenträger:** Mit diesem Parameter werden die von der Substance generierten Texturen in eine Bitmapdatei Baking geführt.
* **Ausgabegröße:** Mit diesem Parameter wird die Textur dynamisch auf die festgelegte Größe skaliert. Das Substance Engine regeneriert die Textur auf die gewünschte Größe.
* **Zufallsparameter:** Dieser Parameter variiert die prozedurale Generierung der Substance. Dieser Parameter eignet sich hervorragend zum Erstellen einer zufälligen Version derselben Substance. Sie können die Substance-Parameter schnell ändern, um eine neue Version der Texturen zu generieren.

## Ausgaben

Mit den Ausgabeoptionen können Sie Substance-Ausgaben aktivieren oder deaktivieren. Eine Ausgabe wird vom Substance Engine generiert und als Textur in der Shader-Struktur gerendert.

![](../../../assets/outputs-02.png){width="300px"}

## Optimierungen

Tweak sind Parameter, die in der Substance-Datei erstellt werden und in MODO bearbeitet werden können. Sie können Kanäle auswählen und im Elementmodus die Steuerelemente mithilfe von Kanal-Haul in einem Popup-Controller zusammenführen.

![](../../../assets/haul.png){width="300px"}
