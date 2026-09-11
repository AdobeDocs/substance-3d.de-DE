---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/generated-textures-packing.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Substance Texturen in Unity generiert, und konfigurieren Sie das Textur-Packing für optimale Shader-Eingänge.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Generated Textures (Packing)
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Generierte Texturen (Packing)
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 6%

---


# Generierte Texturen (Packing)

Die generierten Texturen zeigen die Ausgaben von der Substance an, die vom Substance Engine berechnet werden, um Texturen zu erstellen. Diese Texturen werden den Shader-Eingängen zugeführt. Standardmäßig werden nur die vom Shader verwendeten Basiseingänge erstellt. Wenn &quot;Alle Ausgaben generieren&quot; aktiviert ist, werden alle Texturen hier angezeigt.

![](../../../assets/screen-shot-2022-03-29-at-1-24-16-pm-copy.png)

Wenn &quot;Alle Ausgaben generieren&quot; aktiviert ist

![](../../../assets/screen-shot-2022-03-29-at-1-29-35-pm-copy.png)

## Nutzung

1. Wenn Sie ein Textur-Symbol auswählen, wird die Textur im Projektfenster ausgewählt. Dies funktioniert nicht für Laufzeitordner-Material, da keine Texturen im Projektordner generiert werden.
1. Die Schaltfläche &quot;sRGB&quot; funktioniert ähnlich wie die Option &quot;sRGB (Farb-Textur)&quot; in den Texturen-Importeinstellungen. Damit können Sie festlegen, ob eine Textur im Gamma-Raum (sRGB) oder linear interpretiert werden soll. Das Substance-Plugin behandelt diese Interpretation automatisch, kann aber bei Bedarf überschrieben werden.

   | Substance-Ausgabe | sRGB |
   | --- | --- |
   | Grundfarbe | Aktiviert |
   | Diffus | Aktiviert |
   | Glanz | Aktiviert |
   | Normal | Deaktiviert |
   | Metallisch | Deaktiviert |
   | Rauheit | Deaktiviert |
   | Glanz | Deaktiviert |
   | Höhe | Deaktiviert |
   | Umgebungsverdeckung | Deaktiviert |

## Packing Channels

Sie können eine Textur über das Dropdown-Menü in den Alphakanal einer anderen Textur einfügen. Jede generierte Textur verfügt über ein Dropdown-Menü, das eine Liste aller von den Substance-Materialien generierten Textur-Ausgaben enthält. Wählen Sie einfach eine Karte aus der Liste aus, um sie in den Alphakanal der Textur zu packen. Die Option &quot;Quelle&quot; ist der Alphakanal der Textur.

In diesem Bild habe ich die Höhen-Map ausgewählt:

![](../../../assets/screen-shot-2022-03-29-at-2-48-33-pm.png)

In der folgenden Abbildung können Sie sehen, dass die Height-Ausgabe in den Alphakanal der Grundfarbe-Map gepackt wird.

![](https://helpx-prod.scene7.com/is/image/HelpxProd/screen-shot-2022-03-29-at-2-53-20-pm-copy?$png$&jpegSize=200&wid=1248)

## Zuordnung der Textur der Ausgabe

Darüber hinaus kann die Textur der Ausgabe den Oberflächeneingängen von Unity-Materialien über den Abschnitt Zuordnung der Ausgabe-Textur individuell zugewiesen werden. Die mit der .sbsar-Datei generierten Ausgabe-Texturen werden in der linken Spalte angezeigt und verfügbare Unity Surface-Eingaben werden in der rechten Spalte angezeigt. Letzteres kann über die Dropdown-Menüs geändert werden.

![](../../../assets/image2023-3-27-14-30-24.png)
