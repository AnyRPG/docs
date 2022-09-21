---
description: A quest start item is an item that can start a quest when used.
---

# Quest Start Item

## Creation

To create a quest start item, find (or create) the _GameName/Resources/GameName/Item_ folder (or any subfolder) in the project tab and right click.  Choose _Create > AnyRPG > Inventory > Items > QuestStartItem_.

![](<../../.gitbook/assets/image (2).png>)

## Properties

In addition to the properties shared by all [Items](./), quest start items have the following unique properties.

| Name   | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| ------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Quests | <p>A list of <a href="../quest.md">Quests</a> that the item can start.<br><strong>Start Quest</strong><br>This should always be true to allow the item to start the <a href="../quest.md">Quest</a> in the <em>Quest Name</em> field.<br><strong>End Quest</strong><br>If true, the <a href="../quest.md">Quest</a> can be auto-completed upon starting.<br><strong>Quest Name</strong><br>The name of the <a href="../quest.md">Quest</a> to start when the item is used.</p> |

## Next Steps

* Add a quest start item to a [Vendor Collection](../vendor-collection.md) so it can be purchased from a [Vendor](../interactable-option-configurations/vendor-config.md).
* Add a quest start item to a [Loot Table](../loot-table.md) so that it can drop upon defeat of an enemy.
