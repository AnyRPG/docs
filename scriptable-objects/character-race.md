---
description: >-
  A character race gives characters access to abilities, traits, power
  resources, character stats, weapon skills, and armor skills.
---

# Character Race

## Creation

To create a character race, find (or create) the _GameName/Resources/GameName/CharacterRace_ folder in the project tab and right click.  Choose _Create > AnyRPG > CharacterRace_.

![](<../.gitbook/assets/image (109).png>)

## Properties

| Name                | Description                                                                                                                                                                                   |
| ------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Equipment Names     | A List of equipment that will be equipped by characters that choose the character class when starting a new game.                                                                             |
| Default Hit Effects | A list of [Ability Effects](ability-effects/) to cast on the target when the character does not have a [Weapon](items/weapon.md) equipped and does damage from a standard (auto) attack.      |
| On Hit Effects      | A list of [Ability Effects](ability-effects/) to cast on the target when the [Weapon](items/weapon.md) does damage from any attack, including standard (auto) attacks.                        |
| Capabilities        | Lists of abilities, traits, weapon skills, and armor skills the character class provides.  See [Capabilities](../shared-properties/capabilities.md) for descriptions.                         |
| Primary Stats       | A List of [Stat Scaling Nodes](../shared-properties/stat-scaling-nodes.md) that define primary stat budgets per level and secondary stats and power resources granted by those primary stats. |
| Power Resources     | A list of [Power Resources](power-resource.md) the character will have access to.                                                                                                             |

## Next Steps

* Assign a character race to a [Unit Profile](unit-profile.md).
