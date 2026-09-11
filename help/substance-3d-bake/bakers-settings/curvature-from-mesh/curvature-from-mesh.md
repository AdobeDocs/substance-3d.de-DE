---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/bakers-settings/curvature-from-mesh.html"
breadcrumb-title: ''
description: Generieren Sie präzise Krümmung-Texturen von Meshs mit hoher Poly-Dichte mithilfe von Raytracing für eine präzise Kantenerkennung.
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Curvature from Mesh
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Krümmung aus Gitter
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---


# Krümmung aus Gitter

Die Krümmung des Gitterbäckers erzeugt eine Krümmungstextur aus hochpolaren Gittern. Er ist langsamer als der Basiskrümmungs-[&#128279;](../../bakers-settings/curvature/curvature.md)-Bäcker von , liefert jedoch genauere Ergebnisse.

**Verfügbar in:**

* Substance Designer
* Substance Automation Toolkit
* Substance Painter

## Parameter

| *Parameter* | *Beschreibung* |
| --- | --- |
| **Sekundärstrahlen** | Anzahl der Strahlen, die zum Lesen der nahegelegenen Geometrie emittiert werden. Bei einem hohen Wert wird weniger Rauschen erzeugt, die Berechnung dauert jedoch länger. Der Standardwert ist 32. |
| **Sampling-Radius** | Wie weit die Nahgeometrie berücksichtigt wird, um die Krümmung an der Geometrieoberfläche zu berechnen. Hohe Werte können stärkere Kanten erzeugen, während niedrigere Werte dünnere Kanten erzeugen, aber Informationen verpassen. |
| **Relativ zum Begrenzungsrahmen** | Legt fest, ob der Sampling-Radius in Relation zur Größe des Meshs oder als einheitsbasierte Entfernung definiert wird. |
| **Selbstüberschneidung** | Zuordnung nach Namen der Krümmungen. Gibt an, wie die Bäcker der Low- und High-Poly-Geometrie entsprechen sollen. Es kann verwendet werden, um den Backvorgang zu filtern, ohne dass manuell auseinander (explodieren) Gitter bewegt werden müssen.Mögliche Werte:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Immer</strong> (Standard): Ein solches Gitter wird mit jedem Gitter mit einem hohen Poly-Wert kombiniert.</li><li data-preserve-html="true"><strong>Nach Netzname</strong>: Filtern Sie die Gitter nach ihrem Namen, um eine Übereinstimmung mit unerwünschter Geometrie zu vermeiden.</li></ul>Weitere Informationen zum Anpassen von Geometrien finden Sie unter: [Übereinstimmung nach Name](../../features/matching-by-name/matching-by-name.md). |
| **Automatische Tonzuordnungsgrenzen** | Steuert, wie die Krümmungswerte in die Textur geschrieben werden. Wenn diese Option aktiviert ist, wird der Wertebereich zwischen 0 und 1 normalisiert, basierend auf dem minimalen und maximalen Wert, der während des Backvorgangs gefunden wurde. Wenn diese Option deaktiviert ist, werden der Mindest- und der Höchstwert manuell definiert.  **Hinweis:** Beim Backen von UDIMs/UV-Kacheln sollte dieser Parameter deaktiviert werden, um die Tonzuordnung einheitlich und nicht spezifisch für jede Kachel zu gestalten. Andernfalls könnte dies zu Nahtstellen zwischen den einzelnen Texturen führen. Um die richtigen Mindest-/Höchstwerte manuell zu finden, backen Sie zuerst mit dieser aktivierten Einstellung und sehen Sie dann in der Konsole/im Protokoll nach, welche Werte der Bäcker ausgegeben hat. |
| **Min. für Tonzuordnung** | Wenn **Automatische Tonzuordnungsgrenzen** deaktiviert ist, wird der Mindestwert zum Skalieren des Krümmungsergebnisses so definiert, dass es in die Textur passt. |
| **Max. Tonzuordnung** | Wenn &quot;**Automatische Tonzuordnungsgrenzen**&quot; deaktiviert ist, wird der Maximalwert definiert, um das Krümmungsergebnis so zu skalieren, dass es in die Textur passt. |
| **Normale Karte** | Optionaler Pfad zu einer normalen Textur. Kann verwendet werden, um die interne Berechnung des Bäckers zu ersetzen. |
| **Weltraum** | Wenn diese Option aktiviert ist, wird die normale Textur als World Space Normal statt als Tangent Space interpretiert. |
| **Normale Ausrichtung** | Format der normalen Struktur, wenn in Tangentialraum.Mögliche Werte:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>DirectX</strong> (Standard)</li><li data-preserve-html="true"><strong>OpenGL</strong></li></ul> |
