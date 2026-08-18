---
helpx_url: "https://helpx.adobe.com/de/substance-3d-integrations/game-engines/unity/upgrading-projects-known-issues.html"
breadcrumb-title: ''
description: Erfahren Sie mehr über das Aktualisieren von Unity-Projekten mit Substance-Materialien und bekannte Probleme, die während der Migration vermieden werden können.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Upgrading ProjectsKnown Issues
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Aktualisieren von ProjektenBekannte Probleme
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 1%

---


# Aktualisieren von Projekten/Bekannte Probleme

>[!WARNING]
>
> Das Substance 3D-Plugin für Unity 3.0.0 unterstützt keine Abwärtskompatibilität. Stellen Sie also sicher, dass Sie Unity 2020.3.27x und höher verwenden.
> 
> Unity hat die Standard-Build-Architektur auf x86 anstelle von x86\_64 geändert.\
> Skripte werden nicht ausgeführt, wenn sie auf Substance verweisen. Sie müssen zu x86\_64 zurückkehren, und der Build funktioniert.

## Bekannte Probleme

* Fehler &quot;*Assertion bei Ausdruck fehlgeschlagen&quot; beim Navigieren zu Bedienfeldordnern.*
  * Dies ist ein Fehler, der auf der Unity-Seite auftritt, wenn Änderungen an der Benutzeroberfläche vorgenommen werden, in der Regel sind Miniaturansichtsänderungen eine harmlose Nachricht.
* *Bildeingaben scheinen auf 8 Bit gesperrt zu sein*
  * Dieses Problem wurde in Version 3.8.0-3 behoben. Der richtige Arbeitsablauf wäre, wenn die Benutzer das Standardformat von Unity für die Textur in RGBA64 ändern würden. Das Plug-in sorgt dafür, dass diese Informationen ordnungsgemäß an Substance Engine gesendet werden.
