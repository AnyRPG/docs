---
description: >-
  A power resource is any resource a character can use to cast abilities.  This
  includes health, since it is possible to configure an ability to use up health
  upon casting.
---

# Power Resource

## Creation

To create a power resource, find (or create) the _GameName/Resources/GameName/PowerResource_ folder in the project tab and right click.  Choose _Create > AnyRPG > PowerResource_.

![](<../.gitbook/assets/image (1) (1).png>)



## Properties

| Name                    | Description                                                                                                                                                        |
| ----------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Display Color           | A color that will be used when displaying this resource in unit frames.                                                                                            |
| Base Amount             | A base amount that all characters with this resource will receive.                                                                                                 |
| Amount Per Level        | Every character with this resource will have their maximum amount increased by this much for every level they gain.                                                |
| Tick Rate               | The number of seconds that should elapse between each regeneration of this resource.                                                                               |
| Amount Per Tick         | When not in combat and regeneration occurs, this amount will be restored (or used if the value is negative).                                                       |
| Percent Per Tick        | When not in combat and regeneration occurs, this percentage of the maximum possible current value will be restored.                                                |
| Combat Amount Per Tick  | When in combat and regeneration occurs, this amount will be restored (or used if the value is negative).                                                           |
| Combat Percent Per Tick | When in combat and regeneration occurs, this percentage of the maximum possible current value will be restored.                                                    |
| Maximum Amount          | If this amount is greater than zero, the resource has a fixed maximum amount that will not change based on character level.                                        |
| Is Health               | If true, this is considered to be a health resource.  When all of a character's health resources reach zero, they will die. Multiple health resources are allowed. |
| Fill On Reset           | If true, when the character evades, levels up, or spawns, this resource will be filled to its maximum amount.                                                      |

## Next Steps

* Assign a power resource to a [Unit Profile](unit-profile.md).
* Assign a power resource to a [Character Class](character-class.md).
* Assign a power resource to a [Class Specialization](class-specialization.md).
* Assign a power resource to a [Unit Type](unit-type.md).
* Assign a power resource to a [Character Race](character-race.md).
* Assign a power resource to the System Configuration Manager, making it globally available to all characters.
