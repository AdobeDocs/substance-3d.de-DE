---
helpx_url: "https://helpx.adobe.com/de/substance-3d-integrations/3d-applications/maya/using-workflows.html"
breadcrumb-title: ""
description: Erstellen und verwenden Sie Render-Vorgaben für Substance-Ausgaben in Maya, um automatisch Shader-Netzwerke für verschiedene Renderer zu generieren.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Maya > Using Workflows
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Verwenden von Workflows
user-guide-description: ""
user-guide-title: ""
source-git-commit: 28a9d8cf7a4eed4163f99e8158c9cb8f9da88302
workflow-type: tm+mt
source-wordcount: '568'
ht-degree: 0%
---

# Verwenden von Workflows

Unter Workflows können Sie Render-Vorgaben für Substance-Ausgaben auswählen oder erstellen. Diese Vorgaben sind Shader-Netzwerke für einen Renderer wie Arnold oder Vray.

>[!NOTE]
>
> **Speicherort der Workflowvorgabe**
>
> **Windows**:
> C:\Users\\Documents\maya\2022\substance\workflows\generated
> **MacOS**:
> /Benutzer//Library/Preferences/Autodesk/maya//substance/workflows/generated
> **Linux**:
> /home/maya/content/workflows/generated

![](../../../assets/maya-max-v3-1/maya-all-presets.png)

Um einen Arbeitsablauf zu verwenden, wählen Sie einfach die Vorgabe aus der Liste aus und klicken Sie dann auf die Schaltfläche Netzwerk erstellen .

![](../../../assets/workflow.gif)

## Erstellen eines Workflows

Sie können Ihren eigenen Arbeitsablauf erstellen und ihn der Liste Renderer-Arbeitsablauf hinzufügen. Beim Hinzufügen eines neuen Workflows werden alle Knoten, die nach dem Substance-Knoten erstellt wurden, im Workflow gespeichert. Auf diese Weise können Sie eine beliebige Anzahl von Schattierung-Nodes erstellen, um ein vollständiges benutzerdefiniertes Shader-Netzwerk zu erstellen, das als voreingestellter Workflow gespeichert werden kann.

![](../../../assets/saved-workflow.png)

## Workflows verwalten

### Speichern benutzerdefinierter Workflows

1. Erstellen Sie manuell Substance-Ausgänge und verbinden Sie sie mit einem Material wie aiStandardSurface.
   1. Sie können beliebige Maya- oder Renderknoten verwenden, um das Shader-Netzwerk zu erstellen.
1. Klicken Sie auf die Schaltfläche **Arbeitsablauf erstellen**, und geben Sie einen Namen für die Arbeitsablaufvorgabe ein.

### Duplizieren von Workflows

Sie können einen Arbeitsablauf duplizieren, indem Sie auf die Schaltfläche **Arbeitsablauf duplizieren** klicken.

### Arbeitsabläufe zum Umbenennen und Überschreiben

Sie können vorhandene Workflows umbenennen und Workflows mit aktualisierten Daten überschreiben, indem Sie die Schaltflächen **Umbenennen** und **Überschreiben** verwenden.

### Entfernen von Workflows

Sie können vorhandene Workflows entfernen, indem Sie die Schaltfläche &quot;Arbeitsablauf entfernen&quot; verwenden.

## OpenPBR Workflows

In der Liste &quot;Workflows&quot; sind zwei OpenPBR-Workflows verfügbar: **OpenPBR** und **OpenPBR - V-Ray**. Diese Arbeitsabläufe wurden für die Verwendung mit SBSAR-Dateien entwickelt, die mit dem OpenPBR-Materialmodell in Substance 3D Designer oder Sampler erstellt wurden (OpenPBR ist seit Designer V16.0+ und Sampler V6.0+ das Standardmodell).

### Was ist OpenPBR?

OpenPBR ist ein offenes, physikalisch basiertes Material-Schattierung-Modell, das von Adobe und Autodesk entwickelt wurde und an der Academy Software Foundation (ASWF) mitwirkte. Es bietet eine einheitliche Material-Definition, die mit allen Renderern kompatibel ist. Weitere Informationen finden Sie in der [OpenPBR-Dokumentation](https://experienceleague.adobe.com/de/docs/substance-3d/general-knowledge/openpbr/openpbr-overview).

### Wann sollte ein OpenPBR-Arbeitsablauf verwendet werden?

Verwenden Sie einen OpenPBR-Arbeitsablauf, wenn Ihre Sbsar-Dateien über das OpenPBR-Materialmodell in Substance 3D Designer oder Substance 3D Sampler erstellt wurden. Wenn Ihre SBSAR-Datei mit Adobe Standard Materialmodell (ASM) erstellt wurde, verwenden Sie den älteren Arbeitsablauf, der mit Ihrem Renderer kompatibel ist (Arnold, V-Ray oder V-Ray 6).

>[!NOTE]
>
> Wenn Sie einen OpenPBR-Workflow auf ein ASM-Material oder einen Standardarbeitsablauf auf ein OpenPBR-SBSAR anwenden, verbindet das Plug-In nur Ausgaben, die beiden Materialmodellen gemeinsam sind. Das Ergebnis ist möglicherweise unvollständig.

### Verfügbare OpenPBR-Workflows

**OpenPBR**

Verwendet den nativen Maya openPBRSurface-Knoten. Kompatibel mit Arnold und V-Ray. Dies ist der empfohlene Arbeitsablauf für die meisten Benutzer, die mit OpenPBR-Materialien in Maya arbeiten.

**OpenPBR - V-Ray**

Verwendet das V-Ray-Material (VRayMtl) im OpenPBR-Modus. Empfohlen für Benutzer, deren Pipeline speziell um V-Ray-Material-Setups herum aufgebaut ist.

### Anwenden eines OpenPBR-Workflows

1. Laden Sie Ihre Sbsar-Dateien über die Schaltfläche &quot;Substance laden&quot; in das Plug-in.
1. Wählen Sie in der Liste Workflows **OpenPBR** oder **OpenPBR - V-Ray** aus.
1. Klicken Sie auf **Netzwerk erstellen**, um das Shader-Netzwerk im **Hypershade Material Editor** zu erstellen.
1. Das Plug-in verbindet die SBSAR-Ausgänge automatisch mit den entsprechenden Eingängen des OpenPBR-Nodes.
1. Weisen Sie das Material wie gewohnt Ihrem Mesh zu.

![](../../../assets/maya-max-v3-1/maya-openpbr-overview.png)
