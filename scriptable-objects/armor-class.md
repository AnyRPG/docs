---
description: >-
  An armor class defines how much armor equipment should receive, and optionally
  who can wear the equipment.
---

# Armor Class

{% embed url="https://youtu.be/m75PRa63AFI" %}

## Creation

To create an armor class, find (or create) the _GameName/Resources/GameName/ArmorClass_ folder in the project tab and right click.  Choose _Create > AnyRPG > ArmorClass_.

![](<../.gitbook/assets/image (105) (1).png>)

## Properties

| Name            | Description                                                                                                                                                                                                                                                   |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Armor Per Level | <p>The total amount of armor value provided per level if all equipment slots have armor of this type equipped.<br>The formula per piece of equipment is:<br><code>Item Level * Armor Per Level * Item Quality Multiplier * (1 / Total Armor Slots)</code></p> |

## Next Steps

* Create [Armor](items/armor.md) and assign this armor class to it.
* Configure a [Character Class](character-class.md) to be able to equip gear with this armor class assigned.
* Configure a [Character Race](character-race.md) to be able to equip gear with this armor class assigned.
* Configure a [Class Specialization](class-specialization.md) to be able to equip gear with this armor class assigned.
* Directly Configure a specific [Unit Profile](unit-profile.md) to be able to equip gear with this armor class assigned.
* Configure a [Unit Type](unit-type.md) to be able to equip gear with this armor class assigned.
* Configure the Game Manager for your game so that all characters can equip gear with this armor class assigned.
