---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/getting-started/what-is-baking.html"
breadcrumb-title: ''
description: Erfahre, was Backen ist, und speichere Informationen zu 3D-Meshes in Texturdateien, um deine Substance-Materialien auszugestalten.
helpx_creative_field: ""
helpx_description: "bakers > Getting Started > What is Baking "
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 'Was ist Backen? '
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---


# Was ist Backen?

![](https://upload.wikimedia.org/wikipedia/commons/3/36/Normal_map_example.png)

&#x200B;>> 

(Credits: [Paolo Cignoni](https://commons.wikimedia.org/wiki/File:Normal_map_example.png) - [CC BY-SA 1.0](https://creativecommons.org/licenses/by-sa/1.0))

Backen ist der Name des Prozesses zum **Speichern von Informationen**, die sich auf ein **3D-Gitter** beziehen, in einer **Textur**-Datei ([Bitmap](https://en.wikipedia.org/wiki/Raster_graphics)). Meist handelt es sich dabei um ein anderes Gitter. Dabei werden die Informationen des ersten Gitters auf die zweiten Gitter-UVs übertragen und dann in einer Textur gespeichert.

Manche Anwendungen unterstützen zwar das Backen von Informationen in die Gittereigenschaften (z. B. Scheitelpunktfarben), aber Substance Baker ermöglicht das Backen von Informationen nur bis zu einer Textur. Sie können jedoch die Gittereigenschaften auslesen und sie auf Texturen (wie Scheitelpunktfarben) reduzieren.

## Ist Backen notwendig?

Substance-Software generieren Texturen und diese Texturen können durch Informationen über die Gittergeometrie verbessert werden.\
Viele Filter und Materialien passen sich an die spezifische Geometrie eines 3D-Gitters an, indem sie sich die gebackenen Texturen ansehen. Das Backen kann Informationen darüber liefern, wo Umgebungsschatten sein können, wo die Kanten der Geometrie sind und vieles mehr.

Beispiel : Bei einem alten Wagen kann der Rost unten aufgetragen werden, weil er sich eine Weile nicht bewegt hat. Das Backen der Positionskarte ermöglicht es zu wissen, wo der Boden auf dem Gitter ist, das den Rost-Generator speist und die angepasste Textur erzeugt.

![](../../assets/examples.jpg){width="500px"}

## Wie funktioniert Backen?

Jeder Bäcker führt bestimmte Aktionen durch, um sein eigenes Ergebnis zu erzeugen, aber im Allgemeinen beinhaltet der Backvorgang zwei mögliche Methoden:

* **Backen auf ein Gitter** : stützt sich beim Generieren von Informationen auf das aktuelle Gitter.
* **Sichern von einem Gitter auf ein anderes** : Informationen aus einem Quellnetz berechnen und das Ergebnis auf ein anderes übertragen.

Dieser Backprozess beruht auf den Mascheneigenschaften, weshalb das Gitter sauber und frei von eventuellen Fehlern in seiner Geometrie sein muss.

## Welche Art von Informationen können Sie backen?

Viele Arten von Informationen können gesichert werden. Im Allgemeinen ist jedoch nur ein bestimmter Satz erforderlich, da er extrapoliert werden kann, um später ein fortschrittlicheres Ergebnis zu erzielen. Aus diesem Grund gibt es eine gängige Art von Backverfahren, die in mehreren Software gefunden werden können.

Als Beispiel kann die Substance-Software folgende Informationen ausgeben:

* **Umgebungsschatten** (Verdeckung)
* **Normale** Informationen (Varianten der Oberflächendetails werden als Vektorrichtungen gespeichert)
* **Richtung** (wobei oben oder unten, links oder rechts usw.)
* **Krümmung** (Kanten und Hohlräume der Geometrie)
* **Position** (relative Position der Geometrie innerhalb eines normalisierten Würfels)

Weitere Informationen finden Sie in der [Dokumentation jedes Bäckers](../../bakers-settings/bakers-settings.md).

## Unterschied zwischen &quot;normalen&quot; und &quot;aus Netz&quot; Bäcker

Je nach Prozess verwenden die Bäcker verschiedene Implementierungen. Generell verlassen sich die **-Baker aus Mesh** auf Raytracing-Techniken, um Daten von einem Modell in ein anderes zu extrahieren und zu projizieren.
