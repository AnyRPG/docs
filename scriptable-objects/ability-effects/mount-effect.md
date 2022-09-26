---
description: A mount effect allows a character to summon and ride a mount.
---

# Mount Effect

## Creation

To create an attack effect, find (or create) the _GameName/Resources/GameName/AbilityEffect_ folder (or any subfolder) in the project tab and right click.  Choose _Create > AnyRPG > Abilities > Effects > MountEffect_.

![](<../../.gitbook/assets/image (1).png>)

### Properties

In addition to all the properties of its parent class, [Status Effect](status-effect.md), mount effects have the following properties.

| Name              | Description                                                        |
| ----------------- | ------------------------------------------------------------------ |
| Unit Profile Name | A [Unit Profile](../unit-profile.md) that will serve as the mount. |

## Next steps

* Add a mount effect to an [Ability](../abilities/).
* Add a mount effect to another [Ability Effect](./) to chain them together.
