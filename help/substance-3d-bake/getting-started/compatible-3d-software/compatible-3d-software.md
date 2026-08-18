---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/getting-started/compatible-3d-software.html"
breadcrumb-title: ''
description: Erfahre, welche 3D-Software mit Substance Bakers kompatibel ist und wie du Maschen für optimale Backergebnisse vorbereitest.
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

Die meisten 3D-Programme sind mit Substance Bakers kompatibel, solange sie die Gittergeometrie als Polygone in Dateiformaten exportieren, die von den Anwendungen unterstützt werden.

Allerdings ist beim Export dieser Gitter nicht jede Software hinsichtlich Funktion und Qualität auf dem gleichen Stand. Aus diesem Grund ist es wichtig, eine Masche richtig zu reinigen und sicherzustellen, dass sie mit den Bäckereien kompatibel ist. Weitere Informationen zum Vorbereiten eines Gitters finden Sie in den verschiedenen [Hilfslinien](../../guides/performances-and-opt/performances-and-optimizations.md).

## Softwarekompatibilität

Im Folgenden finden Sie eine Liste der allgemein bekannten 3D-Software und deren Kompatibilität mit den Bäckereien:

| *Name* | *Status* |
| --- | --- |
| **Blender** | Kompatibel: erfordert, dass Modifikatoren vor dem Export abgeflacht werden. |
| **Maya** | Kompatibel: erfordert ein Einfrieren der Transformation und eines Löschverlaufs vor dem Export. |
| **3DS Max** | Kompatibel: erfordert vor dem Export ein Zurücksetzen von xForm. |
| **MODO** | Kompatibel: empfohlen, den Exporter der Registerkarte &quot;Spiel&quot; mit der Einstellung &quot;Unreales statisches Gitter&quot; zu verwenden. |
| **Cinema 4D** | Kompatibel: erfordert, dass Modifikatoren vor dem Export abgeflacht werden. |
| **zBrush** | Nicht kompatibel: In einer anderen 3D-Anwendung müssen zuerst Polyurethan-Low-Poly-Meshes verarbeitet und gereinigt werden. Kompatibel: hochpolare Maschen zum Backen. |

## Dateiformat

Beim Backen von Geometrien ist es wichtig, auch das verwendete Dateiformat zu berücksichtigen. Das Dateiformat definiert die Informationsmenge, die im Gitter gespeichert wird.

Zu viele Informationen können manchmal schädlich sein und zu Fehlern führen. Wir empfehlen in der Regel, verschiedene Dateiformate auszuprobieren, wenn Fehler auftreten, da dies eine einfache Möglichkeit sein kann, Probleme zu beheben und festzustellen, ob der Täter im Bäcker selbst ist oder aus der 3D-Software stammt.

Im Folgenden finden Sie einen kurzen Überblick über die beiden gängigsten Dateiformate, die von Bäckereien unterstützt werden:

| Dateiformat | Information |
| --- | --- |
| **FBX** | Autodesk FBX (Filmbox) ist das Hauptdateiformat, das von Autodesk Software verwendet wird. Es kann als Text oder Binärdatei geschrieben werden.  Unterstützt werden:<ul data-preserve-html="true"><li data-preserve-html="true">UVs (Mehrfachsätze)</li><li data-preserve-html="true">Scheitelpunkt, Tangente und Binormale</li><li data-preserve-html="true">Vertexfarben</li><li data-preserve-html="true">Dreiecksgesicht, Vierecksgesicht und N-Gon-Gesicht</li><li data-preserve-html="true">Kameras</li><li data-preserve-html="true">Lichter</li><li data-preserve-html="true">Gitterunterteilungen</li><li data-preserve-html="true">Glättungsgruppen</li><li data-preserve-html="true">Materialinformationen (z. B. Farbe)</li><li data-preserve-html="true">Bitmap</li></ul> |
| **OBJ** | Wavefront OBJ ist ein sehr einfaches textbasiertes Dateiformat, das folgende Funktionen unterstützt:<ul data-preserve-html="true"><li data-preserve-html="true">UVs (nur ein Satz)</li><li data-preserve-html="true">Scheitelpunkt Normale</li><li data-preserve-html="true">Scheitelpunktfarben (nur beim Export aus Pixologic zBrush)</li><li data-preserve-html="true">Dreiecksgesicht, Vierecksgesicht und N-Gon-Gesicht</li><li data-preserve-html="true">Materialfarbe (wenn <strong>mtl</strong>-Datei vorhanden ist)</li></ul> |
