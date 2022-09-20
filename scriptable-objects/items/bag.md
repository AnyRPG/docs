---
description: >-
  A bag is a type of item that can expand a player's inventory space or bank
  space when equipped.
---

# Bag

## Creation

To create a bag, find (or create) the _GameName/Resources/GameName/Item_ folder (or any subfolder) in the project tab and right click.  Choose _Create > AnyRPG > Inventory > Items > Bag_.

![](<../../.gitbook/assets/image (4).png>)

## Properties

In addition to the properties shared by all [Items](./), bags have the following unique properties.

| Name  | Description                                                                                 |
| ----- | ------------------------------------------------------------------------------------------- |
| Slots | The number of spaces the inventory (or bank) will be expanded by when this bag is equipped. |

## Next Steps

* Configure the _Default Backpack Item_ field in the System Configuration Manager of a game to make this bag the default backpack for a new player.
* Add a bag to a [Vendor Collection](../vendor-collection.md) so it can be purchased from a [Vendor](../interactable-option-configurations/vendor-config.md).
* Add a bag to a [Loot Table](../loot-table/) so that it can drop upon defeat of an enemy.
* Add a bag as an output of a [Recipe](recipe.md) so it can be crafted.
