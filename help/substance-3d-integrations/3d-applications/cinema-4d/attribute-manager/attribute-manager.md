---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/cinema-4d/attribute-manager.html"
breadcrumb-title: ''
description: Verwenden Sie den Attributmanager von Cinema 4D, um die Eigenschaften und Materialeinstellungen von Substance-Assets zu konfigurieren.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Cinema 4D > Attribute Manager
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Attribut-Manager
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---


# Attribut-Manager

Es gibt einen neuen Modus für das Substance von Assets im Attributmanager von Cinema 4D.

Wenn Sie im Substance-Asset-Manager eine Substance auswählen, wechselt der Attributmanager automatisch in den Substance-Asset-Modus. Sie können auch manuell in diesen Modus im Menü &quot;Modus&quot; des Attribut-Managers wechseln.

Im Substance-Asset-Modus haben Sie Zugriff auf alle Eingänge einer Substance und Sie haben auch einen Überblick über alle Ausgabekanäle.

![](../../../assets/cinema-4d-9.png){width="500px"}

## Gruppieren von Substance-Eingängen

Wenn Eingaben eines Substance gruppiert sind, werden diese Gruppen als solche im Attributmanager angezeigt. Es gibt zwei vordefinierte Gruppen: **Grundlegende Eigenschaften** und **Bildeingaben**.

* In der Gruppe &quot;Grundlegende Eigenschaften&quot; werden alle Eingaben angezeigt, die keiner Gruppe im Substance Designer zugewiesen wurden.
* Wie der Name bereits andeutet, werden alle Substance-Eingaben, die mit externen Bildern verknüpft sind, in der Gruppe &quot;Bildeingaben&quot; erfasst.

## Dateinamenparameter

Durch Verwenden des Parameters &quot;Dateiname&quot; im Attributmanager kann der Dateispeicherort von Substance-Assets geändert werden, nachdem sie in eine Szene geladen wurden.

![](../../../assets/cinema-4d-10.png){width="500px"}

Dies kann nicht nur beim Verschieben von Substance-Dateien nützlich sein, sondern auch beim Austausch einer Substance mit einer völlig anderen.

In diesem Fall wird der Anwender gefragt, ob vorhandene Verweise auf vorherige Substance-Ausgabekanäle der neuen Substance neu zugeordnet werden sollen.

![](../../../assets/cinema-4d-11.png){width="500px"}

Wenn die Frage mit &quot;Nein&quot; beantwortet wird, werden die Links zur vorherigen Substance von allen Substance-Shadern gelöscht. Um die Ausgabekanäle neu zuzuordnen, sucht das Plug-in zunächst nach Ausgabekanälen desselben Typs und dann mit demselben Namen.

## Parameter Tri-state

Wenn mehrere Substance gleichzeitig ausgewählt sind, werden die von diesen Substance gemeinsam genutzten Eingaben als Tri-State angezeigt und können für alle ausgewählten Substance gleichzeitig bearbeitet werden (wie alle anderen Parameter in Cinema 4D).

In diesen Fällen werden die Ausgabekanäle wie unten gezeigt angezeigt.

![](../../../assets/cinema-4d-12.png){width="300px"}
