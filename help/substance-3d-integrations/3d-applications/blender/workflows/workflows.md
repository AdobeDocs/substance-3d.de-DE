---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/blender/workflows.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie Substance-Materialien mit Blenderzyklen und Evee-Renderern für verschiedene Workflows verwenden.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Blender > Workflows
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Workflows
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 0%

---


# Workflows

## Arbeiten mit Zyklen

Standardmäßig werden Parameteränderungen im 3D-Ansichtsport nicht automatisch aktualisiert, wenn sie in der Ansicht &quot;Zyklen&quot; angezeigt werden. Um Aktualisierungen in der Ansicht &quot;Zyklen-Rendering&quot; anzuzeigen, aktivieren Sie in den Voreinstellungen die Option **Zyklen Texturen automatisch aktualisieren**, um die Aktualisierung zu erzwingen.

## Multigraph-SBSAR-Dateien

Das Add-on unterstützt .sbrar-Dateien mit mehreren Substance-Diagrammen. Wenn Sie eine Datei mit mehreren Diagrammen laden, wird im Bedienfeld &quot;Substance 3D&quot; ein neues Diagramm-Dropdown-Menü angezeigt. Im Gegensatz zu anderen Parameteränderungen wird das Material beim Umschalten zwischen den Diagrammen nicht automatisch aktualisiert. Aus diesem Grund muss die Schaltfläche **Anwenden** verwendet werden, um das Material nach dem Ändern der Diagramme erneut zuzuweisen.

>[!NOTE]
>
> Standardmäßig fügt die Schaltfläche &quot;Anwenden&quot; das Material in einem neuen Schlitz hinzu, ohne vorherige Materialzuweisungen zu überschreiben. Entferne vorherige Materialien, oder verwende die Dropdown-Liste, um neu angewendete Materialien neu zuzuweisen.

![](https://helpx-prod.scene7.com/is/image/HelpxProd/blender-workflows-multigraphs?$png$&jpegSize=100&wid=168)

## Arbeiten mit Bildeingaben

Wenn Sie ein Substance-Material verwenden, das benutzerdefinierte Bildeingaben zulässt, können Sie mit einem Bildauswahlparameter im Substance 3D-Bedienfeld den Dateibrowser für ein Bild öffnen (Ordnersymbol) oder aus einem Bild auswählen, das in Ihrem Projekt vorhanden ist (Bildsymbol-Dropdownliste).

Mit der Voreinstellung &quot;Bildformat exportieren&quot; können in Blender generierte Bildeingaben in den temporären Ordner gespeichert werden. Weitere Informationen finden Sie auf der Seite [Voreinstellungen](../../../3d-applications/blender/preferences/preferences.md).

![](../../../assets/blender-workflows-image-inputs-steps.png)

## Shader Network-Vorgaben.

Die Shader-Vorgabe kann über die Dropdown-Liste im Abschnitt &quot;Ausgaben&quot; des Substance 3D-Bedienfelds schnell angepasst werden. Diese Shader-Vorgaben passen die Art und Weise an, wie Bildtexturen angewendet werden. Cycles/Eveve Standard verwendet eine reguläre UV-Textur-Koordinatenzuordnung. Die anderen drei Voreinstellungen für Zyklen/Eveve-Projektion verwenden eine generierte Texturkoordinatenzuordnung für Box-, Kugel- oder Zylinderprojektionsmethoden.

Die von Materialien verwendete Standard-Shader-Vorgabe kann im Add-on [Voreinstellungen](../../../3d-applications/blender/preferences/preferences.md) ausgewählt werden.

![](../../../assets/2022-08-12-12-12-33-adobeexpress-1.gif)

## Filtern und Anpassen von Ausgaben

Der Abschnitt &quot;Ausgaben&quot; des Substance 3D-Bedienfelds enthält auch Optionen zum Filtern von Ausgaben. Mit drei Schaltflächen neben der Dropdown-Liste für die Shader-Vorgabe können Sie nach aktivierten Ausgaben (Häkchen), Shader-Ausgaben (Kugel) und allen verfügbaren Ausgaben (Zeilen) filtern.

Die Ausgaben können einzeln über das Kontrollkästchen aktiviert werden. Wenn eine Ausgabe aktiviert ist, wird eine entsprechende Ausgabe in der Texturknotengruppe erstellt. Wenn diese Ausgabe vom Materialknoten Principled BSDF unterstützt wird, wird sie automatisch mit ihr verbunden. Height stellt eine Verbindung zu einem Versatz-Knoten her, und Ambient Verdeckung wird mit der Grundfarbe in einem MixRGB-Knoten kombiniert.\
Das Dropdown-Menü für das Dateiformat neben dem Häkchen kann verwendet werden, um den Dateityp festzulegen, als dem die Ausgabetextur gespeichert wird.

Darüber hinaus können die Standardeinstellungen für die Dateiausgabe im Add-on &quot;[Voreinstellungen](../../../3d-applications/blender/preferences/preferences.md)&quot; geändert werden.

## Materialien auf Objekten austauschen

Klicke auf das Kugelsymbol im Bedienfeld &quot;Materialeigenschaften&quot; des Mischers, um eine Liste der Materialien in deinem Blende-Projekt zu öffnen. Substance-Materialien, die im Bedienfeld erstellt wurden, werden ebenfalls in der Liste angezeigt. Wenn Sie ein Material aus dieser Liste auswählen, wird das aktive Material in diesem Materialschlitz ersetzt.

## Verschiebung

Versatz des Gitters aus Texturen, die im Zyklen-Renderer unterstützt werden, jedoch nicht in &quot;Gleichmäßig&quot;. Um den Versatz anzuzeigen, stellen Sie sicher, dass die Height-Ausgabe aktiviert ist. Das Add-On setzt die Materialeinstellungen automatisch auf **Versatz und Bump** Versatz. Beim Anzeigen des Materials eines Objekts wird jetzt Versatz in der Renderansicht angezeigt. Der Versatz-Maßstab kann im Materialbedienfeld oder auf dem Versatz-Knoten justiert werden.

Um optimale Ergebnisse zu erzielen, sollten Sie höhere Unterteilungsebenen oder hochpolare Gitter für Versätze mit komplexen Materialdetails verwenden.
