---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/3ds-max/3ds-max-plugin-release-notes/3ds-max-2-3-2.html"
breadcrumb-title: ''
description: Lesen Sie die Versionshinweise für das 3ds Max-Plugin Version 2.3.2 , um mehr über neue Funktionen, Verbesserungen und Fehlerbehebungen zu erfahren.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > 3ds Max > 3ds Max Plugin Release Notes > 3ds Max 2.3.2
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 3ds Max 2.3.2
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 0%

---


# 3ds Max 2.3.2

Veröffentlicht am 8. April 2020

Heute haben wir die Version 2.3.2 des Plugins veröffentlicht, die meist ein Bugfix Release auf 2.3.1 ist.

2.3.2 Version:

* Aktualisierte Substance Engine auf 7.2.9
* Problem beim Rendern mit Redshift/VRay behoben, das in 3ds Max 2018, 2019 und 2020 abstürzte
* Debug-Assert-Fehler werden nicht mehr angezeigt
* Der Substance2-Knoten verfügt jetzt über die Skriptschnittstellen für iMultipleOutputChannelsWithValues.
* Der Substance-Quelleintrag im Menü öffnet nun den Substance Launcher zur Registerkarte Source (Quelle), falls er installiert ist
* Substance-Materialien sollten jetzt korrekt aktualisiert werden, wenn Sie mit dem Corona-Renderer arbeiten
* Substance-Ausgaben werden bei Verwendung mit VRay Next nicht mehr vorübergehend durch Bilder ersetzt
* Das Dialogfeld &quot;Renderkompatibilität&quot; wurde entfernt und wird automatisch angezeigt. Sie ist bei Bedarf noch im Dialogfeld &quot;Einstellungen&quot; verfügbar
* Mögliche Probleme beim Exportieren einer FBX-Datei behoben, während Substance-Material in 3ds Max 2021 angewendet wurde

Bekannte Probleme:

* In 3ds Max 2018 wird das Exportieren einer FBX mit einem an das Objekt angehängten Substance-Material im fbxmax.dlu-Plug-in als Absturz angezeigt. Wir sprechen derzeit mit Autodesk, um zu sehen, ob es etwas auf unserer Seite gibt, das getan werden kann, oder ob es sich um eine Einschränkung der älteren Version der fbx-Integration handelt. Die vorherige Problemumgehung war unzuverlässig und wurde entfernt. Dies tritt nicht bei 3ds Max 2019 oder höher auf.

Diese Version wurde für die 3ds Max 2018, 2019, 2020 und 2021 veröffentlicht.
