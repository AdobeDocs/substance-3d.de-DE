---
helpx_url: "https://helpx.adobe.com/de/substance-3d-integrations/3d-applications/blender/preferences.html"
breadcrumb-title: ''
description: Konfigurieren Sie die Voreinstellungen für das Substance 3D-Add-on in Blender, um das Verhalten und die Einstellungen des Plug-ins anzupassen.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Blender > Preferences
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Voreinstellungen
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '845'
ht-degree: 0%

---


# Voreinstellungen

Die Add-On-Voreinstellungen finden Sie im Fenster &quot;Einstellungen&quot; von Blender. Navigieren Sie zu Bearbeiten > Voreinstellungen > Add-ons und suchen Sie nach Knoten: Adobe Substance 3D-Add-on für Blender.

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![Erste Hälfte des Menüs für Add-On-Einstellungen.](../../../assets/blender-prefs-1.png)

</td>
<td style="border: 0;" valign="top">

![Zweite Hälfte des Add-On-Voreinstellungsmenüs.](../../../assets/blender-prefs-2-b.png)

</td>
</tr>
</table>

<b>Deinstallieren</b> - Löscht das Add-On aus dem System und entfernt es aus der Add-On-Liste in Blender.

<b>Fehler melden</b> - Öffnet Substance 3D for Blender Discord.

<b>Ordner &quot;Tools akzeptieren&quot;</b> : Öffnet den Blender-Dateibrowser und wählt den Installationspfad für Substance Integration Tools aus.

<b>Tools öffnen </b>: Öffnen Sie den Systemdateibrowser am Speicherort des Ordners &quot;Integrationstools&quot;.

<b>Pfad zurücksetzen</b> - Setzt den Ordnerpfad der Integrationstools auf den Standardspeicherort zurück.

<b>Deinstallationstools</b> - Entfernt die installierte Version der Substance 3D Integration Tools.

<b>Update Tools</b> - Öffnet den Dateibrowser, um die Zip-Datei für Tools auszuwählen und die Tools zu aktualisieren.

<b>Dokumentation</b> - Öffnet die Dokumentationsseite &quot;Ökosystem und Plug-Ins&quot; im Browser.

<b>Foren</b> - Öffnet die Adobe-Community-Foren im Browser.

<b>Discord Server</b> - Öffnet den Discord-Server für das Ökosystem und die Plug-Ins im Browser.

<b>Kachelung</b> - Passen Sie die X-, Y- und Z-Kachelung des Materials an. Die Sperre kann verwendet werden, um die Verknüpfung der Werte aufzuheben und sie einzeln anzupassen.

<b>Auflösung</b> - Die Standardauflösung für generierte Texturen. Die Sperre kann zum Aufheben der Verknüpfung verwendet werden, um die Auflösung unabhängig voneinander festzulegen.

<b>Typ &quot;</b>&quot; anwenden: Legt das Verhalten der Schaltfläche &quot;Anwenden&quot; fest: <b>Durch Einfügen von </b> wird das aktuelle Material mit dem ausgewählten Substance-Material überschrieben, und durch <b>Anhängen</b> wird das Material dem Objekt in einem neuen Material-Steckplatz hinzugefügt.

<b>Bildformat exportieren</b> - Wenn in Blender generierte Bilder als Bildeingaben für ein Substance-Material verwendet werden, wird dieses Format verwendet, um dieses Bild im Zeitordner zu speichern.

<b>Standardmäßig ausgeblendete Eingabegruppen</b> - Schaltet nach Bedarf um, ob die Eingabegruppen des Substance-Materials standardmäßig erweitert oder ausgeblendet sind.

<b>Nur Texturen standardmäßig aktualisieren</b> - Schaltet die Substance-Parameter für die Wetteraktualisierung um und wirkt sich nur auf die Texturen der Ausgabe im Netzwerk der Blender-Schattierung aus. Wenn Sie diese Option deaktivieren, werden die Knotenverbindungen nach dem Anpassen der Parameter zurückgesetzt. Die Aktivierung wird empfohlen, wenn einem Material weitere Knoten hinzugefügt werden, andernfalls werden diese nach dem Anpassen der Parameter getrennt.

<b>Substance Remote-Engine </b>: Legt die vom Substance Remote-Engine verwendete Hardware fest.

<b>Material automatisch anwenden</b> - Wenn ein Substance-Material erstellt wird, wird das Material automatisch an die ausgewählten Objekte in einem neuen Material-Steckplatz angehängt.

