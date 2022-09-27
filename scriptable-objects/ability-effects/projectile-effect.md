---
description: >-
  A projectile effect spawns a projectile which moves toward a target, and casts
  subsequent effects when it hits the target.
---

# Projectile Effect

## Creation

To create a projectile effect, find (or create) the _GameName/Resources/GameName/AbilityEffect_ folder (or any subfolder) in the project tab and right click.  Choose _Create > AnyRPG > Abilities > Effects > ProjectileEffect_.

![](<../../.gitbook/assets/image (1).png>)

## Properties

In addition to all the properties of its parent class, [Fixed Length Effect](./#fixed-length-effect-properties), projectile effects have the following properties.

| Name                         | Description                                                                                                                               |
| ---------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------- |
| Projectile Speed             | The speed the projectile will travel while moving toward its target.                                                                      |
| Flight Audio Profile Names   | A list of [Audio Profiles](../audio-profile.md) containing audio clips to play while the projectile is traveling.                         |
| Random Flight Audio Profiles | If true, a random [Audio Profile](../audio-profile.md) from the _Flight Audio Profile Names_ list will be played, instead of all of them. |

## Next steps

* Add a projectile effect to an [Ability](../abilities/).
* Add a projectile effect to another [Ability Effect](./) to chain them together.
