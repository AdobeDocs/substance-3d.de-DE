---
helpx_url: "https://helpx.adobe.com/de/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-4/plugin-settings-ue4.html"
breadcrumb-title: ''
description: Konfigurieren Sie die Substance-Plug-in-Einstellungen in Unreal Engine 4 über "Projekteinstellungen", um das Plug-in-Verhalten anzupassen.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 4 > Plugin Settings - UE4
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Plugin Settings - UE4
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '567'
ht-degree: 0%

---


# Plugin Settings - UE4

Um auf die Einstellungen zuzugreifen, gehen Sie zu Bearbeiten > Projekteinstellungen , scrollen Sie nach unten zur Kategorie Plug-ins und klicken Sie auf Substance.

![](../../../../assets/settings-36.png){width="400px"}

## Hardware-Budget

Das Speicherbudget ist die maximale Speichermenge, die für das Substance-Engine verwendet werden darf. Kann erhöht werden, um die Geschwindigkeit der Substanzverarbeitung zu verbessern, verbraucht aber mehr Systemressourcen. (Nicht immer eine hilfreiche Steigerung auf Projektebene).

Die CPU-Kerne geben an, wie viele Kerne das Substance-Engine verwenden darf. Dies umfasst sowohl physische Kerne als auch Hyperthreads. (Wenn die zugewiesene Anzahl größer als die verfügbaren Kerne auf einem System ist, wird standardmäßig alle verfügbaren Kerne verwendet.

## Kochen

Die beim Kochen entfernte Mip-Level-Zahl ändert, wie Texturen für ein Paket erstellt werden. Diese Einstellung kann die Ladezeiten erheblich verbessern und die Paketgröße reduzieren, da die größeren Textur-MIP-Level nicht mehr geladen werden müssen. Die niedrigere Auflösung/die kleineren LODs werden geladen und die höchste wird standardmäßig vom UE4 vorgegeben. Die Stoffe werden dann über das Substance-Engine verarbeitet und zur Laufzeit mit den hochauflösenden LODs aktualisiert.

Das Substance Engine kann CPU oder GPU sein. Mit dem GPU-Engine können Sie 4K-Texturen erstellen. Das CPU-Engine ist auf 2K begrenzt.

## Standardgenerierung:

Der Substance-Generierungsmodus (SGM) steuert, wie die Texturen generiert werden. Dies ist ein globales Umfeld für Substance. Die SGM kann pro Substance in der Substance Factory geändert werden.

**SGM Baking geführt**: Baking führe die Texturen des Stoffes. Sie verlieren die Möglichkeit, Parameter zur Laufzeit zu ändern.

**SGM beim Laden der Synchronisation**: Sperrt die Anwendung, während die Substance geladen werden.

**SGM beim Laden von Sync und Cache**: Zwischenspeichert ein Zwischenergebnis der Textur auf dem Datenträger.

**SGM beim Laden von Async**: Nicht blockierend. Im Hintergrund werden Substance erzeugt.

**SGM beim Laden von Async und Cache**: Zwischenspeichert ein Zwischenergebnis der Textur auf dem Datenträger.

***Plattformstandard ist Async laden und Cache***

## Substance Factory

Um die SGM für eine Substance zu ändern, klicken Sie mit der rechten Maustaste auf die Substance Factory > Elementaktionen > Massenbearbeitung über Eigenschaftsmatrix. Sie können dann die SGM ändern.

![](../../../../assets/sgm.png){width="800px"}

## Optimierung:

Dadurch wird begrenzt, wie viele asynchrone Stoffe pro Charge an das Substance-Engine abgegeben werden können. Niedrigere Zahlen beschleunigen die Geschwindigkeit, mit der eine asynchrone Aufgabe abgeschlossen und aktualisiert wird, wenn höhere Zahlen Batch-Renderings durchführen und mehrere Substanzen gleichzeitig verarbeiten. (Je höher die Zahl, desto abgehackter werden die Aktualisierungen der Texturen, da die Zeit zwischen den Aktualisierungen länger ist).

## Async/Sync-Rendering

Beim Synchronisationsrendering wird der Rendering-Aufruf blockiert. Dadurch wird eine Substance-Grapheninstanz an das neu zu berechnende Substance-Engine übergeben. Die Ausführung wird jedoch gestoppt, bis das Substance-Engine die Verarbeitung der Substanz abgeschlossen hat, bevor mit der weiteren Codeausführung fortgefahren wird. Das Ergebnis wird auch auf Ihrem Bildschirm aktualisiert, sobald der Vorgang abgeschlossen ist.

Async fügt Ihren Graf einer Warteschlange hinzu und sendet mehrere Graf gleichzeitig an das Substance-Engine (von den Substance-Einstellungen aus festgelegt) innerhalb des Plug-in-Updates. Im Gegensatz zum Sync-Rendering läuft das Programm, sobald es versendet wird, wie gewohnt, anstatt darauf zu warten, dass das Substance-Engine abgeschlossen ist. Wenn das Substance-Engine den Stapel fertig gestellt hat, werden die Ergebnisse zurückgesendet, auf die Ergebnisse angewendet und ein weiterer Stapel gestartet.
