---
helpx_url: "https://helpx.adobe.com/de/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-4/unreal-engine-4-scripting.html"
breadcrumb-title: ''
description: Verwenden Sie die Skript-API Substance Unreal Engine 4, um Substance-Material in Ihren Projekten programmgesteuert zu verwalten.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 4 > Unreal Engine 4 Scripting
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Unreal Engine 4-Skripterstellung
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '204'
ht-degree: 0%

---


# Unreal Engine 4-Skripterstellung

Das Substance in Unreal Engine Plugin kann mit Skripten versehen werden. Die Methoden werden in der Datei SubstanceGraphInstance.h des Plug-ins aufgeführt und mit Anmerkungen versehen, die sich normalerweise im folgenden Verzeichnis befindet, wenn das Plug-in vom Marketplace installiert wird:

* **Installation des Engine**: [UE\_4.X.X-Speicherort]\Engine\Plugins\Marketplace\Substance\Source\SubstanceCore\Classes\SubstanceGraphInstance.h
* **Projektinstallation**: [Speicherort des Projektordners]\Plugins\Runtime\Substance\Source\SubstanceCore\Classes\SubstanceGraphInstance.h

  ![](../../../../assets/substancegraphinstance.png)

`BlueprintCallable` gibt an, dass die Methode auch im Blueprint-Editor verwendet werden kann.

## Scripting im Python-Editor von Unreal Engine

Wenn Sie die Methoden verwenden, die in der Datei SubstanceGraphInstance.h im Python-Editor von Unreal Engine aufgeführt sind, müssen sie von Pascal Case in Snake Case konvertiert werden (mit Kleinbuchstaben und einem Unterstrich zwischen den einzelnen Wörtern). Beispiel: `SetInputColor` wird zu `set_input_color`.

Der Python-Editor in Unreal Engine kann über &quot;Fenster&quot; > &quot;Entwicklertools&quot; > &quot;Ausgabeprotokoll&quot; aufgerufen werden und die Dropdown-Liste unten links auf &quot;Python&quot; setzen.

## Beispielskripten

Im Folgenden finden Sie eine Reihe von Beispielskripten, die im Python-Editor verwendet werden können.

## Erstellen eines Substance-Materials

```
## Python example on creating a Substance material.

 

import unreal 

 

## Create factory

sf = unreal.SubstanceFactory() 

factory = sf.import_archive("/Game", "C:/4d/unreal/stylized_lava_cracked.sbsar") 

graph_descs = factory.get_graph_descs() 

mats = unreal.SubstanceUtility.get_substance_included_materials() 

 

## Create graph instance

for graph_desc in graph_descs: 

    print(graph_desc) 

## You could name based on label or on index or another way

    graph_name = "/Game/FirstInstance_" + graph_desc.label 

    material_name = "/Game/FirstMaterial_" + graph_desc.label 

## graph_name = f"/Game/FirstInstance_{graph_desc.index}"

## material_name = f"/Game/FirstMaterial_{graph_desc.index}"

    graph = factory.create_graph_instance(graph_desc, graph_name) 

    graph.create_outputs() 

    graph.create_material(material_name, mats[0]) 

    graph.set_input_color("obsidian_color", unreal.LinearColor(0, 0, 1)) 

    graph.set_input_color("lava_color", unreal.LinearColor(0, 1, 0)) 

    graph.prepare_outputs_for_save() 

    graph.render_sync() 

    graph.save_all_outputs(True)
```


## Erstellen eines einzelnen Grafen eines Substance-Materials

```
## Python example on creating a Substance material.

 

import unreal 

 

## Create factory

sf = unreal.SubstanceFactory() 

factory = sf.import_archive("/Game", "C:/4d/unreal/stylized_lava_cracked.sbsar") 

graph_descs = factory.get_graph_descs() 

mats = unreal.SubstanceUtility.get_substance_included_materials() 

 

## Create only 1 graph instance

graph_desc = graph_descs[0] 

print(graph_desc) 

graph_name = "/Game/MyGraphInstance" 

material_name = "/Game/MyMaterial" 

graph = factory.create_graph_instance(graph_desc, graph_name) 

graph.create_outputs() 

graph.create_material(material_name, mats[0]) 

graph.set_input_color("obsidian_color", unreal.LinearColor(0, 1, 1)) 

graph.set_input_color("lava_color", unreal.LinearColor(1, 0, 0)) 

graph.prepare_outputs_for_save() 

graph.render_sync() 

graph.save_all_outputs(True)
```


## Erstellen Sie mehrere Instanzen eines Substance-Materials mit unterschiedlichen Parametern.

```
## Python example on creating mulitple Substance materials.

 

import unreal 

 

## Create factory. Should only need 1 factory, even if multiple instances are created

sf = unreal.SubstanceFactory() 

factory = sf.import_archive("/Game", "C:/4d/unreal/stylized_lava_cracked.sbsar") 

graph_descs = factory.get_graph_descs() 

mats = unreal.SubstanceUtility.get_substance_included_materials() 

 

## Create first graph instance

for graph_desc in graph_descs: 

    graph_name = "/Game/FirstInstance_" + graph_desc.label 

    material_name = "/Game/FirstMaterial_" + graph_desc.label 

    graph = factory.create_graph_instance(graph_desc, graph_name) 

    graph.create_outputs() 

    graph.create_material(material_name, mats[0]) 

    graph.set_input_color("obsidian_color", unreal.LinearColor(0, 0, 1)) 

    graph.set_input_color("lava_color", unreal.LinearColor(0, 1, 0)) 

    graph.prepare_outputs_for_save() 

    graph.render_sync() 

    graph.save_all_outputs(True) 

 

## Create second graph instance

for graph_desc in graph_descs: 

    graph_name = "/Game/SecondInstance_" + graph_desc.label 

    material_name = "/Game/SecondMaterial_" + graph_desc.label 

    graph = factory.create_graph_instance(graph_desc, graph_name) 

    graph.create_outputs() 

    graph.create_material(material_name, mats[0]) 

    graph.set_input_color("obsidian_color", unreal.LinearColor(1, 0, 1)) 

    graph.set_input_color("lava_color", unreal.LinearColor(1, 1, 0)) 

    graph.prepare_outputs_for_save() 

    graph.render_sync() 

    graph.save_all_outputs(True)
```


## Duplizieren eines Substance-Grafen

```
## Python example on duplicating a Subtance material.

 

import unreal 

 

## Create factory

sf = unreal.SubstanceFactory() 

factory = sf.import_archive("/Game", "C:/4d/unreal/stylized_lava_cracked.sbsar") 

graph_descs = factory.get_graph_descs() 

mats = unreal.SubstanceUtility.get_substance_included_materials() 

 

## Create first graph

for graph_desc in graph_descs: 

    print(graph_desc) 

    graph_name = "/Game/FirstGraph_" + graph_desc.label 

    material_name = "/Game/FirstMaterial_" + graph_desc.label 

    graph = factory.create_graph_instance(graph_desc, graph_name) 

    graph.create_outputs() 

    graph.create_material(material_name, mats[0]) 

    graph.set_input_color("obsidian_color", unreal.LinearColor(0, 0, 1)) 

    graph.set_input_color("lava_color", unreal.LinearColor(0, 1, 0)) 

    graph.prepare_outputs_for_save() 

    graph.render_sync() 

 

## Duplicate graph

new_material_name = "/Game/SecondMaterial" 

new_graph = graph.duplicate() 

new_graph.create_outputs() 

new_graph.create_material(new_material_name, mats[0]) 

new_graph.prepare_outputs_for_save() 

new_graph.render_sync()
```
