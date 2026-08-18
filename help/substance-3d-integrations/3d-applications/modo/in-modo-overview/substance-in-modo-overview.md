---
helpx_url: "https://helpx.adobe.com/de/substance-3d-integrations/3d-applications/modo/substance-in-modo-overview.html"
breadcrumb-title: ''
description: Erfahren Sie mehr über das Substance-Plugin für MODO und wie Sie Substance-Materialien in Ihren Arbeitsablauf importieren und verwenden können.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > MODO > Substance in MODO Overview
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Substance in MODO - Übersicht
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '240'
ht-degree: 5%

---


# Substance in MODO - Übersicht

## Übersicht:

## Öffnen einer Substance

1. Erstellen Sie ein Material oder wählen Sie eine Materialgruppe.
1. Wählen Sie unter Textur > Substance die Option Substance erstellen, oder klicken Sie unter den Substance Kit-Optionen auf die Schaltfläche Erstellen. Dadurch wird ein Substance-Material im Shader-Baum erstellt.
1. Klicken Sie auf SBSAR laden , um eine SBSAR-Datei zu laden.

   ![](../../../assets/load-1.png)

## Erstellen von Ausgaben

Mit dem **Standardmodus - Modus für prinzipielle Schattierung** können Sie Ausgaben mithilfe des Metallic-/Raueit-Workflows erstellen.

1. Klicken Sie im Abschnitt &quot;Ausgaben&quot; der Substance-Eigenschaften auf die für die Schattierung benötigten Ausgaben. Die Substance-Textur wird generiert und dem Schattierungsbaum mit dem richtigen Materialebeneneffekt hinzugefügt. Für den Modus Principled Schattierung benötigen Sie Folgendes:

   | Substance-Ausgabe | Farbraum | Effekt &quot;Materialebene&quot; (Modus &quot;Schattierung mit Prinzipien&quot;) |
   | --- | --- | --- |
   | Grundfarbe | sRGB | Diffuse Farbe |
   | Normal | Linear | Normal |
   | Rauheit | Linear | Rauheit |
   | Metallisch | Linear | Metallisch |

   ![](../../../assets/outputs-3.png)

## Ändern der Auflösung/Parameter

Sie können die Substance-Parameter ändern, um die generierten Texturen zu aktualisieren oder zu ändern. Wenn du einen Parameter änderst, berechnet das Substance Engine die Texturen, die in das MODO-Material eingespeist werden.

1. Navigieren Sie zu den Substance-Eigenschaften für das Substance-Material und ändern Sie im Abschnitt &quot;Änderungen&quot; einen der Parameter.

   ![](../../../assets/params.png)
1. Sie können die Auflösung der generierten Texturen im Dropdown-Menü Ausgabegröße ändern. Substance können so eingestellt werden, dass sie bis zu 8K erzeugen. Das [Substance-GPU-Modul &#x200B;](../../../3d-applications/modo/modo-switch-engine/modo-switch-engine.md) ist für die 8K-Ausgabe erforderlich.
