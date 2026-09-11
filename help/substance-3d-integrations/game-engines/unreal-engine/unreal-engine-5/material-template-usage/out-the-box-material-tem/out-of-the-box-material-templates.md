---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/material-template-usage-ue5/out-of-the-box-material-templates.html"
breadcrumb-title: ''
description: Verwenden Sie vorgefertigte Material-Vorlagen, wenn Sie SBSAR-Materialien in Unreal Engine 5 importieren, um eine schnelle Einrichtung und Workflows zu gewährleisten.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 5 > Material Template Usage - UE5 > Out-of-the-Box Material Templates
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Gebrauchsfertige Vorlagen für Materials
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '547'
ht-degree: 0%

---


# Gebrauchsfertige Vorlagen für Materials

Wenn Sie SBSAR-Materialien in den Inhaltsbrowser importieren, können Sie in der Dropdown-Liste die verschiedenen Material-Vorlagen auswählen, die sofort verfügbar sind.

![](../../../../../assets/screen-shot-2022-05-10-at-8-58-45-pm-copy.png)

## Substance-Standardvorlage

Dies ist eine grundlegende Vorlage für ein Material für ein generisches UV-Erlebnis. Es enthält einige grundlegende Steuerelemente für UV-Mengen, sodass Sie die UVs skalieren können, um Texturen dehnen. Sie können die UV-Skalierung teilen, indem Sie die Option &quot;UV teilen&quot; aktivieren. Außerdem haben Sie einen U-Wert, einen V-Wert, einen UV-Versatz und einen UV-Drehwinkel. Auf diese Weise kannst du sowohl eine UV-Kachelung als auch eine UV-Drehung durchführen.

![](../../../../../assets/screen-shot-2022-05-10-at-9-06-40-pm-copy.png)

## Substance Triplanare Vorlage

Die dreiflächige Vorlage erstellt eine dreiflächige Zuordnung der X-, Y- und Z-Winkel oder -Flächen des Meshs, sodass drei verschiedene Projektionen der Texturen überblendet werden, um die Winkel nahtlos zu überblenden. Triplanare Schablone ermöglicht es Materialien, sich über die verschiedenen Flächen zu mischen, während sich das Objekt beugt

![Detailmenü für ein Substance Triplanar-Material](../../../../../assets/triplanar-template.png)

Die triplanare Vorlage unterstützt die Physische Größe. Wenn also die Physische Größe aktiviert ist, skaliert die triplanare Vorlage die Bilder auf der Grundlage der Physische Größe des Materials. Egal, wie stark du dein Objekt skalierst, diese Textur bleibt immer gleich und hat ein einheitliches Aussehen. Weitere Physische Größen: [Physische Größe - UE5](../../../../../game-engines/unreal-engine/unreal-engine-5/physical-size-ue5/physical-size-ue5.md)

## Substance-Refraktionsvorlage

Die Brechungsschablone wird hauptsächlich für transparente Objekte, z. B. Brillen, verwendet. Damit können Sie den IOR-Wert oder die Standard-Texturen ändern, die Sie für ein gläsernes Material oder ein transparentes Material haben würden.

![](../../../../../assets/screen-shot-2022-05-10-at-9-07-38-pm.png)

## Substance Car Malen Template

Die Car Malen-Vorlage bietet Unterstützung für eine durchsichtige Beschichtung und unterstützt anpassbare Kachelungen und Werte für die UV, durchsichtige coat roughness-Werte und Fresnel-Leistungswerte.

![Detailmenü für ein Substance Car Malen-Material](../../../../../assets/car-paint-template.png)

## Einrichten von Vorlagen für Versatz

>[!IMPORTANT]
>
> Experimentelle Vorlagen
> 
> Warnung: Die folgenden Vorlagen sind experimentell und unterliegen erheblichen Änderungen zwischen den Versionen. Diese Vorlagen nutzen die Nanite-Funktion von Epic, die selbst experimentell zum Zeitpunkt dieser Schrift ist. Sie sind möglicherweise nicht 100 % stabil, und bei der Verwendung in Projekten ist Vorsicht geboten.

Führen Sie die folgenden Schritte aus, um die Nanite Versatz-Unterstützung in Ihren Projekten vollständig zu aktivieren und Versatz-Material mit Ihren Meshs zu verwenden.

1. Navigieren Sie zu Projektordner > Config > DefaultEngine.ini und öffnen Sie ihn
1. Hängen Sie Folgendes an den Abschnitt [/Script/Engine.RendererSettings] an:
   * r.Nanite.AllowTessellation=1
   * r.Nanite.Tessellation=1
1. Wählen Sie den statischen Mesh aus, auf den Sie eine Versatz-Vorlage anwenden möchten, und öffnen Sie die Einstellungen dafür.
1. Aktivieren Sie die Option Nanite-Unterstützung aktivieren .
1. Importieren Sie die gewünschte .sbsar-Datei in den Inhaltsbrowser und wählen Sie entweder die Substance\_Displacement\_Template oder die Datei Susbtance\_Triplanar\_Displacement\_Template
1. Um die Anzahl an Versätzen zu ändern, navigieren Sie zur Material-Vorlage und wählen Sie den Ausgabeknoten aus. Passen Sie dann die Magnitude unter dem Abschnitt Versatz an.

## Vorlage für Substance-Versatz

Ähnlich wie die Substance-Standardvorlage ermöglicht diese Vorlage die Anpassung von U- und V-Werten während der Unterstützung von Nanite-Versätzen.

![Detailmenü für ein Substance-Versatz-Material](../../../../../assets/displacement-template.png)

## Substance Triplanare Versatz-Vorlage

Ähnlich wie bei der Substance Versatz-Vorlage gilt für diese Vorlage die triplanare Projektion mit der Option, Physische Größe mit zusätzlicher Nanite Versatz-Unterstützung zu unterstützen.

![Detailmenü für ein Substance Triplanar Versatz-Material](../../../../../assets/triplanar-displacement-template.png)
