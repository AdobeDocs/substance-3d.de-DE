---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/publishing-for-mobile.html"
breadcrumb-title: ''
description: Optimiere in Unity Substance-Materialien für Plattformen auf dem Smartphone oder Tablet, indem du Einstellungen und Texturauflösungen anpasst.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Publishing for Mobile
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Veröffentlichen für Mobilgeräte
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '226'
ht-degree: 0%

---


# Veröffentlichen für Mobilgeräte

>[!NOTE]
>
> **Texturgröße auf Mobilgeräten**
> 
> Die Auflösung der im Unity-Editor festgelegten Struktur entspricht der Größe, die in der App-Binärdatei veröffentlicht wird. Wenn du die Auflösung des Substance-Materials verringerst, entstehen Texturen mit kleineren Dateigrößen.

## Plattformen

## Apple iOS

1. Stellen Sie sicher, dass das iOS-Modul für die entsprechende Unity-Version heruntergeladen wurde.
1. Ändern Sie in Unity das Buildziel in iOS.
1. Öffnen Sie die Player-Einstellungen und ändern Sie das Feld &quot;Identifikation - Bundle-ID&quot; in ein eindeutigeres Feld. (zum Beispiel: com.Adobe.iosProject)
1. Entwickeln und starten Sie das Spiel.
1. Klicken Sie in Xcode auf das iOS-Gerät und ändern Sie die Dropdown-Liste &quot;Signieren - Team&quot; in Ihre Entwicklerteam-ID.
1. Navigieren Sie auf dem iOS-Gerät zu &quot;Einstellungen - Allgemein - Geräteverwaltung&quot; und klicken Sie auf der angezeigten Entwicklerteam-ID auf &quot;Vertrauen&quot;.
1. Führen Sie den Xcode-Build erneut aus, indem Sie auf die Schaltfläche &quot;Build and Run current scheme&quot; (die Schaltfläche &quot;Play&quot;) klicken.
1. Das Spiel sollte auf dem iOS-Gerät ausgeführt werden.

## Android OS

1. Stellen Sie sicher, dass das Android-Modul für die entsprechende Unity-Version heruntergeladen wird.
1. Ändern Sie in Unity das Buildziel in Android.
1. Öffnen Sie die Player-Einstellungen und ändern Sie das Feld &quot;Identifikation - Bundle-ID&quot; in ein eindeutigeres Feld. (zum Beispiel: com.Adobe.androidProject)
1. Entwickeln und starten Sie das Spiel.
1. Das Spiel sollte auf dem Android-Gerät laufen.
