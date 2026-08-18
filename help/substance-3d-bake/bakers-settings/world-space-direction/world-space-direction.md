---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/bakers-settings/world-space-direction.html"
breadcrumb-title: ''
description: Berechnen Sie Vektorrichtungen im Weltraum und speichern Sie sie in Texturen für gerichtete Effekte und Maskierung.
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > World Space Direction
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Welt-Raum-Richtung
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '155'
ht-degree: 4%

---


# Welt-Raum-Richtung

Mit dem Bäcker &quot;Weltraumrichtung&quot; kannst du eine Vektorrichtung im Weltraum in eine Textur umwandeln.

**Verfügbar in:**

* Substance Designer
* Substance Automation Toolkit

## Parameter

| *Parameter* | *Beschreibung* |
| --- | --- |
| **Eingaberichtung** | Legt fest, aus welcher Eingabe die Richtung berechnet wird.Mögliche Werte:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Von Textur</strong>: Die Vektorrichtung wird durch eine Eingabetextur definiert.</li><li data-preserve-html="true"><strong>Von einheitlichem Vektor</strong> (Standard): Die Vektorrichtung wird mit den Schiebereglern X, Y und Z definiert.</li></ul> |
| **Normale Ausrichtung** | Definiert, ob das normale Format der Ausgabetextur verwendet wird. Dies kehrt den grünen Kanal je nach Format um.Mögliche Werte:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>OpenGL</strong></li><li data-preserve-html="true"><strong>DirectX</strong> (Standard)</li></ul> |
| **X Y Z** | Regler zum Definieren der 3 Komponenten des Richtungsvektors, wenn **Eingangsrichtung** auf **Von einheitlichem Vektor** festgelegt ist. |
| **Richtungsdatei** | Pfad zur Eingabetexturdatei zum Definieren des Richtungsvektors, wenn **Eingaberichtung** auf **Von Textur** festgelegt ist. |
