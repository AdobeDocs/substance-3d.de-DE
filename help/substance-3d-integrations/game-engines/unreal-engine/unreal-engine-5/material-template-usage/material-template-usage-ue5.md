---
helpx_url: "https://helpx.adobe.com/de/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/material-template-usage-ue5.html"
breadcrumb-title: ''
description: Erstellen und verwenden Sie Materialvorlagen in Unreal Engine 5, um festzulegen, wie Substance-Ausgabeknoten mit Materialeingaben verbunden werden.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 5 > Material Template Usage - UE5
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Verwendung der Materialvorlage - UE5
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '197'
ht-degree: 0%

---


# Verwendung der Materialvorlage - UE5

Mit Materialvorlagen kann der Benutzer ein Basismaterial für Stoffe erstellen, das als Vorlage zum Verbinden seiner Ausgabeknoten mit den Eingaben im Material verwendet werden kann.\
Ausgaben mit demselben Namen und Typ wie die Materialeingabe werden automatisch verwendet. Dieses Beispiel für übergeordnetes Material enthält einen Beispielknoten für die &quot;baseColor&quot;-Textur, der ausgefüllt wird, wenn die Substance eine Texturausgabe hat, die auch &quot;baseColor&quot; genannt wird.\
![](../../../../assets/parent-material-sample.png)

Substance-Ausgaben unterstützen das Aktualisieren von Texturen, Single-Float- oder Int-Skalarwerten und Vektorwerten (2-4). Wenn Sie zur Laufzeit float- oder int-Ausgaben verwenden möchten, müssen Sie die dynamicMaterialInstance aus dem Diagramm abrufen, da staticMaterialInstances (alle im Editor generierten Materialien) die Skalarwerte zur Laufzeit nicht ändern können.

![](https://helpx-prod.scene7.com/is/image/HelpxProd/scalar-value?$png$&jpegSize=100&wid=245)

Die Instanz des Substance-Graphen versucht, alle relevanten Ausgabewerte zum Zeitpunkt der Erstellung auszufüllen.

![](https://helpx-prod.scene7.com/is/image/HelpxProd/screen-shot-2022-04-01-at-4-38-31-pm?$png$&jpegSize=200&wid=1076)
