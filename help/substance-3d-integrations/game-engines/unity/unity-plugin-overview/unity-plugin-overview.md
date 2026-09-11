---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/unity-plugin-overview.html"
breadcrumb-title: ''
description: Informieren Sie sich über das Substance 3D-Plug-in für Unity, einschließlich Versionsunterstützung, Funktionen und Integrationsfunktionen.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Plugin Overview
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Unity-Plug-in - Übersicht
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 0%

---


# Unity-Plug-in - Übersicht

## Unterstützung für Unity-Versionen

Das Adobe Substance 3D für Unity Plugin Version 3.0.0 unterstützt derzeit Unity 2020 LTS und höher.

## Herunterladen des Substance-Pakets

1. Das Plug-in kann aus dem Unity Asset Store heruntergeladen werden: <https://assetstore.unity.com/packages/tools/utilities/substance-3d-for-unity-beta-213208>

## Importieren von Substance-Material

1. Klicken Sie mit der rechten Maustaste auf das Projektfenster und wählen Sie &quot;Element importieren&quot;, oder ziehen Sie das Substance-Material, das Sie importieren möchten, in das Bedienfeld &quot;Projektansicht&quot;.
1. Suchen Sie nach dem Substance-Material, das Sie importieren möchten. Substance-Material haben die Dateierweiterung &quot;.sbsar&quot;.
1. Das Substance-Material wird in Ihr Unity-Projekt importiert.

   1. Das Unterelement erstellt eine Hauptimportdatei und einen Ordner mit den Ausgabeordnern und einem generierten Unity-Material. Texturen
1. Anschließend können Sie das Material per Drag-and-Drop auf einen Mesh in der Parameteransicht ziehen und die Szenen dann im Inspektor bearbeiten.

   ![](../../../assets/window-overview.png){width="1000px"}

>[!NOTE]
>
> **Normalen-Map-Konvertierung**
> 
> Das Substance in Unity-Plug-in konvertiert DirectX automatisch in OpenGL. Wenn Sie Materialien aus [Substance Source](https://source.substance3d.com/) verwenden, müssen Sie die normale Ausrichtung nicht in &quot;OGL&quot; ändern. Wenn Sie in Substance Designer Ihr eigenes Material erstellen, sollten Sie unbedingt mit dem Standard-DirectX-Shader arbeiten, da das Plugin die normale Konvertierung automatisch verarbeitet. Weitere Informationen finden Sie unter Arbeiten mit Normalen in Unity.

## Parameter ändern

Parameter und Auflösungen können im Eigenschafteninspektor eingestellt werden. Siehe [Parameter ändern](../../../game-engines/unity/changing-parameters/changing-parameters.md).

[unity\_tweaking\_parameters.mp4](https://helpx.adobe.com/content/dam/help/en/substance-3d/documentation/download/attachments/186056716/unity-tweaking-parameters.mp4)

## Unterstützung für Unity-Render-Pipeline

Das Substance 3D-Plugin unterstützt HDRP und URP. Weitere Informationen werden in Kürze verfügbar sein.

## Anleitung
