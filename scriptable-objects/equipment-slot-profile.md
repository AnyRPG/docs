---
description: >-
  An equipment slot profile defines a physical slot that equipment can be placed
  in when equipped on a character. Most games will probably not need to adjust
  these.
---

# Equipment Slot Profile

## Creation

To create an equipment set, find (or create) the _GameName/Resources/GameName/EquipmentSlotProfile_ folder in the project tab and right click.  Choose _Create > AnyRPG > Equipment> EquipmentSlot_.

![](<../.gitbook/assets/image (101).png>)



## Properties

| Name                     | Description                                                                                                                          |
| ------------------------ | ------------------------------------------------------------------------------------------------------------------------------------ |
| Main Weapon Slot         | If true, the icon from any [Item](items/) equipped in this slot will be used for auto-attack [Abilities](abilities/) on action bars. |
| Stat Weight              | A weighted value to control distribution of [Stats](character-stat.md) among gear.                                                   |
| Equipment Slot Type List | A list of [Equipment Slot Types](equipment-slot-type.md) that can be equipped in this physical slot.                                 |
| Set On Hit Audio         | If true, items in this list will set on-hit audio sounds if they have one.  This is mostly useful for weapon slots.                  |

## Next Steps

* If new equipment slot profiles are defined, a custom UI will need to be created that will display the new slots.
