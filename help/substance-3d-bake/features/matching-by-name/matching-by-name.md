---
helpx_url: 'https://helpx.adobe.com/de/substance-3d-bake/features/matching-by-name.html'
breadcrumb-title: ''
description: Verwenden Sie die Funktion "Namensgleich", um Mesh mit niedriger und hoher Poly-Zahl zu isolieren und Geometrieausblutungen während des Baking führend Vorgangs zu verhindern.
helpx_creative_field: ''
helpx_description: bakers > Features > Matching by Name
helpx_experience_level: ''
helpx_learn_topic: ''
helpx_tags: ''
title: Zuordnung nach Name
user-guide-description: ''
user-guide-title: ''
source-git-commit: d57629bee333101dd9f40f30ed24ff84b6b8c6f1
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 0%

---


# Zuordnung nach Name

![](../../assets/banner-matching-by-name.jpg)

&quot;Mit Namen abgleichen&quot; ist der Name einer Datenmethode, die in Substance Bakers verwendet werden kann, um Mesh mit niedrigem Poly- und hohem Poly-Wert auf der Grundlage ihres Namens zu isolieren.

Diese Funktion ist sehr nützlich, um zu vermeiden, dass beim Baking führ Geometrien übereinander verlaufen, um saubere Texturen zu erzielen. Es wird vermieden, dass Mesh (oft als &quot;Explodieren&quot; bezeichnet) entfernt werden müssen, um dasselbe Ergebnis zu erzielen.

## Wann wird die Zuordnung nach Name verwendet?

### Normalen-Map Baking führend mit Mesh-Blutung

In diesem Beispiel verläuft der Helm, der sich oben auf dem Kopf der Figur befindet, über die Fläche der Figur.

Durch Aktivieren von &quot;Passend nach Name&quot; können wir den Helm ignorieren und die Fläche richtig Baking geführt. *Dieses Ergebnis basiert auf der Haupt-Match-Einstellung.*

| *Mesh* | *Übereinstimmung nach Name von* | *Übereinstimmung nach Name auf* |
| --- | --- | --- |
| ![](../../assets/baking-demo-vela.png){width="250px"} | ![](../../assets/baking-demo-vela-normal-nomatch.png){width="250px"} | ![](../../assets/baking-demo-vela-normal-withmatch.png){width="250px"} |

### Rückseite für schwebende Geometrie ignorieren

In diesem Beispiel sind die &quot;Schaltflächen&quot; am oberen Rand des Kastens schwebende Geometrie, sie sind nicht mit der High-Poly-Mesh verbunden. Daher werden standardmäßig Schatten auf dem darunter liegenden Feld Geworfen, wodurch die Geometriebegrenzung angezeigt wird.

Durch Aktivieren der Einstellung &quot;Abgleich nach Name&quot; für die Einstellung &quot;**Hintergrundfläche ignorieren**&quot; kann die ambient occlusion Baking geführt werden, während der Bereich unter den Schaltflächen ignoriert wird, damit sie wie ein einzelnes Feld aussieht.*Dieses Ergebnis basiert auf der Verwendung der Einstellung &quot;Hintergrund ignorieren&quot;.*

| *Mesh* | *Übereinstimmung nach Name von* | *Übereinstimmung nach Name auf* |
| --- | --- | --- |
| ![](../../assets/ignorebf-mesh.png){width="250px"} | ![](../../assets/ignorebf-off.png){width="250px"} | ![](../../assets/ignorebf-on.png){width="250px"} |

## Wie funktioniert die Zuordnung nach Namen?

Das System &quot;Matching By Name&quot; liest den Geometrienamen sowohl in den niedrigen als auch in den hohen Meshs und verwendet ein Schlüsselwort (das Suffix), um die Namen zu identifizieren bzw. abzugleichen. Standardmäßig verwenden die Baker das spezifische Suffix, sie können sich jedoch ändern (siehe unten).

Folgende Suffixe werden derzeit unterstützt:

| *Suffixtyp* | *Standardwert* | *Nutzung* |
| --- | --- | --- |
| Hohe Poly | *\_high* | Wird verwendet, um den Namen der High-Poly-Mesh zu isolieren, die mit dem niedrigen Poly übereinstimmt. |
| Niedriger Poly-Wert | *\_low* | Wird verwendet, um den Namen der Low-Poly-Mesh zu isolieren, die mit dem hohen Poly übereinstimmt. |
| Rückseite ignorieren | *\_ignorebf* | Wird zum Ignorieren von Rückseiten für Baker verwendet, die Sekundärstrahlen verwenden, z. B. den Ambient occlusion.*Dieses Suffix sollte nur auf den Meshs mit hohen Poly-Werten vorhanden sein, z. B.:**Mesh\_hoch\_ignorebf*** |

Einige Regeln, die zu berücksichtigen sind, damit diese Funktion ordnungsgemäß funktioniert:

