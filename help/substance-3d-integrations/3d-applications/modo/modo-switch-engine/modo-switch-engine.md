---
helpx_url: "https://helpx.adobe.com/de/substance-3d-integrations/3d-applications/modo/modo-switch-engine.html"
breadcrumb-title: ''
description: Wechseln Sie in MODO zwischen CPU- und GPU-Substance-Engines, um die Leistung je nach Hardware zu optimieren.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > MODO > Modo Switch Engine
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Modo Switch Engine
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---


# Modo Switch Engine

## Switching-Substance Engine

Es gibt zwei Versionen des Substance Engine, die CPU und die GPU. Die GPU-Engine wird verwendet, um Texturen mit mehr als 2K zu erstellen. Die CPU-Engine ist nur in der Lage, Texturen bis zu 2K zu erzeugen. Wenn Sie Texturen mit höherer Auflösung benötigen, müssen Sie zur GPU-Engine wechseln.

Wählen Sie im Menü &quot;Substance Kit&quot; die Option &quot;Substance Settings&quot; und dann &quot;Switch Substance Engine&quot;. Sie müssen MODO neu starten, damit die GPU-Engine aktiviert wird. Diese Einstellung dient als globale Voreinstellung. Die GPU-Engine wird dann jedes Mal aktiviert, wenn Sie MODO ausführen, bis sie manuell umgeschaltet wird.

>[!NOTE]
>
> **Für die Verwendung der Substance-GPU-Engine ist eine GPU mit dediziertem Video-RAM von mindestens 1 GB erforderlich. Integrierte GPUs werden nicht unterstützt.**\
> Nvidia: GeForce 650M 1 GB oder höher\
> AMD: 6870M oder höher

![](../../../assets/switch.png)
