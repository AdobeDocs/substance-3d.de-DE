---
helpx_url: "https://helpx.adobe.com/de/substance-3d-bake/bakers-settings/ambient-occlusion-from-mesh.html"
breadcrumb-title: ""
description: Baking präziser ambient occlusion-Texturen von Meshs mit hoher Poly-Qualität unter Verwendung von Raytracing-Techniken für verbesserte Realismus.
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Ambient Occlusion from Mesh
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Ambient occlusion von Mesh
user-guide-description: ""
user-guide-title: ""
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '531'
ht-degree: 2%
---

# Ambient occlusion von Mesh

Das Ambient occlusion von Mesh Baker erlaubt es, eine Ambient occlusion-Textur von hohen Poly-Meshs Baking führen. Sie ist langsamer als der [ambient occlusion](../../bakers-settings/ambient-occlusion/ambient-occlusion.md)-Baker, liefert aber genauere Ergebnisse.

**Verfügbar in:**

* Substance Designer
* Substance Automation Toolkit
* Substance Painter

## Parameter

| *Parameter* | *Beschreibung* |
| --- | --- |
| **Sekundärstrahlen** | Anzahl der Verdeckungsstrahl. Bei einem hohen Wert wird weniger Rauschen erzeugt, die Berechnung dauert jedoch länger. Der Standardwert ist 64. |
| **Min. Verdeckungsabstand** | Mindestabstand, ab dem die Verdeckungsstrahl auf die hohe Poly-Geometrie treffen. Der Standardwert ist 0,00001. |
| **Max. Verdeckungsabstand** | Maximale Entfernung, in der die Verdeckungsstrahl auf die hohe Poly-Geometrie treffen. Der Standardwert ist 0,1. |
| **Relativ zum Begrenzungsrahmen** | Wenn diese Option aktiviert ist, sind die Einheiten relativ zum Begrenzungsrahmen des Objekts (1,0 entspricht der diagonalen Länge des Begrenzungsrahmens). Wenn diese Option deaktiviert ist, werden für den Mindest- und den Höchstwert jeweils die Einheiten verwendet, die beim Exportieren des Meshs definiert werden (Verdeckungsabstand, Zentimeter oder eine beliebige Einheit für die exportierte Szene). |
| **Spread Angle** | Maximaler Ausbreitungswinkel der Verdeckungsstrahlen. Der Standardwert ist 180. |
| **Verteilung** | Angular-Verteilung von Okklusionsstrahlen. Legt fest, wie die Strahlen innerhalb eines Kegels in der Größe des Ausbreitungswinkels gestreut werden.Mögliche Werte:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Kosinus</strong> (Standard): Realistisch, kann aber in sehr dünnen, verdeckten Bereichen zu einer weißen Linie führen. Eignet sich besser für Schattierung und Beleuchtung.</li><li data-preserve-html="true"><strong>Einheitlich</strong>: Nützlich zum Erstellen linearer Farbverläufe. Eignet sich besser für Ebenenmasken und andere Filter.</li></ul> |
| **Hintergrundfläche ignorieren** | Dieser Parameter legt fest, ob die Strahlen der Verdeckung die Treffer auf der Rückseite ignorieren (wenn die hohe Polynormalität in die entgegengesetzte Richtung weist wie die niedrige Polynormalität, von der aus der Strahl gebrannt wird). Meistens sollte diese Einstellung aktiviert sein, um Artefakte zu vermeiden. Mögliche Werte:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Nie</strong> (Standard): Hintergründe werden nie ignoriert.</li><li data-preserve-html="true"><strong>Immer</strong>: Flächen werden immer ignoriert.</li><li data-preserve-html="true"><strong>Nach Netzname</strong>: Rückseiten werden nur für Gitter ignoriert, die mit dem Schlüsselwort des Suffix übereinstimmen. Weitere Informationen finden Sie in den [allgemeinen Parametern](../../bakers-settings/common-parameters/common-parameters.md).</li></ul> |
| **Selbstverdeckung** | Übereinstimmender Name für die Verdeckung. Gibt an, wie die Bäcker der Low- und High-Poly-Geometrie entsprechen sollen. Es kann verwendet werden, um den Backvorgang zu filtern, ohne dass manuell auseinander (explodieren) Gitter bewegt werden müssen.Mögliche Werte:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Immer</strong> (Standard): Ein solches Gitter wird mit jedem Gitter mit einem hohen Poly-Wert kombiniert.</li><li data-preserve-html="true"><strong>Nach Netzname</strong>: Filtern Sie die Gitter nach ihrem Namen, um eine Übereinstimmung mit unerwünschter Geometrie zu vermeiden.</li></ul>Weitere Informationen zum Anpassen von Geometrien finden Sie unter: [Übereinstimmung nach Name](../../features/matching-by-name/matching-by-name.md). |
| **Normale Karte** | Optionaler Pfad zu einer normalen Textur. Kann verwendet werden, um die interne Berechnung des Bakers zu ersetzen. |
| **Welt-Raum** | Wenn diese Option aktiviert ist, wird die normale Textur als Welt-Raum-Normale statt als Tangentialraum interpretiert. |
| **Normale Ausrichtung** | Format der Textur &quot;Normal&quot;, wenn in Tangentialraum.Mögliche Werte:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>DirectX</strong> (Standard)</li><li data-preserve-html="true"><strong>OpenGL</strong></li></ul> |
| **Dämpfung** | Definiert, wie die Verdeckung durch Verdeckungsabstand gedämpft wird.Mögliche Werte:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Keine</strong>: keine Dämpfung.</li><li data-preserve-html="true"><strong>Linear</strong> (Standard) : Dämpfung.</li><li data-preserve-html="true"><strong>Glatt</strong>: weiche Dämpfung.</li></ul> |
| **Boden-Ebene** | Wenn diese Option aktiviert ist, simulieren Sie eine Ebene unter dem Mesh-Begrenzungsrahmen auf der XZ-Achse, um mit Sekundärstrahlen zu kollidieren. Dies simuliert Schatten, die von einem unsichtbaren Grundriss kommen. |
| **Offset der Boden-Ebene** | Ermöglicht eine Verschiebung des Plans vom Mesh weg, um die Effektintensität zu reduzieren. Der Wert ist absolut und nicht relativ zur Größe des Meshs. |
