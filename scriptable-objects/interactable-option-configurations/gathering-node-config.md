---
description: >-
  A gathering node config creates a gathering node interactable option, allowing
  the player to gather crafting resources.
---

# Gathering Node Config

## Creation

To create a gathering node config, find (or create) the _GameName/Resources/GameName/InteractableOptionConfig_ folder in the project tab and right click.  Choose _Create > AnyRPG > Interactable > GatheringNodeConfig_.

![](<../../.gitbook/assets/image (2).png>)

## Properties

| Name             | Description                                                                                                              |
| ---------------- | ------------------------------------------------------------------------------------------------------------------------ |
| Loot Table Names | A list of [Loot Tables](../loot-table.md) containing [Items](../items/) this node can drop when gathering is performed.  |
| Spawn Timer      | The number seconds after all [Items](../items/) have been looted before the node resets and spawns again.                |
| Ability Name     | The name of a [Gather Ability](../abilities/gather-ability.md) the player must know to interact with the gathering node. |

## Next Steps

* Add a gathering node config to an Interactable to allow gathering from it.
