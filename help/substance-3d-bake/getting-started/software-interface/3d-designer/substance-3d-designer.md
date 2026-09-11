---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/getting-started/software-interface/substance-3d-designer.html"
breadcrumb-title: ''
description: Hier erfahren Sie, wie Sie in Substance 3D Designer das Fenster "Baking führ" öffnen und verwenden, um Modellinformationen in Texturen Baking führen.
helpx_creative_field: ""
helpx_description: bakers > Getting Started > Software Interface > Substance 3D Designer
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Substance 3D Designer
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 2%

---


# Substance 3D Designer

![](../../../assets/sd-mesh-right-click.png)

Auf das Baking führend Fenster kann über die Meshdatei im Fenster [Explorer](https://helpx.adobe.com/substance-3d/unlisted/documentation/sddoc/the-explorer-129368147.html) zugegriffen werden. Klicken Sie mit der rechten Maustaste auf den Namen des Meshs, und wählen Sie &quot;**Modellinformationen Baking geführt**&quot; aus, um das Baking führend Fenster zu öffnen.

## Überblick

![](../../../assets/sd-window-overview.png){width="500px"}

Das Baking führend Fenster von ist in mehrere Bedienfelder unterteilt, die im Folgenden beschrieben werden.

### Zu Baking führend Element

![](../../../assets/sd-mesh-selection.png)

Dieses Bedienfeld steuert, welcher Teil des Low-Poly-Meshs für den Baking führ verwendet wird.

Dieses Bedienfeld listet die Geometrie auf, die sich innerhalb der Meshdatei mit niedriger Poly-Dichte befindet. Standardmäßig basiert die Liste auf den einzelnen Materialien, die in der Datei gefunden wurden, kann jedoch bei Bedarf auf Unter-Mesh umgestellt werden. Sie können Elemente deaktivieren, die beim Baking führ ignoriert werden sollen.

### Ausgabe

![](../../../assets/sd-output.png)

Dieses Bedienfeld steuert, wo sich die Baking geführt Textur befindet.

| *Parameter* | *Beschreibung* |
| --- | --- |
| **Methode** | Steuert, wie die Baking geführt Texturen mit dem Substance-Paket gespeichert werden.Mögliche Werte:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Eingebettet</strong> : Die Baking geführt Texturen werden in einem Unterordner neben dem Substance-Paket mit einem bestimmten Namen gespeichert.</li><li data-preserve-html="true"><strong>Verknüpft</strong> (Standard) : Die gebackene Textur wird in dem definierten Ordner gespeichert und dann in das Substance-Paket aufgenommen.</li></ul> |
| **Ordner** | Speicherort der Texturen, die als Stapel vorliegen. Klicken Sie auf drei Punkte, um ein Dateidialogfeld zu öffnen, und wählen Sie den Exportordner aus. Rechts wird ein Häkchen angezeigt, das angibt, ob der Ordner tatsächlich existiert oder nicht. |
| **Name** | Namenskonvention der gebackenen Texturen. Klicken Sie auf die Schaltfläche mit den drei Punkten, um eine Dropdown-Liste zu öffnen und andere Platzhalter einzufügen (Backname, benutzerdefiniert, Material, Gitter). |
| **Beispiel** | Simulieren Sie einen Dateinamen, um die Namenskonvention zu testen. |
| **Ressource in einen netzspezifischen Ordner platzieren** | Wenn diese Option aktiviert ist, werden die Texturen in einem Ordner gespeichert, der als Gitterdatei bezeichnet wird. |

### Hochauflösende Meshes

![](../../../assets/sd-high.png)

Dieses Bedienfeld steuert die Liste der Gitter mit hohem Poly-Wert und die zugehörigen Einstellungen. Weitere Informationen finden Sie in den [allgemeinen Parametern](../../../bakers-settings/common-parameters/common-parameters.md).

### Standardwerte

![](../../../assets/sd-default-values.png)

Weitere Informationen finden Sie in den [allgemeinen Parametern](../../../bakers-settings/common-parameters/common-parameters.md).

### Liste und Einstellungen der Baker

![](../../../assets/sd-baker-list.png)

Im Baker können Sie auswählen, welche Baking geführt Textur Sie generieren möchten. Standardmäßig ist die Liste leer.

* **Neuen Bäcker hinzufügen:** Klicken Sie auf die Schaltfläche &quot;Bäcker hinzufügen&quot;.
* **Einen Bäcker entfernen:** Wählen Sie den Bäcker in der Liste aus und klicken Sie dann auf die Schaltfläche &quot;Bäcker löschen&quot;.
* **Einen Bäcker nach oben verschieben:** Wählen Sie den Bäcker in der Liste aus und klicken Sie dann auf die Schaltfläche &quot;Nach oben ziehen&quot;.
* **Einen Baker nach unten bewegen**&#x200B;Wählen Sie den Baker in der Liste aus und klicken Sie dann auf die Schaltfläche &quot;Nach unten schieben&quot;.

Jeder Bäcker in der erbt standardmäßig die Standardwerte (siehe oben). Die Größe (Auflösung) kann beispielsweise überschrieben werden, indem man auf die Zelle in der Zeile des Bakers klickt. Dies gilt auch für die anderen Einstellungen in der Zeile.

Wenn Sie auf einen Baker in der Liste klicken, wird die Parameteransicht des Bakers mit ihren spezifischen Parametern aktualisiert.

Weitere Informationen zu den spezifischen Parametern finden Sie unter: [Baker-Einstellungen](../../../bakers-settings/bakers-settings.md).
