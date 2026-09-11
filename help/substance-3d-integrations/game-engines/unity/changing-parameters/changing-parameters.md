---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/changing-parameters.html"
breadcrumb-title: ''
description: Ändern Sie die Parameter des Substance-Materials in Unity, um das Erscheinungsbild und die Eigenschaften des Materials zur Laufzeit anzupassen.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Changing parameters
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Parameter ändern
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '208'
ht-degree: 0%

---


# Parameter ändern

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

Die Parameter für das Substance-Material sind auf dem Substance-Grafen-Objekt (SGO) verfügbar.

1. Wählen Sie im Projektfenster das Datenlogo für den Graf aus, den Sie anpassen möchten. Das SBSAR-Logo ist grün.

   ![](../../../assets/screen-shot-2022-03-29-at-2-27-56-pm.png)

## Prozedurale Eigenschaften

1. **Alle Ausgaben generieren**: Generiert alle Ausgaben aus der Substance-sbsar-Datei. Standardmäßig werden nur Ausgaben erstellt, die von Standard-Shadern verwendet werden.
1. **Mipmaps generieren**: Generiert MIP-Texturen für jede Substance-Ausgabe.
1. **Zufallsparameter**: Diese Schaltfläche ändert die Zufallsgeschwindigkeit, die der Substance-Graf zum Generieren der Texturen verwendet. Wenn Sie diesen Wert ändern, wird für die berechnete Textur ein neues Ergebnis basierend auf dem Startwert erstellt.
1. Die in der Substance-Datei gelegt Parameter sind in Unity verfügbar. Das Editor-Steuerelement basiert auf dem Parametertyp, der für den Substance erstellt wurde.
1. **Vorgabenbehandlung:** Sie können Substance-Vorgabedateien (Unterleisten) exportieren oder importieren. Beim Exportieren einer Vorgabe wird eine Vorgabedatei erstellt, die auf den Parametereinstellungen für die Substance basiert. Sie können Vorgabedateien aus Substance Designer und Substance Player exportieren, die dann mit der Schaltfläche &quot;Vorgabe importieren&quot; importiert werden können. Dies ist hilfreich, um Substance-Vorgaben über Anwendungen und Teams hinweg freizugeben.

</td>
<td style="border: 0;" valign="top">

![](../../../assets/changing-parameters.png)

</td>
</tr>
</table>
