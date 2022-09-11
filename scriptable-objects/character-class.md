---
description: >-
  A character class gives characters access to abilities, traits, power
  resources, character stats, weapon skills, and armor skills.
---

# Character Class

## Creation

To create a character class, find (or create) the _GameName/Resources/GameName/CharacterClass_ folder in the project tab and right click.  Choose _Create > AnyRPG > CharacterClass_.

![](<../.gitbook/assets/image (131).png>)

## Properties

| Name                   | Description                                                                                                                                                                                   |
| ---------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| New Game Option        | If true, the character class can be chosen for new characters when starting a new game.                                                                                                       |
| Equipment Names        | A List of equipment that will be equipped by characters that choose the character class when starting a new game.                                                                             |
| Capabilities           | Lists of abilities, traits, weapon skills, and armor skills the character class provides.  See [Capabilities](../shared-properties/capabilities.md) for descriptions.                         |
| Unit Type Capabilities | Lists of [Unit Types](unit-type.md) and corresponding [Capabilities](../shared-properties/capabilities.md).  Use this property to restrict certain capabilities to specific unit types.       |
| Primary Stats          | A List of [Stat Scaling Nodes](../shared-properties/stat-scaling-nodes.md) that define primary stat budgets per level and secondary stats and power resources granted by those primary stats. |
| Power Resources        | A list of [Power Resources](power-resource.md) the character will have access to.                                                                                                             |
| Valid Pet Types        | A list of [Unit Types](unit-type.md) the character can keep as pets.  This property will only be used if the character class has an ability that allows them to capture a pet.                |

## Next Steps

* Enable Character Class selection in the System Configuration Manager of a game.
