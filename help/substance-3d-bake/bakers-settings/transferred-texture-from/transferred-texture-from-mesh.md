---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/bakers-settings/transferred-texture-from-mesh.html"
breadcrumb-title: ''
description: Übertragen Sie Texturen zwischen Netzen basierend auf ihren UVs, einschließlich Unterstützung für normale Map-Konvertierungen.
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Transferred Texture from Mesh
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Textur aus Mesh übertragen
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '238'
ht-degree: 3%

---


# Textur aus Mesh übertragen

Die übertragene Textur von mesh baker ermöglicht die Konvertierung einer Textur von einem Mesh in ein anderes basierend auf ihren jeweiligen UVs. Dieser Bäcker unterstützt auch die Übertragung oder normale Karten (die besondere Konvertierungen erfordern). Um zu funktionieren, benötigen beide Gitter UV-Definitionen.

**Verfügbar in:**

* Substance Designer
* Substance Automation Toolkit

## Parameter

| *Parameter* | *Beschreibung* |
| --- | --- |
| **Texturdatei** | Pfad zur Eingabetexturdatei, die übertragen wird. |
| **UV-Satz** | Gitter-UVs, die auf dem High-Poly-Gitter verwendet werden, um die Textur zu lesen und auf das Low-Poly-Gitter zu projizieren. |
| **Filtermodus** | Definiert, wie die Pixelinterpolation der Textur erfolgen soll.Mögliche Werte:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Nächste</strong>: Keine Interpolation, verwenden Sie das Pixel, das einer bestimmten Position am nächsten kommt. Präzise Aliasing-Effekte.</li><li data-preserve-html="true"><strong>Bilinear</strong> (Standard): Verwenden Sie die vier nächstgelegenen Pixel für eine bestimmte Position. Kein Aliasing, kann aber unscharf sein.</li></ul> |
| **Normale Karte** | Wenn diese Option aktiviert ist, wird der Bäcker darauf hingewiesen, dass die zu übertragende Eingabetextur eine normale Map ist. Dies weist den Bäcker an, besondere Konvertierungen auf die Textur anzuwenden, um sie mit dem Zielgitter kompatibel zu machen. |
| **Zuordnungstyp** | Definiert den Typ der Normalmap für die Eingabetextur.Mögliche Werte:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Weltraum</strong></li><li data-preserve-html="true"><strong>Tangentialraum</strong> (Standard)</li></ul> |
| **Normale Ausrichtung** | Definiert das Normalformat der Eingabe-Textur, wenn **Zuordnungstyp** auf **Tangentialraum** festgelegt ist.Mögliche Werte:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>OpenGL</strong></li><li data-preserve-html="true"><strong>DirectX</strong> (Standard)</li></ul> |
