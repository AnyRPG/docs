---
description: >-
  An aoe effect is a type of intermediate effect that is responsible for
  choosing multiple valid targets and casting any additional ability effects on
  them.
---

# AOE Effect

## Creation

To create an aoe effect, find (or create) the _GameName/Resources/GameName/AbilityEffect_ folder (or any subfolder) in the project tab and right click.  Choose _Create > AnyRPG > Abilities > Effects > AOEEffect_.

![](../../.gitbook/assets/image.png)

### Properties

In addition to all the properties of its parent class, [Fixed Length Effect](./#fixed-length-effect-properties), aoe effects have a single property, _AOE Properties_, with the following fields.

| Name                   | Description                                                                                                                                 |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- |
| Aoe Radius             | The radius from the center of the target location which will be used to find valid targets.                                                 |
| Use Radius             | If true, the target finding algorithm will use a sphere with a radius to find targets.                                                      |
| Use Extents            | If true, the target finding algorithm will use extents to find targets.                                                                     |
| Aoe Center             | A Vector3 offset from the default center to use for finding targets.                                                                        |
| Aoe Extents            | If _Use Extents_ is true, then these extents will be used to create the bounding box to find valid targets within it.                       |
| Max Targets            | The maximum number of valid targets that can be returned.  0 is unlimited.                                                                  |
| Prefer Closest Targets | If true, and _Max Targets_ is not unlimited, the targets will be sorted by distance from the center, and the closest ones will be returned. |
| Inter Target Delay     | Set this value to a positive non-zero number if you want a delay between the time each target has additional effects cast on them.          |

## Next steps

* Add an aoe effect to an [Ability](../abilities/).
* Add an aoe effect to another [Ability Effect](./) to chain them together.
