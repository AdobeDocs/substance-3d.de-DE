---
helpx_url: "https://helpx.adobe.com/de/substance-3d-integrations/3d-applications/modo/working-with-references.html"
breadcrumb-title: ''
description: Verwalten Sie Substance-Materialreferenzen in MODO, um Materialien über mehrere Objekte und Szenen hinweg auszutauschen.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > MODO > Working with References
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Arbeiten mit Verweisen
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---


# Arbeiten mit Verweisen

## Arbeiten mit Verweisen

Substance-Materialien können mit referenzierten Szenen verwendet werden. Wenn Sie jedoch eine Ausgabe für eine Substance in einer referenzierten Szene deaktivieren müssen, müssen Sie die Ausgaben manuell entfernen. Wenn Sie einfach die Ausgabe auf den Substance-Eigenschaften deaktivieren, werden die Ausgaben für referenzierte Substance nicht entfernt, wenn Sie die standardmäßigen Referenzierungsvoreinstellungen von MODO verwenden.\
Damit das referenzierte Substance-Material seine eigenen generierten Ausgaben löschen kann, müssen Sie zunächst die Referenzüberschreibungen für die Szene ändern, um die Ausgaben manuell zu entfernen. Wählen Sie &quot;Element&quot; > &quot;Referenzen&quot; > &quot;Referenzüberschreibungen bearbeiten&quot; und setzen Sie &quot;Löschen&quot; auf &quot;Wenn dies nach Element zulässig ist&quot;. Dadurch können Sie Substance-Ausgaben manuell entfernen\
aus der Shader-Struktur und dem Clip-Browser für jede Szene, die nach dieser Änderung geöffnet oder erstellt wird.

Weitere Informationen zu Referenzüberschreibungen finden Sie in der MODO-Dokumentation.\
<http://modo.docs.thefoundry.co.uk/modo/801/help/pages/modointerface/ImportReference.html>
