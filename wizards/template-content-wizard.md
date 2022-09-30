---
description: >-
  The Template Content Wizard allows you to quickly install template content in
  your game.
---

# Template Content Wizard

{% embed url="https://youtu.be/zLSnaNzm-Uk" %}

## Accessing the Wizard

The template content wizard requires that one of your game scenes with either a GameManager or SceneConfig object is open in the editor so that it can determine which game to install the content into.

The Template Content Wizard can be opened by clicking _Tools_ in the menu bar, and selecting _AnyRPG > Wizard > Template Content Wizard_.

![](<../.gitbook/assets/image (87).png>)

![](<../.gitbook/assets/image (95).png>)

## Settings

| Name                       | Description                                                                                                                                                                                               |
| -------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Game Name                  | The name of the game in your Unity project to install the template content in.  This will be automatically filled in if you have any scene with the GameManager or SceneConfig prefabs open.              |
| Replace Existing Resources | If true, resources with the same name and folder location will be overwritten.  This can be useful if you have made modifications to resources, and want to reset them to their original template values. |
| Replace Existing Prefabs   | If true, prefabs with the same name and folder location will be overwritten.  This can be useful if you have made modifications to prefabs, and want to reset them to their default values.               |
| Scriptable Content         | A list of template content packages to install.                                                                                                                                                           |

## Available Template Content

Most of the content in the [Features Demo Game](../getting-started/included-sample-games.md#features-demo-game) can be installed using the Template Content Wizard.  There are over 1000 template packages available, so it can be helpful to know what is available.  You browse template packages by looking in the AnyRPG/Core/Content/TemplatePackages folder in your project.

![](<../.gitbook/assets/image (57).png>)

## Template Packages

A Template package consists of resources (Scriptable Objects) and prefabs.  Template packages can also have dependencies on other template packages to make re-using packages easy.  In general, any package you choose will install all dependencies for it to work without needing to manually install them.

![](<../.gitbook/assets/image (96).png>)

## Installing Content

Select content from the object browser window or drag it into the list, and click Install.

![](<../.gitbook/assets/image (47).png>)

## Using Template Content

### Prefabs

After install template content that includes prefabs such as interactables or unit (character) spawners, you will need to add those prefabs to a scene.  You can find them under the Prefab folder in your game folder.  Once you find a prefab, just drag it into the scene whereever you want it placed.

![](<../.gitbook/assets/image (45).png>)

### Scriptable Objects

Some types of template content do not include any prefabs that can be added to a scene, but still require you to define where you want to use them. Examples include vendor collections and loot tables.

In the screenshot below you can see how you would add vendor collections to a vendor NPC Unit Profile to make them available to purchase on the vendor in game.

![](<../.gitbook/assets/image (93).png>)

![](<../.gitbook/assets/image (21) (1).png>)
