---
description: A recipe item is an item that reaches the player a recipe when used.
---

# Recipe Item

## Creation

To create a recipe item, find (or create) the _GameName/Resources/GameName/Item_ folder (or any subfolder) in the project tab and right click.  Choose _Create > AnyRPG > Inventory > Items > RecipeItem_.

![](<../../.gitbook/assets/image (1) (2) (1).png>)

## Properties

In addition to the properties shared by all [Items](./), recipe items have the following unique properties.

| Name        | Description                                                       |
| ----------- | ----------------------------------------------------------------- |
| Recipe Name | The name of a [Recipe](recipe.md) to learn when the item is used. |

## Next Steps

* Add a recipe item to a [Vendor Collection](../vendor-collection.md) so it can be purchased from a [Vendor](../interactable-option-configurations/vendor-config.md).
* Add a recipe item to a [Loot Table](../loot-table.md) so that it can drop upon defeat of an enemy.
