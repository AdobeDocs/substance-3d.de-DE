---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/blender/the-substance-3d-panel.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie das Bedienfeld "Substance 3D" in Blender verwenden, um Materialien, Parameter und Ausgaben zu verwalten.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Blender > The Substance 3D Panel
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Das Bedienfeld "Substance 3D"
user-guide-description: ''
user-guide-title: ''
source-git-commit: 4a060ee1aaa1731c04e70d5512e3271cd63d0381
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 0%

---


# Das Bedienfeld &quot;Substance 3D&quot;

![](../../../assets/blender-substance3dpanel.png)

## Bedienfeldsteuerelemente

**Erstellen** - Öffnet den Dateibrowser zum Auswählen eines Substance 3D-Materials. Standardmäßig wird dadurch ein Mischermaterial erstellt, das Texturen verwendet, die aus der .sbsar-Datei generiert wurden.

**Anwenden** - Hängen Sie das ausgewählte Substance 3D-Material an die ausgewählten Objekte in einem neuen Materialschlitz an. Vorherige Materialzuweisungen für das Objekt werden dadurch nicht überschrieben.

**Substance 3D Community Assets** : Öffnet die Substance 3D Community Assets-Seite im Webbrowser.

**Substance 3D Assets** - Öffnet die Substance 3D Assets-Quellseite im Webbrowser.

**Ausgewähltes Substance 3D-Material duplizieren** - Lädt eine neue Instanz des ausgewählten Substance 3D-Materials. Die Parameter verschiedener Instanzen desselben Substance-Materials können unabhängig voneinander eingestellt werden.

**Aktualisieren** - Lädt das Substance 3D-Material erneut

>[!WARNING]
>
> **Warnung:**
> 
> Mit der Schaltfläche &quot;Aktualisieren&quot; werden alle Benutzeränderungen am Shader-Diagramm rückgängig gemacht. Kopieren Sie vor der Aktualisierung alle vom Benutzer hinzugefügten Knoten, um sie nach der Aktualisierung in das Diagramm einzufügen.

**Entfernen** - Entfernt das ausgewählte Substance 3D-Material aus dem Bedienfeld.

>[!NOTE]
>
> Das aus dem Substance-Material erstellte Mischermaterial bleibt im Projekt erhalten. Es kann manuell aus Objekten gelöscht oder entfernt werden.

**Geladene 3D-Substance-Materialien** - Zeigt eine Liste der Substance-Materialien an, die in die .blend-Datei geladen wurden.

## Diagrammparameter

**Ausgabeauflösung** - Dropdowns für die Auflösung mit und Height. Sie können die Verknüpfung aufheben, um die Werte unabhängig voneinander anzupassen.

**Zufallsverteilung und Zufallsverteilung** - Die Schaltfläche &quot;Zufallsverteilung&quot; generiert einen neuen Zufallswert, um Parameter zu ändern, die Zufallswerte verwenden können. Der Zufallswert kann auch manuell eingestellt werden.

## Arbeiten mit Vorgaben

SBSAR-Dateien können mit Vorgaben veröffentlicht werden, die Sie im Dropdown-Feld Vorgaben finden. Um eigene Vorgaben zu erstellen, passen Sie die Parameter wie gewünscht an und verwenden Sie die Schaltfläche **Speichern**. Es gibt zusätzliche Optionen, um die ausgewählte Voreinstellung als .sbsprs -Datei zu exportieren und die ausgewählte Voreinstellung aus der Dropdown-Liste zu löschen. Die Schaltfläche **Laden** kann zum Importieren von Vorgaben aus .sbsprs-Dateien verwendet werden.

## Substance-Parameter

Parameter, die in Substance Designer gelegt wurden, können mit den Substance Parameter-Steuerelementen angepasst werden. Diese Parameter werden vom Ersteller des Substance-Materials festgelegt und variieren zwischen den Materialien. Durch Anpassen dieser Parameter werden die generierten Texturen aktualisiert, wie durch das Verarbeitungssymbol neben dem Namen des Materials im Abschnitt Geladene 3D-Substance-Materialien angegeben.

Das Dateiformat der Ausgabe-Texturen kann über die Dropdown-Menüs geändert werden.

Weitere Informationen finden Sie auf der Designer-Dokumentationsseite unter [, das einen Parameter Legt](https://experienceleague.adobe.com/en/docs/substance-3d-designer/using/substance-graphs/manage-parameters/exposing-a-parameter).

## Technische Parameter

Substance-Material können eine Reihe von technischen Parametern aufweisen. Dies sind zusätzliche Steuerelemente für Farbkorrekturen und andere Material-Anpassungen.
