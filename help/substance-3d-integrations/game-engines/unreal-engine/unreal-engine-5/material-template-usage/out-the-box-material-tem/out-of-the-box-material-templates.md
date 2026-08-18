---
helpx_url: "https://helpx.adobe.com/de/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/material-template-usage-ue5/out-of-the-box-material-templates.html"
breadcrumb-title: ''
description: Verwenden Sie vorgefertigte Materialvorlagen, wenn Sie SBSAR-Materialien in Unreal Engine 5 importieren, um eine schnelle Einrichtung und Workflows zu gewährleisten.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 5 > Material Template Usage - UE5 > Out-of-the-Box Material Templates
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Gebrauchsfertige Materialvorlagen
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '547'
ht-degree: 0%

---


# Gebrauchsfertige Materialvorlagen

Beim Importieren von SBSAR-Materialien in den Inhaltsbrowser können Sie die verschiedenen Materialvorlagen in der Dropdown-Liste auswählen, die sofort verfügbar sind.

![](../../../../../assets/screen-shot-2022-05-10-at-8-58-45-pm-copy.png)

## Substance-Standardvorlage

Dies ist eine grundlegende Materialvorlage für ein generisches UV-Erlebnis. Es enthält einige grundlegende Steuerelemente für UV-Mengen, sodass Sie die UVs skalieren können, um Texturen zu dehnen. Sie können die UV-Skalierung aufteilen, indem Sie die Option &quot;UV aufteilen&quot; aktivieren. Außerdem haben Sie U-Menge, V-Menge, UV-Versatz und einen UV-Drehwinkel. So kannst du sowohl eine UV-Kachelung als auch eine UV-Drehung durchführen.

![](../../../../../assets/screen-shot-2022-05-10-at-9-06-40-pm-copy.png)

## Substance Triplanare Vorlage

Die dreiflächige Schablone erstellt eine dreiflächige Zuordnung der X-, Y- und Z-Winkel oder -Flächen des Gitters, sodass drei verschiedene Vorsprünge der Texturen miteinander vermischt werden, um die Winkel nahtlos zu vermischen. Triplanare Schablone ermöglicht es, Materialien auf den verschiedenen Flächen miteinander zu vermischen, während sich das Objekt biegt

![Detailmenü für ein Substance-Triplanarmaterial](../../../../../assets/triplanar-template.png)

Die Triplanar-Vorlage unterstützt Physische Größen. Wenn also Physische Größe aktiviert ist, skaliert die Triplanar-Vorlage die Bilder auf der Grundlage der Physische Größe des Materials. Egal, wie stark du dein Objekt skalierst, diese Textur bleibt immer gleich und hat ein einheitliches Aussehen. Weitere Physische Größen: [Physische Größe - UE5](../../../../../game-engines/unreal-engine/unreal-engine-5/physical-size-ue5/physical-size-ue5.md)

## Substance-Refraktionsvorlage

Die Brechungsschablone wird hauptsächlich für transparente Objekte, z. B. Brillen, verwendet. Damit können Sie den IOR-Wert oder die Standardtexturen ändern, die Sie für ein Glasmaterial oder transparentes Material haben würden.

![](../../../../../assets/screen-shot-2022-05-10-at-9-07-38-pm.png)

## Substance-Automobil-Malvorlage

Die Car Paint-Vorlage bietet Unterstützung für eine klare Beschichtung und unterstützt anpassbare UV-Kacheln und -Werte, Werte für die klare Beschichtung und Fresnelleistungswerte.

![Detailmenü für ein Substance-Autolackmaterial](../../../../../assets/car-paint-template.png)

## Einrichten von Vorlagen für Versatz

>[!IMPORTANT]
>
> Experimentelle Vorlagen
> 
> Warnung: Die folgenden Vorlagen sind experimentell und unterliegen erheblichen Änderungen zwischen den Versionen. Diese Vorlagen nutzen die Nanite-Funktion von Epic, die selbst experimentell zum Zeitpunkt dieser Schrift ist. Sie sind möglicherweise nicht 100 % stabil, und bei der Verwendung in Projekten ist Vorsicht geboten.

Führen Sie die folgenden Schritte aus, um die Nanite Versatz-Unterstützung in Ihren Projekten vollständig zu aktivieren und Versatz-Materialien mit Ihren Netzen zu verwenden.

1. Navigieren Sie zu Projektordner > Config > DefaultEngine.ini und öffnen Sie ihn
1. Hängen Sie Folgendes an den Abschnitt [/Script/Engine.RendererSettings] an:
   * r.Nanite.AllowTessellation=1
   * r.Nanite.Tessellation=1
1. Wählen Sie das statische Gitter aus, auf das Sie eine Versatz-Vorlage anwenden möchten, und öffnen Sie dessen Einstellungen.
1. Aktivieren Sie die Option Nanite-Unterstützung aktivieren .
1. Importieren Sie die gewünschte .sbsar-Datei in den Inhaltsbrowser und wählen Sie entweder die Substance\_Displacement\_Template oder die Datei Susbtance\_Triplanar\_Displacement\_Template
1. Um die Menge an Versatz zu ändern, navigieren Sie zur Materialvorlage und wählen Sie den Ausgabeknoten aus. Passen Sie dann die Magnitude unter dem Abschnitt Versatz an.

## Vorlage für Substance-Versatz

Ähnlich wie die Substance-Standardvorlage ermöglicht diese Vorlage die Anpassung von U- und V-Werten während der Unterstützung von Nanite-Versätzen.

![Detailmenü für ein Substance-Versatz-Material](../../../../../assets/displacement-template.png)

## Substance Triplanare Versatz-Vorlage

Ähnlich wie die Substance Versatz-Vorlage wendet diese Vorlage eine triplanare Projektion an, mit der Option, Physische Größen mit zusätzlicher Nanit-Versatz-Unterstützung zu unterstützen.

![Detailmenü für ein Material für einen Substance Triplanar-Versatz](../../../../../assets/triplanar-displacement-template.png)
