---
description: Items are objects that can be placed in the character inventory.
---

# Items

## Creation

To create an item, find (or create) the _GameName/Resources/GameName/Item_ folder in the project tab and right click.  Choose _Create > AnyRPG > Inventory > Item_.

![](<../../.gitbook/assets/image (128).png>)

## Properties

| Name                             | Description                                                                                                                                                                                                                                              |
| -------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Stack Size                       | The number of this type of item that can fit in a single inventory slot.                                                                                                                                                                                 |
| Item Quality                     | The quality of the item. See [Item Quality](../item-quality.md).                                                                                                                                                                                         |
| Random Item Quality              | If true, this item will be assigned a random item quality when purchased, crafted, or looted.                                                                                                                                                            |
| Dynamic Level                    | If true, This item will scale in level so that it is the same level as the character.                                                                                                                                                                    |
| Freeze Drop Level                | If true, and the item also has dynamic level set to true, the item level will be frozen at whatever level it was when purchased, crafted, or looted.                                                                                                     |
| Level Cap                        | For dynamic level items, the maximum level it can scale up to.  0 means no limit.                                                                                                                                                                        |
| Item Level                       | If the item is not dynamic level, then it will be fixed at this level.                                                                                                                                                                                   |
| Use Level                        | The level that the character has to be to use this item.  This field does not apply to items that have no direct use, such as crafting ingredients.                                                                                                      |
| Currency Name                    | The currency that is required to purchase the item.  See [Currency](../currency.md).                                                                                                                                                                     |
| Dynamic Currency Amount          | If true, the purchase and sale price will scale with level.                                                                                                                                                                                              |
| Price Per Level                  | If dynamic currency amount is true, this is the amount per level this item will cost.                                                                                                                                                                    |
| Base Price                       | The base item price.  If dynamic currency amount is true, this price is added to the dynamic price.                                                                                                                                                      |
| Unique Item                      | If true, the character cannot have more than one of these items in their inventory or bank.                                                                                                                                                              |
| Character Class Requirement List | If this list is not empty, the character must be one of the listed character classes to use or equip this item, and for the item to be dropped if the loot table is configured to match this restriction.  See [Character Class](../character-class.md). |
