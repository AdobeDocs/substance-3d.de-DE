---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/getting-started/compatible-3d-software.html"
breadcrumb-title: ''
description: Finde heraus, welche 3D-Software mit Substance Bakers kompatibel ist, und bereite die Mesh auf ein optimales Baking vor.
helpx_creative_field: ""
helpx_description: bakers > Getting Started > Compatible 3D software
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Kompatible 3D-Software
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 2%

---


# Kompatible 3D-Software

Die meisten 3D-Programme sind mit Substance Bakers kompatibel, solange sie Mesh-Geometrien als Polygone in Dateiformaten exportieren, die von den Programmen unterstützt werden.

Allerdings ist beim Export dieser Meshs nicht jede Software hinsichtlich Funktion und Qualität auf dem gleichen Stand. Aus diesem Grund ist es wichtig, einen Mesh ordnungsgemäß zu reinigen und sicherzustellen, dass er mit den Bakern kompatibel ist. Weitere Informationen zum Vorbereiten eines Meshs finden Sie in den verschiedenen [Handbüchern](../../guides/performances-and-opt/performances-and-optimizations.md).

## Softwarekompatibilität

Im Folgenden finden Sie eine Liste der allgemein bekannten 3D-Software und ihrer Kompatibilität mit den Bakern:

| *Name* | *Status* |
| --- | --- |
| **Blender** | Kompatibel: erfordert, dass Modifikatoren vor dem Export abgeflacht werden. |
| **Maya** | Kompatibel: erfordert ein Einfrieren des transformieren- und Löschverlaufs vor dem Export. |
| **3DS Max** | Kompatibel: erfordert vor dem Export ein Zurücksetzen von xForm. |
| **MODO** | Kompatibel: empfohlen, den Exporter &quot;Game Tab&quot; zu verwenden, der auf &quot;Unreal Static Mesh&quot; festgelegt ist. |
| **Cinema 4D** | Kompatibel: erfordert, dass Modifikatoren vor dem Export abgeflacht werden. |
| **zBrush** | Nicht kompatibel: Meshs mit wenig Poly müssen zuerst in einer anderen 3D-Anwendung bearbeitet und gereinigt werden. Kompatibel: hochpolare Meshs für das Baking. |

## Dateiformat

Beim Baking der Geometrie ist es wichtig, auch das verwendete Dateiformat zu berücksichtigen. Das Dateiformat definiert die Informationsmenge, die im Mesh gespeichert wird.

Zu viele Informationen können manchmal schädlich sein und zu Fehlern führen. Wir empfehlen in der Regel, verschiedene Dateiformate auszuprobieren, wenn Fehler auftreten, da dies eine einfache Möglichkeit sein kann, Probleme zu beheben und festzustellen, ob der Täter sich im Baker selbst befindet oder von der 3D-Software stammt.

Im Folgenden finden Sie einen kurzen Überblick über die beiden gängigsten Dateiformate, die von den Bakern unterstützt werden:

| Dateiformat | Information |
| --- | --- |
| **FBX** | Autodesk FBX (Filmbox) ist das Hauptdateiformat, das von Autodesk Software verwendet wird. Es kann als Text oder Binärdatei geschrieben werden.  Unterstützt werden:<ul data-preserve-html="true"><li data-preserve-html="true">UVs (Mehrfachsätze)</li><li data-preserve-html="true">Scheitelpunkt, Tangente und Binormale</li><li data-preserve-html="true">Vertexfarben</li><li data-preserve-html="true">Dreieck Fläche, Quad Fläche und N-Gon Fläche</li><li data-preserve-html="true">Kameras</li><li data-preserve-html="true">Lichter</li><li data-preserve-html="true">Mesh Unterteilungen</li><li data-preserve-html="true">Glättungsgruppen</li><li data-preserve-html="true">Material-Informationen (z. B. Farbe)</li><li data-preserve-html="true">Bitmap</li></ul> |
| **OBJ** | Wavefront OBJ ist ein sehr einfaches textbasiertes Dateiformat, das folgende Funktionen unterstützt:<ul data-preserve-html="true"><li data-preserve-html="true">UVs (nur ein Satz)</li><li data-preserve-html="true">Scheitelpunkt Normale</li><li data-preserve-html="true">Scheitelpunkt-Farben (nur beim Export aus Pixologic zBrush)</li><li data-preserve-html="true">Dreieck Fläche, Quad Fläche und N-Gon Fläche</li><li data-preserve-html="true">Material-Farbe (wenn die Datei <strong>mtl</strong> vorhanden ist)</li></ul> |
