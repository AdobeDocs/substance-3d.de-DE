---
helpx_url: "https://helpx.adobe.com/de/substance-3d-bake/features/tangent-space.html"
breadcrumb-title: ''
description: Erfahre, wie Substance Baker die Berechnung des Tangentenraums verarbeitet und den Algorithmus für deinen Workflow anpasst.
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

Substance Baker können die vorhandenen Tangenten und Binormale auf das Gitter mit geringer Poly-Zahl laden oder neu berechnen. Bei der Neuberechnung kann ein benutzerdefinierter Tangent-Space-Algorithmus definiert werden (standardmäßig MikkTSpace).

## Tangent-Leerzeichen-Zusatzmodulliste

## Substance Painter

Substance Painters das Tangent-Space-Plug-in nicht geändert werden kann, lautet es immer **MikkTSpace**. Es gibt jedoch einen Parameter, mit dem sich das Verhalten leicht ändern lässt, um die Kompatibilität mit anderen Anwendungen zu gewährleisten:

| *Parameter* | *Kompatibel* *Anwendung* |
| --- | --- |
| **Tangentenraum pro Fragment berechnen: Deaktiviert** | Kompatibel mit xNormal, Unity 5.3 oder höher. |
| **Tangentenraum pro Fragment berechnen: Aktiviert** | Kompatibel mit Unreal Engine 4, Blender und Unity HDRP-Arbeitsablauf. |

## Substance Designer

Substance Designer unterstützt den folgenden Algorithmus:

| *Dateiname* | *Beschreibung* |
| --- | --- |
| **mikktspace.dll** | MikkTSpace, Tangent Space Algorithmus basiert auf Morten S. Mikkelsen Arbeit.Kompatibel mit xNormal, Unity 5.3 oder höher. |
| **mikkunrealtspace.dll** | MikkTSpace, Tangent Space Algorithmus basiert auf Morten S. Mikkelsen Arbeit.Kompatibel mit Unreal Engine 4, Blender und Unity HDRP-Arbeitsablauf. |
| **unityspace.dll** | Tangent-Space-Algorithmus basierend auf Unity 4. |

>[!NOTE]
>
> Es ist möglich, ein benutzerdefiniertes Tangent Space-Plug-in zu schreiben. Eine Headerdatei mit dem Namen **tangentspaceplugin.h** ist im Installationsordner unter **Substance Designer/SDK/tangentspace** verfügbar und kann als Schnittstelle verwendet werden.

## Festlegen eines benutzerdefinierten Tangentialraums

## Substance Painter

Substance Painter unterstützt derzeit keine benutzerdefinierten Tangent-Space-Plug-ins. Dies bedeutet, dass Tangents und Binormalitäten, die nicht auf dem Low-Poly-Gitter (verwendet, um das Projekt zu erstellen) vorhanden sind, auf der Grundlage des MikkTSpace-Algorithmus neu berechnet werden.

## Substance Designer

So legen Sie den Tangentenraumalgorithmus im Substance Designer fest:

1. Wählen Sie **Bearbeiten** > **Voreinstellungen**.

   ![](../../assets/sd-edit-pref.png)
1. Klicken Sie auf **Projekte**.

   ![](../../assets/sd-pref-projects.png)
1. Navigieren Sie zur Registerkarte **Allgemein**. Scrollen Sie, bis der Abschnitt **3D-Szenen** sichtbar ist.

   ![](../../assets/sd-tab-general.png)
1. Klicken Sie auf die **drei Punkte** (...) , um ein benutzerdefiniertes Plug-in zu laden.

## Substance Automation Toolkit

Beim Backen mit dem Automation Toolkit ist es möglich, das Tangent Space-Plug-in mit einem bestimmten Befehlszeilenargument anzugeben:

```
sbsbaker normal-from-mesh --tangent-space-plugin "C:/Substance Designer/plugins⁄tangentspace⁄mikktspace.dll" ...
```
