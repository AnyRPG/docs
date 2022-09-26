---
description: >-
  An attack effect does damage to a target, draining one or more power
  resources.
---

# Attack Effect

## Creation

To create an attack effect, find (or create) the _GameName/Resources/GameName/AbilityEffect_ folder (or any subfolder) in the project tab and right click.  Choose _Create > AnyRPG > Abilities > Effects > AttackEffect_.

![](<../../.gitbook/assets/image (3) (5).png>)

### Properties

In addition to all the properties of its parent class, [Amount Effect](./#amount-effect-properties), attack effects have the following properties.

| Name                 | Description                                                                                                                                                                                                                                                                       |
| -------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Weapon Attack        | If true, this attack will be considered to have been landed by the equipped [Weapon](../items/weapon.md).  It will play [Weapon](../items/weapon.md) sounds, as well as trigger [Weapon](../items/weapon.md) effects and active [Status Effect](status-effect.md) on-hit effects. |
| Damage Type          | <p>An enumeration of damage types.<br><strong>Physical</strong><br><a href="../items/weapon.md">Weapon</a> damage and physical power will be added to the damage amounts.<br><strong>Ability</strong><br>Spell power will be added to the damage amounts.</p>                     |
| Ignore Armor Percent | If the _Damage Type_ is _Physical_, the percentage of the target armor to ignore when dealing damage.                                                                                                                                                                             |

## Next steps

* Add an attack effect to an [Ability](../abilities/).
* Add an attack effect to another [Ability Effect](./) to chain them together.
