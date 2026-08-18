---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/changing-parameters.html"
breadcrumb-title: ''
description: Ändern Sie die Substance-Materialparameter in Unity, um das Aussehen und die Eigenschaften des Materials zur Laufzeit anzupassen.
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

1. Wählen Sie im Projektfenster das Logo der SBSAR-Datei für das Diagramm aus, das Sie anpassen möchten. Das SBSAR-Logo ist grün.

   ![](../../../assets/screen-shot-2022-03-29-at-2-27-56-pm.png)

## Verfahrenseigenschaften

1. **Alle Ausgaben generieren**: Generiert alle Ausgaben aus der Substance-SBSAR-Datei. Standardmäßig werden nur Ausgaben erstellt, die von Standard-Shadern verwendet werden.
1. **Mipmaps generieren**: Generiert MIP-Texturen für jede Substance-Ausgabe.
1. **Zufallsparameter**: Mit dieser Schaltfläche wird der Zufallswert geändert, den das Substance-Diagramm zum Generieren der Texturen verwendet. Wenn Sie diesen Wert ändern, wird ein neues Ergebnis für die berechnete Textur basierend auf dem Startwert erstellt.
1. Die in der Substance-Datei angezeigten Parameter sind in Unity verfügbar. Das Editor-Steuerelement basiert auf dem Parametertyp, der für den Substance erstellt wurde.
1. **Vorgabenbehandlung:** Sie können Substance-Vorgabedateien (Unterleisten) exportieren oder importieren. Beim Exportieren einer Vorgabe wird eine Vorgabedatei erstellt, die auf den Parametereinstellungen für die Substance basiert. Sie können Vorgabedateien von Substance Designer und Substance Player exportieren, die dann mit der Schaltfläche &quot;Vorgabe importieren&quot; importiert werden können. Dies ist hilfreich, um Substance-Vorgaben über Anwendungen und Teams hinweg freizugeben.

</td>
<td style="border: 0;" valign="top">

![](../../../assets/changing-parameters.png)

</td>
</tr>
</table>
