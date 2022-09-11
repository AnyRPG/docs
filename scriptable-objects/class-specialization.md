---
description: >-
  A class specialization gives characters access to abilities, traits, power
  resources, character stats, weapon skills, and armor skills.
---

# Class Specialization

## Creation

To create a class specialization, find (or create) the _GameName/Resources/GameName/ClassSpecialization_ folder in the project tab and right click.  Choose _Create > AnyRPG > CharacterClassSpecialization_.

![](<../.gitbook/assets/image (127).png>)

## Properties

| Name                 | Description                                                                                                                                                                                                 |
| -------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| New Game Option      | If true, the class specialization can be chosen for new characters when starting a new game.                                                                                                                |
| Equipment Names      | A list of [Equipment](items/equipment.md) that will be equipped by characters that choose the character class when starting a new game.                                                                     |
| Class Names          | A list of [Character Class](character-class.md) names.  The character must be one of the classes in the list to choose the class specialization.                                                            |
| Capabilities         | Lists of [Abilities](abilities/), traits, [Weapon Skills](weapon-skill.md), and armor skills the class specialization provides.  See [Capabilities](../shared-properties/capabilities.md) for descriptions. |
| Primary Stats        | A List of [Stat Scaling Nodes](../shared-properties/stat-scaling-nodes.md) that define primary stat budgets per level and secondary stats and power resources granted by those primary stats.               |
| Power Resources      | A list of [Power Resources](power-resource.md) the character will have access to.                                                                                                                           |
| Power Enhancer Stats | Deprecated.  No longer in use.                                                                                                                                                                              |
| Valid Pet Types      | A list of [Unit Types](unit-type.md) the character can keep as pets.  This property will only be used if the character has an ability that allows them to capture a pet.                                    |

## Next Steps

* Enable Character Class Specialization selection in the System Configuration Manager of a game.
