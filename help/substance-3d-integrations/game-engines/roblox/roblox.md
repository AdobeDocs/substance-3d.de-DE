---
helpx_url: "https://helpx.adobe.com/de/substance-3d-integrations/game-engines/roblox.html"
breadcrumb-title: ''
description: Verwenden Sie Substance-Materialien in Roblox Studio mit dem PBR-Workflow für metallische Raueit für immersive 3D-Erlebnisse.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Roblox
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Roblox
user-guide-description: ''
user-guide-title: ''
source-git-commit: 4a060ee1aaa1731c04e70d5512e3271cd63d0381
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 0%

---


# Roblox

[Roblox](https://www.roblox.com/) ist eine Plattform für immersive 3D-Multiplayer-Erlebnisse. Roblox Studio, das Roblox-Designtool, unterstützt den Workflow für die metallische Raueit von PBR.

<table>
<tr style="border: 0;">
<td width="58.30%" style="border: 0;" valign="top">

## Substance 3D Designer-Vorlage

Um Texturen für Roblox zu erstellen, können Sie die Substance 3D-Datei unten als [Substance-Kompositionsgrafik](https://experienceleague.adobe.com/de/docs/substance-3d-designer/using/substance-graphs/substance-compositing-graphs)-Vorlage in [Substance 3D Designer](https://experienceleague.adobe.com/en/docs/substance-3d-designer/home) verwenden.

[![Bild des SBS-Dateiformatsymbols, das mit der RoboBlox-Vorlage verknüpft ist.](../../assets/sbs.png){width="64px"}](https://helpx.adobe.com/content/dam/roblox.sbs)

Diese Graphvorlage ermöglicht die Vorkonfiguration der endgültigen Texturdateinamen und -typen. Diese Vorlage kann installiert und wiederverwendet werden, um neue Materialien zu erstellen, die immer den Roblox-Materialrichtlinien entsprechen.

</td>
<td width="41.60%" style="border: 0;" valign="top">

![](https://helpx-prod.scene7.com/is/image/HelpxProd/roblox-template?$png$&jpegSize=100&wid=401){width="200px"}

</td>
</tr>
</table>

## Workflow von Designer zu Roblox

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

### Vorlage installieren

Zunächst *installieren* Sie die Roblox-Vorlage.

* Laden Sie die oben verknüpfte Vorlagendatei herunter.
* Rufen Sie das Benutzerdokumentverzeichnis von Designer auf:
* (Creative Cloud-Desktop) `/Documents/Adobe/Adobe Substance 3D Designer`\
  (Steam) `/Documents/Allegorithmic/Substance Designer/`
* Erstellen Sie einen Vorlagenordner.
* Platzieren Sie die Datei in diesem Ordner.

</td>
<td style="border: 0;" valign="top">

![](../../assets/roblox-01-place-template.gif){width="512px"}

</td>
</tr>
</table>

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

### Vorlage erkennen

Lassen Sie Designer *den Vorlagenordner überwachen*, um nach Diagrammvorlagen zu suchen.

* Wechseln Sie in Designer zu **Bearbeiten > Voreinstellungen...1**
* Wechseln Sie im Fenster [Voreinstellungen](https://experienceleague.adobe.com/de/docs/substance-3d-designer/using/workspace/preferences/preferences-window) zu **Projekte > Benutzerprojekt > Allgemein**
* Klicken Sie in der Liste **Vorlagenverzeichnisse** auf die Schaltfläche **+**.
* Wechseln Sie zum Verzeichnis `templates` und klicken Sie auf **Ordner auswählen**.
* Klicken Sie auf die Schaltfläche **OK**.
* Gehen Sie zu **Datei > Neu > Substance-Diagramm...1**
* Überprüfen Sie, ob die Vorlage &quot;`Roblox`&quot; im Fenster &quot;[Neues Substance-Diagramm](https://helpx.adobe.com/de/substance-3d/unlisted/documentation/sddoc/create-a-graph-102400068.html)&quot; am unteren Rand der Vorlagenliste aufgeführt ist.

</td>
<td style="border: 0;" valign="top">

![](../../assets/roblox-02-detect-template.gif){width="512px"}

</td>
</tr>
</table>

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

### Texturen exportieren

Erstellen Sie ein Diagramm mit der Roblox-Vorlage und exportieren Sie Bitmaps aus diesem Diagramm, sobald Sie die Arbeit an einem Material abgeschlossen haben.

* Wählen Sie im Fenster [Neues Substance-Diagramm](https://helpx.adobe.com/de/substance-3d/unlisted/documentation/sddoc/create-a-graph-102400068.html) die Vorlage `Roblox` aus.
* Legen Sie einen beliebigen Bezeichner und andere Parameter für das Diagramm fest und klicken Sie auf **OK**.
* Arbeiten Sie in der [Diagrammansicht](https://experienceleague.adobe.com/de/docs/substance-3d-designer/using/workspace/graph-view/the-graph-view) an Ihrem Material. Lesen Sie [hier](https://experienceleague.adobe.com/de/docs/substance-3d-designer/using/getting-started/workflow-overview), um mit dem Arbeitsablauf zu beginnen.
* Wenn Sie fertig sind, gehen Sie zu **Tools > Bitmaps exportieren...** in der Diagrammansicht *Symbolleiste*
* Legen Sie im Fenster [Bitmaps exportieren](https://experienceleague.adobe.com/de/docs/substance-3d-designer/using/substance-graphs/exporting-bitmaps) einen gültigen Pfad **Ziel** fest. Stellen Sie sicher, dass *alle* die Ausgaben *aktiviert* sind, und klicken Sie auf **Exportieren**.
* Überprüfen Sie, ob die Texturen ordnungsgemäß in den Pfad **Ziel** exportiert wurden.

</td>
<td style="border: 0;" valign="top">

![](../../assets/roblox-03-export-textures.gif){width="512px"}

</td>
</tr>
</table>

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

### Erstellen von Material in Roblox

Erstellen Sie in Roblox eine Materialvariante und weisen Sie die aus Designer exportierten Texturen zu.

* Wählen Sie die Registerkarte **Modell** aus, und klicken Sie auf **Materialmanager**.
* Wählen Sie eine *Materialvorlage* aus, und klicken Sie auf die Schaltfläche **Variante erstellen**
* Legen Sie im Fenster **Variante erstellen** einen Namen für das Material fest.
* Klicken Sie für *jeden Materialkanal* auf die Schaltfläche **Importieren** und wählen Sie die entsprechende Textur aus, die aus Designer exportiert wurde.
* Klicken Sie auf **Speichern**.

</td>
<td style="border: 0;" valign="top">

![](../../assets/roblox-04-roblox-create-material.gif){width="512px"}

</td>
</tr>
</table>

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

### Material anwenden

Verwenden Sie Ihre neue Materialvariante in Ihrer Roblox-Szene

* *Wählen Sie* beliebige Teile oder Gitter in Ihrer Roblox-Szene aus.
* Wählen Sie im **Materialmanager** Ihre *Materialvariante* aus und klicken Sie auf die Schaltfläche **Auf ausgewählte Teile anwenden**

>[!NOTE]
>
> Wenn die Texturfarbe in Roblox anders aussieht, überprüfen Sie das **Color**-Attribut in der Kategorie **Aussehen** in den Eigenschaften des Objekts, auf das der Materialvariante angewendet wird, und stellen Sie sicher, dass es auf *Reinweiß* festgelegt ist - d. h. auf RGB (255, 255, 255), das in Roblox mit *Institutionelles Weiß* gekennzeichnet ist.

</td>
<td style="border: 0;" valign="top">

![](../../assets/roblox-05-roblox-apply-material.gif){width="512px"}

</td>
</tr>
</table>

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

### Anpassen der Unterteilung

Der Wiederholungsgrad des Materials auf einer Oberfläche - d.h. die Kachelung - kann jederzeit eingestellt werden.

* Wählen Sie im **Materialmanager** Ihre *Materialvariante* aus und klicken Sie auf die Schaltfläche **Bearbeiten**
* Passen Sie im Fenster &quot;**Variant bearbeiten**&quot; den Wert der Eigenschaft &quot;**Studs pro Kachel**&quot; unter &quot;**Additional**&quot; an - ein *Lower*-Wert führt zu *more*-Wiederholung

</td>
<td style="border: 0;" valign="top">

![](../../assets/roblox-06-roblox-adjust-tiling.gif){width="512px"}

</td>
</tr>
</table>
