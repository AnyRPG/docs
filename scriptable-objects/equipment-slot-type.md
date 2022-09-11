---
description: >-
  An equipment slot type is an abstraction that allows the user to define
  multiple physical equipment slots that equipment can be equipped in.
---

# Equipment Slot Type

## Creation

To create an equipment set, find (or create) the _GameName/Resources/GameName/EquipmentSlotType_ folder in the project tab and right click.  Choose _Create > AnyRPG > Equipment> EquipmentSlotType_.

![](<../.gitbook/assets/image (105).png>)



## Properties

| Name                    | Description                                                                                                                        |
| ----------------------- | ---------------------------------------------------------------------------------------------------------------------------------- |
| Stat Weight             | A weighted value to control distribution of [Stats](character-stat.md) among gear.                                                 |
| Exclusive Slot Profiles | A list of [Equipment Slot Profiles](equipment-slot-profile.md) that will be unequipped if equipment of this slot type is equipped. |
| Exclusive Slot Types    | A list of equipment slot types that will be unequipped if equipment of this slot type is equipped.                                 |

## Next Steps

* Assign an equipment slot type to a piece of [Equipment](items/equipment.md).
