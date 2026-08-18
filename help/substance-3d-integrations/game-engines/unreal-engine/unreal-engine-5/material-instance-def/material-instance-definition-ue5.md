---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/material-instance-definition-ue5.html"
breadcrumb-title: ''
description: Erstellen Sie Materialinstanzdefinitionen mit Substance-Materialien in Unreal Engine 5, um die GPU-Rendering-Leistung zu optimieren.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 5 > Material Instance Definition - UE5
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Materialinstanzdefinition - UE5
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '271'
ht-degree: 0%

---


# Materialinstanzdefinition - UE5

Sie können UE5-Materialinstanzen mit Substance verwenden. Dadurch wird ein großer Schritt im GPU-Rendering-Prozess gespeichert, indem kein neues Material in den Prozess hochgeladen wird. Eine MID kann zur Laufzeit oder im Editor erstellt werden. Mit Version 5.0.0 haben wir die volle Unterstützung für Materialinstanzen hinzugefügt.

## Erstellen einer Materialinstanz im Editor

1. Klicken Sie mit der rechten Maustaste auf das mit der Substanz erstellte UE5-Material und wählen Sie &quot;Materialinstanz erstellen&quot;. Dadurch wird ein UE5-Instanzmaterial erstellt.

   ![](https://helpx-prod.scene7.com/is/image/HelpxProd/screen-shot-2022-03-31-at-6-07-08-pm?$png$&jpegSize=300&wid=1472)
1. Mache einen Rechtsklick bzw. Ctrl-Klick auf die Factory der Substance-Instanz, und wähle &quot;Graph-Instanz erstellen&quot;. Dadurch wird eine Instanz des Graphen erstellt und ein weiteres UE5-Material erstellt. Löschen Sie das neu erstellte UE5-Material, da es nicht verwendet wird.

   ![](../../../../assets/screen-shot-2022-03-31-at-6-10-38-pm.png)
1. Doppelklicken Sie auf die Materialinstanz, die Sie in Schritt 1 erstellt haben, und aktivieren Sie die Texturparameter für alle Maps.
1. Legen Sie die Textur auf die neue INST-Textur fest, die aus Schritt 2 erstellt wurde. Dadurch wird die Materialinstanz so festgelegt, dass die Substance-Ausgabemaps aus dem instanzierten Diagramm verwendet werden.

   ![](../../../../assets/screen-shot-2022-03-31-at-6-13-18-pm.png)

Sie haben jetzt eine UE5-Materialinstanz, die einen bestimmten Satz von Substance-Texturen verwendet. Dies ist eine optimierte Art, mit mehreren Substanzen in einem UE5-Projekt zu arbeiten. Um zu erfahren, wie Sie eine MID mithilfe von Blueprint erstellen, lesen Sie bitte diese Seite. [Blueprint(UE5): Dynamische Materialinstanz &#x200B;](https://helpx.adobe.com/substance-3d/unlisted/documentation/integrations/blueprint-dynamic-material-instance-152535142.html)
