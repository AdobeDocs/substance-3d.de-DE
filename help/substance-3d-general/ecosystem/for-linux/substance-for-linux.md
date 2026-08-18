---
helpx_url: "https://helpx.adobe.com/de/substance-3d-general/ecosystem/substance-for-linux.html"
breadcrumb-title: ''
description: Erfahren Sie, wie Sie Substance 3D-Anwendungen unter Linux über das Adobe Download Access-Portal herunterladen, installieren und aktivieren.
helpx_creative_field: ""
helpx_description: Substance 3D General
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Substance 3D für Linux (ADA)
user-guide-description: ''
user-guide-title: ''
source-git-commit: 081136918fdf7f431ecee47e5ce64d8b5235bb1b
workflow-type: tm+mt
source-wordcount: '370'
ht-degree: 0%

---


# Implementierungshandbuch

Nachdem Sie Substance 3D für Linux® über Ihren Unternehmensvertrag erworben haben, werden die entsprechenden Produkte und Lizenzen im [Adobe Download Access (ADA)](https://download-access.adobe.com/lws/downloads)-Portal bereitgestellt. Sie müssen sowohl die Software-Builds als auch die Lizenzschlüsseldateien von ADA herunterladen, um die Software erfolgreich bereitstellen zu können.

## Laden Sie Software-Builds und Lizenzschlüsseldateien herunter:

Melden Sie sich bei [Adobe Download Access](https://download-access.adobe.com/lws/downloads) an. Hier finden Sie die Software-Builds und Lizenzschlüsseldateien:

1. Wählen Sie in der Dropdown-Liste &quot;Konto&quot; das Konto aus, für das Sie Substance 3D Linux erworben haben.

   ![](../../assets/ADA1.png)
1. Navigieren Sie zu Downloads mit dem Link in der Kopfzeile der Seite.

   ![](../../assets/ADA2.png)
1. Klicken Sie auf Downloads für das entsprechende Produkt anzeigen.

   ![](../../assets/ADA3.png)
1. ADA lädt die dieser ID zugeordneten Lizenzinformationen und zeigt sie in der folgenden Tabelle an.
1. Klicken Sie in der Zeile &quot;Digitales Zertifikat&quot; auf &quot;Herunterladen&quot;, um die ZIP-Datei mit den Lizenzschlüsseldateien herunterzuladen.

   * Die ZIP-Datei enthält einen Lizenzschlüssel pro Produkt.
   * Der Lizenzschlüssel aktiviert das Produkt auf jedem Ihrer lizenzierten Computer.

   ![](../../assets/ADA4.png)
1. Klicken Sie auf &quot;Substance 3D&quot; Sampler, Painter oder Designer, um die Software-Builds von Substance 3D Painter, Substance 3D Designer und Substance 3D Sampler anzuzeigen.
1. Klicken Sie auf &quot;Herunterladen&quot;, um die Installationsdatei des Produkts herunterzuladen, das Sie installieren möchten.

   ![](../../assets/ADA5.png)
1. Es erscheint eine Benachrichtigung &quot;Software herunterladen&quot;. Auf &quot;Akzeptieren&quot; klicken

   ![](../../assets/ADA6.png)

## Installation und Aktivierung

Installieren der Software:

1. Doppelklicken Sie auf die EXE-Datei des Produkts, um den Installationsassistenten zu starten.
1. Führen Sie die Installationsschritte aus, um die Installation abzuschließen.

Es gibt zwei Optionen für die Softwareaktivierung: entweder lokale Aktivierung oder Netzwerkaktivierung.

### Lokale Aktivierung

1. Entpacken Sie den ZIP-Ordner, der von ADA heruntergeladen wurde.
1. Starten Sie die Software, die Sie aktivieren möchten.
1. Wählen Sie im Aktivierungsassistenten die Option &quot;Mit Lizenzschlüsseldatei aktivieren&quot;.

   ![](../../assets/LinuxActivation3.png)
1. Klicken Sie auf &quot;Durchsuchen&quot; und zeigen Sie auf den Speicherort der entsprechenden Lizenzschlüsseldatei.
1. Klicken Sie auf &quot;Weiter&quot;, um die Software zu aktivieren.

### Netzwerkaktivierung

1. Entpacken Sie den ZIP-Ordner, der von ADA heruntergeladen wurde.
1. Legen Sie die entpackten Lizenzschlüsseldateien in einem gemeinsam genutzten bereitgestellten Netzwerk ab.
1. Richten Sie auf dem Computer des Benutzers eine Umgebungsvariable ein, die auf die Lizenzschlüsseldatei verweist, wie auf diesen Seiten erläutert:

   * Substance 3D Painter - <https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/pipeline-and-integration/configuration/environment-variables>
   * Substance 3D Designer - <https://experienceleague.adobe.com/en/docs/substance-3d-designer/using/pipeline-and-project-configuration/environment-variables>
   * Substance 3D Sampler - <https://experienceleague.adobe.com/en/docs/substance-3d-sampler/using/pipeline-and-integrations/environment-variables>
