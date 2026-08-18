---
helpx_url: "https://helpx.adobe.com/de/substance-3d-integrations/3d-applications/modo/working-with-normals.html"
breadcrumb-title: ''
description: Konfigurieren Sie die normalen Ausrichtungseinstellungen für Karten in MODO, um sicherzustellen, dass das normale Rendering von Karten mit Substance-Materialien korrekt ist.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > MODO > Working with Normals
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Arbeiten mit Normalen
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '151'
ht-degree: 0%

---


# Arbeiten mit Normalen

Arbeiten mit normalen Daten - Festlegen der richtigen Ausrichtung

Stock-Substance verwenden die normale Ausrichtung von DX. MODO verwendet jedoch OGL. Sie können die Normale spiegeln, indem Sie den Parameter Normales Format auf 1,0 festlegen. Das Substance-Plugin interpretiert nur die auf der Substance festgelegten Parameter. Möglicherweise tritt eine Substance auf, die nicht über den Parameter &quot;normal\_format&quot; verfügt, da es Sache des Autors der Substance ist, dieses Steuerelement benutzerdefinierten Substance hinzuzufügen. Wenn Sie auf einen Substance stoßen, der diesen Parameter nicht hat, können Sie den grünen Kanal auf der Texturebene der Normalmap spiegeln, um die Ausrichtung zu korrigieren.

>[!NOTE]
>
> Das Spiegeln des grünen Kanals ist nur möglich, wenn die Substance die falsche Normalausrichtung hat und der Autor kein Steuerelement erstellt hat, um die Substance-Normalausrichtung zu spiegeln

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../../assets/normal-1.png)

</td>
<td style="border: 0;" valign="top">

![](../../../assets/invert-2.png)

</td>
</tr>
</table>
