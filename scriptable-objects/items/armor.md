---
description: >-
  Armor is wearable equipment that can have an armor class associated with it,
  optionally restricting who can wear it based on their known armor skills.
---

# Armor

## Creation

To create a faction, find (or create) the _GameName/Resources/GameName/Item/Equipment_ folder (or any subfolder of that folder) in the project tab and right click.  Choose _Create > AnyRPG > Inventory > Equipment > Armor_.

![](<../../.gitbook/assets/image (4) (1) (1).png>)

## Properties

In addition to the properties shared by all [Equipment](equipment.md), armor has the following unique properties.

| Name                | Description                                                                                                                           |
| ------------------- | ------------------------------------------------------------------------------------------------------------------------------------- |
| Require Armor Class | If true, this armor can only be equipped if the character knows the [Armor Class](../armor-class.md) in the _Armor Class Name_ field. |
| Armor Class Name    | The name of the [Armor Class](../armor-class.md) that this armor gets its armor properties from.                                      |

## Next Steps

* Configure a [Unit Profile](../unit-profile.md)'s _Equipment Name List_ to provide this armor to newly created characters.
* Configure a [Character Class](../character-class.md)' _Equipment Names_ list to provide this armor to newly created characters of that class.
* Configure a [Character Race](../character-race.md)'s _Equipment Names_ list to provide this armor to newly created characters of that race.
* Configure a [Class Specialization](../class-specialization.md)'s _Equipment Names_ list to provide this armor to a newly created characters of that specialization.
* Add armor to a [Loot Table](../loot-table.md) so that it can drop when an enemy is defeated.
* Add armor to a [Vendor Collection](../vendor-collection.md) and make it available on a vendor.
* Add armor to an [Equipment Set](../equipment-set.md) to give it unique set bonuses when one or more pieces of a set are equipped.
* Add armor as an output to a [Recipe](recipe.md) so that it can be crafted.
