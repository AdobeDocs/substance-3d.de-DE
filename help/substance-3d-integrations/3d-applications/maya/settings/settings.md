---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/maya/settings.html"
breadcrumb-title: ''
description: Konfigurieren Sie die Substance-Plugin-Einstellungen in Maya über das Substance-Shelf oder das Menü, um das Verhalten anzupassen.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Maya > Settings
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Einstellungen
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 1%

---


# Einstellungen

Das Substance-Einstellungsmenü kann über das Substance-Shelf oder das Substance-Menü aufgerufen werden. Die Einstellungen für dieses Menü werden in einer editierbaren Konfigurationsdatei &quot;substance.cfg&quot; gespeichert.

>[!NOTE]
>
> **Speicherorte für Konfigurationsdateien**
> 
> **Windows**:\
> C:\Users\\Documents\maya\\substance\\
> **MacOS**:\
> /Users//Library/Preferences/Autodesk/maya//substance/\
> **Linux**:\
> /home/maya/de/substance/

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

## Standardauflösung

Legt die Standardauflösung für einen Substance-Knoten fest, wenn die SBSAR-Datei geladen wird.

## Arbeitsablauf beim Rendern

Legt den standardmäßigen Rendering-Arbeitsablauf fest, der auf dem Substance-Knoten verwendet wird.

## Substance-Engine

Festlegen von Voreinstellungen für das Substance Engine und global für alle Substance-Knoten. Die Substance-Engine wird zur Berechnung der Substance-Texturen verwendet.

### Motortyp

Das Substance Engine ist als CPU- und GPU-Engine verfügbar. Um den Motor zu wechseln, muss Maya neu gestartet werden. Die GPU-Engine ermöglicht eine höhere Auflösung als die CPU-Engine.

>[!WARNING]
>
> Es kann Unterschiede zwischen der CPU und der GPU-Engine geben. Für konsistente Ergebnisse ist es daher am besten, den Typ auf die gleiche Engine festzulegen, die auch im Substance Designer verwendet wird.

Die CPU-Kerne und der Engine-Speicher sind Einstellungen für die Menge an Ressourcen, die die Substance-Engine verwenden darf.

### Blockieren von Renderings

Mit dieser Option können Sie festlegen, ob der Substance-Engine-Compute die Maya-UI-Prozesse blockiert. Wenn diese Option aktiviert ist, hat die Substance-Engine Vorrang und blockiert die Maya-UI-Prozesse. Wenn diese Option deaktiviert ist, werden die Maya-Benutzeroberflächenprozesse nicht durch Substance-Engine-Berechnungen blockiert.

## Cache-Ausgaben auf Festplatte

Legt den Standardspeicherort, den Dateityp und den Cacheordner für alle neu erstellten Substance-Knoten in einem Projekt fest.

## Rendererweiterungen

Aktivieren Sie Rendering-Erweiterungen, um Substance-Ausgaben direkt mit Arnold Shaders zu verwenden.

## Physische Größe

Aktivieren Sie diese Option, wenn die Physische Größe standardmäßig verwendet werden soll, wenn sbsar-Dateien geladen werden und wenn sie beim erneuten Laden des sbsar neu berechnet werden soll.

</td>
<td style="border: 0;" valign="top">

![](../../../assets/settings-35.png)

</td>
</tr>
</table>
