---
description: >-
  A lootable character config creates a lootable character interactable,
  allowing the player to loot the character when it dies.
---

# Lootable Character Config

## Creation

To create a lootable character config, find (or create) the _GameName/Resources/GameName/InteractableOptionConfig_ folder in the project tab and right click.  Choose _Create > AnyRPG > Interactable > LootableCharacterConfig_.

![](<../../.gitbook/assets/image (7).png>)

## Properties

| Name               | Description                                                                                                                                              |
| ------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Automatic Currency | If true, when killed, this character will drop the system defined [Currency](../currency.md) amount for its level and [Toughness](../unit-toughness.md). |
| Loot Table Names   | The names of [Loot Tables](../loot-table.md) containing [Items](../items/) that can potentially drop when the character dies.                            |

## Next Steps

* Add a lootable character config to a [Unit Profile](../unit-profile.md) to allow the player to collect loot from it when it dies.
