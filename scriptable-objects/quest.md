---
description: >-
  A quest is a type of mission that a player can undertake in order to complete
  objectives to gain experience, currency, or other types of rewards.
---

# Quest

## Creation

To create a quest, find (or create) the _GameName/Resources/GameName/Quest_ folder in the project tab and right click.  Choose _Create > AnyRPG > Quests > Quest_.

![](<../.gitbook/assets/image (2) (2).png>)

## Properties

| Name                        | Description                                                                                                                                                                                                                                                                                                                                                            |
| --------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Is Achievement              | If true, this quest will be automatically tracked invisibly without appearing in the quest log, and appear in the achievements UI window when complete.                                                                                                                                                                                                                |
| Repeatable Quest            | If true, the quest can be accepted and completed more than once.                                                                                                                                                                                                                                                                                                       |
| Has Opening Dialog          | If true, a Dialog with the same name as the quest will be used (if found) and will be required to be completed before the quest can be accepted.                                                                                                                                                                                                                       |
| Experience Level            | The level that is considered appropriate for the quest. This value is used to calculate experience reward reduction if the player is a higher level than this value.                                                                                                                                                                                                   |
| Dynamic Level               | If true, the quest will always be considered to be the same level as the player.                                                                                                                                                                                                                                                                                       |
| Extra Levels                | If dynamic level is true, this value can be used to make the quest a higher level than the player.                                                                                                                                                                                                                                                                     |
| Base Experience Reward      | The base experience for the quest, not scaled by level, and in addition to any automatic quest xp configured at the game level (in the System Configuration Manager).                                                                                                                                                                                                  |
| Experience Reward Per Level | The experience for the quest, scaled by level, and in addition to any automatic quest xp configured at the game level (in the System Configuration Manager).                                                                                                                                                                                                           |
| Automatic Currency Reward   | If true, the quest will reward [Currency](currency.md) based on the system quest currency reward settings (in the System Configuration Manager).                                                                                                                                                                                                                       |
| Reward Currency Name        | The name of a [Currency](currency.md) that will be rewarded to the player when the quest is complete.                                                                                                                                                                                                                                                                  |
| Base Currency Reward        | The base [Currency](currency.md) reward for the quest, not scaled by level, and in addition to any automatic currency reward configured at the game level (in the System Configuration Manager).                                                                                                                                                                       |
| Currency Reward Per Level   | The [Currency](currency.md) rewarded for completing the quest, scaled by level, and in addition to any automatic [Currency](currency.md) reward configured at the game level (in the System Configuration Manager).                                                                                                                                                    |
| Max Item Rewards            | The maximum number of [Item](items/) rewards that can be chosen, if there is more than one possible [Item](items/) reward.                                                                                                                                                                                                                                             |
| Item Reward Names           | The names of [Items](items/) that will be given as rewards for completing the quest.                                                                                                                                                                                                                                                                                   |
| Max Faction Rewards         | The maximum number of [Faction](faction.md) rewards that can be chosen, if there is more than one possible [Faction](faction.md) reward.                                                                                                                                                                                                                               |
| Faction Rewards             | <p>A list of <a href="faction.md">Faction</a> names and values that will be given as rewards for completing the quest.<br><strong>Faction Name</strong><br>The name of the <a href="faction.md">Faction</a> whom the player will receive increased reputation with.<br><strong>Reputation Amount</strong><br><strong></strong>The amount of reputation to receive.</p> |
| Max Ability Rewards         | The maximum number of [Ability](abilities/) rewards that can be chosen, if there is more than one possible [Ability](abilities/) reward.                                                                                                                                                                                                                               |
| Ability Reward Names        | The names of [Abilities](abilities/) that will be given as rewards for completing the quest.                                                                                                                                                                                                                                                                           |
| Max Skill Rewards           | The maximum number of [Skill](skill.md) rewards that can be chosen, if there is more than one possible [Skill](skill.md) reward.                                                                                                                                                                                                                                       |
| Skill Reward Names          | The names of [Skills](skill.md) that will be given as rewards for completing the quest.                                                                                                                                                                                                                                                                                |
| Steps                       | A list of steps, with [Objectives](quest.md#undefined) for each step, that must be completed in order to finish the quest.                                                                                                                                                                                                                                             |
| Prerequisite Conditions     | A list of [Prerequisite Conditions](../shared-properties/prerequisite-conditions.md) that must be met to start the quest.                                                                                                                                                                                                                                              |
| Turn In Items               | If true, any items that are part of an Item Objective will be removed from the player inventory when the quest is turned in.                                                                                                                                                                                                                                           |
| Allow Raw Complete          | If true, the player can complete the quest directly, without having the quest in the quest log.                                                                                                                                                                                                                                                                        |

### Quest Objectives

There are many different types of quest objectives which will be covered below.  They all share the following properties.

| Name                  | Description                                                                                                                                                         |
| --------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Amount                | The amount of the specific objective that must be completed for the objective to be complete.                                                                       |
| Override Display Name | By default, the name of the specific objective will be shown in the quest log.  If this field is not empty, the text shown in this field will be displayed instead. |

#### Ability Objective

| Name         | Description                                                          |
| ------------ | -------------------------------------------------------------------- |
| Ability Name | The name of an [Ability](abilities/) that must be learned.           |
| Require Use  | If true, the [Ability](abilities/) must be used, instead of learned. |

#### Collect Objective

| Name          | Description                                                                                                        |
| ------------- | ------------------------------------------------------------------------------------------------------------------ |
| Item Name     | The name of an [Item](items/) that must be collected.                                                              |
| Partial Match | If true, the _Item Name_ can be a substring of a longer name and does not have to match the exact name and length. |

#### Dialog Objective

| Name        | Description                                               |
| ----------- | --------------------------------------------------------- |
| Dialog Name | The name of a [Dialog](dialog.md) that must be completed. |

#### Kill Objective

| Name        | Description                                                                                          |
| ----------- | ---------------------------------------------------------------------------------------------------- |
| Target Name | The name of an enemy that must be killed.  This can match a character name or [Faction](faction.md). |

#### Quest Quest Objective

| Name       | Description                                                   |
| ---------- | ------------------------------------------------------------- |
| Quest Name | The name of another [Quest](quest.md) that must be completed. |

#### Trade Skill Objective

| Name       | Description                                           |
| ---------- | ----------------------------------------------------- |
| Skill Name | The name of a [Skill](skill.md) that must be learned. |

#### Use Interactable Objective

| Name               | Description                                                                                                            |
| ------------------ | ---------------------------------------------------------------------------------------------------------------------- |
| Interactable Name  | The name of an [Interactable](interactable-option-configurations/) that must be used (interacted with).                |
| Require Completion | If true, and the interactable is of the type that opens a popup window, the function the window provides must be used. |

#### Visit Zone Objective

| Name      | Description                                                |
| --------- | ---------------------------------------------------------- |
| Zone Name | The name of a [Scene](scene-node.md) that must be visited. |

## Next Steps

* Add a quest to a [Quest Start Item](items/quest-start-item.md).
* Add a quest to a [Quest Giver](interactable-option-configurations/quest-giver-config.md).
