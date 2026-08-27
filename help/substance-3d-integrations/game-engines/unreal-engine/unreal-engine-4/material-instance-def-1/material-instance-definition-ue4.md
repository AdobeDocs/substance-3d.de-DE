---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-4/material-instance-definition-ue4.html"
breadcrumb-title: ''
description: Erstellen Sie Materialinstanzdefinitionen mit Substance-Materialien in Unreal Engine 4, um die GPU-Rendering-Leistung zu optimieren.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 4 > Material Instance Definition - UE4
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Materialinstanzdefinition - UE4
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '366'
ht-degree: 0%

---


# Materialinstanzdefinition - UE4

Sie können UE4-Materialinstanzen mit Substance verwenden. Dadurch wird ein großer Schritt im GPU-Rendering-Prozess gespeichert, indem kein neues zu verarbeitendes Material hochgeladen wird. Eine MID kann zur Laufzeit oder im Editor erstellt werden. Mit der Version 4.24.0.3 haben wir die vollständige Unterstützung für Materialinstanzen hinzugefügt und einen neuen Materialvorlagenarbeitsablauf mit numerischen Ausgaben eingeführt, die vom Substance Engine unterstützt werden. Mit Materialvorlagen können Sie genau definieren, wie Sie Ihre Substance-Materialschattierungen in UE4 konfigurieren möchten.

Beim Importieren einer SBSAR-Datei können Sie auswählen, mit welcher Vorlage Sie arbeiten möchten.

![](../../../../assets/ue4-material-templates.png)

Im Lieferumfang sind Vorlagen für die Arbeit mit Versatz, Brechung und Materialien mit Weltausrichtung enthalten, die integrierte Steuerelemente für die Anpassung von Kachelung, Texturgröße, Versatz und Emissionsparametern enthalten. Mit dem Materialvorlagensystem können Sie auch Ihre eigenen benutzerdefinierten Vorlagen bereitstellen.

![](../../../../assets/ue4-material-instance-params.png)

## Erstellen einer Materialinstanz im Editor

1. Klicken Sie mit der rechten Maustaste auf das mit der Substanz erstellte UE4-Material und wählen Sie &quot;Materialinstanz erstellen&quot;. Dadurch wird ein UE4-instanziertes Material erstellt.

   ![](https://helpx-prod.scene7.com/is/image/HelpxProd/01-12?$png$&jpegSize=100&wid=592){width="560px"}
1. Mache einen Rechtsklick bzw. Ctrl-Klick auf die Factory der Substance-Instanz, und wähle &quot;Graph-Instanz erstellen&quot;. Dadurch wird eine Instanz des Graphen erstellt und ein weiteres UE4-Material erstellt. Löschen Sie das neu erstellte UE4-Material, da es nicht verwendet wird.

   ![](../../../../assets/02-10.png){width="300px"}
1. Doppelklicken Sie auf die Materialinstanz, die Sie in Schritt 1 erstellt haben, und aktivieren Sie die Texturparameter für alle Maps.
1. Legen Sie die Textur auf die neue INST-Textur fest, die aus Schritt 2 erstellt wurde. Dadurch wird die Materialinstanz so festgelegt, dass die Substance-Ausgabemaps aus dem instanzierten Diagramm verwendet werden.

   ![](https://helpx-prod.scene7.com/is/image/HelpxProd/03-6?$png$&jpegSize=200&wid=1011){width="800px"}

Sie haben jetzt eine UE4-Materialinstanz, die einen bestimmten Satz von Substance-Texturen verwendet. Dies ist eine optimierte Art, mit mehreren Substanzen in einem UE4-Projekt zu arbeiten. Um zu erfahren, wie Sie eine MID mithilfe von Blueprint erstellen, lesen Sie bitte diese Seite. [Blueprint(UE4): Dynamische Materialinstanz ](https://helpx.adobe.com/substance-3d/unlisted/documentation/integrations/blueprint-dynamic-material-instance-152535142.html)
