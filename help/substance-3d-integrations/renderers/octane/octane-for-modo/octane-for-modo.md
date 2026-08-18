---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/renderers/octane/octane-for-modo.html"
breadcrumb-title: ''
description: Verwenden Sie Substance-Materialien mit Octane-Renderer in MODO über Live DB-Materialien und die richtigen Ausgabekonfigurationen.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Octane > Octane for MODO
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Oktan für MODO
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 0%

---


# Oktan für MODO

## Substance in MODO-Plug-in

Die Substance-Ausgaben funktionieren nativ mit Octane. Sie können die folgenden Substance-Ausgaben und Texturebenen-Effektkonfigurationen verwenden.

1. Erstelle eine Substance > Struktur > Substance erstellen. Wähle als Modus &quot;Unreales Material&quot;. Wenn du die Option &quot;Unrealistisches Material&quot; verwendest, kannst du die Struktur im Viewport &quot;Erweitertes OGL&quot; anzeigen.
1. Erstellen Sie Ausgaben für Grundfarbe, Metallisch, Raueit und Normal.
1. MODO verwendet OGL Normal-Karten. In den Substance-Eigenschaften müssen Sie die Normalrichtung in OpenGL ändern.

   ![](../../../assets/ogl.png)
1. Laden Sie die Substance PBR-Vorgabe. Diese Vorgabe ist ein &quot;Octane Override&quot;. Ziehe die Vorlage in deine Shader-Gruppe.

   [Substance\_PBR.lxp](https://helpx.adobe.com/content/dam/help/en/substance-3d/documentation/integrations/files/162005234/162005272/1/1502792782697/substance-pbr.lxp)
1. Wählen Sie das irreguläre Format aus und ziehen Sie die Substance-Ausgaben aus dem Clip-Browser in die Schemaansicht. Nehmen Sie den Knoten mit der Dateinamenausgabe und verbinden Sie ihn mit dem entsprechenden Eingabeknoten, d. h. Grundfarbe → Grundfarbe.

   ![](../../../assets/connect-6.png)
1. Alle anderen Substance-Ausgänge anschließen

   ![](../../../assets/outputs-4.png){width="640px"}
