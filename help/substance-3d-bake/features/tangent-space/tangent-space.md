---
helpx_url: "https://helpx.adobe.com/de/substance-3d-bake/features/tangent-space.html"
breadcrumb-title: ''
description: Erfahre, wie Substance Bakers die Berechnung des Tangente-Raums anwendet und den Algorithmus an deinen Workflow anpasst.
helpx_creative_field: ""
helpx_description: bakers > Features > Tangent Space
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Tangentialraum
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 2%

---


# Tangentialraum

Substance Baker können entweder die auf dem Mesh mit niedrigem Poly-Anteil vorhandenen Tangenten und Binormale laden oder sie neu berechnen. Bei der Neuberechnung kann ein benutzerdefinierter Tangentialraum-Algorithmus (standardmäßig MikkTSpace) definiert werden.

## Liste der Tangentialraum-Plug-ins

## Substance Painter

Substance Painters die Tangentialraum-Plug-in nicht geändert werden kann, ist sie immer **MikkTSpace**. Es gibt jedoch einen Parameter, mit dem sich das Verhalten leicht ändern lässt, um die Kompatibilität mit anderen Anwendungen zu gewährleisten:

| *Parameter* | *Kompatibel* *Anwendung* |
| --- | --- |
| **Tangente-Speicherplatz pro Fragment berechnen: Deaktiviert** | Kompatibel mit xNormal, Unity 5.3 oder höher. |
| **Tangente-Speicherplatz pro Fragment berechnen: Aktiviert** | Kompatibel mit den Workflows Unreal Engine 4, Blender und Unity HDRP. |

## Substance Designer

Substance Designer unterstützt den folgenden Algorithmus:

| *Dateiname* | *Beschreibung* |
| --- | --- |
| **mikktspace.dll** | MikkTSpace, Tangentialraum-Algorithmus auf Basis von Morten S. Mikkelsen Arbeit.Kompatibel mit xNormal, Unity 5.3 oder höher. |
| **mikkunrealtspace.dll** | MikkTSpace, Tangentialraum-Algorithmus auf Basis von Morten S. Mikkelsen Arbeit.Kompatibel mit den Workflows Unreal Engine 4, Blender und Unity HDRP. |
| **unityspace.dll** | Tangentialraum-Algorithmus auf Basis von Unity 4. |

>[!NOTE]
>
> Es ist möglich, eine benutzerdefinierte Tangentialraum-Plug-in zu schreiben. Eine Headerdatei mit dem Namen **tangentspaceplugin.h** ist im Installationsordner unter **Substance Designer/SDK/tangentspace** verfügbar und kann als Schnittstelle verwendet werden.

## Festlegen eines benutzerdefinierten Tangentialraums

## Substance Painter

Substance Painter unterstützt derzeit keine benutzerdefinierten Tangentialraum-Plug-ins. Dies bedeutet, dass Tangenten und Binormalitäten, die auf dem Low-Poly-Mesh (der zum Erstellen des Projekts verwendet wird) nicht vorhanden sind, auf der Grundlage des MikkTSpace-Algorithmus neu berechnet werden.

## Substance Designer

Gehen Sie wie folgt vor, um den Algorithmus für den Tangente-Raum im Substance Designer festzulegen:

1. Wählen Sie **Bearbeiten** > **Voreinstellungen**.

   ![](../../assets/sd-edit-pref.png)
1. Klicken Sie auf **Projekte**.

   ![](../../assets/sd-pref-projects.png)
1. Navigieren Sie zur Registerkarte **Allgemein**. Scrollen Sie, bis der Abschnitt **3D-Szenen** sichtbar ist.

   ![](../../assets/sd-tab-general.png)
1. Klicken Sie auf die **drei Punkte** (...) , um ein benutzerdefiniertes Plug-in zu laden.

## Substance Automation Toolkit

Beim Baking mit dem Automation Toolkit ist es möglich, die Tangentialraum-Plug-in mit einem bestimmten Befehlszeilenargument anzugeben:

```
sbsbaker normal-from-mesh --tangent-space-plugin "C:/Substance Designer/plugins⁄tangentspace⁄mikktspace.dll" ...
```
