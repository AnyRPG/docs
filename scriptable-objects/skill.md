---
description: A skill allows you to learn abilities that let you gather or craft items.
---

# Skill

## Creation

To create a skill, find (or create) the _GameName/Resources/GameName/Recipe_ folder in the project tab and right click.  Choose _Create > AnyRPG > Skills > Skill_.

![](<../.gitbook/assets/image (1) (2) (2) (1).png>)

## Properties

| Name           | Description                                                                                                                                                                                                                                                            |
| -------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Required Level | The minimum level which the character must reach to learn this skill.                                                                                                                                                                                                  |
| Auto Learn     | If true, this skill will be automatically learned upon reaching the _Required Level_.                                                                                                                                                                                  |
| Ability Names  | A list of [Abilities](abilities/) that will be learned when the skill is learned.  These should generally be [Gathering Abilities](abilities/gather-ability.md) or [Crafting Abilities](abilities/craft-ability.md), but that is a suggestion, not a hard requirement. |

## Next Steps

* Add a skill as a reward for completing a [Quest](quest.md).
* Add a skill to a [Skill Trainer](interactable-option-configurations/skill-trainer-config.md) so the trainer can teach it.
