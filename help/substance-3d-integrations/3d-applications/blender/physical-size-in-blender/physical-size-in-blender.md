---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/blender/physical-size-in-blender.html"
breadcrumb-title: ''
description: Verwenden Sie die Physische Größe-Einstellungen, um Substance-Materialien in Blender basierend auf den realen Abmessungen zu skalieren.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Blender > Physical size in Blender
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Physische Größe in Blender
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 0%

---


# Physische Größe in Blender

Physische Größe in Substance-Materialien ermöglicht die Skalierung von Materialien auf Basis ihrer Größe in der Welt. Die Abmessungen werden in Substance-Applikationen wie Designer festgelegt und im Abschnitt &quot;Physische Größe&quot; des Plug-in-Bedienfelds angezeigt.

![](../../../assets/blender-physical-size.png)

Wenn die Physische Größe aktiviert ist, werden die Materialien entsprechend ihrer tatsächlichen Größe in Zentimetern unterteilt. Die Kachelung des Materials bleibt unabhängig von der Größe des Objekts gleich. Die Funktion kann aktiviert werden, indem zum Physische Größe-Shader im Add-On-Bedienfeld gewechselt wird. Nachdem Sie die Skalierung eines Objekts angepasst haben, sollte die Skalierung mit Strg/Befehl+A angewendet werden, um die Textur der Physische Größe exakt zu kacheln.

## Anpassen der Physische Größe

Die Werte im Zuordnungsknoten können für die künstlerische Kontrolle über die Kachelung der Physische Größe angepasst werden. Darüber hinaus kann ein Objekt wie z. B. Leer für die Textur-Koordinateneingabe verwendet werden, um die Textur-Zuordnung mithilfe der Transformationen des Eingabeobjekts zu steuern (siehe Beispiel unten).

![](../../../assets/blender-physical-szie-empty.gif)
