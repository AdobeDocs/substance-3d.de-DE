---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/renderers/corona.html"
breadcrumb-title: ''
description: Verwenden Sie Substance-Materialien mit dem Corona-Renderer in 3ds Max mit dem Specular/Glossiness-Workflow und den erforderlichen Maps.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Corona
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Corona
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 1%

---


# Corona

Für das Rendering mit Corona können Sie Karten verwenden, die aus Substance Painter oder dem Substance-Plugin exportiert wurden. Corona verwendet den Specular/Glossiness-Workflow mit einer 1/IOR-Karte. Sie benötigen die folgenden Karten:

* Diffus
* Reflexion (Specular)
* Glanz
* 1/IOR (konvertiert)

Die 1/IOR-Map kann nur aus dem Metall-/Raueit-Workflow konvertiert werden, der der Standardarbeitsablauf sowohl in Substance Designer als auch in Substance Painter ist.

1. Exportieren Sie Maps aus dem Substance Painter mit der Voreinstellung &quot;Corona&quot;.
1. Bei benutzerdefinierten Substance können Sie den konvertierten Knoten basecolor\_metallic\_rauigkeit, der auf die Vorgabe &quot;Variieren&quot; festgelegt ist, verwenden, um die benutzerdefinierten Ausgaben zu erstellen.
1. Für 3ds Max und Cinema 4D verwenden Sie ein Corona-Material mit Ebenen, um metallische und dielektrische Materialien zu verarbeiten und die Notwendigkeit der Konvertierung einer 1/IOR-Karte zu umgehen.

## Inhaltsverzeichnis

* [Corona für 3ds Max](../../renderers/corona/corona-for-3ds-max/corona-for-3ds-max.md)
* [Corona - Substance Painter](../../renderers/corona/corona-painter/corona-substance-painter.md)
