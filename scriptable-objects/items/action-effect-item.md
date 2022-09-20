---
description: >-
  Action effect items perform an animated action and cast an ability effect when
  used.  They are commonly used as flasks and scrolls.
---

# Action Effect Item

{% embed url="https://youtu.be/UR4pH60Rluo" %}

## Creation

To create an action effect item, find (or create) the _GameName/Resources/GameName/Item_ folder in the project tab and right click.  Choose _Create > AnyRPG > Inventory > Items > Action Effect Item_.

![](<../../.gitbook/assets/image (118).png>)

## Properties

Action effect Items are a type of item.  See [Items](./) for their base properties.

| Name              | Description                                                                                                                                                                                                                                                                                                                                           |
| ----------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Tool Tip          | This text will appear in the tooltip "Use:" section and describes what the item does when used.                                                                                                                                                                                                                                                       |
| Cool Down         | The time in seconds that must pass after using this item before another item of the same type can be used again.                                                                                                                                                                                                                                      |
| Action Type       | <p><strong>None</strong><br>This item will not cause the character to perform any action when used.<br><strong>Inline</strong><br>The action properties will be defined directly.<br><strong>Named</strong><br>The action properties defined by the named <a href="../animated-action.md">Animated Action</a> will be performed by the character.</p> |
| Action Name       | The name of an [Animated Action](../animated-action.md) the character will perform when the item is used.                                                                                                                                                                                                                                             |
| Action Properties | [Animated Action](../animated-action.md) properties defined directly on this item that the character will perform when the item is used.                                                                                                                                                                                                              |
| Use Inline Effect | If true, the effect properties defined in the Inline Effect field will be cast.                                                                                                                                                                                                                                                                       |
| Effect Name       | If _Inline Effect_ is false the Ability Effect with this name will be cast.                                                                                                                                                                                                                                                                           |
| Inline Effect     | Ability Effect properties to cast when the item is used if _Use Inline Effect_ is true.                                                                                                                                                                                                                                                               |

## Next Steps

* Add an action effect item to a [Vendor Collection](../vendor-collection.md) so it can be purchased from a [Vendor](../interactable-option-configurations/vendor-config.md).
* Add an action effect item to a [Loot Table](../loot-table/) so that it can drop upon defeat of an enemy.
* Add an action effect item as an output to a [Recipe](recipe.md) so that it can be crafted.
