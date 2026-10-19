---
helpx_url: 'https://helpx.adobe.com/de/substance-3d-general/ecosystem/general-system-requirements.html'
breadcrumb-title: ''
description: Prüfen Sie die Systemanforderungen für Substance 3D-Anwendungen, um sicherzustellen, dass Ihre Hardware die Mindestanforderungen, empfohlenen oder optimalen Spezifikationen erfüllt.
helpx_creative_field: ''
helpx_description: General Knowledge > Ecosystem > General system requirements
helpx_experience_level: ''
helpx_learn_topic: ''
helpx_tags: ''
title: Allgemeine Systemanforderungen
user-guide-description: ''
user-guide-title: ''
source-git-commit: eef3d78f33034f2c24f4c4471d9ccac805184525
workflow-type: tm+mt
source-wordcount: '625'
ht-degree: 2%
---

# Allgemeine Systemanforderungen

## Hardware-Anforderungen

+++Windows

|  | Minimum | Empfohlen | Optimal |
| --- | --- | --- | --- |
| **Betriebssystem** | Windows 11 64-Bit Version 23H2 | Windows 11 64-Bit Version 24H1 | Windows 11 64-Bit Version 24H2 |
| **CPU** | Intel Core i5 AMD Ryzen 5 | Intel Core i7 AMD Ryzen 7 | Intel Core i9 AMD Ryzen 9 |
| **GPU** | NVIDIA GeForce RTX 2060 Super NVIDIA Quadro RTX 4000 AMD Radeon RX 5700 XT AMD Radeon Pro W5700 | NVIDIA GeForce RTX 3080 NVIDIA Quadro RTX A4000 AMD Radeon RX 6800 XT AMD Radeon Pro W7700 | NVIDIA GeForce RTX 4090 NVIDIA Quadro RTX 5000 ADA Generation AMD Radeon RX 7900 XTX AMD Radeon Pro W7800 |
| **VRAM** | 8 GB | 16 GB | 24 GB |
| **RAM** | 16 GB | 32 GB | 64 GB |
| **Speicher** | SSD mit 30 GB verfügbarem Speicherplatz | SSD mit 50 GB verfügbarem Speicherplatz | SSD mit 70 GB verfügbarem Speicherplatz |

+++

+++macOS

|  | Minimum | Empfohlen | Optimal |
| --- | --- | --- | --- |
| **Betriebssystem** | macOS 15 Sequoia | macOS 27 Golden Gate | macOS 27 Golden Gate |
| **CPU** | Apple M1 | Apple M2 Pro | Apple M4 Pro |
| **GPU** | Apple M1 | Apple M2 Pro | Apple M4 Pro |
| **RAM** | 16 GB | 32 GB | 64 GB |
| **Speicher** | SSD mit 30 GB verfügbarem Speicherplatz | SSD mit 50 GB verfügbarem Speicherplatz | SSD mit 70 GB verfügbarem Speicherplatz |

>[!WARNING]
>
> Für Pipelines, die unter Berücksichtigung der [VFX Reference Platform](https://vfxplatform.com/) erstellt wurden, können Substance 3D-Anwendungen weiterhin auf macOS 14 Sonoma installiert werden. Substance-Apps werden jedoch nicht mehr mit Betriebssystemversionen getestet, die die Mindestsystemanforderungen erfüllen, sodass die Stabilität nicht gewährleistet ist. Es wird empfohlen, auf eine neuere Betriebssystemversion zu aktualisieren.

+++

+++Linux

|  | Minimum | Empfohlen | Optimal |
| --- | --- | --- | --- |
| **Betriebssystem** | **Enterprise ETLA** RHEL 8.6 oder höher oder RHEL 9.2 oder höher **Steam** Ubuntu 22.04.1 LTS | **Enterprise ETLA** RHEL 8.6 oder höher oder RHEL 9.4 oder höher **Steam** Ubuntu 22.04.1 LTS oder höher | **Enterprise ETLA** RHEL 8.6 oder höher oder RHEL 9.4 oder höher **Steam** Ubuntu 22.04.1 LTS oder höher |

**Red Hat Enterprise Linux (RHEL) 9.x**: Das von unseren Anwendungen benötigte xcb-util-cursor-Paket wurde am 10. Mai 2024 aus dem EPEL 9-Repository entfernt. Ab diesem Datum wird das Paket vom Standard-RHEL 9-Repository unterstützt, das mit der Veröffentlichung von RHEL 9.4 zusammenfällt. Kunden, die RHEL-Versionen vor 9.4 verwenden, können das xcb-util-cursor-Paket nach dem 10. Mai 2024 nicht mehr aus dem EPEL 9-Repository beziehen.

Weitere Informationen zur Verfügbarkeit dieses Pakets im Standard-RHEL 9-Repository finden Sie unter: [Red Hat Enterprise Linux 9 - Paketmanifest - AppStream-Repository](https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux/9/html-single/package_manifest/index#AppStream-repository)

Weitere Informationen zu dieser Änderung finden Sie unter: [Red Hat Bugzilla - Fehler 2238273](https://bugzilla.redhat.com/show_bug.cgi?id=2238273) , [Red Hat Bugzilla - Fehler 2212302](https://bugzilla.redhat.com/show_bug.cgi?id=2212302)

+++

+++VR

| Branding | Modelle |
| --- | --- |
| Meta | Rift, Rift S, Quest, Quest 2 (mit Link), Quest Pro |

+++

Weitere Informationen finden Sie in den Anforderungen der einzelnen Anwendungen:

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../assets/sa-appicon-noshadow-256.png" alt="Substance 3D Sampler-Symbol" width="64px"/><br><a href="https://experienceleague.adobe.com/de/docs/substance-3d-sampler/using/getting-started/system-requirements">Substance 3D Sampler</a></td>
    <td style="border: 0;" valign="top"><img src="../../assets/ds-appicon-noshadow-256.png" alt="Substance 3D Designer-Symbol" width="64px"/><br><a href="https://experienceleague.adobe.com/de/docs/substance-3d-designer/using/getting-started/system-requirements">Substance 3D</a> <a href="https://experienceleague.adobe.com/de/docs/substance-3d-designer/using/getting-started/system-requirements">Designer</a></td>
    <td style="border: 0;" valign="top"><img src="../../assets/pt-appicon-noshadow-256.png" alt="Substance 3D Painter-Symbol" width="64px"/><br><a href="https://experienceleague.adobe.com/de/docs/substance-3d-painter/using/getting-started/system-requirements">Substance 3D Painter</a></td>
  </tr>
</table>

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../assets/md-appicon-noshadow-256.png" alt="Substance 3D Modeler-Symbol" width="64px"/><br><a href="https://helpx.adobe.com/substance-3d-modeler/getting-started/system-requirements.html">Substance 3D Modeler</a></td>
    <td style="border: 0;" valign="top"><img src="../../assets/sg-appicon-noshadow-256.png" alt="Substance 3D Stager-Symbol" width="64px"/><br><a href="https://helpx.adobe.com/substance-3d-stager/getting-started/system-requirements.html">Substance 3D Stager</a></td>
    <td style="border: 0;" valign="top"></td>
  </tr>
</table>

## Weitere Hinweise

### Nicht unterstützte Konfiguration

* Apple-Computerkonfigurationen mit eGPUs und vom Benutzer installierten GPUs werden nicht unterstützt.
* Virtuelle Windows-Computer werden nicht unterstützt.
* Windows-Server-Betriebssystem wird nicht unterstützt.
