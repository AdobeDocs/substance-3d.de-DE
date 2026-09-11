---
helpx_url: "https://helpx.adobe.com/de/substance-3d-integrations/3d-applications/3ds-max/3ds-max-plugin-release-notes/3ds-max-2-7-0.html"
breadcrumb-title: ''
description: Lesen Sie die Versionshinweise für das 3ds Max-Plugin Version 2.7.0 , um mehr über neue Funktionen, Verbesserungen und Fehlerbehebungen zu erfahren.
helpx_creative_field: ""
helpx_description: Substance 3D Integrations
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 3ds Max 2.7.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---


# 3ds Max 2.7.0

<b>hinzugefügt/aktualisiert:</b>

* Das Substance-Engine wurde im 3ds Max-Plug-in auf Version 9 aktualisiert, wodurch Leistung und Kompatibilität verbessert wurden.

<b>Fest:</b>

* Es wurde ein Absturz-Problem in den 3ds Max-Versionen 2019, 2022, 2023 und 2024 behoben, bei dem das Ziehen eines Substance 2-Knotens in den Slate Material Editor zu einem Absturz führte. Der Substance 2-Knoten kann jetzt sicher in den Slate Material Editor gezogen und dort abgelegt werden.
* Es wurde ein Problem im Substance-Plug-in für 3ds Max behoben, bei dem die Auswahl von &quot;Substance zu Arnold&quot; und anderen Workflows keine wichtigen Knoten im Material Slate Editor erzeugten, sondern fälschlicherweise ein Maxscript mit einem Kompilierungsfehler öffnete. Knoten für Workflows wie Arnold werden jetzt korrekt generiert und automatisch verbunden.
* Es wurde ein Problem behoben, bei dem das Exportieren von Startelementen/Voreinstellungen (.sbsar - Substance2 Textur Map) aus Substance 3D Sampler und das Konvertieren dieser Elemente in Corona Renderer ( 6 bis 9hf1) innerhalb des 3ds Max zu beschädigten Materialien, einem Rendering mit schwarzer Grundfarbe und beschädigten Bump-Normalen führte. Darüber hinaus behebt dieses Update die Unzugänglichkeit der Registerkarte &quot;Substance-Eigenschaften&quot; in den Materialien, ein Problem, das sich auch auf die Konvertierung in Vray auswirkte.
* Es wurde ein Problem im 3ds Max-Plug-in behoben, durch das das Verbinden oder Trennen von Eingängen von Substance2-Texturen mit dem Corona-Material zu Abstürzen führte
* Es wurde ein Kompatibilitätsproblem in 3ds Max 2024 behoben, bei dem in eine MaxScript-Datei eingebettete oder aufgerufene Python-Skripte standardmäßig nicht zulässig waren
* Es wurde ein Problem im 3Ds Max-Plugin behoben, durch das das Importieren und Ausführen des Substance-zu-Corona-Plugins dazu führte, dass Materials in Shader-Vorschauen und Renderings schwarz und glänzend angezeigt wurden. Dieses Problem wurde nun erfolgreich behoben, um die korrekte Anzeige und Darstellung von Substance-Maps mit dem Corona-Renderer sicherzustellen.

Diese Version wurde für die 3ds Max 2021, 2022 und 2023 veröffentlicht
