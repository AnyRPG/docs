---
description: >-
  A direct effect is a type of intermediate effect that can be used to chain
  multiple effects together.
---

# Direct Effect

## Creation

To create a direct effect, find (or create) the _GameName/Resources/GameName/AbilityEffect_ folder (or any subfolder) in the project tab and right click.  Choose _Create > AnyRPG > Abilities > Effects > DirectEffect_.

![](<../../.gitbook/assets/image (1) (1).png>)

### Properties

Direct Effects do not have any properties other than the properties provided by their parent class, [Fixed Length Effect](./#fixed-length-effect-properties).

## Usage

Direct Effects will cast Tick Ability Effects, and Complete Ability Effects, but will never cast Hit Ability Effects.  Hit Abilty Effects will be cast by [Projectile Effects](projectile-effect.md), [AOE Effects](aoe-effect.md), and [Channeled Effects](channeled-effect.md).

## Next steps

* Add a direct effect to an [Ability](../abilities/).
* Add a direct effect to another [Ability Effect](./) to chain them together.
