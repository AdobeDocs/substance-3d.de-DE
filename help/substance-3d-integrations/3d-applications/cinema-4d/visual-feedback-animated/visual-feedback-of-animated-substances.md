---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/cinema-4d/visual-feedback-of-animated-substances.html"
breadcrumb-title: ''
description: Aktiviere die animierte Vorschau in Cinema 4D, um das Feedback zu animierten Substance-Materialien im Viewport anzuzeigen.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Cinema 4D > Visual Feedback of Animated Substances
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Visuelles Feedback von animierten Substance
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 3%

---


# Visuelles Feedback von animierten Substance

Um visuelles Feedback zu einer animierten Substance im Viewport von Cinema 4D zu erhalten, sollte die Option &quot;Animierte Vorschau&quot; für diese Materialien aktiviert sein.

Diese Option finden Sie im Material Editor unter Editor (siehe unten). Wenn ein Material mit dem Befehl &quot;Material(e) erstellen&quot; erstellt wurde, ist diese Option standardmäßig aktiviert.

![](../../../assets/cinema-4d-13.png){width="500px"}


## Erstellen von Materialien

Mit dem Befehl &quot;Material(e) erstellen&quot; im Substance Asset Manager können Sie Cinema 4D-Materialien einfach und schnell mit einer Substance erstellen.

Daher wird die folgende Kanalzuordnung verwendet:

|  |  |
| --- | --- |
| **Substance-Ausgabekanal** | **Cinema 4D-Materialkanal** |
| Diffus | Color |
| Ausstrahlend | Luminanz |
| Spiegelung | Reflexion |
| Umgebung | Umgebung |
| Bump | Bump |
| Deckkraft | Alpha |
| Glanz | Reflexion / Standard-Specular |
| Höhe | Verschiebung |
| Normal | Normal |

Diese Beziehung wird nur für den Befehl &quot;Material erstellen&quot; verwendet und das erstellte Material kann anschließend geändert werden. Mit diesem Befehl können Sie schnell ein Basismaterial erstellen, das Sie dann anpassen können, indem Sie nur einige wenige Kanäle verändern.

Innerhalb des Substance Shaders sind Sie nicht auf die wenigen Ausgabekanäle beschränkt, die oben aufgelistet sind, sondern können jeden Ausgabekanal verwenden, den eine Substance zur Verfügung stellen kann.

## Manuelles Erstellen von Substance-Material

Anstatt den Befehl &quot;Material erstellen&quot; zu verwenden, können Sie Materialien auch manuell mit dem Substance-Shader erstellen.

Wählen Sie einfach den Substance-Shader in einem Materialkanal aus und ziehen Sie ihn auf die gewünschte Substance. Der nächste Schritt besteht darin, den Ausgabekanal der Substance auszuwählen, der in diesem Shader verwendet werden soll, und schon sind Sie fertig.

So zum Beispiel:

![](../../../assets/cinema-4d-15.png){width="800px"}

Diese Methode bietet viel kreative Freiheit und ermöglicht Folgendes:

* Weisen Sie Substance-Ausgabekanäle beliebigen Cinema 4D-Materialkanälen zu. Es besteht keine Notwendigkeit, sich darauf zu beschränken, sie nur in den vorgesehenen Kanälen zu verwenden.
* Weisen Sie einen einzelnen Substance-Ausgabekanal mehreren Cinema 4D-Materialkanälen zu.
* Weisen Sie einem einzigen Cinema 4D-Material Ausgabekanäle mehrerer Substance zu.

## Einschränkungen

* Keyframes auf Substance-Eingabeparametern werden in der Zeitleiste angezeigt, nicht jedoch im Schieberegler &quot;Leistung&quot; von Cinema 4D (der Schieberegler &quot;Zeitleiste&quot; unter den Ansichtsfenstern).
* Aufgrund einer Einschränkung sollten auf Substance-Ausgabekanälen keine benutzerdefinierten Farbprofile verwendet werden.
* Unter bestimmten Umständen werden die Bildeingaben der Substance nicht mehr angezeigt\
  Der Befehl &quot;Zusammenfügen...&quot; von Cinema 4D kombiniert zwei Szenen zu einer Szene. Dies geschieht, wenn sich in der zusammenzufügenden Szene Substance im Projektverzeichnis befinden, deren Bildeingaben sich auf Bilder im Projektverzeichnis beziehen. In solchen Fällen müssen die Bildeingaben anschließend manuell neu verknüpft werden.
* Wenn sich Substance im Projektordner (oder an einer anderen Stelle im globalen Suchpfad) befinden, funktionieren sie in Cineware nicht. In diesem Fall werden sie rot gerendert, als ob die Substance fehlt. Um dieses Problem zu umgehen, müssen die Substance-Archive außerhalb des Projektverzeichnisses gespeichert werden, sodass sie durch einen absoluten Pfad referenziert werden. Sie können den Dateinamen-Parameter verwenden, um den Dateispeicherort zu ändern, nachdem die Dateien außerhalb des Projektpfads verschoben wurden.
