---
description: >-
  A knock back effect knocks the character away from the caster, sending them
  flying backwards in the air.
---

# Knock Back Effect

## Creation

To create a knock back effect, find (or create) the _GameName/Resources/GameName/AbilityEffect_ folder (or any subfolder) in the project tab and right click.  Choose _Create > AnyRPG > Abilities > Effects > KnockBackEffect_.

![](<../../.gitbook/assets/image (5) (1).png>)

## Properties

In addition to all the properties of its parent class, [Fixed Length Effect](knock-back-effect.md), knock back effects have the following properties.

| Name                | Description                                                                                                                                                                                                                                    |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Knockback Type      | <p>An enumeration of knockback types.<br><strong>Knockback</strong><br>The knockback direction will be calculated from the caster to the target.<br><strong>Explosion</strong><br>The knockback direction will be calculated from a point.</p> |
| Knock Back Velocity | The speed the character should be knocked back at.                                                                                                                                                                                             |
| Knock Back Angle    | The angle the character should be knocked upwards at.                                                                                                                                                                                          |
| Explosion Radius    | The radius from the center point point of the explosion where targets will be affected.                                                                                                                                                        |
| Explosion Force     | The amount of force to apply to targets of the explosion.                                                                                                                                                                                      |
| Upward Modifier     | The amount of upward force to apply to targets of the explosion.                                                                                                                                                                               |
| Explosion Mask      | The layers to hit when performing the explosion.                                                                                                                                                                                               |

## Next steps

* Add a knock back effect to an [Ability](../abilities/).
* Add a knock back effect to another [Ability Effect](./) to chain them together.
