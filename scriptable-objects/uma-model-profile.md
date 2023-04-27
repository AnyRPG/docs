---
description: >-
  An UMA model profile contains information about an UMA model so that the
  character editor can show the the correct slots.
---

# UMA Model Profile

## Creation

To create an UMA model profile, find (or create) the _GameName/Resources/GameName/UMAModelProfile_ folder in the project tab and right click.  Choose _Create > AnyRPG > UMAModelProfile_.

![](<../.gitbook/assets/image (2).png>)

## Properties

Swappable mesh model profiles, contain one property, Model Options, which contains a list of Slot Options with following fields.

| Name             | Description                                                                                                                                                                                                                       |
| ---------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Slot Name        | The name of the UMA wardrobe slot this option applies to.                                                                                                                                                                         |
| Recipe List Type | <p><strong>Deny</strong><br>All the recipes in the Recipe Names list will not be shown in the character editor.<br><strong>Allow</strong><br>Only the recipes in the Recipe Names list will be shown in the character editor.</p> |
| Recipe Names     | A list of UMA wardrobe recipes.                                                                                                                                                                                                   |

## Next Steps

* Add an UMA model profile to a [Unit Prefab Profile](unit-prefab-profile.md).
