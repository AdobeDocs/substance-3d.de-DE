---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/blender/release-notes/add-on-0-9-1.html"
breadcrumb-title: ''
description: Lesen Sie die Versionshinweise für die Blender-Add-On-Version 0.9.1, um mehr über neue Funktionen, Verbesserungen und Fehlerbehebungen zu erfahren.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Blender > Release Notes > Add-on 0.9.1
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Add-on 0.9.1
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '463'
ht-degree: 0%

---


# Add-on 0.9.1

**Versionshinweise für Add-on-Version 0.91+**

* Hinweis: *Die Plug-In-Version 0.91+ ist nicht abwärtskompatibel mit früheren Versionen des Plug-Ins!*
* Neuarchitektur der internen Code-Basis, um die Leistung und Stabilität des Plug-ins zu verbessern
* Überarbeitete Benutzeroberfläche zur Verbesserung der allgemeinen Benutzererfahrung
* Neue Benutzeroberfläche, die die Möglichkeit bietet, die Standardkachelung zu ändern
* Zusätzliche Unterstützung für die Aktualisierung von Texturen in der Zyklen-Renderansicht
* Fehlerbehandlung in der Konsole wurde hinzugefügt, um zu benachrichtigen, wenn ein Stoff nicht geladen wurde
* Das überlagerte Menü mit Schnellaktionen wurde aktualisiert

**Voreinstellungsabschnitt: Hinzugefügt/aktualisiert:**

* Parameter &quot;Bildformat exportieren&quot; Wenn in Blender erzeugte Bilder als Bildeingaben für ein Substance-Material verwendet werden, wird dieses Format verwendet, um das Bild im temporären Ordner zu speichern.
* Pfad zur Sbsar-Bibliothek; Gibt den Ordner an, der standardmäßig geöffnet wird, wenn die Schaltfläche &quot;Laden&quot; zum Suchen nach einer Substance-Datei verwendet wird.
* Ein Standard-Texturexportpfad (Temporaler Ordner), der den Pfad emuliert, der von Substance 3D Painter zum Verarbeiten nicht gespeicherter Dateiexporte verwendet wird
* Relativer Pfad mit der oben beschriebenen Struktur und der Option, Schlüssel wie $matName zum Erstellen von Unterordnern zu verwenden
* Sbsar-Dateien relativer Pfad zum Erstellen eines Unterordners, der die in Ihrer Angleichungsdatei verwendeten Sbsar-Dateien verpackt, wenn Sie das Projekt speichern
* Möglichkeit, verschiedene Shader-Netzwerke dynamisch in den Einstellungen festzulegen - Im Shader-Netzwerk die Möglichkeit, je nach Shader-Anforderungen verschiedene Variablen pro Shader festzulegen
* Im Abschnitt &quot;Ausgaben&quot; des Shader-Netzwerks können Sie festlegen, ob eine Ausgabe standardmäßig aktiviert ist
* Möglichkeit, den Farbraum festzulegen (dies unterstützt Asse, lineare exr- und Blender-Arbeitsabläufe, nicht nur srgb)
* Standardauswahl von Bildformat und Bittiefe
* Eine generische Ausgabe zum Einrichten der Werte für die Ausgabe verwendet, die nicht im Shader definiert sind, z. B. wenn Sie eine andere Ausgabe haben, die vom Shader standardmäßig nicht verwendet wird, z. B. eine Maske.
* Ein Filter zum Ändern des Ausgabetyps (1 Nur aktivierte Ausgaben, 2 Alle Ausgaben, die im Shader und auf der Substance vorliegen, 3 Alle auf der Substance verfügbaren Ausgaben)
* Unterstützung für benutzerdefinierte Tastaturbefehle (bearbeitet)

**Abschnitt des Substance 3D-Bedienfelds: Hinzugefügt/aktualisiert:**

* Möglichkeit zum Anpassen und Sperren des Kachelungen- und Auflösungsparameterwerts
* Aktualisierte voreingestellte Benutzeroberfläche - Die Dropdown-Liste &quot;Shader-Typ&quot;, um den Typ des Grafen zu ändern, den die Benutzer haben möchten
* Der Eingabeparameter des Bilds wurde in den Standard-Bildeingang geändert, der in Blender verwendet wird. Sie können jetzt Blender-Bilder und nicht nur Dateien verwenden
* Möglichkeit, jederzeit in mehreren Blender-Instanzen zu arbeiten
* Unterstützung für die automatische Hervorhebung der Material im Substance 3D-Bedienfeld, wenn das Material im Viewport ausgewählt ist
