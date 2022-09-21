---
description: >-
  A prefab profile contains a link to a Unity Prefab and information about how
  to position and scale it relative to its parent.
---

# Prefab Profile

## Creation

To create a prefab profile, find (or create) the _GameName/Resources/GameName/PrefabProfile_ folder in the project tab and right click.  Choose _Create > AnyRPG > PrefabProfile_.

![](../.gitbook/assets/image.png)

## Properties

| Name                        | Description                                                                                                                                           |
| --------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------- |
| Prefab                      | A link to a Unity Prefab to spawn.                                                                                                                    |
| Position                    | The Vector3 position of the _Prefab_ relative to its parent, when held (unsheathed).                                                                  |
| Rotation Is Global          | If true, the value in the _Rotation_ property will be considered global, rather than local (relative to the parent).                                  |
| Rotation                    | The Vector3 rotation of the _Prefab_ when held (unsheathed).                                                                                          |
| Scale                       | The Vector3 scale of the _Prefab_ relative to the parent when held (unsheathed).                                                                      |
| Target Bone                 | The GameObject in the hierarchy to attach the _Prefab_ to when held (unsheathed).                                                                     |
| Unsheath Audio Profile name | The name of an [Audio Profile](audio-profile.md) that contains a link to an audio clip to play when the _Prefab_ is moved to the unsheathed position. |
| Sheathed Position           | The Vector3 position of the _Prefab_ relative to its parent, when sheathed.                                                                           |
| Sheathed Rotation           | The Vector3 rotation of the _Prefab_ when sheathed.                                                                                                   |
| Sheathed Scale              | The Vector3 scale of the _Prefab_ relative to the parent when sheathed.                                                                               |
| Sheathed Target Bone        | The GameObject in the hierarchy to attach the _Prefab_ to when sheathed.                                                                              |
| Sheath Audio Profile Name   | The name of an [Audio Profile](audio-profile.md) that contains a link to an audio clip to play when the _Prefab_ is moved to the sheathed position.   |
| Use Item Pickup             | If true, the following values will be used for item pickups instead of the default (sheathed) values.                                                 |
| Pickup Position             | The Vector3 position of the _Prefab_ relative to its parent, when used as an item pickup.                                                             |
| Pickup Rotation             | The Vector3 rotation of the _Prefab_ when used as an item pickup.                                                                                     |
| Pickup Scale                | The Vector3 scale of the _Prefab_ relative to the parent when used as an item pickup.                                                                 |

## Next Steps

* Use prefab profile for an [Equipment](items/equipment.md) model.
* Use a prefab profile for a [Weapon](items/weapon.md) model.
* Use a prefab profile for an [Armor](items/armor.md) model.
* Use a prefab profile for a character model of a [Unit Profile](unit-profile.md).
* Use a prefab profile for a [Gathering Node](interactable-option-configurations/gathering-node-config.md).
* Use a prefab profile for a [Mount](ability-effects/mount-effect.md).
* Use a prefab profile for a [Projectile](ability-effects/projectile-effect.md).
* Use a prefab profile for a [Status Effect](ability-effects/status-effect.md).
* Use a prefab profile for a casting effect of an [Ability](abilities/).
