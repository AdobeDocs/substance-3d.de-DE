---
helpx_url: "https://helpx.adobe.com/de/substance-3d-integrations/3d-applications/3ds-max/troubleshooting.html"
breadcrumb-title: ''
description: Diagnostizieren und beheben Sie Probleme mit dem Substance-Plugin in 3ds Max mithilfe des Script Listener, um Fehlermeldungen zu erhalten.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > 3ds Max > Troubleshooting
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Fehlerbehebung
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 1%

---


# Fehlerbehebung

Der Scripting Listener kann verwendet werden, um Fehler zu diagnostizieren, die bei der Verwendung des Plug-ins auftreten. Um den Skript-Listener zu öffnen, navigieren Sie zu Skriptmenü > Skriptlistener. Wenn während der Verwendung des Plug-ins ein Fehler auftritt, wird eine entsprechende Fehlermeldung in diesem Script Listener-Fenster angezeigt. Weitere Informationen finden Sie in der [Dokumentation des offiziellen Skripteditors](https://help.autodesk.com/view/3DSMAX/2023/ENU/?guid=GUID-C8019A8A-207F-48A0-985E-18D47FAD8F36).

Um einen Fehler zu melden, nehmen Sie am #3dsmax-plugin auf dem [Substance Discord-Server](https://discord.com/invite/substance3d) teil oder besuchen Sie [Adobe Communities](https://community.adobe.com/t5/substance-3d-plugins/ct-p/ct-substance-3d-plugins?page=1&sort=latest_replies&lang=all&tabid=all&topics=label-autodesk3dsmax). Relevante Informationen aus dem Konsolenprotokoll und alle Reproduktionsschritte für das Problem können in die Berichte aufgenommen werden.

## Bekannte Probleme

* *Das Ersetzen einer .sbsar-Datei, die eine diffuse Ausgabe verwendet, durch eine .sbsar-Datei, die keine diffuse Ausgabe verwendet, führt aufgrund der Trennung der fehlenden diffuse Ausgabe zu schwarzem Rendering.*
  * Dieses Verhalten wird für mehrere Ausgabeknoten erwartet. Anstatt diese .sbsars mit demselben Knoten zu laden, sollten Sie für jeden Knoten einen anderen Substance verwenden.
