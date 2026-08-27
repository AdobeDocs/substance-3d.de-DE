---
helpx_url: "https://helpx.adobe.com/de/substance-3d-bake/common-issues/normal-map-has-strange-colorful-gradients.html"
breadcrumb-title: ''
description: Experimentiere mit farbigen Verläufen in Normalen-Map. Überprüfe Mesh-Normalwerte, Glättungsgruppen und UV-Mapping.
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Normal map has strange colorful gradients
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Normale Karte hat seltsame farbige Verläufe
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---


# Normale Karte hat seltsame farbige Verläufe

Das Ergebnis des Bakers ist eine Reihe sehr starker farbiger Farbverläufe.

![](../../assets/color-gradient.png)


## Erläuterung

Farbverläufe treten in der Regel auf, wenn beim Baking führ eine Diskrepanz zwischen dem Mesh mit hohem und niedrigem Poly besteht. Diese Diskrepanz kann durch den folgenden Grund erklärt werden:

* Der Mesh mit hohem und niedrigem Poly <b>überlappen sich nicht </b> richtig (siehe Abbildung unten).
* Das High-Poly ist <b>fehlende Geometrie</b>, die das Low-Poly abzudecken versucht.
* Der Mesh mit hohem oder niedrigem Poly hat invertierte Scheitelpunkt-Normalen.

Wenn dies geschieht, versucht der Baking führend Prozess, die Geometrie anzupassen, die nicht existiert, was zu etwas Leerem führt. Der Baker füllt diesen leeren Bereich mit einer Farbe, die aus den Nachbarpixeln in den Texturen extrahiert wurde, wodurch der farbige Farbverlauf erstellt wird (es sei denn, <b>Diffusion</b> ist deaktiviert).

## Lösung

Angesichts der wenigen möglichen Gründe, die zu keiner Überschneidung zwischen den Meshs führen, müssen einige Lösungen in Betracht gezogen werden:

* Stellen Sie sicher, dass Sie die Mesh-Transformation einfrieren/zurücksetzen (x-Form zurücksetzen usw.), um sicherzustellen, dass alle Meshs konsistent sind.
* Importieren Sie sowohl den Low- als auch den High-Poly-Mesh in Ihre 3D-Modellierungssoftware, um sicherzustellen, dass sie sich korrekt überlappen
* Stellen Sie sicher, dass Ihre Namenskonvention gültig ist, wenn Sie die Funktion [Abgleich nach Name](../../features/matching-by-name/matching-by-name.md) verwenden (Sie können sie überprüfen, indem Sie die Protokolldatei, in der die Namen der Mesh gedruckt werden sollen, Baking geführt und dann überprüft haben).

### Beispiel

Unten sehen Sie ein Beispiel mit einer Kugel mit hohem und niedrigem Poly. Auf der linken Seite überlappen sich die Mesh nicht, da das Poly weggeschoben wurde:

![](../../assets/baking-gradients.jpg)
