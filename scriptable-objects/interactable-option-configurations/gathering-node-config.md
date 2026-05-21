---
description: >-
  A gathering node config creates a gathering node interactable option, allowing
  the player to gather crafting resources.
---

# Gathering Node Config

{% embed url="https://youtu.be/DuNoF0h7lUc" %}

## Creation

To create a gathering node config, find (or create) the _GameName/Resources/GameName/InteractableOptionConfig_ folder in the project tab and right click.  Choose _Create > AnyRPG > Interactable > GatheringNodeConfig_.

## Properties

| Name                           | Description                                                                                                                                                                                                                |
| ------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Loot Table Names               | A list of [Loot Tables](../loot-table.md) containing [Items](../items/) this node can drop when gathering is performed.                                                                                                    |
| Spawn Timer                    | The number seconds after all [Items](../items/) have been looted before the node resets and spawns again.                                                                                                                  |
| Ability Name                   | The name of a [Gather Ability](../abilities/gather-ability.md) the player must know to interact with the gathering node.                                                                                                   |
| Skill Name                     | The skill required to gather from this node, or empty for none.                                                                                                                                                            |
| Required Skill Level           | The required skill level to gather from this node.                                                                                                                                                                         |
| Chance To Gain Level           | The chance to gain a skill level when gathering from this node. 1 = 100% chance, 0.5 = 50% chance, etc. This only applies if skill experience is not in use for this skill.                                                |
| Skill Experience Reward        | The amount of skill experience to give when gathering from this node.                                                                                                                                                      |
| Max Skill Experience Level     | The maximum skill level at which skill experience will be granted for this node. If the character skill is higher than this level, they will get no skill experience. 0 means this node will never stop giving experience. |
| Character Experience Reward    | The amount of character experience to give when gathering from this node.                                                                                                                                                  |
| Max Character Experience Level | The maximum character level at which character experience will be granted for this node. If the character is higher than this level, they will get no experience. 0 means this node will never stop giving experience.     |

## Next Steps

* Add a gathering node config to an Interactable to allow gathering from it.