<b>Material für ausgewählte Objekte automatisch markieren</b> - Ändern Sie das markierte Material im Bedienfeld &quot;Substance 3D&quot;, wenn ein Objekt mit diesem Material ausgewählt ist.

<b>Zyklen Automatische Aktualisierung von Texturen</b> - Erzwingt die Aktualisierung der Textur im 3D-Viewport, während die Zyklen-Renderansicht verwendet wird.

<b>Bestätigung zum Löschen der Vorgabe entfernen</b> - Entfernt das Bestätigungsfenster, das beim Löschen von Materialvorgaben angezeigt wird.

<b>Material mit aktiviertem gefälschtem Benutzer erstellen</b> - Legt fest, ob das Material mit aktiviertem oder deaktiviertem &quot;gefälschtem Benutzer&quot; erstellt wird. Mischerdaten, die als gefälschter Benutzer markiert sind, werden nach dem Schließen nicht bereinigt, auch wenn die Daten nicht verwendet werden.

<b>Das Substance-Remote-Engine &quot;</b>&quot; automatisch starten - Schaltet um, wenn das Substance-Remote-Engine beim Starten von Blender initialisiert wird. Wenn diese Option deaktiviert ist, startet das Remote-Engine nur, wenn ein Benutzer den Tastaturbefehl lädt oder verwendet.

>[!NOTE]
>
> HINWEIS: Bei Verwendung von Substance Connector muss das SRE aktiv sein, damit die sendende Anwendung Blender als Endpunkt erkennt.

<b>SBSAR-Bibliothekspfad</b> - Der Ordner, der standardmäßig geöffnet wird, wenn die Schaltfläche &quot;Laden&quot; zum Suchen nach einer Substance-Datei verwendet wird.

<b>Temporärer Ordner </b>: Dieser Ordner ist der Standardspeicherort, an dem Texturen gespeichert werden, bevor eine Datei zum ersten Mal gespeichert wird.

<b>SBSAR-Dateien beim Speichern in </b> kopieren - Wenn diese Option aktiviert ist, werden SBSAR-Dateien in den angegebenen relativen Pfad kopiert, wenn die Datei gespeichert wird. Dies kann die gemeinsame Nutzung von Projekten zwischen Geräten erleichtern.

<b>Kopieren Sie beim Speichern die Texturen nach </b>: Wenn eine Datei zum ersten Mal gespeichert wird, werden die Texturen im temporären Ordner an diesen Speicherort kopiert. Die Variable $matname wird verwendet, um Unterordner für jedes Material zu erstellen.

<b>Shader-Vorgabe</b>: Legt die standardmäßige Shader-Vorgabe fest, die beim Erstellen von Blender-Materialien aus Substance-Dateien verwendet wird. Kann auf den Standard für UV-basierte Zuordnung oder auf die Projektion für box-, sphere- und zylinder-Projektion-basierte Zuordnung gesetzt werden.

<b>Versatz mittlerer Stufe</b> - Der Standardwert ist die Grundlage für Versatz im Versatz. Höhere Werte als der Standardwert schieben die Flächen nach außen und niedrigere Werte ziehen die Flächen nach innen.

<b>Versatz-Skalierung</b>: Der Standardskalierungswert im Versatz-Knoten.

<b>Emissive-Intensität</b> - Der Standardwert für die Emissions-Stärke im Knoten Principled BSDF.

<b>Überblendung der Projektion</b>: Legt den Grad der Überblendung zwischen den Winkeln für die Projektion-Methodenschattierer fest.

<b>AO Mix</b> - Wenn Ambient occlusion als Ausgabe aktiviert ist, bestimmt dieser Wert den Standardfaktorwert des MixRGB-Knotens, der zum Kombinieren der Grundfarbe- und Ambient occlusion-Texturen verwendet wird.

<b>Ausgaben</b> - Die einzelnen Ausgaben von Materialien können aktiviert oder deaktiviert werden. Der Standardfarbraum, das Dateiformat und die Tiefe der Farben der einzelnen Ausgaben können ebenfalls angepasst werden.

<b>Tastaturbefehle </b> - Passen Sie die Tastaturbefehl-Tasten an, die zum Aufrufen eines schwebenden Menüs, zum Laden eines Substance-Materials und zum Anwenden des aktuellen Materials verwendet werden. Tastaturbefehl-Updates müssen neu gestartet werden.
