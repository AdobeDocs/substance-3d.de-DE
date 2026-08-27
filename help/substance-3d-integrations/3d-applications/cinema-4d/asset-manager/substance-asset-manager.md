---
helpx_url: "https://helpx.adobe.com/de/substance-3d-integrations/3d-applications/cinema-4d/substance-asset-manager.html"
breadcrumb-title: ''
description: Verwenden Sie den Substance Asset Manager in Cinema 4D, um Substance-Materialien in Ihrer Szene hinzuzufügen, zu entfernen und zu organisieren.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Cinema 4D > Substance Asset Manager
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Substance Asset Manager
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '651'
ht-degree: 0%

---


# Substance Asset Manager

Im Fenster &quot;Substance Asset Manager&quot; werden alle Substance aufgelistet, die in eine Szene geladen wurden. Hier können Sie Substance hinzufügen, entfernen und neu organisieren.

Wenn Sie im Substance Asset Manager eine Substance auswählen (mit der linken Maustaste klicken), wird die Substance im Attributmanager von Cinema 4D geöffnet. Dort können Sie die Parameter und Keyframe-Substance-Eingaben wie jeden anderen Parameter in Cinema 4D ändern.

>[!NOTE]
>
> Der Attributmanager verfügt über einen speziellen Substance-Asset-Modus, der sich als nützlich erweist, um einen speziellen Attributmanager für Substance in Ihrem Cinema 4D-Layout zu haben.

![](../../../assets/cinema-4d-4.png){width="500px"}

## Dateimenü

## Element laden...

Laden Sie eine neue Substance in die Szene (wie im Menü &quot;Plug-ins&quot;).

Schließen

Schließt den Substance Asset Manager. Geladene Substance bleiben natürlich in der Szene.

## Bearbeitungsmenü

## Alle Substance auswählen

Wählt alle im Asset Manager aufgelisteten Substance aus. Dasselbe lässt sich durch Drücken von Strg+A erreichen, während die Maus über den Asset Manager bewegt wird.

## Auswahl aller Substance aufheben

Hebt die Auswahl aller im Asset Manager aufgelisteten Substance auf. Dasselbe lässt sich durch Drücken von Umschalt+Strg+A erreichen, während die Maus über den Asset Manager bewegt wird.

## Aus ausgewähltem Material auswählen

Wählt alle Substance aus, auf die von den derzeit *ausgewählten* Materialien verwiesen wird.

## Auswählen aus markiertem Material

Wählt alle Substance aus, auf die von den derzeit *markierten* Materialien verwiesen wird. In Cinema 4D wird ein Material markiert, wenn ein Objekt oder Tag ausgewählt wird, das dieses Material verwendet.

## Material(e) auswählen

Wählt alle Materialien aus, die auf die aktuell ausgewählten Substance verweisen.

## Aktionsmenü

## Material(s) erstellen

Erstellen Sie neue Cinema 4D-Material aus den aktuell ausgewählten Substance. Die Material-Kanäle werden automatisch mit Substance-Shadern initialisiert, die sich auf die jeweiligen Ausgabekanäle der Substance beziehen.

## Substance duplizieren

Duplizieren Sie die aktuell ausgewählten Substance. Dies kann nützlich sein, um dieselbe Substance mit verschiedenen Parametersätzen auf mehreren Materialien zu verwenden.

## Substance erneut importieren

Diese Funktion kann verwendet werden, um zu den Standardwerten einer Substance zurückzukehren oder externe Änderungen (z.B. vom Substance Designer) zu integrieren.\
Hinweis: **Alle** Parameteränderungen an den Substance-Eingängen gehen verloren!

## Substance(s) entfernen

Entfernt die aktuell ausgewählten Substance aus der Szene. Dasselbe lässt sich durch Drücken der Löschtaste erreichen, während der Mauszeiger über den Asset Manager bewegt wird.

## Nicht verwendete Substance löschen

Entfernt alle Substance, auf die derzeit kein Material verweist.

## Substance Engine-Menü

Der Inhalt dieses Menüs hängt vom Betriebssystem ab, auf dem Cinema 4D ausgeführt wird. Das Ändern des Substance Engine wird erst nach einem Neustart von Cinema 4D wirksam.

## Kontextmenü

Wenn Sie mit der rechten Maustaste auf eine ausgewählte Substance klicken, wird das Kontextmenü angezeigt. Ihre Funktionalität ist identisch mit den gleichnamigen Funktionen in den oben genannten Menüs:

* Entfernen
* Material(s) erstellen
* Substance duplizieren
* Substance erneut importieren
* Alle Substance auswählen
* Auswahl aller Substance aufheben
* Material(e) auswählen

## Drag &amp; Drop

Sie können mit dem Substance Asset Manager per Drag &amp; Drop interagieren. Es stehen mehrere Optionen zur Verfügung:

* Laden Sie Substance(s) per Drag &amp; Drop vom Explorer oder Finder in die Szene, indem Sie sie einfach auf den Substance Asset Manager ablegen.
* Substance können in das Verknüpfungsfeld von Substance-Shadern gezogen werden, um einen Shader und ein Substance-Asset zu verbinden.
* Im Modus &quot;Unsortiert&quot; (siehe unten) können Sie Substance im Elementmanager neu anordnen, indem Sie sie an eine neue Position ziehen.


## Sortieren in Substance Asset Manager

## Unsortierter Modus

## Der Substance Asset Manager befindet sich standardmäßig im **unsortierten Modus**. Die Kopfzelle der Namensspalte zeigt rechts keinen Pfeil an. Sie können die Substanzen per Drag-and-Drop nach Ihren Wünschen neu anordnen.

![](../../../assets/cinema-4d-3.png){width="500px"}

![](../../../assets/cinema-4d-5.png){width="500px"}

## Vorschau in Substance Asset Manager

## Substance Asset Manager zeigt kleine Symbole mit einer Vorschau der verfügbaren Kanäle für jede Substance an.

## Die Vorschauen werden einfach in der Reihenfolge der Ausgabekanäle auf der Substance angezeigt. Die Spalte, in der eine Vorschau angezeigt wird, hat keine Bedeutung.
