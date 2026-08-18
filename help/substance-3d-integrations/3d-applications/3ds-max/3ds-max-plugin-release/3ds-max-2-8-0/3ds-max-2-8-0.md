---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/3ds-max/3ds-max-plugin-release-notes/3ds-max-2-8-0.html"
breadcrumb-title: ''
description: Lesen Sie die Versionshinweise für das 3ds Max-Plugin der Version 2.8.0, um mehr über neue Funktionen, Verbesserungen und Fehlerbehebungen zu erfahren.
helpx_creative_field: ""
helpx_description: Substance 3D Integrations
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 3ds Max 2.8.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 0%

---


# 3ds Max 2.8.0

<b>Hinzugefügt/aktualisiert:
</b>

* Unterstützung für die bedingte Sichtbarkeit von Parametern (&quot;visible if&quot;); -Parameter werden jetzt ausgeblendet, wenn die Bedingungen nicht erfüllt sind, wobei ihre jeweiligen Gruppen sichtbar bleiben.
* Corona Renderer im 3ds Max-Plugin auf Version 10 aktualisiert, wodurch die Rendering-Funktionen und
* Das neueste Update verbessert die Rendering-Geschwindigkeit und die CPU-Auslastung in 3ds Max 2024 bei Verwendung von Substance deutlich und stimmt die Leistung stärker mit der Effizienz ab, die in 3ds Max 2022 beobachtet wurde.

<b>Fest:</b>

* Das Substance-Plugin wurde verbessert, um die Tastatureingabewerte innerhalb des praktischen Bereichs für jeden Parameter zu beschränken und Probleme mit der Schiebereglersteuerung und manuellen Wertanpassungen zu vermeiden.
* Es wurde ein Problem behoben, bei dem das Kopieren von Substance2-Texturkonvertierungen (.sbsar) im Slate Material Editor zu einer unbeabsichtigten Instanziierung des kopierten Knotens führte und möglicherweise zu Abstürzen im Zusammenhang mit d3d11.dll führte.
* Es wurde ein Absturzproblem in 3ds Max behoben, das beim Rendern benutzerdefinierter/bearbeiteter kopierter Materialsubstanzen (.sbsar) mit Corona Interactive auftrat
* Es wurde ein Problem im Substance2-Knoten von 3ds Max behoben, bei dem die Schieberegler für Ganzzahl 3 und 4 nicht reagierten und nur die Werte durch manuelle numerische Eingabe aktualisiert wurden. Darüber hinaus wurden diese Werte im Gleitkommaformat falsch angezeigt. Die Schieberegler sind jetzt funktionsfähig und geben die gewünschten Werttypen genau wieder.
* Es wurde ein Problem in 3ds Max 2021 mit Corona Render behoben, bei dem Substance-Materialien im Viewport korrekt angezeigt, aber bei der Dateiübertragung auf einen anderen PC grau dargestellt wurden. Benutzer müssen keine Materialien mehr von Grund auf neu einrichten oder Vorgaben laden, um ein ordnungsgemäßes Rendering zu ermöglichen.
* Es wurde ein Absturzproblem im 3ds Max-Plug-in behoben, das beim Versuch auftrat, Substance-Knoten im Slate Material Editor zu duplizieren.
* Es wurde ein Problem behoben, bei dem die Einstellung für das CPU-Kernlimit im Substance-Plug-in nach dem Neustart von 3ds Max nicht gespeichert wurde, um sicherzustellen, dass benutzerkonfigurierte Werte jetzt sitzungsübergreifend beibehalten werden.

Diese Version wurde für die 3ds Max 2021, 2022 und 2023 veröffentlicht
