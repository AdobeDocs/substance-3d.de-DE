---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/modo/custom-materials.html"
breadcrumb-title: ''
description: Verwenden Sie benutzerdefinierte Materialien von Unreal, Unity und glTF in MODO mit dem Substance-Plugin für spezielle Workflows.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > MODO > Custom Materials
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Eigene Materialien
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 12%

---


# Eigene Materialien

Das Substance-Plugin unterstützt die benutzerdefinierten Materialien Unreal, Unity und glTF. Bevor Sie eine SBSAR-Datei laden, können Sie auswählen, welchen Schattierung-Modus Sie verwenden möchten.

## Inhaltsverzeichnis

## Einheitsmaterial

Bei Verwendung des Einheitsmaterials wird der Effekt &quot;Materialebene&quot; automatisch eingestellt. Das Substance Plugin platziert das Unity Material direkt über dem Substance Item Material.

| Substance-Ausgabe | Farbraum | Effekt &quot;Materialebene&quot; |
| --- | --- | --- |
| Grundfarbe | sRGB | Unity-Albedo |
| Glanz | Linear | Unity-Smoothness |
| Metallisch | Linear | Unity Metallic |
| Normal | Linear | Unity Normal |
| Ausstrahlend | sRGB | Unity-Emission **\*auf sRGB für Image-Standbild festgelegt** |
| Höhe | Linear | Unity Bump |
| Umgebungsverdeckung | Linear | Unity Ambient-Verdeckung |

![](../../../assets/unity-1.png){width="600px"}

## Unreales Material

Bei Verwendung des unrealen Materials wird der Effekt &quot;Materialebene&quot; automatisch eingestellt. Das Substance Plugin platziert das Unreal Material direkt über dem Substance Item Material.

| Substance-Ausgabe | Farbraum | Effekt &quot;Material-Ebene&quot; |
| --- | --- | --- |
| Grundfarbe | sRGB | Unwirkliche Grundfarbe |
| Rauheit | Linear | Unwirkliche Rauheit |
| Metallisch | Linear | Unwirklich Metallic |
| Normal | Linear | Unreal Normal |
| Höhe | Linear | Unregelmäßiger Bump |
| Ausstrahlend | sRGB | Unreale Emissive **\*auf sRGB für Bildstandbild festgelegt** |
| Umgebungsverdeckung | Linear | Unechtes Ambient occlusion |
| Deckkraft | Linear | Unreale Deckkraft **\*muss die Option &quot;Invertiert&quot; für die Textur** deaktivieren. |

![](https://helpx-prod.scene7.com/is/image/HelpxProd/unreal?$png$&jpegSize=200&wid=1343){width="600px"}

Möglicherweise musst du die Normalität umkehren. Sie können dies über das Menü &quot;Tweak&quot; (Anpassungen) tun, wenn der Substance über eine Steuerung für die normale Ausrichtung verfügt. Wenn nicht, kann dies auf der Textur selbst geschehen. Weitere Informationen finden Sie auf der Seite &quot;**[Arbeiten mit Normalen](../../../3d-applications/modo/working-with-normals/working-with-normals.md)**&quot;.

## glTF-Material

Bei Verwendung des glTF-Materials wird der Material-Ebeneneffekt automatisch eingestellt. Das Substance-Plugin platziert das glTF-Material direkt über dem Substance Item-Material.

| Substance-Ausgabe | Farbraum | Effekt &quot;Material-Ebene&quot; |
| --- | --- | --- |
| Grundfarbe | sRGB | glTF-Grundfarbe |
| Rauheit | Linear | glTF-Rauheit |
| Metallisch | Linear | glTF Metallic |
| Normal | Linear | glTF Normal |
| Ausstrahlend | sRGB | glTF Emissive **\*auf sRGB für Standbild** festgelegt |
| Umgebungsverdeckung | Linear | glTF Ambient occlusion |

![](../../../assets/gltf.png){width="600px"}

Möglicherweise musst du die Normalität umkehren. Sie können dies über das Menü &quot;Tweak&quot; (Anpassungen) tun, wenn der Substance über eine Steuerung für die normale Ausrichtung verfügt. Wenn nicht, kann dies an der Textur selbst vorgenommen werden. Weitere Informationen finden Sie auf der Seite &quot;**[Arbeiten mit Normalen](../../../3d-applications/modo/working-with-normals/working-with-normals.md)**&quot;.
