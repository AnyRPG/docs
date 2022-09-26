---
description: >-
  A capture pet effect captures a pet, allowing the caster to call it to follow
  them and aid them in combat at any time.
---

# Capture Pet Effect

## Creation

To create a capture pet effect, find (or create) the _GameName/Resources/GameName/AbilityEffect_ folder (or any subfolder) in the project tab and right click.  Choose _Create > AnyRPG > Abilities > Effects > CapturePetEffect_.

![](<../../.gitbook/assets/image (13).png>)

### Properties

In addition to all the properties of its parent class, [Fixed Length Effect](./#fixed-length-effect-properties), capture pet effects have the following properties.

| Name                   | Description                                                              |
| ---------------------- | ------------------------------------------------------------------------ |
| Unit Type Restrictions | A list of [Unit Types](../unit-type.md) that the ability can be cast on. |

## Next steps

* Add a capture pet effect to an [Ability](../abilities/).
* Add a capture pet effect to another [Ability Effect](./) to chain them together.
