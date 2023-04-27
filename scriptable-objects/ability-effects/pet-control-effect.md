---
description: >-
  A pet control effect is a special type of status effect that ensures that a
  character will automatically summon a pet whenever it does not have an active
  pet.
---

# Pet Control Effect

## Creation

To create a pet control effect, find (or create) the _GameName/Resources/GameName/AbilityEffect_ folder (or any subfolder) in the project tab and right click.  Choose _Create > AnyRPG > Abilities > Effects > PetControlEffect_.

![](<../../.gitbook/assets/image (3) (1) (4).png>)

## Properties

In addition to all the properties of its parent class, [Status Effect](status-effect.md), pet control effects have the following properties.

| Name             | Description                                              |
| ---------------- | -------------------------------------------------------- |
| Pet Effect Names | A list of [Pet Effects](pet-effect.md) that summon pets. |

## Next steps

* Add a pet control effect to an [Ability](../abilities/).
* Add a pet control effect to another [Ability Effect](./) to chain them together.
