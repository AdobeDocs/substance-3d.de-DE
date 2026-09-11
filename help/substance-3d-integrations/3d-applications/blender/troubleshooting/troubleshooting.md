---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/blender/troubleshooting.html"
breadcrumb-title: ''
description: Diagnostizieren und beheben Sie häufige Probleme mit dem Substance 3D-Add-on in Blender über die Systemkonsole.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Blender > Troubleshooting
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Fehlerbehebung
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '812'
ht-degree: 0%

---


# Fehlerbehebung

Die Systemkonsole kann verwendet werden, um Fehler zu diagnostizieren, die bei der Verwendung des Add-Ons aufgetreten sind. Das Konsolenfenster von Blender wird je nach Betriebssystem unterschiedlich geöffnet. Ausführliche Anweisungen finden Sie in den Schritten auf der [-Dokumentationsseite von Blender auf der Systemkonsole &#x200B;](https://docs.blender.org/manual/en/2.79/advanced/command_line/introduction.html#console-window-status-and-error-messages). Die Konsolenausgabe kann hilfreich sein, wenn unerwartete Probleme auftreten, z. B. wenn Texturen nicht geladen werden oder Materialien bei der Verarbeitung hängen bleiben.

Um einen Fehler zu melden, nehmen Sie am #substance-blender-beta auf dem [Substance Discord-Server](https://discord.com/invite/substance3d) teil oder besuchen Sie [Adobe Communities](https://community.adobe.com/t5/substance-3d-plugins/ct-p/ct-substance-3d-plugins?page=1&sort=latest_replies&lang=all&tabid=all&topics=label-blender). Relevante Informationen aus dem Konsolenprotokoll und alle Reproduktionsschritte für das Problem können in die Berichte aufgenommen werden.

## Häufige Probleme und Lösungen

* *WMIC-bezogene Konsolenfehler.*
  * *Gelegentlich enthalten Windows-Installationen kein WMIC, was in diesem Fall erforderlich ist. So können Sie dies manuell beheben:*
    * Wechseln Sie zu Einstellungen - System - Optionale Funktionen
    * Wählen Sie &quot;Funktionen anzeigen&quot; und dann &quot;Optionale Funktion hinzufügen&quot; aus.
    * Daraufhin wird ein neues Fenster angezeigt. Scrollen Sie in der Liste nach unten, um WMIC zu suchen. Aktivieren Sie das Kontrollkästchen, und drücken Sie dann die Taste Weiter.
    * Sie sollten jetzt zu einem neuen Fenster weitergeleitet werden, das den Fortschritt der WMIC-Installation unter den letzten Aktionen anzeigt.
    * *Beachten Sie, dass der Download einige Minuten dauern kann. Setzen Sie danach Ihren Computer zurück und starten Sie Blender und das Add-on neu. Wenn Sie im Substance 3D-Bedienfeld auf &quot;Laden&quot; klicken, sollte jetzt das Dateibrowserfenster angezeigt werden.*
  * Wenn das Problem dadurch nicht gelöst wird, müssen Sie möglicherweise auch WMIC in Ihren PATH-Variablen definieren. Weitere Informationen zu Ihrer spezifischen Version von Windows finden Sie in der Dokumentation .
* *Nach dem Aktualisieren des Add-Ons und dem Laden eines Materials werden nicht alle Einstellungen im Substance 3D-Bedienfeld angezeigt.*
  * Dies kann passieren, wenn Sie eine ältere Version des Add-Ons entfernen und eine neuere Version in derselben Sitzung installieren, da ältere Dateien immer noch im System zwischengespeichert werden können.\
    Beim Neustart des Mischers sollten die Änderungen wirksam werden.
* *Probleme bei der Installation des Add-Ons./ Material bleiben bei der Verarbeitung zwischen den Sitzungen hängen. / Materialien generieren keine Texturen zwischen den Sitzungen. / Fehler beim Laden von .sbsar-Dateien.*
  * Dies kann ein Problem bei der Installation der Integrationstools sein und wird in der Regel durch manuelles Entfernen der Tools behoben. Auf der Seite [Deinstallieren des Add-ons](../../../3d-applications/blender/uninstalling-the-add-on/uninstalling-the-add-on.md) finden Sie Anweisungen zum manuellen Entfernen.
* *Materialien werden in der Zyklen-Renderansicht nicht aktualisiert*.
  * Standardmäßig aktualisiert das Add-on die Texturen in der Renderansicht &quot;Zyklen&quot; nicht. Sie können jedoch eine Aktualisierung erzwingen, indem Sie die Texturen für die automatische Aktualisierung <b>Cycles</b> in den Add-On-Einstellungen aktivieren.
* Parameter scheinen nach dem Speichern während der Zyklen-Renderansicht zurückgesetzt zu werden.
  * Dies ist ein bekanntes Caching-Problem auf der Mischerseite, das nur visuell angezeigt wird. Beim Speichern wird keine Meldung zum Aktualisieren der generierten Textur an das Remote-Engine gesendet. Die Texturen werden normal angezeigt, nachdem Sie die Zyklen-Renderansicht verlassen und zurück zu ihr gewechselt sind.
* *Material werden nach dem Rückgängigmachen/Ändern von Parametern nicht mehr aktualisiert.*
  * Material können möglicherweise nicht aktualisiert werden, nachdem Aktionen rückgängig gemacht wurden. Die Parameter werden in den vorherigen Zustand zurückgesetzt, die Texturen werden jedoch nicht rückgängig gemacht. Damit die Textur erneut aktualisiert wird, verwenden Sie die Schaltfläche &quot;Aktualisieren&quot;, um die Parameter auf die Standardeinstellungen zurückzusetzen und die Texturen neu zu laden.
* *Die im Substance Designer festgelegten Farben werden im Farbwähler des Mischers leicht unterschiedlich angezeigt, und die Farbwerte sind nicht identisch.*
  * Der Mischer wendet eine Gamma-Korrektur nur auf Farben für den Farbwähler des Mischers an. Dies verursacht zwar eine Diskrepanz im Farbwähler, aber die in den Texturen angezeigten Farben stimmen mit den in Substance-Apps festgelegten Werten überein.
* *Konsolenfehler &quot;wmic is not Recognition&quot; beim Laden eines Materials in Windows.*
  * Dieses Problem tritt auf, wenn C:\Windows\System32\wbem\ nicht in PATH-Systemvariablen enthalten ist. Weitere Informationen zu Ihrer spezifischen Version von Windows finden Sie in der Dokumentation .
* *Fehler &quot;Ungültiger CPU-Typ ist ausführbar&quot; in Mac.*
  * Dieses Problem tritt auf, wenn Rosetta auf ARM-Computern mit Mac nicht aktiviert ist. Weitere Informationen finden Sie unter [Apple Rosetta-Seite](https://support.apple.com/en-us/102527). Weitere Anweisungen finden Sie außerdem in diesem [Installationshandbuch](https://medium.com/@jithmisha/fix-for-macbook-air-m1-m2-bad-cpu-type-in-executable-error-3719a0a1cb6).
* *Änderungen am Shader-Graf werden rückgängig gemacht, wenn die Schaltfläche &quot;Aktualisieren&quot; oder die Aktualisierungsparameter verwendet werden.*
  * Das Add-on hat Verbindungen im Diagramm nach Änderungen oder Aktualisierungen aktualisiert. Um dies zu umgehen, duplizieren Sie das aus der .sbsar-Datei erstellte Mischermaterial und geben Sie ihm einen neuen Namen Ihrer Wahl. Fügen Sie Ihre Knoten nur zum Duplikat hinzu. Die Texturen werden in der Knotengruppe aktualisiert, wobei vom Benutzer hinzugefügte Knoten erhalten bleiben. Kopieren Sie diese Knoten beim Aktualisieren und fügen Sie sie nach der Aktualisierung wieder in ein neues Diagramm ein.
