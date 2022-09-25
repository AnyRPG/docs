---
description: >-
  An item pickup config creates an item pickup interactable option, allowing the
  player to loot items.
---

# Item Pickup Config

## Creation

To create an item pickup config, find (or create) the _GameName/Resources/GameName/InteractableOptionConfig_ folder in the project tab and right click.  Choose _Create > AnyRPG > Interactable > ItemPickupConfig_.

![](<../../.gitbook/assets/image (8).png>)

## Properties

| Name             | Description                                                                                                             |
| ---------------- | ----------------------------------------------------------------------------------------------------------------------- |
| Loot Table Names | A list of [Loot Tables](../loot-table.md) containing [Items](../items/) this node can drop when gathering is performed. |
| Spawn Timer      | The number seconds after all [Items](../items/) have been looted before the node resets and spawns again.               |

## Next Steps

* Add an item pickup config to an Interactable to allow looting items from it.
