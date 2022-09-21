---
description: >-
  A scriptable content template is a list of scriptable objects, prefabs, and
  other scriptable content templates that can be installed in a new game using a
  wizard to save time.
---

# Scriptable Content Template

## Creation

Unlike most scriptable objects, a scriptable content template itself is not loaded into memory because it contains configuration information for installing content.  This means it can be created in any folder and should definitely not be located in a _Resources_ folder or any subfolder of a resources folder. To create one, setup a folder that is not a child of a _Resources_ folder and right click.  Choose _Create > AnyRPG > Scriptable Content Template_.

![](<../.gitbook/assets/image (111).png>)

## Properties

| Name         | Description                                                                                                                                                                                                                                                                            |
| ------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Resources    | A list of links to scriptable objects that will be installed in a game when the wizard is used to install this template.  If the word 'Template' exists in their file name, it will be removed when they are installed.                                                                |
| Prefabs      | A list of links to prefabs that will be installed in a game when the wizard is used to install this template.  If the word 'Template' exists in their file name, it will be removed when they are installed.                                                                           |
| Dependencies | A list of links to other scriptable content templates that will be installed in a game when the wizard is used to install this template.  The use of dependencies is a convenience feature to allow re-using common sets of scriptable objects and prefabs between multiple templates. |

## Next Steps

* Use the _Template Content Wizard_, found under the _Menu Tools > AnyRPG > Wizard > Template Content Wizard_ to install template content in a new game.
