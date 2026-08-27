---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/bakers-settings/ambient-occlusion-from-mesh.html"
breadcrumb-title: ''
description: Mit Raytracing-Techniken lassen sich realitätsgetreue Strukturen in der Verdeckung aus hochpolaren Meshes erzeugen.
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Ambient Occlusion from Mesh
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Umgebende Verdeckung aus Mesh
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '531'
ht-degree: 2%

---


# Umgebende Verdeckung aus Mesh

Die Ambient Verdeckung von Mesh Baker ermöglicht es, eine Ambient Verdeckung Textur aus hohen Poly-Meshes zu backen. Es ist langsamer als die [Umgebungs-Verdeckung](../../bakers-settings/ambient-occlusion/ambient-occlusion.md), liefert jedoch präzisere Ergebnisse.

**Verfügbar in:**

* Substance Designer
* Substance Automation Toolkit
* Substance Painter

## Parameter

| *Parameter* | *Beschreibung* |
| --- | --- |
| **Sekundärstrahlen** | Anzahl der Verdeckungen. Ein hoher Wert erzeugt weniger Rauschen, die Berechnung dauert jedoch länger. Der Standardwert ist 64. |
| **Min. Okcluderentfernung** | Mindestabstand, ab dem die Strahlen der Verdeckung auf die hohe Polygeometrie treffen. Der Standardwert ist 0,00001. |
| **Max. Okcluderentfernung** | Maximale Entfernung zwischen den Strahlen der Verdeckung und der hohen Polygeometrie. Der Standardwert ist 0,1. |
| **Relativ zum Begrenzungsrahmen** | Wenn diese Option aktiviert ist, sind die Einheiten relativ zum Begrenzungsrahmen des Objekts (1,0 entspricht der diagonalen Länge des Begrenzungsrahmens). Wenn diese Option deaktiviert ist, werden für die minimalen und maximalen Okklusionsabstände die Einheiten verwendet, die beim Exportieren des Gitters definiert werden (Meter, Zentimeter oder die beliebige Einheit der exportierten Szene). |
| **Spread Angle** | Maximaler Ausbreitungswinkel der Verdeckungsstrahlen. Der Standardwert ist 180. |
| **Verteilung** | Angular-Verteilung von Okklusionsstrahlen. Legt fest, wie die Strahlen innerhalb eines Kegels in der Größe des Ausbreitungswinkels gestreut werden.Mögliche Werte:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Kosinus</strong> (Standard): Realistisch, kann aber in sehr dünnen, verdeckten Bereichen zu einer weißen Linie führen. Eignet sich besser für Schattierung und Beleuchtung.</li><li data-preserve-html="true"><strong>Einheitlich</strong>: Nützlich zum Erstellen linearer Farbverläufe. Eignet sich besser für Ebenenmasken und andere Filter.</li></ul> |
| **Hintergrundfläche ignorieren** | Dieser Parameter legt fest, ob die Strahlen der Verdeckung die Treffer auf der Rückseite ignorieren (wenn die hohe Polynormalität in die entgegengesetzte Richtung weist wie die niedrige Polynormalität, von der aus der Strahl gebrannt wird). Meistens sollte diese Einstellung aktiviert sein, um Artefakte zu vermeiden. Mögliche Werte:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Nie</strong> (Standard): Hintergründe werden nie ignoriert.</li><li data-preserve-html="true"><strong>Immer</strong>: Flächen werden immer ignoriert.</li><li data-preserve-html="true"><strong>Nach Netzname</strong>: Rückseiten werden nur für Gitter ignoriert, die mit dem Schlüsselwort des Suffix übereinstimmen. Weitere Informationen finden Sie in den [allgemeinen Parametern](../../bakers-settings/common-parameters/common-parameters.md).</li></ul> |
| **Selbstverdeckung** | Übereinstimmender Name für die Verdeckung. Gibt an, wie die Bäcker der Low- und High-Poly-Geometrie entsprechen sollen. Es kann verwendet werden, um den Backvorgang zu filtern, ohne dass manuell auseinander (explodieren) Gitter bewegt werden müssen.Mögliche Werte:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Immer</strong> (Standard): Ein solches Gitter wird mit jedem Gitter mit einem hohen Poly-Wert kombiniert.</li><li data-preserve-html="true"><strong>Nach Netzname</strong>: Filtern Sie die Gitter nach ihrem Namen, um eine Übereinstimmung mit unerwünschter Geometrie zu vermeiden.</li></ul>Weitere Informationen zum Anpassen von Geometrien finden Sie unter: [Übereinstimmung nach Name](../../features/matching-by-name/matching-by-name.md). |
| **Normale Karte** | Optionaler Pfad zu einer normalen Textur. Kann verwendet werden, um die interne Berechnung des Bäckers zu ersetzen. |
| **Weltraum** | Wenn diese Option aktiviert ist, wird die normale Textur als World Space Normal statt als Tangent Space interpretiert. |
| **Normale Ausrichtung** | Format der normalen Struktur, wenn in Tangentialraum.Mögliche Werte:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>DirectX</strong> (Standard)</li><li data-preserve-html="true"><strong>OpenGL</strong></li></ul> |
| **Dämpfung** | Legt fest, wie die Verdeckung durch die Okklusionsdistanz gedämpft wird.Mögliche Werte:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Keine</strong>: keine Dämpfung.</li><li data-preserve-html="true"><strong>Linear</strong> (Standard) : Dämpfung.</li><li data-preserve-html="true"><strong>Glatt</strong>: weiche Dämpfung.</li></ul> |
| **Grundebene** | Wenn diese Option aktiviert ist, simulieren Sie eine Ebene unter dem Gitterbegrenzungsrahmen auf der XZ-Achse, um mit Sekundärstrahlen zu kollidieren. Dies simuliert Schatten, die von einem unsichtbaren Grundriss kommen. |
| **Versatz der Grundebene** | Ermöglicht die Verschiebung des Plans vom Gitter weg, um die Intensität des Effekts zu reduzieren. Der Wert ist absolut und nicht relativ zur Maschengröße. |
