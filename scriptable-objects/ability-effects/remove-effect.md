---
description: A remove effect removes a status effect from the target.
---

# Remove Effect

## Creation

To create a remove effect, find (or create) the _GameName/Resources/GameName/AbilityEffect_ folder (or any subfolder) in the project tab and right click.  Choose _Create > AnyRPG > Abilities > Effects > RemoveEffect_.

![](<../../.gitbook/assets/image (2) (1) (1).png>)

## Properties

In addition to all the properties of its parent class, [Fixed Length Effect](./#fixed-length-effect-properties), remove effects have the following properties.

| Name              | Description                                                                            |
| ----------------- | -------------------------------------------------------------------------------------- |
| Max Clear Effects | The maximum amount of [Status Effects](status-effect.md) to remove. 0 is unlimited.    |
| Effect Type Names | A list of [Status Effect Types](../status-effect-type.md) that this effect can remove. |

## Next steps

* Add a remove effect to an [Ability](../abilities/).
* Add a remove effect to another [Ability Effect](./) to chain them together.
