---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/installing-to-source-builds-ue5.html"
breadcrumb-title: ''
description: Installiere das Substance 3D-Plug-in in den Quell-Builds von Unreal Engine 5, um deine Engine zu modifizieren.
helpx_creative_field: ""
helpx_description: Substance 3D Integrations
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Installation auf Quellcode-Builds - UE5
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '303'
ht-degree: 0%

---


# Installation auf Quellcode-Builds - UE5

Das Substance-Plug-in kann mit Versionen von Unreal Engine verwendet werden, die aus dem Quellcode erstellt wurden. Dazu kann das Plug-in entweder in einem Ordner &quot;C++project&quot; oder im Ordner &quot;Engine&quot; eines Quell-Builds installiert werden.

>[!NOTE]
>
> Für diese Methoden ist es erforderlich, dass Sie eine Version des Plug-ins vom Marketplace heruntergeladen haben. Der Substance-Plugin-Ordner kann zwischen Computern und UE-Builds übertragen werden.

## Installieren in einem C++-Projektordner

1. Erstellen Sie im Projektordner einen Plug-ins -Ordner, falls noch kein Ordner vorhanden ist.
1. Erstellen Sie im Ordner &quot;Plug-ins&quot; einen Runtime-Ordner.
1. Platzieren Sie den Substance-Ordner im Ordner &quot;Runtime&quot;. LINUX-BENUTZER: Suchen Sie nach Schritt 3 den Ordner &quot;include&quot; im Ordner &quot;Substance&quot; und benennen Sie ihn um, um das &quot;i&quot; groß zu machen (include > Include).
1. Starten Sie Unreal Engine.
1. Öffnen Sie das C++-Projekt über den Launcher.
1. Nach dem Starten des Projekts wird Unreal Engine gefragt, ob Sie Plug-in-Komponenten vor dem Start neu erstellen möchten, wählen Sie &quot;Ja&quot;. Dies erfolgt über Microsoft Visual Studio (Windows, Linux) oder Xcode (Mac).
1. Unechtes Engine wird geschlossen, aber die Komponenten werden im Hintergrund erstellt. Dieser Vorgang kann etwa 5 Minuten dauern. Das Projekt wird anschließend geöffnet. Wenn dies fehlschlägt, wird ein Fehlerfenster angezeigt.

## Installieren im Engine-Ordner

>[!NOTE]
>
> Die obigen Schritte müssen ausgeführt werden, um den Binärordner des Plug-ins neu zu erstellen, bevor das Plug-in im Ordner &quot;Engine&quot; installiert werden kann.

1. Kopieren Sie den Substance-Ordner aus dem Projektordner > Plug-ins > Laufzeit.
1. Öffnen Sie den Versionsordner von Unreal Engine und navigieren Sie zu Engine > Plug-ins > Marktplatz.
1. Fügen Sie den Substance-Ordner ein.
1. Öffnen Sie den Unreal Engine Editor. Erstellen Sie bei Bedarf ein neues Projekt.
1. Öffnen Sie das Menü Plug-ins und überprüfen Sie, ob das Substance-Plug-in aktiviert ist.
