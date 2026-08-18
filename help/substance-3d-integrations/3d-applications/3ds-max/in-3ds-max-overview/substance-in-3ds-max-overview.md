---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/3ds-max/substance-in-3ds-max-overview.html"
breadcrumb-title: ''
description: Erfahren Sie mehr über das Substance-Plug-in für 3ds Max und wie Sie Substance-Materialien importieren und in Ihren Projekten verwenden können.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > 3ds Max > Substance in 3ds Max Overview
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Substance in 3ds Max - Übersicht
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '296'
ht-degree: 0%

---


# Substance in 3ds Max - Übersicht

## Übersicht über Plug-ins:

## Öffnen einer Substance

1. Öffnen Sie den Slate-Editor, suchen Sie nach Substance und ziehen Sie den Knoten Substance2 in die Ansicht.
1. Doppelklicken Sie auf den Substance-Knoten, um die Eigenschaften zu aktivieren, und laden Sie unter Substance Package Browser eine Substance.

   >[!NOTE]
   >
   > Sie können die .sbsar-Datei auch per Drag &amp; Drop in den Slate Editor ziehen, um den Knoten automatisch zu erstellen und die Sbar zu importieren.
1. Wenn eine Substance mehrere Graphen enthält, können Sie den Graphen, den Sie als Material ausgeben möchten, im Dropdown-Menü Ausgewählter Graph auswählen.

   ![](https://helpx-prod.scene7.com/is/image/HelpxProd/max8?$png$&jpegSize=100&wid=341)

   ![](../../../assets/max1.png)
1. Wählen Sie den Substance-Knoten aus, und wählen Sie im Menü &quot;Substance&quot; einen unterstützten Renderer aus. Das Material wird erstellt und kann auf das Objekt angewendet werden. Substance-Texturen werden in das Rendering-Material eingebunden.

   | Unterstützte Renderer |
   | --- |
   | Arnold |
   | variieren |
   | Corona |
   | Oktan |

   ![](../../../assets/max3.png)

## Ändern der Auflösung:

1. Legen Sie die gewünschte Auflösung für die berechneten Substance-Texturen in den Substance-Ausgabeeinstellungen fest.
1. Stellen Sie bei Auflösungen bis zu 8K sicher, dass Sie das GPU-Modul verwenden, das in den [Substance-Einstellungen](../../../3d-applications/3ds-max/settings-1/substance-settings.md) festgelegt ist.

   ![](../../../assets/max6.png)

## Parameter ändern:

1. Doppelklicken Sie auf den Substance-Knoten, um die Substance-Parameter im Parameterfenster zu laden.
1. Ändern Sie die Parameter, um die Substance-Texturen automatisch zu aktualisieren.

   ![](https://helpx-prod.scene7.com/is/image/HelpxProd/max4?$png$&jpegSize=200&wid=1276){width="500px"}

## Ausgabevorschau festlegen:

Sie können einen bestimmten Kanal für die Miniaturansicht für den Substance-Knoten festlegen.

1. Wählen Sie in der Dropdown-Liste Ausgabevorschau den Kanal aus, den Sie für die Knoten-Miniaturansicht verwenden möchten.

   ![](../../../assets/max7.png)

## Substance kacheln:

Sie können die Eigenschaften &quot;Koordinaten&quot; verwenden, um Substance-Texturen zu kacheln und Kartenkanäle festzulegen.

![](../../../assets/max10.png)
