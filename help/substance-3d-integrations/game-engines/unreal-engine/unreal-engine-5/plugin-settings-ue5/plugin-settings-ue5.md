---
helpx_url: "https://helpx.adobe.com/de/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/plugin-settings-ue5.html"
breadcrumb-title: ''
description: Konfigurieren Sie die Substance-Plug-in-Einstellungen in Unreal Engine 5 über "Projekteinstellungen", um das Plug-in-Verhalten anzupassen.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 5 > Plugin Settings - UE5
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Plug-in-Einstellungen - UE5
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---


# Plug-in-Einstellungen - UE5

Um auf die Einstellungen zuzugreifen, gehen Sie zu Bearbeiten > Projekteinstellungen , scrollen Sie nach unten zur Kategorie Plug-ins und klicken Sie auf Substance.

![](../../../../assets/screen-shot-2022-03-31-at-5-50-29-pm.png)

## Hardware-Budget

Das Speicherbudget ist die maximale Speichermenge, die für die Substance-Engine verwendet werden darf. Kann erhöht werden, um die Substance-Verarbeitung zu beschleunigen, benötigt jedoch mehr Systemressourcen. (Nicht immer eine hilfreiche Steigerung auf Projektebene).

CPU-Kerne bestimmt, wie viele Kerne die Substance-Engine verwenden darf. Dies umfasst sowohl physische Kerne als auch Hyperthreads. (Wenn die zugewiesene Anzahl größer als die verfügbaren Kerne auf einem System ist, wird standardmäßig alle verfügbaren Kerne verwendet.

## Kochen

Die beim Kochen entfernte Mip-Level-Zahl ändert, wie Texturen für ein Paket erstellt werden. Diese Einstellung kann die Ladezeiten erheblich verbessern und die Paketgröße reduzieren, da die größeren Textur-MIP-Level nicht mehr geladen werden müssen. Die niedrigere Auflösung/die kleineren LODs werden geladen und die höchsten werden standardmäßig mit UE5 vorgegeben. Die Substance werden dann über die Substance-Engine verarbeitet und zur Laufzeit mit den hochauflösenden LODs aktualisiert.

Das Substance Engine kann CPU oder GPU sein. Mit der GPU-Engine können Sie 4K-Texturen erstellen. Die CPU-Engine ist auf 2K begrenzt.

## Optimierung:

Dadurch wird begrenzt, wie viele asynchrone Substanzen pro Charge an den Substance-Motor übergeben werden können. Niedrigere Zahlen beschleunigen den Abschluss und die Aktualisierung einer asynchronen Aufgabe, bei der höhere Zahlen Batch-Renderings durchführen und mehrere Substance gleichzeitig verarbeiten. (Je höher die Anzahl, desto abgehackter werden die Texturaktualisierungen, da die Zeit zwischen den Aktualisierungen länger ist).

## Async/Sync-Rendering

Beim Synchronisationsrendering wird der Rendering-Aufruf blockiert. Dadurch wird eine Substance-Graph-Instanz an die neu zu berechnende Substance-Engine übergeben. Die Ausführung wird jedoch angehalten, bis die Substance-Engine die Verarbeitung der Substance abgeschlossen hat, bevor mit der weiteren Codeausführung fortgefahren wird. Das Ergebnis wird auch auf Ihrem Bildschirm aktualisiert, sobald der Vorgang abgeschlossen ist.

Async fügt das Diagramm zu einer Warteschlange hinzu und sendet mehrere Graphen gleichzeitig an die Substance-Engine (von den Substance-Einstellungen aus eingestellt) innerhalb des Plug-in-Updates. Im Gegensatz zum Synchronisationsrendering läuft das Programm, sobald es versendet wird, wie gewohnt weiter, anstatt darauf zu warten, dass die Substance-Engine vollständig ist. Wenn die Substance-Engine diesen Stapel fertig gestellt hat, werden die Ergebnisse zurückgesendet, auf die Ausgaben angewendet und ein weiterer Stapel gestartet.
