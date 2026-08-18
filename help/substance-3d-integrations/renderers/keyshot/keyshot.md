---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/renderers/keyshot.html"
breadcrumb-title: ''
description: Verwenden Sie Substance-Materialien im Keyshot-Renderer für die Produktvisualisierung mit exportierten Texturmaps.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Keyshot
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Keyshot
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 8%

---


# Keyshot

*Keyshot 6.1.72*[&#x200B; Beispielszene herunterladen](https://www.dropbox.com/s/rvjsbbcx7c74aah/keyshot.zip?dl=0)

## Substance Painter Export

1. Für Keyshot müssen Sie eine Exportvorgabe mit &quot;Diffus&quot;, &quot;Spiegelung&quot;, &quot;Metallisch&quot;, &quot;Raueit&quot; und &quot;Normal&quot; (direktes X) konfigurieren.

   ![](https://helpx-prod.scene7.com/is/image/HelpxProd/key-01?$png$&jpegSize=300&wid=1794)

## Erweiterte Materialeinrichtung

Sie werden 2 fortgeschrittene Materialien verwenden. Das eine wird für Metallic und das andere für Dielektrikum.

1. Setze das Material auf &quot;Erweitert&quot;, und erstelle ein Diagramm.

   **Metallisch:**\
   a. Legen Sie den Brechungsindex auf 10 fest.\
   b. Legen Sie die Karten wie in der folgenden Tabelle angegeben fest.

   | Textur des Substance Painters | Erweiterter Materialkanal |
   | --- | --- |
   | Diffus | Diffus |
   | Metallisch | Deckkraft |
   | Normal | Bump \*Normal aktiviert |
   | Rauheit | Rauheit |
   | Spiegelung | Glanz |

1. Neues erweitertes Material erstellen

   **Dielektrisch:**\
   a. Legen Sie den Brechungsindex auf 1,5 fest.\
   b. Legen Sie die Karten wie in der folgenden Tabelle angegeben fest.

   | Textur des Substance Painters | Erweiterter Materialkanal |
   | --- | --- |
   | Diffus | Diffus |
   | Normal | Bump \*Normal aktiviert |
   | Rauheit | Rauheit |
   | Spiegelung | Glanz |

1. Nehmen Sie die Ausgabe des Metallic Advanced Material und fügen Sie sie dem + des DiElectric Advanced Material hinzu. Dadurch wird auf dem Material das Feld &quot;Beschriftung&quot; erstellt.

   ![](../../assets/key-02.png)
