---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-questions/what-is-the-difference-between-the-opengl-and-directx-normal-format.html"
breadcrumb-title: ''
description: Lerne die Unterschiede zwischen OpenGL und den DirectX-Normalen-Map-Format kennen und erfahre, wann du welche verwendest.
helpx_creative_field: ""
helpx_description: "bakers > Common Questions > What is the difference between the OpenGL and DirectX normal format "
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 'Was ist der Unterschied zwischen dem Normalformat von OpenGL und DirectX? '
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '185'
ht-degree: 0%

---


# Was ist der Unterschied zwischen dem OpenGL- und dem DirectX-Normalformat?

>[!WARNING]
>
> **Frage**
> 
> Was ist der Unterschied zwischen dem OpenGL- und dem DirectX-Normalformat?

>[!NOTE]
>
> **Erklärung**
> 
> OpenGL und DirectX sind zwei grafische APIs (Funktionssätze), die Programmierer in ihrer Anwendung verwenden, um mit der GPU (Graphic Processing Unit) zu kommunizieren. Bei normalen Maps ergibt sich der Unterschied, wie der grüne Kanal einer RGB-Textur interpretiert werden soll. OpenGL erwartet, dass das erste Pixel am unteren Ende liegt, während DirectX erwartet, dass es am oberen Ende liegt. Dies ist oft der Grund, warum es in verschiedenen technischen Diskussionen empfohlen wird, zu versuchen, den grünen Kanal einer normalen Karte umzukehren, um zu sehen, ob es sich besser verhält, wie es die Pixelwerte umkehrt (zuerst wird der letzte). OpenGL kann als **Y+** (von unten nach oben) bezeichnet werden, während DirectX als **Y-** (von oben nach unten) bezeichnet wird.
> 
> Welches Format verwendet werden soll, erfahren Sie in der Zielanwendung, in der Ihre Texturen verwendet werden.
