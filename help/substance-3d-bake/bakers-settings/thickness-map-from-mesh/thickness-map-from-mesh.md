---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/bakers-settings/thickness-map-from-mesh.html"
breadcrumb-title: ''
description: Generiere Dicken-Map, indem du Strahlen von Mesh-Oberflächen nach innen Wirft, um sie in SSS-Shadern und Maskierungen zu verwenden.
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Thickness Map from Mesh
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Stärke-Map aus Mesh
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 5%

---


# Stärke-Map aus Mesh

Die Dicken-Map aus Mesh ist dem ambient occlusion-Baker sehr ähnlich, Wirft aber Strahlen von der Oberfläche des Meshs nach innen. Diese Textur kann in einem Sub Surface Scattering (SSS)-Shader oder zum Maskieren von Texturen verwendet werden.

Die Textureigenschaften sind wie folgt definiert:

* Schwarze Werte stellen die schmalen Teile des Modells dar.
* Weiße Werte stellen die dicken Teile des Modells dar.

**Verfügbar in:**

* Substance Painter
* Substance Designer
* Substance Automation Toolkit

## Parameter

| *Parameter* | *Beschreibung* |
| --- | --- |
| **Sekundärstrahlen** | Anzahl der Verdeckungen. Bei einem hohen Wert wird weniger Rauschen erzeugt, die Berechnung dauert jedoch länger. Der Standardwert ist 64. |
| **Min. Verdeckungsabstand** | Mindestabstand, ab dem die Verdeckungsstrahl auf die hohe Poly-Geometrie treffen. Der Standardwert ist 0,00001. |
| **Max. Verdeckungsabstand** | Maximale Entfernung, in der die Verdeckungsstrahl auf die hohe Poly-Geometrie treffen. Der Standardwert ist 0,1. |
| **Relativ zum Begrenzungsrahmen** | Wenn diese Option aktiviert ist, sind die Einheiten relativ zum Begrenzungsrahmen des Objekts (1,0 entspricht der diagonalen Länge des Begrenzungsrahmens). Wenn diese Option deaktiviert ist, werden für den Mindest- und den Höchstwert jeweils die Einheiten verwendet, die beim Exportieren des Meshs definiert werden (Verdeckungsabstand, Zentimeter oder eine beliebige Einheit für die exportierte Szene). |
| **Spread Angle** | Maximaler Ausbreitungswinkel der Verdeckungsstrahlen. Der Standardwert ist 180. |
| **Verteilung** | Angular-Verteilung von Okklusionsstrahlen.Mögliche Werte:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Kosinus</strong> (Standard)</li><li data-preserve-html="true"><strong>Einheitlich</strong></li></ul> |
| **Hintergrundfläche ignorieren** | Wenn diese Option aktiviert ist, ignorieren Verdeckungsstrahl Treffer auf einer Rückseite (wenn die hohe Polynormalrichtung in die entgegengesetzte Fläche geht wie die niedrige Polynorm, von der aus der Strahl gebrannt wird). Meistens sollte diese Einstellung aktiviert sein, um Artefakte zu vermeiden. |
| **Selbstverdeckung** | Übereinstimmender Name für die Verdeckung. Gibt an, wie die Bäcker der Low- und High-Poly-Geometrie entsprechen sollen. Es kann verwendet werden, um den Backvorgang zu filtern, ohne dass manuell auseinander (explodieren) Gitter bewegt werden müssen.Mögliche Werte:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Immer</strong> (Standard): Ein solches Gitter wird mit jedem Gitter mit einem hohen Poly-Wert kombiniert.</li><li data-preserve-html="true"><strong>Nach Netzname</strong>: Filtern Sie die Gitter nach ihrem Namen, um eine Übereinstimmung mit unerwünschter Geometrie zu vermeiden.</li></ul>Weitere Informationen zum Anpassen von Geometrien finden Sie unter: [Übereinstimmung nach Name](../../features/matching-by-name/matching-by-name.md). |
| **Automatische Normalisierung** | Legt fest, ob die Ausgabewerte so skaliert werden sollen, dass sie in einen Bereich von 0 bis 1 passen (der hellste Punkt wird auf reinweiß und der dunkelste Punkt auf reinschwarz gesetzt). |
