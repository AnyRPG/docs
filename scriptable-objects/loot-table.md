---
description: >-
  A loot table is a list of items that can drop from any lootable source such as
  characters, item pickups, and gathering nodes.
---

# Loot Table

## Creation

To create a loot table, find (or create) the _GameName/Resources/GameName/LootTable_ folder in the project tab and right click.  Choose _Create > AnyRPG > LootTable_.

![](<../.gitbook/assets/image (99).png>)



## Properties

| Name                     | Description                                                                                                                                                                                                                                                             |
| ------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Ignore Global Drop Limit | Any lootable source can have a global limit on the number of items dropped, no matter how many loot tables it has.  If this option is true, that limit will be ignored, and the drop limit from this loot table will be used instead when rolling loot from this table. |
| Drop Limit               | If _Ignore Global Drop Limit_ is true, this number will be the limit of the number of [Items](items/) dropped from this table.                                                                                                                                          |
| Loot Groups              | A list of [Loot Groups](loot-table.md#properties-1) that shares drop chance and limit settings.                                                                                                                                                                         |

### Loot Groups

| Name                     | Description                                                                                                                                               |
| ------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Guaranteed Drop          | If true, the number of [Items](items/) defined in the _Drop Limit_ field for this group will be guaranteed to drop, using their _Drop Chance_ as weights. |
| Group Chance             | The chance this group will attempt to drop [Items](items/).                                                                                               |
| Drop Limit               | The amount of [Items](items/) that can drop from this list.  0 is unlimited.                                                                              |
| Unique Limit             | The limit to the number of times the same [Item](items/) can drop.  0 is unlimited.                                                                       |
| Ignore Global Drop Limit | If true, the [Items](items/) on this list will ignore any parent drop limits.                                                                             |
| Loot                     | A list of [Items](items/) that can drop.                                                                                                                  |

#### Loot

| Name                    | Description                                                                                                                                                                                    |
| ----------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Item Name               | The name of an [Item](items/) that can drop.                                                                                                                                                   |
| Drop Chance             | The percentage chance that this [Item](items/) can drop.                                                                                                                                       |
| Min Drops               | The minimum number of this [Item](items/) that will drop.                                                                                                                                      |
| Max Drops               | The maximum number of this [Item](items/) that will drop.                                                                                                                                      |
| Match Item Restrictions | If true, [Character Class](character-class.md) restrictions on the item must match for it to drop.  This is useful to prevent items from dropping that do no match the player's current class. |
| Prerequisite Conditions | A list of [Prerequisite Conditions](../shared-properties/prerequisite-conditions.md) that must be met for this item to drop.                                                                   |

## Next Steps

* Add a loot table to a [Unit Profile](unit-profile.md).
* Add a loot table to Gathering Node.
* Add a loot table to an Item Pickup.
* Add a loot table to a [Scene Node](scene-node.md).
