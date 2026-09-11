---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/renderers/color-management.html"
breadcrumb-title: ''
description: Erfahren Sie mehr über Farbmanagement und Gammakorrektur bei der Verwendung von Substance-Materialien mit verschiedenen Renderern.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Color Management
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Farbmanagement
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 2%

---


# Farbmanagement

Wir werden einen vereinfachten Ansatz wählen, indem wir darauf hinweisen, dass lineares Space Rendering die richtige Mathematik für Beleuchtungsberechnungen bietet. Sie schafft eine Umgebung, in der leichte Interaktionen glaubwürdig und realistisch dargestellt werden können. Für eine Diskussion über lineares Space Rendering müssen wir das Konzept der Gamma-Korrektur einführen. Bei der Bildcodierung für Anzeige- und Speicherzwecke ist die Gamma-Korrektur der Optimierungsprozess zur Verringerung der Bandbreite und Bitzuweisung. Dieser Prozess nutzt die Wahrnehmung des menschlichen Auges von der Helligkeit, die ungefähr der Würfelwurzel der Luminanz folgt.

>[!NOTE]
>
> Lineares Raum-Rendering ist ein hochkomplexes Thema. Weitere Informationen finden Sie im kostenlosen [PBR GUIDE VOLUME ONE](https://academy.substance3d.com/courses/the-pbr-guide-part-1) auf [Substance Academy](https://academy.substance3d.com/).

## Farbmanagement

In diesem Dokument wird die Arbeit mit Texturen beschrieben, die aus **Substance Painter** und **Substance Designer** in [3D-Software](https://www.adobe.com/products/substance3d/3d-augmented-reality.html) und Renderern exportiert wurden.

Wie ein als Eingabe in einen Materialkanal verwendetes Bild korrekt interpretiert wird, hängt davon ab, wie das Bild in der Szene verwendet wird. Der Farbraum, die Codierung und die Tatsache, ob die Farbwerte proportional zu **auf die Szene verweisenden Luminanzen** oder **auf die Anzeige verweisenden Luminanzen** sind, spielen ebenfalls eine wichtige Rolle.

* Bilder, die zur Darstellung von **Nicht-Farbdaten** verwendet werden, sollten nicht transformiert werden. Dies sind in der Regel **Normal**, **Rauheit**, **metallic**, **Versatz** und **Umgebung** **Verdeckung** Zuordnungen.
* Bilder, die Farben darstellen, die wir sehen, können mehrere Szenarien haben. Beispielsweise müssen Bilder, die bereits **szenenlinear** sind, in der Regel nicht konvertiert werden, z. B. **Bilder mit hohem Dynamikbereich**, die in Formaten wie **OpenEXR** und **HDR** gespeichert sind.
* Für Bilder, die zur Anzeige erstellt wurden (**display-related**), muss ihr Gamma entfernt werden. Dazu gehören die meisten Formate wie **PNG**, **JPEG** und **BMP**. Diese Bilder sind **base** **color**, **diffuse**, **Specular** und **emissive**.

Dies ist zwar eine zu starke Vereinfachung, aber es kann hilfreich sein, sich den Prozess wie folgt vorzustellen:

* &quot;auf die Szene bezogen (z. B. linear)&quot; : Keine Konvertierung anwenden
* &quot;anzeigebezogen (z. B. sRGB)&quot; : Inverse-transformieren anwenden, um das Bild für eine korrekte Berechnung zu &quot;linearisieren&quot;.

>[!NOTE]
>
> Die Konvertierung der sRGB-Decodierungsfunktion (EOTF) vom Gamma- in den Linearraum wird in Substance Painter und Substance Designer verwendet und ist in der IEC 61966-2-1:1999-Norm definiert.

Der Substance Designer kann so konfiguriert werden, dass er [OpenColorIO](https://opencolorio.org/) für das Farbmanagement verwendet. Dadurch können Sie *konsistente* Farbtransformationen und Bilddarstellung über mehrere Anwendungen hinweg durchführen. In diesem Modus arbeitet Substance Designer intern mit **linearen RGB**-Farben. Da 8 Bittiefen normalerweise nicht ausreichen, um Linearfarben darzustellen, wird empfohlen, mindestens ** **16-bit** Tiefen für Farbtexturen im [Diagramm](https://docs.substance3d.com/display/SDDOC/Graph+View) zu verwenden.

![](https://helpx-prod.scene7.com/is/image/HelpxProd/sd-cm?$png$&jpegSize=200&wid=686)

Als wir [ACE](https://www.oscars.org/science-technology/sci-tech-projects/aces) eingeführt haben, verfügen wir jetzt über zwei verschiedene Farbräume: den linearen sRGB (die &quot;no gamma&quot;-Version von sRGB) und den [ACEScg](https://acescolorspace.com/), einen Farbraum mit großem Farbumfang (&quot;Szene-bezogen&quot; oder &quot;linear&quot;), der besser für das CG-Rendering geeignet ist.

*Gamut-Plotgrafik -<https://acescolorspace.com/>*

Substance Designer unterstützt auch **Adobe Color Engine (ACE)**. Mit **ACE** können Sie Ihren Arbeitsfarbraum zwischen **sRGB**, **linearem sRGB** und **ACEScg** wählen. Bei Verwendung von **sRGB** ist **ACE** so ziemlich mit dem Legacy-Modus identisch. Bei Verwendung eines linearen Farbraums entspricht **ACE** mehr oder weniger [OpenColorIO](https://opencolorio.org/index.html).

## Substance-Plug-ins

Wenn Sie Substance-Material über das Substance-Integrations-Plug-in verwenden, werden die Ausgaben für linear/gamma automatisch über die Integration und das Farbmanagement der Host-Anwendung gekennzeichnet. Es ist jedoch wichtig, den Prozess zu verstehen: Wenn Substance-Maps als exportierte Bitmaps und nicht als Substance-Materialien verwendet werden, müssen Sie die Texturen je nach verwendetem Renderer möglicherweise manuell als **gamma-codiert** oder **raw** markieren. Üblicherweise sind 8- oder 16-Bit-PNG-, JPG-, TGA- oder TIF-Dateien gamma-codiert, während **sRGB OETF**- und EXR-Dateien linear sind.

## 3D-Anwendungen

### Arbeiten mit Texturen

* [Substance von Texturen in Maya](../../renderers/color-management/textures-in-maya/substance-textures-in-maya.md)
* [Substance von Texturen in 3ds Max](../../renderers/color-management/textures-in-3ds-max/substance-textures-in-3ds-max.md)
