---
title: Häufige Fragen
description: Hier finden Sie Antworten auf häufig gestellte Fragen zu OpenPBR und Substance 3D.
source-git-commit: a3ceb4df30f08099799bc2caecc5446d3832fc06
workflow-type: tm+mt
source-wordcount: '1424'
ht-degree: 0%

---


# Häufig gestellte Fragen zu OpenPBR

## Das OpenPBR-Modell

+++Was ist OpenPBR und welche Version wird von Painter unterstützt?

OpenPBR ist eine von der Academy Software Foundation gehostete Open-Material-Spezifikation, die ein standardisiertes Anwendungsmodell definiert, das für eine konsistente Schattierung über Anwendungen hinweg entwickelt wurde. Die Dokumentation von [Painter enthält weitere Informationen zur Verwendung von OpenPBR](https://experienceleague.adobe.com/de/docs/substance-3d-painter/using/home).

+++

+++Was bedeutet es, wenn eine Anwendung &quot;Support OpenPBR&quot; beansprucht, und wie kann ich herausfinden, wie gut eine bestimmte Anwendung sie unterstützt?

Es gibt kein formelles Zertifizierungsverfahren, daher kann der Anspruch verschiedene Dinge bedeuten. In der Praxis variieren die Implementierungen: Einige decken die gesamte Spezifikation ab, andere nur eine Untergruppe. Dadurch werden Features wie Dünnschichtfotografie, Streuung oder bestimmte Untergrundverhalten ausgelassen. Beachten Sie auch, dass &quot;MaterialX-Unterstützung&quot; und &quot;OpenPBR-Unterstützung&quot; nicht dasselbe sind. Eine Anwendung kann eine Anwendung unterstützen, ohne die andere vollständig zu implementieren.

Um herauszufinden, was eine bestimmte Anwendung tatsächlich unterstützt, verwenden Sie eine Kombination von Ansätzen: Lesen Sie die Versionshinweise (Support wird häufig schrittweise hinzugefügt). Laden Sie den ASWF OpenPBR Playground und vergleichen Sie diese mit einem Referenz-Rendering, um Lücken schnell zu überdecken. oder bei Studios mit erheblichen Pipeline-Investitionen den Anbieter direkt nach den unterstützten Funktionen und deren Roadmap fragen.

+++

+++Kann OpenPBR für verschiedene Anwendungen und Renderer die gleichen Ergebnisse garantieren?

Nicht ganz, und das ist beabsichtigt. OpenPBR definiert ein freigegebenes Materialmodell, aber das endgültige Erscheinungsbild wird auch durch Beleuchtung, Rendering-Algorithmen, Farbmanagement und die Übereinstimmung jeder Implementierung mit der Spezifikation bestimmt.

In der Praxis bedeutet die Maximierung dieser Garantie: Exportieren über USD mit MaterialX-Integration eine frühzeitige Validierung der Hin- und Rückfahrt mithilfe des ASWF-Spielplatzes für den OpenPBR-Shader und nicht am Ende der Produktion; Bestätigung der Support-Level Ihrer Anbieter für alle von Ihnen verwendeten erweiterten Funktionen; und im Voraus zustimmen, welche Funktionen in freigegebenen Materialien verwendet werden und welche nicht. Portabilität sollte aktiv validiert werden, nicht vorausgesetzt.

+++

+++Gibt es Material, die OpenPBR nicht genau darstellen kann?

Ja. OpenPBR ist ein parametrisches Modell. Parameter wie Rauheit, Metallität und IOR decken den größten Teil der Anwendungsfälle bei der Produktion ab, können jedoch nicht die Genauigkeit von Material-Messformaten wie X-Rite AxF replizieren, die tatsächliche optische Daten aus einer physischen Probe erfassen. Für allgemeine Produktionsarbeiten ist OpenPBR gut geeignet; bei Anwendungen, die eine exakte Stichprobenübereinstimmung erfordern, kann ein gemessenes Format geeigneter sein.

Auto-Malen ist eine gute Illustration. Es ist möglich, Auto-Malen in OpenPBR mit ein paar Einschränkungen zu erstellen. OpenPBR verfügt nicht über einen speziellen Malen-Shader für Autos, sodass er für bestimmte Anwendungen in der Automobilindustrie möglicherweise nicht ausreicht. Darüber hinaus hängt es einfach von der Art des Malen ab - einige Car-Malen werden immer Eigenschaften haben, die außerhalb des Anwendungsbereichs eines bestimmten Shaders liegen. Aber mit diesen Aspekten im Hinterkopf ist Auto-Malen ganz natürlich mit der Schichtenarchitektur der OpenPBR verbunden.

+++

## Einrichtung und Konvertierung

+++Muss ich OpenUSD oder MaterialX lernen, um OpenPBR verwenden zu können?

Nein. Für die meisten Künstler ist OpenPBR einfach das Materialmodell, das in den Tools enthalten ist, die sie bereits verwenden. Substance 3D Painter, Maya 2025.3 und 3ds Max 2026 verwenden alle OpenPBR als Standard-Material; Damit arbeiten wir einfach mit dem Standard-Shader. USD und MaterialX werden nur relevant, wenn Materialien zwischen Anwendungen wechseln müssen. Bei Arbeitsabläufen mit nur einer Anwendung ist die native Unterstützung ausreichend. für Multi-DCC-Pipelines bieten USD und MaterialX die Austauschinfrastruktur, jedoch weitgehend hinter den Szenen.

Der beste Austauschpfad für gemeinsam genutzte Materialbibliotheken ist jedoch die USD mit MaterialX-Integration, die einen standardisierten Container für Material-Beschreibungen bietet, der vom Renderer unabhängig ist. Arbeitsabläufe für den Export von Materialien als eigenständige Elemente (ohne zugehöriges Modell, zur Verwendung in einer gemeinsam genutzten Bibliothek) befinden sich noch in der aktiven Entwicklung und werden noch nicht überall vollständig unterstützt. Bevor Sie einen Commit für eine davon abhängige Bibliotheksarchitektur ausführen, sollten Sie Ihre spezifische Pipeline anhand der aktuellen Funktionen überprüfen.

+++

+++Wie erstelle ich in Substance 3D Painter ein neues OpenPBR-Projekt?

Ein Projekt, das ohne Vorlage erstellt wurde, verwendet standardmäßig den OpenPBR-Shader. Der OpenPBR Shader ist nun die erste Option im neuen Projektfenster, die ASM ersetzt. Es sind auch spezielle Vorlagen für bestimmte Workflows verfügbar (Anisotropie, Coat, Fuzz, Volumenstreuung). Beim Importieren einer USD-Datei, die ein OpenPBR-Material enthält, wird das Projekt automatisch konfiguriert. Die Beispielprojekte, die mit Substance 3D Painter ausgeliefert wurden, wurden ebenfalls auf den OpenPBR-Arbeitsablauf aktualisiert und sind ein guter Ausgangspunkt, um sich mit der Funktionsweise in der Praxis vertraut zu machen.

+++

+++Kann ich ein bestehendes Adobe Standard Material (ASM)-Projekt in OpenPBR konvertieren?

Es findet keine automatische Konvertierung statt. Vorhandene ASM-Projekte behalten ihren aktuellen Shader, wenn sie geöffnet werden, und ASM-Vorlagen bleiben für neue Projekte verfügbar.

Um manuell zu OpenPBR zu migrieren, wählen Sie den OpenPBR-Shader im Fenster &quot;Shader-Einstellungen&quot; aus und fügen Sie dann die entsprechenden OpenPBR-Kanäle über &quot;Kanaleinstellungen&quot; > &quot;Textursatz hinzufügen oder entfernen&quot; hinzu. Überprüfe anschließend deine vorhandenen Ebenen, um sicherzustellen, dass ihre Inhalte auf die gewünschten Kanäle abzielen.

+++

+++Müssen meine benutzerdefinierten Shader für OpenPBR aktualisiert werden?

Nein - bestehende benutzerdefinierte Shader funktionieren weiterhin, da die entsprechenden Shader-Bibliotheken veraltet sind und nicht entfernt werden. Es wird jedoch empfohlen, zu den neuen Shader-Bibliotheken zu migrieren. sie sind sauberer und leichter zu bearbeiten. Weitere Informationen finden Sie im Shader-API-Änderungsprotokoll im Hilfemenü.

+++

## App-interne Verwendung

+++Wo kann ich meine Aufmerksamkeit auf die vielen verfügbaren OpenPBR-Parameter lenken?

Aller Anfang ist einfach. Bei den meisten undurchsichtigen Oberflächen sind die Grundfarbe, die Specular-Rauheit und die Metalness-Eigenschaften die größten Unterschiede zwischen den Materialien. Fügen Sie IOR hinzu, wenn es auf den richtigen Reflexionsgrad ankommt. Verfeinern Sie die Specular-Farbe, wenn das Material einen Graswinkel-Farbton hat. Ermöglichen Sie Übertragung, Untergrund, Beschichtung, Fuzz, Dünnfilm und Streuung nur, wenn Sie dafür einen klaren, referenzgesteuerten Grund haben, da jeder zusätzliche Kanal die Komplexität und die potenziellen Renderkosten erhöht. Durch das Ausblenden oder Reduzieren nicht verwendeter Parametergruppen bleibt Ihr Arbeitsbereich fokussiert und das Risiko unbeabsichtigter Effekte wird reduziert.

+++

+++Ich habe eine Rauheit-Map. Soll ich sie an eine Base Diffuse-Rauheit oder Specular-Rauheit anschließen?

Specular-Rauheit: Steuert die Spiegelungsschärfe und ist das direkte Äquivalent der Rauheit, die in anderen PBR-Workflows eingegeben wird. Die Rauheit der Basis-Diffuse ist ein separater, spezieller Parameter, der nur die diffuse Streuung beeinflusst. Bei den meisten Arbeitsabläufen kann es an der Standardeinstellung bleiben.

+++

+++Warum hat das Ändern der Grundfarbe keine Auswirkungen, wenn ich Volumenstreuung verwende?

Es gibt eine &#39;Prioritätshierarchie&#39;, die bestimmt, wie viel Einfluss jeder Parameter auf das endgültige Erscheinungsbild des Materials hat. So zum Beispiel:

* Metalismus an erster Stelle: wenn &quot;Metalness&quot; = 1 ist, werden die Teile &quot;Untergrund&quot; und &quot;Transmission&quot; deaktiviert.
* Übertragungsgewicht kommt als Nächstes: wenn Übertragungsgewicht = 1, Untergrund fehlt.
* Das Untergrundgewicht kommt danach.
* Diffuse Grundfarbe kommt als letztes: die Basis-Diffuse trägt nur bei, wenn keiner der oben genannten Werte auf 1 gesetzt ist.

Wenn also im angegebenen Beispiel die Flächengewicht auf 1 (der Höchstwert) festgelegt ist, bestimmt sie das gesamte Erscheinungsbild. Die Änderung des Werts der Grundfarbe hat keine Auswirkungen, da die Diffuse der Basisdaten im Wesentlichen keinen Beitrag leistet. Wenn dagegen für &quot;Metalness&quot; der Höchstwert von 1 festgelegt ist, hat die Änderung der Werte für das Übertragungsgewicht, das Unteroberflächengewicht und die Grundfarbe der Diffuse keine Auswirkungen auf das endgültige Erscheinungsbild des Materials. Transmission, Subsurface und Diffuse sind alle dielektrisch (nicht-metallisch), sodass die Einstellung &quot;Metalness&quot; auf 1 jeden nicht-metallischen Beitrag entfernt.

+++

+++Warum verhält sich die Übertragung unerwartet? Warum wird beispielsweise mein Mesh sehr dunkel angezeigt, wenn ich ihn aktiviere?

Der häufigste Grund ist, dass die Tiefe der Übertragung zu niedrig eingestellt ist. Dieser Parameter legt fest, wie weit das Licht reicht, bis die Übertragungsfarbe die volle Sättigung erreicht. bei niedrigen Werten erscheint selbst dünne Geometrie dunkel und dicht. Erhöhe den Wert, bis er etwa der physischen Skalierung deines Objekts entspricht. Wenn das Material dann zu klar aussieht, passen Sie Übertragungsfarbe und Tiefe gemeinsam an, um die richtige Balance zu finden.

Eine Streuung kann eine weitere Komplexitätsschicht hinzufügen. Die Übertragungsfarbe ist kein einfacher Farbton. Seine Wirkung hängt davon ab, wie weit das Licht durch das Objekt fällt (gesteuert durch die Übertragungsfarbe). Die Tiefe der Transmission ist hier ebenfalls maßgeblich. Streuung Color hingegen steuert eine Bewegung, die von einem anderen Licht durchflutet werden kann - indem es innerhalb des Materials hin- und herspringt, anstatt direkt durch das Bild zu gehen. Da die Streuung in eine Richtung erfolgt, ändert sich das Ergebnis auch in Abhängigkeit davon, wo sich die Lichtquelle befindet. Eine Anpassung ohne Berücksichtigung der anderen ist eine häufige Quelle unerwarteter Ergebnisse.

+++

+++Ich habe Thin-Film aktiviert, kann aber keinen Effekt sehen. Was fehlt mir?

Überprüfen Sie zuerst den Wert für die Thickness. Gegen intuitiv führen dünnere Werte zu einer sichtbareren Iridizenz - die meisten Effekte treten zwischen 0 und 1 Mikrometer auf. Wenn der Effekt noch subtil ist, passen Sie den IOR an, wodurch sich sowohl die Intensität als auch die Farbe der Interferenz verschieben. Prüfen Sie außerdem, ob das Dünnschichtgewicht über Null liegt.

+++
