---
helpx_url: "https://helpx.adobe.com/de/substance-3d-integrations/game-engines/unity/optimization-guidelines.html"
breadcrumb-title: ''
description: Befolgen Sie die Optimierungsrichtlinien, um die Komplexität des Substance-Materials mit der Rendering-Leistung in Unity in Einklang zu bringen.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Optimization Guidelines
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Optimierungsrichtlinien
user-guide-description: ''
user-guide-title: ''
source-git-commit: 4a060ee1aaa1731c04e70d5512e3271cd63d0381
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 0%

---


# Optimierungsrichtlinien

Je komplexer Ihre Substance-Materialien sind, desto mehr Verarbeitungsleistung wird zum Rendern benötigt. Substance-Materialien müssen daher **ein Gleichgewicht zwischen Komplexität und Rendering-Geschwindigkeit herstellen**. Dies ist *besonders* wichtig, wenn sie in Echtzeit-Grafikanwendungen wie Spielen verwendet werden.

Wenn du eigene Substance-Materialien erstellst, achte auf die folgenden Richtlinien zur Optimierung.

[Richtlinien zur Optimierung von Substance Designern](https://docs.substance3d.com/display/SDDOC/Performance+Optimization+Guidelines)

Eine der größten Einschränkungen, auf die Sie achten sollten, sind Knoten mit einer absoluten Auflösung von 4K oder höher.

>[!WARNING]
>
> **Achten Sie sorgfältig auf die Auflösungseinstellungen und die relativen Auflösungseinstellungen für die übergeordneten Elemente!**\
> Hohe Werte wirken sich stark auf die Leistung aus. Überlege dir also, wie das Material voraussichtlich verwendet wird und ob du die Datengröße reduzieren kannst.
>   
> Die Substance-CPU-Engine kann mit 4K berechnen, aber sie ist sehr langsam und kann dazu führen, dass eine Integration hängt oder möglicherweise abstürzt.

Im folgenden Beispiel wird die Ausgabegröße eines [Kachel-Sampler](https://experienceleague.adobe.com/en/docs/substance-3d-designer/using/substance-graphs/nodes-reference-for-substance-graphs/node-library/texture-generators/patterns/tile-sampler)-Knotens auf [Absolut](https://experienceleague.adobe.com/en/docs/substance-3d-designer/using/substance-graphs/output-size) 4096 festgelegt. Es führt dazu, dass mehrere Knoten stromabwärts mit 4K berechnet werden, bevor sie für die endgültige Ausgabeauflösung 2048 herunterskaliert werden.

![](../../../assets/absolute.png){width="1000px"}
