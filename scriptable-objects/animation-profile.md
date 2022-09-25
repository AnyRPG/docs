---
description: >-
  An animation profile stores a list of animations for re-use in unit prefab
  properties or weapons.
---

# Animation Profile

{% embed url="https://youtu.be/alKWYpFfJeI" %}

## Creation

To create an animation profile, find (or create) the _GameName/Resources/GameName/AnimationProfile_ folder in the project tab and right click.  Choose _Create > AnyRPG > Animation > Profile_.

![](<../.gitbook/assets/image (116) (1).png>)

## Properties

| Name                           | Description                                                                                                                                                                                                                                                   |
| ------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Use Root Motion                | If true, root motion will be enabled on the character while the animation is playing, causing the player to move according to the position data in the animation.                                                                                             |
| Suppress Adjust Animator Speed | If true, the animations will play at their default speed no matter the movement speed or casting speed of the character being animated.                                                                                                                       |
| Attack Clips                   | A list of possible animations to play when the character is performing attacks that do not have their own animation profile assigned.  If this animation profile is assigned to a special animated attack, then the list will only be applied to that attack. |
| Cast Clips                     | A list of possible animations to play when the character is casting spells that do not have their own animation profile assigned.  If this animation profile is assigned to a specific spell, then the list will only be applied to that spell.               |
| Take Damage Clips              | Not yet implemented.                                                                                                                                                                                                                                          |
| Out Of Combat Movement         | Animations to play when the character not in combat.                                                                                                                                                                                                          |
| Full Combat Mirror             | If true, the character will use the out of combat animations when they are in combat.  This can be useful if a character has no specific in-combat animations included.                                                                                       |
| \<Animation Name> Mirror       | Each combat animation can instead use an out of combat animation if these boxes are true.  This setting is useful when a character only includes a partial set of combat animations.                                                                          |
| Combat \<Animation Name> Clip  | An animation clip to play for a specific state when in combat.                                                                                                                                                                                                |
| Death Clip                     | An animation clip to play when the character dies.                                                                                                                                                                                                            |
| Revive Clip                    | An animation clip to play when the character is being revived from dead.                                                                                                                                                                                      |
| Levitated Clip                 | An animation clip to play when the character is being levitated off the ground.                                                                                                                                                                               |
| Swim Idle Clip                 | An animation clip to play when the character is in the water and not moving.                                                                                                                                                                                  |
| Swim Move Clip                 | An animation clip to play when the character is in the water and moving.                                                                                                                                                                                      |
| Fly Idle Clip                  | An animation clip to play when the character is flying, but not moving.                                                                                                                                                                                       |
| Fly Move Clip                  | An animation clip to play when the character is flying, and moving.                                                                                                                                                                                           |

## Configuration

Not all available animations need to be assigned since any animation profile used for a character or weapon will only override the base animation profile in use.

If this animation profile will be used for an animated attack, the animation(s) should be placed in the _Attack Clips_ list.

If this animation profile will be used for an ability (spell) the animation(s) should be placed in the _Cast Clips_ list.

## Next Steps

* Assign the animation profile to a [Weapon](items/weapon.md) to override the movement and auto-attack animations used while that weapon is equipped.
* Assign the animation profile to a [Weapon Skill](weapon-skill.md) to override the movement and auto-attack animations for any weapon with that weapon skill assigned while equipped.
* Assign the animation profile to an [Animated Ability](abilities/animated-ability.md) to use the Attack Clips for the attack animations.
* Assign the animation profile to an [Ability](abilities/) to use the Cast Clips for casting animations.
* Assign the animation profile to a [Unit Prefab Profile](unit-prefab-profile.md), or _Unit Prefab Properties_ on a [Unit Profile](unit-profile.md) to override the default system animations for that character.
