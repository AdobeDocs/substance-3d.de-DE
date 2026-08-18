---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/modo/working-with-emissive.html"
breadcrumb-title: ''
description: Konfigurieren Sie emissive Eigenschaften für das Substance von Materialien in MODO, um den Lichtbetrag und die Farbeinstellungen zu steuern.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > MODO > Working with Emissive
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Arbeiten mit emissiven
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '201'
ht-degree: 0%

---


# Arbeiten mit emissiven

## Arbeiten mit emissionsfähigem Licht (Leuchtmenge und Farbe)

Substance kann eine optionale Emissionsausgabe haben. Sie können dies als &quot;Leuchtender Betrag&quot; und &quot;Farbe&quot; in MODO verwenden. Wenn Sie die Emissions-Ausgabe aktivieren, wird sie auf den Effekt &quot;Leuchtender Betrag&quot; eingestellt. Standardmäßig wird dieser Kanal auf der Registerkarte Texturbild-Standbild als Linear interpretiert.\
Mache einen Rechtsklick bzw. Ctrl-Klick auf die Struktur im Shader-Baum. Wähle &quot;Duplizieren&quot;. Stelle dann die duplizierte Emissionstextur auf den Effekt &quot;Luminöse Farbe&quot; ein. Du kannst dann den hohen und den niedrigen Wert der Textur ändern, um den Effekt &quot;Leuchtender Betrag&quot; noch intensiver wirken zu lassen.

>[!NOTE]
>
> Wenn die Struktur auf &quot;Luminöse Farbe&quot; eingestellt ist, müssen Sie die Interpretation auf der Registerkarte &quot;BildStandbild&quot; auf sRGB festlegen.

Um einen Blüteneffekt zu erhalten, müssen Sie &quot;Blüte&quot; im Renderfenster aktivieren und den Schwellenwert und den Radius festlegen.

![](../../../assets/bloom.png)

Bei den Materialien Unreal und Unity wird die emittierende Leistung speziell vom Material verarbeitet.\
Unreal = Unreal Emissive\
Unity = Unity Emission

Die Texturen &quot;Unreal Emissive&quot; und &quot;Unity Emission&quot; müssen auf der Registerkarte &quot;Bildstil&quot; von &quot;Linear&quot; in &quot;sRGB&quot; geändert werden.
