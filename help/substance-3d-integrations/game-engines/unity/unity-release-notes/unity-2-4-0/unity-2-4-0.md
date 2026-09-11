---
helpx_url: "https://helpx.adobe.com/de/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-2-4-0.html"
breadcrumb-title: ''
description: Lesen Sie die Versionshinweise für Unity-Plug-in Version 2.4.0, um mehr über neue Funktionen, Verbesserungen und Fehlerbehebungen zu erfahren.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 2.4.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Unity 2.4.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 0%

---


# Unity 2.4.0

>[!WARNING]
>
> Unity hat die Standard-Build-Architektur auf x86 anstelle von x86\_64 geändert.\
> Skripte werden nicht ausgeführt, wenn sie auf Substance verweisen. Sie müssen zu x86\_64 zurückkehren, und der Build funktioniert.

## Neue Funktionen:

* Unterstützung für HDRP-Projekte hinzugefügt (Vorschau)
* Hinzugefügte Voreinstellungen im Menü &quot;Substance&quot;
* Es wurde die Möglichkeit hinzugefügt, die Standardeinstellung für den Import von Substance-Auflösungen festzulegen
* Möglichkeit zum Festlegen der standardmäßigen normalen Komprimierung hinzugefügt
* Es wurde die Möglichkeit hinzugefügt, alle Ausgaben für einen Import eines Substance zu generieren.
* Unterstützung für benutzerdefinierte Ausgaben + Ausgaben mit derselben Verwendung
* Einstellungen für die Plattformauflösung hinzugefügt
* Fehlerbehebungen für die IL2CPP-Unterstützung hinzugefügt

### Fehlerbehebungen:

* Es wurde ein Fehler behoben, durch den das Öffnen einer Substance Source unter Mac einen Linux-Fehler auslöste.
* Verkürzte Zeit, die beim Wechseln von Plattformen benötigt wird. Die Konvertierung von Texturen für mobile Plattformen erfolgt jetzt im Build und nicht beim Wechseln der Zielplattform.
* Assertionsfehler beim Importieren von SBSAR
* Das Aktualisieren von Projekten mit .NET 3.5 führt zum Bruch von Substance-Materialien
* Substance-Quelle wird im Linux-Dialogfeld unter OS X nicht unterstützt
* Namensänderung des Grafen zerstört Prefabs und Szene im ForceText-Serialisierungsmodus
* Substance von Materialien mit mehreren Ausgaben mit derselben Verwendung unterbricht das Plug-in unterstützt keine benutzerdefinierten Ausgaben in sbsar

### Bekannte Probleme:

* Beim Upgrade eines Projekts von 2017-2018/2019 muss Unity nach dem Importieren des Substance-Plug-ins durch den Benutzer neu gestartet werden, damit das Projekt aktualisiert wird.\
  Problemumgehung: Erstellen Sie ein Paket der Assets/des Projekts und importieren Sie dieses Paket mit dem Plug-in 2.4.0 in ein neueres Projekt. Die Substance-Dateien sollten korrekt konvertiert werden.
* Unity hat die Standard-Buildarchitektur in x86 geändert. Derzeit unterstützt das Substance-Plugin nur x86\_64.

**Nicht mehr vollständig unterstützt:**

* Substance Live Link wurde aus dem Asset Store-Paket entfernt. (Das Paket kann weiterhin von der Substance share heruntergeladen werden.)
