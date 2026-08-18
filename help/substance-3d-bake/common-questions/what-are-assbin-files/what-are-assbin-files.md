---
helpx_url: "https://helpx.adobe.com/de/substance-3d-bake/common-questions/what-are-assbin-files.html"
breadcrumb-title: ''
description: Erfahren Sie, was Assbin-Dateien sind und wie sie als Geometrie-Cache-Dateien verwendet werden, um Backvorgänge zu beschleunigen.
helpx_creative_field: ""
helpx_description: "bakers > Common Questions > What are Assbin files "
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 'Was sind Assbin-Dateien? '
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '148'
ht-degree: 0%

---


# Was sind Assbin-Dateien?

>[!WARNING]
>
> **Frage**
> 
> Nach dem Backen in Substance Painter habe ich eine oder mehrere Dateien neben meinen High-Poly-Meshes mit der Dateierweiterung &quot;assbin&quot; gefunden, was sind sie ? Kann ich sie sicher entfernen?

>[!NOTE]
>
> **Lösung**
> 
> Assbin-Dateien vorverarbeitete Versionen der High-Poly-Meshes, die während des Backprozesses verwendet werden. Sie sind schneller zu lesen als die ursprünglichen Gitterdateien, was es ermöglicht, schneller erneut zu backen, wenn Sie die Baker-Einstellungen iterieren. Sie können sicher entfernt werden. Substance Painter wird sie bei Bedarf regenerieren. Dies kann sich jedoch auf die Backleistung auswirken.
> 
> Es ist möglich, diese Dateien nie zu generieren, indem Sie in den Substance Painter [Hauptvoreinstellungen](https://helpx.adobe.com/de/substance-3d/unlisted/documentation/spdoc/general-71008262.html) wechseln und die Option &quot;Vorverarbeitete Szenendateien speichern&quot; deaktivieren.
