---
description: >-
  A currency item is an item that provides a specific amount of a specific
  currency to a player when used.
---

# Currency Item

## Creation

To create a currency item, find (or create) the _GameName/Resources/GameName/Item_ folder (or any subfolder) in the project tab and right click.  Choose _Create > AnyRPG > Inventory > Items > Currency Item_.

![](<../../.gitbook/assets/image (2) (1) (2) (1).png>)

## Properties

In addition to the properties shared by all [Items](./), currency items have the following unique properties.

| Name                 | Description                                                                |
| -------------------- | -------------------------------------------------------------------------- |
| Gain Currency Name   | The name of the [Currency](../currency.md) that will be gained upon use.   |
| Gain Currency Amount | The amount of the [Currency](../currency.md) that will be gained upon use. |

## Next Steps

* Add a currency item to a [Vendor Collection](../vendor-collection.md) so it can be purchased from a [Vendor](../interactable-option-configurations/vendor-config.md).
* Add a currency item to a [Loot Table](../loot-table.md) so that it can drop upon defeat of an enemy.

