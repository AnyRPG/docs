---
description: >-
  A channeled effect is a type of intermediate effect that is responsible for
  delaying the cast of subsequent effects.
---

# Channeled Effect

## Creation

To create a channeled effect, find (or create) the _GameName/Resources/GameName/AbilityEffect_ folder (or any subfolder) in the project tab and right click.  Choose _Create > AnyRPG > Abilities > Effects > ChanneledEffect_.

![](<../../.gitbook/assets/image (14).png>)

### Properties

In addition to all the properties of its parent class, [Fixed Length Effect](./#fixed-length-effect-properties), channeled effects have the following properties.

| Name         | Description                                                                                                                      |
| ------------ | -------------------------------------------------------------------------------------------------------------------------------- |
| Effect Delay | The delay, in seconds, that should pass after spawning the visual effects, before any subsequent [Ability Effects](./) are cast. |

## Next steps

* Add a channeled effect to an [Ability](../abilities/).
* Add a channeled effect to another [Ability Effect](./) to chain them together.
