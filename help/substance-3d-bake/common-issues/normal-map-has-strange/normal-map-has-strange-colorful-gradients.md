---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-issues/normal-map-has-strange-colorful-gradients.html"
breadcrumb-title: ''
description: Korrigieren Sie seltsame farbige Verläufe in normalen Maps, indem Sie Mesh-Normalen, Glättungsgruppen und UV-Mapping überprüfen.
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

Das Ergebnis des Bäckers ist eine Reihe sehr starker bunter Farbverläufe.

![](../../assets/color-gradient.png)


## Erläuterung

Farbverläufe treten in der Regel auf, wenn während des Backvorgangs eine Diskrepanz zwischen dem High-Poly- und dem Low-Poly-Gitter besteht. Diese Diskrepanz kann durch den folgenden Grund erklärt werden:

* Das Gitter mit hohem und niedrigem Poly <b>überlappen sich nicht </b> ordnungsgemäß (siehe Abbildung unten).
* Das High-Poly ist <b>fehlende Geometrie</b>, die das Low-Poly abzudecken versucht.
* Das High-Poly- oder Low-Poly-Gitter hat invertierte Scheitelpunktnormalen.

Wenn das passiert, versuchen Sie den Backvorgang, Geometrie, die nicht vorhanden ist, entsprechen, was zu etwas leeren. Der Bäcker füllt diesen leeren Bereich mit einer Farbe, die aus den benachbarten Pixeln in den Texturen extrahiert wird, wodurch der farbige Verlauf erstellt wird (es sei denn, <b>Diffusion</b> ist deaktiviert).

## Lösung

Angesichts der wenigen möglichen Gründe, die zu keiner Überschneidung zwischen den Maschen führen, müssen einige Lösungen in Betracht gezogen werden:

* Stellen Sie sicher, dass Sie die Gittertransformation einfrieren/zurücksetzen (x-Form zurücksetzen usw.), um sicherzustellen, dass alle Gitter konsistent sind.
* Importieren Sie sowohl das Polygonnetz mit niedriger als auch das Polygonnetz in Ihre 3D-Modellierungssoftware, um sicherzustellen, dass sie sich korrekt überlappen.
* Stellen Sie sicher, dass Ihre Namenskonvention gültig ist, wenn Sie die Funktion [Abgleich nach Name](../../features/matching-by-name/matching-by-name.md) verwenden (Sie können sie überprüfen, indem Sie die Protokolldatei sichern und dann in die Protokolldatei schauen, in der die Netznamen gedruckt werden sollen).

### Beispiel

Unten sehen Sie ein Beispiel mit einer Kugel mit hohem und niedrigem Poly. Auf der linken Seite überlappen sich die Gitter nicht, da das Poly weggeschoben wurde:

![](../../assets/baking-gradients.jpg)
