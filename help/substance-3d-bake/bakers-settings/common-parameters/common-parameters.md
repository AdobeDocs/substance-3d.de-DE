---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/bakers-settings/common-parameters.html"
breadcrumb-title: ''
description: Erfahren Sie mehr über allgemeine Parameter, die für alle Bäcker gelten, und wie Sie sie für eine optimale Texturgenerierung konfigurieren können.
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Common Parameters
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Häufig verwendete Parameter
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '1068'
ht-degree: 1%

---


# Häufig verwendete Parameter

Allgemeine Parameter gelten für alle Bäcker. Diese Parameter legen in der Regel fest, wie sich die Bäcker verhalten und mit Netzen mit hohem Poly arbeiten, aber wie die endgültigen Texturen erzeugt werden. Einige dieser Parameter können von bestimmten Bäckern überschrieben werden.

Die meisten dieser Parameter stehen in der gesamten Software (einschließlich des Substance Automation Toolkit) zur Verfügung, ihr Verhalten kann jedoch leicht abweichen. oder einige sind je nach Software-Workflow und -Implementierung möglicherweise nicht verfügbar.

## Allgemeine Parameter

Diese Parameter beeinflussen die Art und Weise, wie Bäcker Strukturen erzeugen.

| *Name* | *Beschreibung* |
| --- | --- |
| **Größe**(Standardgröße oder Ausgabegröße) | Steuern Sie die Auflösung der Textur der Backausgabe (in Pixeln).Verfügbare Werte:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>32</strong></li><li data-preserve-html="true"><strong>64</strong></li><li data-preserve-html="true"><strong>128</strong></li><li data-preserve-html="true"><strong>256</strong></li><li data-preserve-html="true"><strong>512</strong></li><li data-preserve-html="true"><strong>1024</strong></li><li data-preserve-html="true"><strong>2048</strong> (Standard)</li><li data-preserve-html="true"><strong>4096</strong></li><li data-preserve-html="true"><strong>8192</strong></li></ul>Nicht quadratische Auflösungen werden ebenfalls unterstützt, z. B.: 2048 x 1024 (Verhältnis 2:1). Im Substance Designer kann dieser Parameter vom Bäcker selbst überschrieben werden. |
| **Format** | Dateiformat der Texturen.*Nicht verfügbar im Substance Painter.* Siehe: [So exportieren Sie die durch Baking erzeugte Map](../../common-questions/how-export-the-baked-maps/how-to-export-the-baked-maps.md). |
| **Anti-Aliasing** | Steuert das Anti-Aliasing. Damit können Sie die Qualität von Texturen im Hintergrund verbessern und Aliasing bei unterschiedlichen Geometrien reduzieren.Weitere Informationen zum Aliasing finden Sie unter: [Aliasing bei UV-Nähten](../../common-issues/aliasing-on-uv-seams/aliasing-on-uv-seams.md) und [Aliasing bei Wikipedia](https://en.wikipedia.org/wiki/Aliasing).Verfügbare Werte:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Keine</strong> (Standard)</li><li data-preserve-html="true"><strong>Subsampling 2x2</strong></li><li data-preserve-html="true"><strong>Subsampling 4x4</strong></li><li data-preserve-html="true"><strong>Subsampling 8x8</strong></li></ul>  **Hinweis:** Das Aktivieren von Anti-Aliasing kann die Backzeit erheblich verlängern, da das Anti-Aliasing funktioniert, indem die Textur mit einer höheren Auflösung berechnet und dann auf die ursprünglich ausgewählte Größe zurückskaliert wird. Das bedeutet, dass eine 2K-Textur mit einem 2x2-Subsampling tatsächlich eine 4K-Textur berechnet.Manchmal ist es vorzuziehen, die Anzahl der Strahlen im Bäcker zu erhöhen, anstatt die Unterabtastung zu erhöhen. So könnten bessere Ergebnisse erzielt werden, ohne zu lange zu warten. |
| **UV-Satz** | Steuert, welche UVs aus dem Low-Poly-Gitter zur Berechnung der eingebrannten Texturen verwendet werden.*Nicht verfügbar im Substance Painter.* |
|  |  |
| **Dilation (px)** | Verlängern/Verlängern Sie die Pixel der UVs außerhalb oder an ihren Rändern um die angegebene Pixelanzahl. Dadurch können Nähte an UV-Rändern vermieden werden, wenn diese Ränder nicht perfekt an den Texturpixeln ausgerichtet sind oder wenn die Texturauflösung reduziert wird (z. B.: mipmaps). Dies ist ein Nachbearbeitungsprozess, der nach dem Backvorgang angewendet wird. Sie kann auch als &quot;padding&quot; (Auffüllung) bezeichnet werden.Weitere Informationen zur Erweiterung finden Sie unter: [Aliasing bei UV-Nähten](../../common-issues/aliasing-on-uv-seams/aliasing-on-uv-seams.md) und [Auffüllung](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/padding-134643719.html). |
| **Diffusion anwenden** | Wenn diese Option aktiviert ist, wird die Außenseite der UVs mit geglätteten Verlaufsfarben basierend auf den UV-Rändern gefüllt. Dieses Verfahren stellt sicher, dass bei reduzierter Texturgröße die Textur stabil bleibt und keine übermäßig sichtbaren Nähte erzeugt werden (z. B.: mipmaps). Dies ist ein Nachbearbeitungsprozess, der nach dem Backvorgang angewendet wird. |
| **Durchschnittliche Normale** | Wenn diese Option aktiviert ist, wird die durchschnittliche Normale eines Scheitelpunktes berechnet, um zu wissen, in welche Richtung Strahlen während des Gitteranpassungsprozesses des Backens gesendet werden sollen. Ist die Option deaktiviert, folgen die Strahlen den ursprünglichen Scheitelpunktnormalen des Gitters. |

## Hochpolparameter

Die folgenden Parameter steuern das Backen von Maschen mit hohem Poly- und niedrigem Poly-Wert (&quot;aus Maschen&quot;-Backen).

| *Name* | *Beschreibung* |
| --- | --- |
| **High-Definition-Netze** | Eine Liste von Dateien (oder Substance-Paketressourcen), die hochgepolte Gitter enthält. Sie werden von den Bäckerinnen in den Speicher geladen, wenn der Backprozess beginnt, unterschiedliche Informationen zu berechnen und diese Gitterinformationen in Texturen zu speichern. Diese Liste wird ignoriert, wenn &quot;**Niedrig als High Definition verwenden**&quot; aktiviert ist. |
| **Niedrig als hochauflösendes Gitter verwenden** oder **Gitter mit niedriger Polung als hochauflösendes Gitter verwenden** | Wenn diese Option aktiviert ist, wird die Liste der hochpolaren Maschen, die den Bäckern bereitgestellt wird, ignoriert, und das niedrigpolare Maschen wird stattdessen auf sich selbst gebacken.Dieser Parameter ist nützlich, wenn Sie direkt mit einem Gitter mit hoher Poly-Intensität arbeiten. Wenn Sie beispielsweise eine Umgebungstextur für ein High-Poly-Fahrzeug backen, während diese Verdeckung aktiviert ist, wird der Strahlenabstand ignoriert und der Bäcker erzeugt einen perfekten Backvorgang (keine Strahlausfälle oder Geometriefehler). |
|  |  |
| **Abstand mit Käfig einstellen** oder **Käfig verwenden** | Gibt an, ob eine Gitterdatei für den Käfig im Backvorgang anstelle der Werte für den Strahlenabstand verwendet werden soll. Der Käfig steuert den maximalen Abstand und die Richtung des Strahls. |
| **Cage-Datei** | Pfad zur Gitterdatei, die den Käfig enthält. |
| **Frontalwert** oder **Maximale Frontalentfernung** | Steuert, wie weit der Strahl über der Oberfläche mit geringer Polung beginnen soll, um eine Geometrie mit hoher Polung entlang seines Pfades zu finden.*Diese Einstellung hat keine Auswirkungen, wenn ein Käfig verwendet wird.* |
| **Rückwert** oder **Max. Rückentfernung** | Steuert, wie weit der Strahl unterhalb der Oberfläche mit geringer Polung anhalten soll, um eine Geometrie mit hoher Poly auf dem Pfad zu finden.*Diese Einstellung hat keine Auswirkungen, wenn ein Käfig verwendet wird.* |
| **Relativ zum Begrenzungsrahmen** | Wenn diese Option aktiviert ist, basieren die Berechnung des Strahlenabstands und anderer Größen auf dem normalisierten Abstand des Gitters mit geringer Poly-Struktur. Wenn diese Option deaktiviert ist, basiert die Berechnung des Strahlenabstands auf Einheiten, die beim Export im Gitter mit geringer Poly-Intensität angegeben wurden (Meter, Zentimeter usw.). Es kann manchmal nützlich sein, diese Einstellung zu deaktivieren und den Strahlenabstand manuell einzugeben, wenn ein Objekt präzise Messungen enthält. |
|  |  |
| **Übereinstimmung** | Gibt an, wie die Bäcker der Low- und High-Poly-Geometrie entsprechen sollen. Es kann verwendet werden, um den Backvorgang zu filtern, ohne dass manuell auseinander (explodieren) Gitter bewegt werden müssen.Mögliche Werte:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Immer</strong> (Standard): Ein solches Gitter wird mit jedem Gitter mit einem hohen Poly-Wert kombiniert.</li><li data-preserve-html="true"><strong>Nach Netzname</strong>: Filtern Sie die Gitter nach ihrem Namen, um eine Übereinstimmung mit unerwünschter Geometrie zu vermeiden.</li></ul>Weitere Informationen zum Anpassen von Geometrien finden Sie unter: [Übereinstimmung nach Name](../../features/matching-by-name/matching-by-name.md). |
| **Übereinstimmende Suffixe** oder **Suffix für hohes Poly-Gitter** **Suffix für niedriges Poly-Gitter** | Mit der Funktion &quot;Matching by Name&quot; wird die Geometrie anhand von Netznamensuffixen identifiziert und gruppiert. Verfügbare Suffixe:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Gitter mit geringer Polung</strong>: Suffix zur Identifizierung von Maschen mit geringem Poly-Anteil in der Szene</li><li data-preserve-html="true"><strong>Hochpolgitter</strong>: Suffix zum Identifizieren von hohen Polygonmaschen in der Szene</li><li data-preserve-html="true"><strong>Rückseiten ignorieren</strong>: Suffix zum Identifizieren von Gittern, die von bestimmten Bakern ignoriert werden sollen (z. B. [Verdeckung aus Gitter](../../bakers-settings/ambient-occlusion-from/ambient-occlusion-from-mesh.md))</li></ul>Weitere Informationen zum Anpassen von Geometrien finden Sie unter: [Übereinstimmung nach Name](../../features/matching-by-name/matching-by-name.md) . |
|  |  |
| **Neigungskorrektur verwenden** | Wenn diese Option aktiviert ist, wird die Strahlrichtung ausgehend von **Durchschnittliche Normale** oder der ursprünglichen Geometrienormalen je nach Eingabetextur berechnet. Bei Schwarzwerten in der Textur wird die durchschnittliche Normalität berechnet, bei Weißwerten die ursprüngliche Gitternormalität.*Nicht verfügbar im Substance Painter.* |
| **Karte verzerren** | Pfad zur Texturdatei, die für die Verzerrungseffekt-Projektion verwendet wird. |
| **Neigungskorrektur umkehren** | Kehrt den Wert der Eingabetextur um (Schwarz wird weiß und Weiß wird schwarz). |