* Die Zuordnung nach Name muss in [Allgemeine Parameter](../../bakers-settings/common-parameters/common-parameters.md) aktiviert sein, da sie standardmäßig **deaktiviert ist**.
* In einigen Bakern (z. B. [Ambient occlusion](../../bakers-settings/ambient-occlusion-from/ambient-occlusion-from-mesh.md)) ist möglicherweise eine sekundäre Einstellung &quot;Übereinstimmend nach Name&quot; aktiviert, da sie Sekundärstrahlen erzeugen.
* Bei der Zuordnung wird zwischen Groß- und Kleinschreibung unterschieden. Dies bedeutet, dass ein Mesh mit dem Namen &quot;**Vela**&quot; nicht mit einem anderen mit dem Namen &quot;**Vela**&quot; übereinstimmt.
* Je nachdem, wo sich das Suffix im Geometrienamen befindet, können mehrere Mesh zugeordnet werden.

Im Folgenden finden Sie Beispiele für die Funktionsweise der Zuordnung (unter Verwendung des Standardsuffixes):

| Name der niedrigen Gruppe | Passt zu hoher Poly-Rate | Entspricht nicht der hohen Poly |
| --- | --- | --- |
| <ul data-preserve-html="true"><li data-preserve-html="true">body_low</li></ul> | <ul data-preserve-html="true"><li data-preserve-html="true">body_high</li><li data-preserve-html="true">body_high_top</li><li data-preserve-html="true">body_high_1</li><li data-preserve-html="true">body_high_2</li></ul> | <ul data-preserve-html="true"><li data-preserve-html="true">körperbetont</li><li data-preserve-html="true">body_top_high</li></ul> |
| <ul data-preserve-html="true"><li data-preserve-html="true">Überschrift_niedrig</li></ul> | <ul data-preserve-html="true"><li data-preserve-html="true">Überschrift_hoch</li></ul> | <ul data-preserve-html="true"><li data-preserve-html="true">head_high</li></ul> |
| <ul data-preserve-html="true"><li data-preserve-html="true">Leg_low_top</li></ul> | <ul data-preserve-html="true"><li data-preserve-html="true">Bein_hoch</li><li data-preserve-html="true">Leg_high_top</li><li data-preserve-html="true">Leg_high_high_top</li></ul> | <ul data-preserve-html="true"><li data-preserve-html="true">Leg_top_high</li></ul> |

## Bäcker einrichten

### Aktivieren der Zuordnung nach Name

Die Zuordnung nach Name kann in den [allgemeinen Parametern](../../bakers-settings/common-parameters/common-parameters.md) der Baker-Einstellungen aktiviert werden:

| *Software* | *Konfiguration wird festgelegt* |
| --- | --- |
| **Substance Painter** | <ol class="steps" data-preserve-html="true"> <li class="step" data-preserve-html="true">     Öffnen Sie das Fenster &quot;Backen&quot; (über die Einstellungen für den Textursatz).    </li> <li class="step" data-preserve-html="true">     Zeigen Sie die allgemeinen Parameter an.    </li> <li class="step" data-preserve-html="true">     Ändern Sie die Einstellung &quot;<strong>Match</strong>&quot; von &quot;Always&quot; in &quot;By Mesh Name&quot;.<br/> <img data-preserve-html="true" src="../../assets/baking-match-setting-sp.png"/>    </li> </ol> |
| **Substance Designer** | <ol class="steps" data-preserve-html="true"> <li class="step" data-preserve-html="true">     Öffnen Sie das Backfenster (durch Klicken mit der rechten Maustaste auf ein verknüpftes Gitter im Explorer-Fenster).    </li> <li class="step" data-preserve-html="true">     Ändern Sie die Einstellung &quot;<strong>Match</strong>&quot; von &quot;Immer&quot; in &quot;Nach Gittername&quot;. 2<br/> <br/>    </li> </ol> |

### Ändern der Suffixnamen

Die Standardsuffixe lauten \_low und \_high und können wie folgt geändert werden:

* **Substance Painter**: Im [Baking führend Fenster](../../getting-started/software-interface/3d-painter/substance-3d-painter.md) innerhalb der allgemeinen Parameter.
* **Substance Designer**: In den [Projekteinstellungen](https://experienceleague.adobe.com/de/docs/substance-3d-designer/using/workspace/preferences/project-settings) unter den Baking geführt Einstellungen.

## High-Poly-Meshs von zBrush

Aus zBrush exportierte Mesh mit hoher Poly-Qualität können für den Baking führ mit der Funktion &quot;Passender Name&quot; verwendet werden. Es können jedoch einige Einstellungen vorgenommen werden:

| *Dateiformat* | *Beschreibung* |
| --- | --- |
| **FBX** | Es gibt keine spezifischen Parameter zum Aktivieren/Deaktivieren, Meshdateien können unverändert verwendet werden. |
| **OBJ** | OBJ von zBrush exportierten Dateien funktionieren standardmäßig nicht mit **Übereinstimmender Name**. Es ist auch möglich, Substance Painter anzuweisen, den Dateinamen des Meshs zu verwenden, anstatt Mesh anhand ihres Namens abzugleichen.Gehen Sie hierzu wie folgt vor:<ol data-preserve-html="true"><li data-preserve-html="true"><strong>Deaktivieren Sie </strong> den Gruppenparameter (Grp) für <strong>jedes</strong>-Untertool.</li><li data-preserve-html="true"><strong>Name</strong> die OBJ Datei entsprechend (z. B.: <strong>body_high.obj</strong>).</li></ol> ![](../../assets/zbrush-setting.png) |
