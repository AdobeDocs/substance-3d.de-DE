---
helpx_url: "https://helpx.adobe.com/de/substance-3d-bake/common-questions/why-is-matching-by-name-not-working-with-ambient-occlusion-thickness.html"
breadcrumb-title: ''
description: Erfahren Sie, warum das Anpassen nach Namen nicht mit "Umgebende Verdeckung"- und "Thickness"-Bäkern funktioniert, und finden Sie Alternativen.
helpx_creative_field: ""
helpx_description: "bakers > Common Questions > Why is Matching by Name not working with Ambient OcclusionThickness "
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 'Warum funktioniert die Namensübereinstimmung nicht mit der Umgebungsokklusions-Dicke? '
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '109'
ht-degree: 0%

---


# Warum funktioniert die Zuordnung nach Name nicht mit umgebender Verdeckung/Thickness?

>[!WARNING]
>
> **Frage**
> 
> Ich habe [Übereinstimmend mit Name](../../features/matching-by-name/matching-by-name.md) in den [allgemeinen Parametern](../../bakers-settings/common-parameters/common-parameters.md) aktiviert, um meine niedrigen und hohen Polygitter zu filtern und zu sortieren. Warum ignoriert der Bäcker für Umgebungsgeräusche diese Verdeckung?

>[!NOTE]
>
> **Erklärung**
> 
> Die Bäcker &quot;Ambient Verdeckung, Thickness&quot; und &quot;Bent Normale&quot; starten Sekundärstrahlen, wenn sie ihre Texturen berechnen. Für diese Strahlen gibt es eine eigene Einstellung für die Zuordnung nach Name.

>[!NOTE]
>
> **Lösung : Substance Painter**
> 
> Lösung: Aktivieren Sie die Namensfilterung für die Sekundärstrahlen in den Bäckerparametern.
