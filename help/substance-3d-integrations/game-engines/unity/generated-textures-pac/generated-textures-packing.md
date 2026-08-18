---
helpx_url: "https://helpx.adobe.com/de/substance-3d-integrations/game-engines/unity/generated-textures-packing.html"
breadcrumb-title: ''
description: Erfahren Sie, wie das Substance Texturen in Unity generiert, und konfigurieren Sie das Textur-Packing für optimale Shader-Eingaben.
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

Die generierten Texturen zeigen die Ausgaben von der Substance an, die vom Substance Engine berechnet werden, um Texturen zu erzeugen. Diese Texturen werden in die Shader-Eingänge eingespeist. Standardmäßig werden nur die vom Shader verwendeten Basiseingaben erstellt. Wenn &quot;Alle Ausgaben generieren&quot; aktiviert ist, werden alle Texturen hier angezeigt.

![](../../../assets/screen-shot-2022-03-29-at-1-24-16-pm-copy.png)

Wenn &quot;Alle Ausgaben generieren&quot; aktiviert ist

![](../../../assets/screen-shot-2022-03-29-at-1-29-35-pm-copy.png)

## Nutzung

1. Wenn Sie ein Textursymbol auswählen, wird die Textur im Projektfenster ausgewählt. Dies funktioniert nicht für Laufzeitmaterialien, da Texturen nicht im Projektordner generiert werden.
1. Die Schaltfläche &quot;sRGB&quot; funktioniert ähnlich wie die Option &quot;sRGB (Farbstruktur)&quot; in den Einstellungen für den Texturimport. Damit können Sie festlegen, ob eine Textur im Gamma-Raum (sRGB) oder linear interpretiert werden soll. Das Substance-Plugin behandelt diese Interpretation automatisch, kann aber bei Bedarf überschrieben werden.

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

Du kannst eine Struktur in den Alphakanal einer anderen Struktur einfügen, indem du das Dropdown-Menü wählst. Jede generierte Textur verfügt über ein Dropdown-Menü, das eine Liste aller Texturausgaben enthält, die von den Substance-Materialien generiert werden. Wählen Sie einfach eine Karte aus der Liste aus, um sie in den Alphakanal der Textur zu packen. Die Option &quot;Quelle&quot; ist der Alphakanal der Textur.

In diesem Height habe ich die Bildzuordnung ausgewählt:

![](../../../assets/screen-shot-2022-03-29-at-2-48-33-pm.png)

In der folgenden Abbildung sehen Sie, dass die Height-Ausgabe in den Alphakanal der Grundfarbkarte gepackt wird.

![](https://helpx-prod.scene7.com/is/image/HelpxProd/screen-shot-2022-03-29-at-2-53-20-pm-copy?$png$&jpegSize=200&wid=1248)

## Ausgabetexturzuordnung

Darüber hinaus kann die Ausgabetextur den Oberflächeneingängen von Unity-Materialien über den Abschnitt &quot;Ausgabetexturzuordnung&quot; individuell zugewiesen werden. Die mit der .sbsar-Datei generierten Ausgabetexturen werden in der linken Spalte angezeigt und verfügbare Unity-Oberflächeneingaben werden in der rechten Spalte angezeigt. Letzteres kann über die Dropdown-Menüs geändert werden.

![](../../../assets/image2023-3-27-14-30-24.png)
