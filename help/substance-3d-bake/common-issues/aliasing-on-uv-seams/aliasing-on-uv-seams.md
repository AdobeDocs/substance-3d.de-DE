---
helpx_url: "https://helpx.adobe.com/de/substance-3d-bake/common-issues/aliasing-on-uv-seams.html"
breadcrumb-title: ''
description: Korrigieren Sie Aliasing-Artefakte, die während des Backens an UV-Nahtstellen auftreten, indem Sie die Einstellungen für Glättung und Auffüllung anpassen.
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Aliasing on UV Seams
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Aliasing bei UV-Nähten
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '204'
ht-degree: 0%

---


# Aliasing bei UV-Nähten

>[!WARNING]
>
> **Problem**
> 
> Nach dem Backen erscheinen dunkle Flecken oder Punkte am Rand der UV-Naht:
> 
> ![](../../assets/edge-aliasing.png)

>[!NOTE]
>
> **Erklärung**
> 
> Wenn der Bäcker Informationen in die Textur schreibt, müssen sie von der Geometrie in Pixel konvertiert werden. Die Verarbeitung dieser Informationen kann [Aliasing](https://en.wikipedia.org/wiki/Aliasing) einführen. Aliasing tritt häufig auf, weil die Geometrie der UVs nicht am Pixelraster ausgerichtet ist oder weil die UVs nicht genügend Pixel abdecken, um eine ausreichende Auflösung zu erzielen.
> 
> In den folgenden Bildern ist die Geometrie die rote Überlagerung. Der Bäcker markiert ein Pixel als voll, wenn mehr als die Hälfte seiner Oberfläche von der Geometrie bedeckt ist (weiße Quadrate sind volle Pixel und schwarze Quadrate sind leere Pixel). Im rechten Bild ist das Pixelraster doppelt so hoch wie die Auflösung, was eine genauere Darstellung der Geometrie ermöglicht.
> 
> ![](../../assets/aliasing-example-large.png)
> 
> ![](../../assets/aliasing-example-small.png)

>[!NOTE]
>
> **Lösung**
> 
> * Erhöhen Sie die Ausgabetexturauflösung der Bäcker.
> * Erhöhen Sie die Einstellung für das Glätten (Hinweis : die Berechnung kann mehr Zeit in Anspruch nehmen).
> * Richten Sie die UVs im UV-Editor der 3D-Modellierungssoftware am Pixelraster aus.
> * Geben Sie ein besseres Texturverhältnis zu UVs.
