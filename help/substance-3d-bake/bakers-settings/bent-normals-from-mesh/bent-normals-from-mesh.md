---
helpx_url: "https://helpx.adobe.com/de/substance-3d-bake/bakers-settings/bent-normals-from-mesh.html"
breadcrumb-title: ''
description: Berechnen Sie bent normals-Texturen, die die Durchschnittsrichtung der Umgebungsbeleuchtung bei Meshs mit hohem Poly-Anteil beschreiben.
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Bent Normals from Mesh
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Gebeugte Normale aus Mesh
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 3%

---


# Gebeugte Normale aus Mesh

Die Bent normals aus dem Mesh-Baker berechnen eine Textur, die die Durchschnittsrichtung der Umgebungsbeleuchtung beschreibt. Dieser Baker wird von der [Ambient occlusion vom Mesh](../../bakers-settings/ambient-occlusion-from/ambient-occlusion-from-mesh.md)-Baker abgeleitet.

**Verfügbar in:**

* Painter
* Designer
* Automatisierungs-Toolkit

## Parameter

| *Parameter* | *Beschreibung* |
| --- | --- |
| **Sekundärstrahlen** | Anzahl der Verdeckungen. Ein hoher Wert erzeugt weniger Rauschen, ist aber länger zu berechnen. |
| **Min. Verdeckungsabstand** | Mindestabstand, ab dem die Verdeckungsstrahlen auf die hohe Poly-Geometrie treffen&#x200B;**.** |
| **Max. Verdeckungsabstand** | Maximale Entfernung, in der die Verdeckungsstrahl auf die hohe Poly-Geometrie treffen. |
| **Relativ zum Begrenzungsrahmen** | Wenn diese Option aktiviert ist, basieren die Berechnungen des Strahlenabstands auf dem normalisierten Raum (0 bis 1) des Meshs mit geringer Poly-Intensität. Wenn diese Option deaktiviert ist, basiert die Berechnung des Strahlenabstands auf den Einheiten, die beim Export im Mesh mit niedriger Poly angegeben wurden (m, cm usw.). |
| **Spread Angle** | Maximaler Ausbreitungswinkel der Verdeckungsstrahlen. Der Standardwert ist 180. |
| **Verteilung** | Angular-Verteilung von Okklusionsstrahlen.Mögliche Werte:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Kosinus</strong> (Standard)</li><li data-preserve-html="true"><strong>Einheitlich</strong></li></ul> |
| **Hintergrundfläche ignorieren** | Wenn diese Option aktiviert ist, ignorieren Verdeckungsstrahl Treffer auf einer Rückseite (wenn die hohe Polynormalrichtung in die entgegengesetzte Fläche geht wie die niedrige Polynorm, von der aus der Strahl gebrannt wird). Meistens sollte diese Einstellung aktiviert sein, um Artefakte zu vermeiden. |
| **Selbstverdeckung** | Übereinstimmender Name für die Verdeckung. Gibt an, wie die Bäcker der Low- und High-Poly-Geometrie entsprechen sollen. Es kann verwendet werden, um den Backvorgang zu filtern, ohne dass manuell auseinander (explodieren) Gitter bewegt werden müssen.Mögliche Werte:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Immer</strong> (Standard): Ein solches Gitter wird mit jedem Gitter mit einem hohen Poly-Wert kombiniert.</li><li data-preserve-html="true"><strong>Nach Netzname</strong>: Filtern Sie die Gitter nach ihrem Namen, um eine Übereinstimmung mit unerwünschter Geometrie zu vermeiden.</li></ul>Weitere Informationen zum Anpassen von Geometrien finden Sie unter: [Übereinstimmung nach Name](../../features/matching-by-name/matching-by-name.md). |
| **Zuordnungstyp** | Definiert den Typ der Ausgabetextur.Mögliche Werte:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Welt-Raum</strong></li><li data-preserve-html="true"><strong>Tangentialraum</strong> (Standard)</li></ul> |
| **Normale Ausrichtung** | Steuert das normale Format der Ausgabetextur, wenn **Matttyp** auf &quot;Tangent-Leerzeichen&quot; festgelegt ist.Mögliche Werte:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>OpenGL</strong> <strong> <br/></strong></li><li data-preserve-html="true"><strong>DirectX</strong> (Standard)<strong> <br/></strong></li></ul> |
