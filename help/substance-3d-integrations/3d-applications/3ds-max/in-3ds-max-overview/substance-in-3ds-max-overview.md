---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/3ds-max/substance-in-3ds-max-overview.html"
breadcrumb-title: ""
description: Erfahren Sie mehr über das Substance-Plug-in für 3ds Max und wie Sie Substance-Materialien importieren und in Ihren Projekten verwenden können.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > 3ds Max > Substance in 3ds Max Overview
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Substance in 3ds Max - Übersicht
user-guide-description: ""
user-guide-title: ""
source-git-commit: 28a9d8cf7a4eed4163f99e8158c9cb8f9da88302
workflow-type: tm+mt
source-wordcount: '653'
ht-degree: 0%
---

# Substance in 3ds Max - Übersicht

## Übersicht über Plug-ins

## Öffnen einer Substance

1. Öffnen Sie den Slate-Editor, suchen Sie nach Substance und ziehen Sie den Knoten Substance2 in die Ansicht.
1. Doppelklicken Sie auf den Substance-Knoten, um die Eigenschaften zu aktivieren, und laden Sie unter Substance Package Browser eine Substance.

   >[!NOTE]
   >
   > Sie können die sbsar-Datei auch per Drag &amp; Drop in den Slate Editor ziehen, um den Knoten automatisch zu erstellen und die Leiste zu importieren.

1. Wenn eine Substance mehrere Graf enthält, können Sie den Graf, den Sie als Material ausgeben möchten, im Dropdown-Menü Ausgewählter Graf auswählen.

   ![](../../../assets/max1.png)

1. Wählen Sie den Substance-Knoten aus, und wählen Sie im Menü &quot;Substance&quot; einen unterstützten Renderer aus. Das Material wird erstellt und kann auf das Objekt angewendet werden. Substance-Texturen sind an das Rendering-Material angeschlossen.

>[!NOTE]
>
> Nachdem der Knoten **&quot;Substance2&quot;** ausgewählt wurde, müssen Sie zuerst auf die Substance **Laden klicken...**, um eine sbsar-Datei auszuwählen, und wählen Sie dann einen unterstützten Renderer aus dem oberen Menü aus (z. B. &quot;Substance nach Arnold&quot;).
>
>Unterstützte Renderer sind Arnold, V-Ray, Corona und Octane. [Erfahren Sie mehr über Workflows in 3DS Max, um herauszufinden, wie Sie OpenPBR-Material verwenden.](../using-workflows-3ds-max/using-workflows-in-3ds-max.md)

![](../../../assets/max3.png)

## Ändern der Auflösung

1. Legen Sie die gewünschte Auflösung für die berechneten Substance-Texturen in den Substance-Ausgabeeinstellungen fest.
1. Stellen Sie bei Auflösungen bis zu 8K sicher, dass Sie das GPU-Engine verwenden, das in den [Substance-Einstellungen](../../../3d-applications/3ds-max/settings-1/substance-settings.md) festgelegt ist.

   ![](../../../assets/max6.png)

## Parameter ändern

1. Doppelklicken Sie auf den Substance-Knoten, um die Substance-Parameter im Parameterfenster zu laden.
1. Ändern Sie die Parameter, um die Substance-Texturen automatisch zu aktualisieren.

   ![](https://helpx-prod.scene7.com/is/image/HelpxProd/max4?$png$&jpegSize=200&wid=1276){width="500px"}

## Ausgabevorschau festlegen

Sie können einen bestimmten Kanal für die Miniaturansicht für den Substance-Knoten festlegen.

1. Wählen Sie in der Dropdown-Liste Ausgabevorschau den Kanal aus, den Sie für die Knoten-Miniaturansicht verwenden möchten.

   ![](../../../assets/max7.png)

## Kachelung Substance

Sie können die Eigenschaften &quot;Koordinaten&quot; verwenden, um Substance-Texturen anzuordnen und Kartenkanäle festzulegen.

![](../../../assets/max10.png)

## OpenPBR Workflows

Zwei OpenPBR-Workflows sind in der Liste **Workflows** im Menü **Substance verfügbar**: **Substance auf OpenPBR** und **Substance auf V-Ray OpenPBR**. Diese Arbeitsabläufe wurden für die Verwendung mit SBSAR-Dateien entwickelt, die mit dem OpenPBR-Materialmodell in Substance 3D Designer oder Sampler erstellt wurden (OpenPBR ist seit Designer V16.0+ und Sampler V6.0+ das Standardmodell).

![](../../../assets/maya-max-v3-1/3ds-max-openpbr-node-preview.png)

### Was ist OpenPBR?

OpenPBR ist ein offenes, physikalisch basiertes Material-Schattierung-Modell, das von Adobe und Autodesk entwickelt wurde und an der Academy Software Foundation (ASWF) mitwirkte. Es bietet eine einheitliche Material-Definition, die mit allen Renderern kompatibel ist. Weitere Informationen finden Sie in der [OpenPBR-Dokumentation](https://experienceleague.adobe.com/en/docs/substance-3d/general-knowledge/openpbr/openpbr-overview).

### Wann sollte ein OpenPBR-Arbeitsablauf verwendet werden?

Verwenden Sie einen OpenPBR-Arbeitsablauf, wenn Ihre Sbsar-Dateien über das OpenPBR-Materialmodell in Substance 3D Designer oder Substance 3D Sampler erstellt wurden. Wenn Ihre SBSAR-Datei mit Adobe Standard Materialmodell (ASM) erstellt wurde, verwenden Sie den älteren Arbeitsablauf, der mit Ihrem Renderer kompatibel ist (Arnold, V-Ray oder V-Ray 6).

>[!NOTE]
>
> Wenn Sie einen OpenPBR-Workflow auf ein ASM-Material oder einen Standardarbeitsablauf auf ein OpenPBR-SBSAR anwenden, verbindet das Plug-In nur Ausgaben, die beiden Materialmodellen gemeinsam sind. Das Ergebnis ist möglicherweise unvollständig.

### Verfügbare OpenPBR-Workflows

**OpenPBR**

Verwendet den nativen 3ds Max openPBRSurface-Knoten. Kompatibel mit Arnold und V-Ray. Dies ist der empfohlene Arbeitsablauf für die meisten Benutzer, die mit OpenPBR-Materialien in 3ds Max arbeiten.

**OpenPBR - V-Ray**

Verwendet das V-Ray-Material (VRayMtl) im OpenPBR-Modus. Empfohlen für Benutzer, deren Pipeline speziell um V-Ray-Material-Setups herum aufgebaut ist.

### Anwenden eines OpenPBR-Workflows

![](../../../assets/maya-max-v3-1/3dsmax-substance-to-openpbr.png)

1. Wählen Sie Ihre Sbsar-Datei (OpenPBR) mit der Schaltfläche Substance laden aus.
1. Wählen Sie im oberen Menü OpenPBR oder OpenPBR - V-Ray aus.
1. Klicken Sie auf Netzwerk erstellen, um das Shader-Netzwerk im Slate Material Editor zu erstellen.
1. Das Plug-in verbindet die SBSAR-Ausgänge automatisch mit den entsprechenden Eingängen des OpenPBR-Nodes.
1. Weisen Sie das Material wie gewohnt Ihrem Mesh zu.

![](../../../assets/maya-max-v3-1/3ds-max-openpbr-overview.png)
