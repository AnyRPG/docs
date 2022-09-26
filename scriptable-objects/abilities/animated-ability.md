---
description: >-
  An animated ability is an attack-type ability, where the damage to the target
  should occur in the middle of the animation, based on animation events.
---

# Animated Ability

## Creation

To create an animated ability, find (or create) the _GameName/Resources/GameName/BaseAbility_ folder (or any subfolder) in the project tab and right click.  Choose _Create > AnyRPG > Abilities > AnimatedAbility_.

![](<../../.gitbook/assets/image (2).png>)

## Properties

| Name                       | Description                                                                                                                                                                                 |
| -------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Is Auto Attack             | If true, this ability will be used as an auto-attack, and automatically cast on an enemy target when in combat and in range.                                                                |
| Use Unit Attack Animations | If true, the _Attack Clips_ will be used from the currently active [Animations](../animation-profile.md) for the character, instead of any animation clips defined directly in the ability. |
| Use Auto Attack Animations | This option is only valid if this is not an auto-attack ability.  If true, it will use the current auto-attack animations so it looks good with any weapon.                                 |
| Use Weapon Hit Sound       | If true, the current Weapon default hit sound will be played when the attack hits an enemy.                                                                                                 |

## Next steps

* Add an animated ability to the _Capabilities_ of a [Character Class](../character-class.md).
* Add an animated ability to the _Capabilities_ of a [Class Specialization](../class-specialization.md).
* Add an animated ability to the _Capabilities_ of a [Unit Type](../unit-type.md).
* Add an animated ability to the _Capabilities_ of a [Faction](../faction.md).
* Add an animated ability to the _Capabilities_ of a [Unit Profile](../unit-profile.md).
