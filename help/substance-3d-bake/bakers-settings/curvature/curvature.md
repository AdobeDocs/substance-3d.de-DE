---
helpx_url: "https://helpx.adobe.com/de/substance-3d-bake/bakers-settings/curvature.html"
breadcrumb-title: ''
description: Extrahieren Sie Krümmungsinformationen aus Ihrem Gitter, um Texturen zu erstellen, die Hohlräume und Kanten Ihrer Geometrie hervorheben.
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Curvature
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Biegung
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 3%

---


# Biegung

Mit dem Kurvenzeichner-Werkzeug kannst du eine Krümmungsstruktur extrahieren. Diese Textur enthält Informationen zu Hohlräumen und Kanten, die sich auf die Geometrie beziehen.

Die Textureigenschaften sind wie folgt definiert:

* Schwarze Werte stellen konkave Bereiche dar.
* Weiße Werte stellen konvexe Bereiche dar.
* Grauwerte stellen neutrale Bereiche dar (überwiegend flach).

**Verfügbar in:**

* Substance Designer
* Substance Automation Toolkit
* Substance Painter

## Parameter

| *Parameter* | *Beschreibung* |
| --- | --- |
| **Algorithmus** | Legt fest, wie die Krümmungsinformationen im Gitter berechnet werden. |
| **Details** | Legt fest, wie stark die Informationen in der Krümmung sein werden. Ein hoher Wert kann mehr Details erzeugen, aber weniger subtil. |
| **Seams aktivieren** | Wenn diese Option aktiviert ist, versucht der Bäcker, die Nahtstellen zwischen den UV-Inseln zu reduzieren, indem er die Texel an den Rändern von einer Seite zur anderen kopiert. |
| **Nähte** **Intensität** | Wenn **Nähte aktivieren** aktiviert ist, steuert dieser Parameter die Stärke der Nahtfixierung. |
