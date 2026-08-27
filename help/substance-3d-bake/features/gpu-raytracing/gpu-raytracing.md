---
helpx_url: "https://helpx.adobe.com/de/substance-3d-bake/features/gpu-raytracing.html"
breadcrumb-title: ''
description: Aktivieren Sie hardwarebeschleunigtes GPU-Raytracing, um Backberechnungen für schnellere Workflows um das 25fache oder mehr zu beschleunigen.
helpx_creative_field: ""
helpx_description: bakers > Features > GPU Raytracing
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: GPU-Raytracing
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '326'
ht-degree: 18%

---


# GPU-Raytracing

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

Einige Bäcker unterstützen die Hardwarebeschleunigung des Raytracing auf der GPU, wodurch die Rechengeschwindigkeit in der Regel um den Faktor 25 oder mehr erhöht wird.

## Hardware-Anforderungen

Die Raytracing-Funktion wird automatisch aktiviert, wenn das System die folgenden Anforderungen erfüllt:

* Eine kompatible GPU ist installiert\* (RTX-Serie, Titan V oder GeForce 10xx)
* GPU-Treiber sind auf dem neuesten Stand
* Windows 10 &#39;Fall Creator&#39;/Oktober-Update (Version 1809) oder höher ist installiert\*\*

</td>
<td style="border: 0;" valign="top">

![GPU-Raytracing-Ein/Aus-Vergleich](../../assets/rtx-ao-demo.gif "GPU-Raytracing-Ein/Aus-Vergleich"){zoomable="yes"}

</td>
</tr>
</table>

\*: Kompatible NVIDIA-GPUs enthalten alle GPUs, die die Pascal-Architektur oder eine neuere verwenden. D. h. die GTX 10-Serie, die Titan V-Serie, die RTX 20-Serie oder neuere Versionen.

\*\*: Um Ihre Windows Version zu überprüfen, klicken Sie auf das Startmenü, geben Sie &#39;winver&#39; ein und drücken Sie die Eingabetaste.\
Sie können das Update über die [dedizierte Seite](https://support.microsoft.com/en-us/help/4028685/windows-10-get-the-update) auf der Microsoft-Support-Website abrufen.

>[!TIP]
>
> Bei Problemen können GPU-Raytracing in den Anwendungsvoreinstellungen deaktiviert werden.

## Unterstützte Bäcker

In den folgenden Tabellen ist die GPU-Raytracing-Unterstützung für jeden Bäcker nach der Substance 3D-Bäckerversion aufgeführt:

+++Version 3 und höher

| Baker | Unterstützt GPU-Raytracing |
| --- | --- |
| Umgebungsverdeckung | <div><img alt="(Häkchen)&quot; data-preserve-html=&quot;true" src="../../assets/check.svg"/></div> |
| Normal gebogen | <div><img alt="(Häkchen)&quot; data-preserve-html=&quot;true" src="../../assets/check.svg"/></div> |
| Color | <div><img alt="(Häkchen)&quot; data-preserve-html=&quot;true" src="../../assets/check.svg"/></div> |
| Biegung | <div><img alt="(Häkchen)&quot; data-preserve-html=&quot;true" src="../../assets/check.svg"/></div> |
| Höhe | <div><img alt="(Häkchen)&quot; data-preserve-html=&quot;true" src="../../assets/check.svg"/></div> |
| Normal | <div><img alt="(Häkchen)&quot; data-preserve-html=&quot;true" src="../../assets/check.svg"/></div> |
| Normalen-Welt-Raum | <div><img alt="(Fehler)&quot; data-preserve-html=&quot;true" src="../../assets/error.svg"/></div> |



| Baker | Unterstützt GPU-Raytracing |
| --- | --- |
| Deckkraftmaske | <div><img alt="(Häkchen)&quot; data-preserve-html=&quot;true" src="../../assets/check.svg"/></div> |
| Position | <div><img alt="(Häkchen)&quot; data-preserve-html=&quot;true" src="../../assets/check.svg"/></div> |
| Niedrige Position | <div><img alt="(Fehler)&quot; data-preserve-html=&quot;true" src="../../assets/error.svg"/></div> |
| Stärke | <div><img alt="(Häkchen)&quot; data-preserve-html=&quot;true" src="../../assets/check.svg"/></div> |
| Transferierte Textur | <div><img alt="(Häkchen)&quot; data-preserve-html=&quot;true" src="../../assets/check.svg"/></div> |
| Welt zu Tangente | <div><img alt="(Fehler)&quot; data-preserve-html=&quot;true" src="../../assets/error.svg"/></div> |


+++

+++Version 2

| Baker | Unterstützt GPU-Raytracing |
| --- | --- |
| Umgebungsverdeckung | <div><img alt="(Fehler)&quot; data-preserve-html=&quot;true" src="../../assets/error.svg"/></div> |
| Umgebungsverdeckung aus Mesh | <div><img alt="(Häkchen)&quot; data-preserve-html=&quot;true" src="../../assets/check.svg"/></div> \* |
| Normal gebogen aus Mesh | <div><img alt="(Häkchen)&quot; data-preserve-html=&quot;true" src="../../assets/check.svg"/></div> \* |
| Farbe aus Mesh | <div><img alt="(Fehler)&quot; data-preserve-html=&quot;true" src="../../assets/error.svg"/></div> \* |
| UV zu SVG konvertieren | <div><img alt="(Fehler)&quot; data-preserve-html=&quot;true" src="../../assets/error.svg"/></div> |
| Krümmung aus Mesh | <div><img alt="(Häkchen)&quot; data-preserve-html=&quot;true" src="../../assets/check.svg"/></div> \* |
| Höhe aus Mesh | <div><img alt="(Fehler)&quot; data-preserve-html=&quot;true" src="../../assets/error.svg"/></div> \* |
| Normal aus Mesh | <div><img alt="(Fehler)&quot; data-preserve-html=&quot;true" src="../../assets/error.svg"/></div> \* |



| Baker | Unterstützt GPU-Raytracing |
| --- | --- |
| Deckkraftmaske aus Gitter | <div><img alt="(Fehler)&quot; data-preserve-html=&quot;true" src="../../assets/error.svg"/></div> \* |
| Position aus Mesh | <div><img alt="(Fehler)&quot; data-preserve-html=&quot;true" src="../../assets/error.svg"/></div> \* |
| Position | <div><img alt="(Fehler)&quot; data-preserve-html=&quot;true" src="../../assets/error.svg"/></div> |
| Dicke aus Mesh | <div><img alt="(Häkchen)&quot; data-preserve-html=&quot;true" src="../../assets/check.svg"/></div> \* |
| Transferierte Textur aus Mesh | <div><img alt="(Fehler)&quot; data-preserve-html=&quot;true" src="../../assets/error.svg"/></div> \* |
| Welt-Raumrichtung | <div><img alt="(Fehler)&quot; data-preserve-html=&quot;true" src="../../assets/error.svg"/></div> |
| Welt-Raum-Normale | <div><img alt="(Fehler)&quot; data-preserve-html=&quot;true" src="../../assets/error.svg"/></div> |


\*: Unterstützt CPU-Raytracing, das deutlich langsamer ist als GPU-Raytracing.

+++
