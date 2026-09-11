---
helpx_url: "https://helpx.adobe.com/de/substance-3d-bake/bakers-settings/common-parameters.html"
breadcrumb-title: ''
description: Erfahren Sie mehr über allgemeine Parameter, die für alle Baker gelten, und wie Sie diese für eine optimale Generierung der Textur konfigurieren können.
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

Allgemeine Parameter gelten für alle Baker. Diese Parameter legen in der Regel fest, wie sich die Baker verhalten und mit Meshs arbeiten, die eine hohe Poly-Zahl aufweisen, aber wie die endgültigen Texturen generiert werden. Einige dieser Parameter können von bestimmten Bakern überschrieben werden.

Die meisten dieser Parameter stehen in der gesamten Software (einschließlich des Substance Automation Toolkit) zur Verfügung, ihr Verhalten kann jedoch leicht abweichen. oder einige sind je nach Software-Workflow und -Implementierung möglicherweise nicht verfügbar.

## Allgemeine Parameter

Diese Parameter beeinflussen die Art und Weise, wie Baker Texturen generieren.

| *Name* | *Beschreibung* |
| --- | --- |
| **Größe**(Standardgröße oder Ausgabegröße) | Steuern Sie die Auflösung der Baking führend Ausgabe-Textur (in Pixeln).Verfügbare Werte:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>32</strong></li><li data-preserve-html="true"><strong>64</strong></li><li data-preserve-html="true"><strong>128</strong></li><li data-preserve-html="true"><strong>256</strong></li><li data-preserve-html="true"><strong>512</strong></li><li data-preserve-html="true"><strong>1024</strong></li><li data-preserve-html="true"><strong>2048</strong> (Standard)</li><li data-preserve-html="true"><strong>4096</strong></li><li data-preserve-html="true"><strong>8192</strong></li></ul>Nicht quadratische Auflösungen werden ebenfalls unterstützt, z. B.: 2048 x 1024 (Verhältnis 2:1). Im Substance Designer kann dieser Parameter vom Baker selbst überschrieben werden. |
| **Format** | Dateiformat der Baking geführt Texturen.*Nicht verfügbar im Substance Painter.* Siehe: [So exportieren Sie die durch Baking erzeugte Map](../../common-questions/how-export-the-baked-maps/how-to-export-the-baked-maps.md). |
| **Anti-Aliasing** | Steuert das Anti-Aliasing. Dadurch kann die Qualität Baking geführt Texturen verbessert und Aliasing bei unterschiedlichen Geometrien reduziert werden.Weitere Informationen zum Aliasing finden Sie unter: [Aliasing auf UV-Nähte](../../common-issues/aliasing-on-uv-seams/aliasing-on-uv-seams.md) und [Aliasing auf Wikipedia](https://en.wikipedia.org/wiki/Aliasing).Verfügbare Werte:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Keine</strong> (Standard)</li><li data-preserve-html="true"><strong>Subsampling 2x2</strong></li><li data-preserve-html="true"><strong>Subsampling 4x4</strong></li><li data-preserve-html="true"><strong>Subsampling 8x8</strong></li></ul>  **Hinweis:** Das Aktivieren von Anti-Aliasing kann den Zeitaufwand für das Baking erheblich erhöhen, da Anti-Aliasing funktioniert, indem die Textur mit einer höheren Auflösung berechnet und dann wieder auf die ursprünglich ausgewählte Größe herunterskaliert wird. Das bedeutet, dass eine 2K-Textur mit einem 2x2-Subsampling tatsächlich eine 4K-Textur berechnet.Manchmal ist es besser, die Anzahl der Strahlen im Baker zu erhöhen, als den Subsampling zu erhöhen. So könnten bessere Ergebnisse erzielt werden, ohne zu lange zu warten. |
| **UV-Satz** | Steuert, welche UVs des Low-Poly-Meshs zur Berechnung der Baking geführt Texturen verwendet werden.*Nicht verfügbar im Substance Painter.* |
|  |  |
| **Ausdehnung (px)** | Verlängern/Verlängern Sie die Pixel der UVs außerhalb oder an ihren Rändern um die angegebene Pixelanzahl. Dadurch können Nähte an UV-Rändern vermieden werden, wenn diese Ränder nicht perfekt an den Textur-Pixeln ausgerichtet sind oder wenn die Auflösung der Textur reduziert wird (z. B.: mipmaps). Dies ist ein Nachbearbeitungsprozess, der nach dem Baking angewendet wird. Sie kann auch als &quot;padding&quot; (Auffüllung) bezeichnet werden.Weitere Informationen zur Ausdehnung finden Sie unter: [Aliasing auf UV &#x200B;](../../common-issues/aliasing-on-uv-seams/aliasing-on-uv-seams.md) und [Auffüllung](https://helpx.adobe.com/de/substance-3d/unlisted/documentation/spdoc/padding-134643719.html). |
| **Diffusion anwenden** | Wenn diese Option aktiviert ist, wird die Außenseite der UVs mit geglätteten Verlaufsfarben basierend auf den UV-Rändern gefüllt. Dieses Verfahren stellt sicher, dass die Textur bei verringerter Dateigröße stabil bleibt und keine übermäßig sichtbaren Nähte erzeugt (z. B.: mipmaps). Dies ist ein Nachbearbeitungsprozess, der nach dem Baking angewendet wird. |
| **Durchschnittliche Normale** | Wenn diese Option aktiviert ist, wird die Durchschnittsnorm eines Scheitelpunkts berechnet, um zu wissen, in welche Richtung Strahlen während des Mesh-Abgleichvorgangs des Bakings gesendet werden sollen. Wenn diese Option deaktiviert ist, folgen die Strahlen den Original-Scheitelpunkt-Normalen des Meshs. |

## Hochpolparameter

Die folgenden Parameter steuern das Baking von Meshs mit hohem bis niedrigem Poly (&quot;von Mesh&quot;-Baker).

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
| **Übereinstimmende Suffixe** oder **High-Poly-Mesh-Suffix** **Low-Poly-Mesh-Suffix** | Mesh-Namenssuffixe zum Identifizieren und Gruppieren der Geometrie bei Verwendung der Funktion &quot;Nach Name zuordnen&quot;. Verfügbare Suffixe:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Low-Poly-Mesh</strong>: Suffix zum Identifizieren von niedrigen Poly-Meshs in der Szene</li><li data-preserve-html="true"><strong>High-Poly-Mesh</strong>: Suffix zum Identifizieren von hohen Poly-Meshs in der Szene</li><li data-preserve-html="true"><strong>Rückseiten ignorieren</strong>: Suffix zum Identifizieren von Meshs, die von bestimmten Bakern ignoriert werden sollen (z. B. [Ambient occlusion Von Mesh](../../bakers-settings/ambient-occlusion-from/ambient-occlusion-from-mesh.md))</li></ul>Weitere Informationen zum Anpassen von Geometrien finden Sie unter: [Übereinstimmung nach Name](../../features/matching-by-name/matching-by-name.md) . |
|  |  |
| **Verzerrungskorrektur verwenden** | Wenn diese Option aktiviert ist, wird die Strahlrichtung ausgehend von **Durchschnittliche Normale** oder der Originalgeometrienormale berechnet, je nach der eingegebenen Textur. Bei Schwarzwerten in der Textur wird die berechnete Durchschnittsnorm verwendet, während bei Weißwerten die ursprüngliche Mesh-Normale verwendet wird.*Nicht verfügbar im Substance Painter.* |
| **Karte verzerren** | Pfad zur Textur-Datei, die zum Neigen der Projektion verwendet wird. |
| **Verzerrungskorrektur umkehren** | Kehrt den Wert der Eingabe-Textur um (Schwarz wird Weiß und Weiß wird Schwarz). |
