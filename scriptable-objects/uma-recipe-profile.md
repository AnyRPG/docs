---
description: >-
  An UMA recipe profile contains information about how UMA gear will be
  displayed, including which UMA recipes to show, and what shared colors to use.
---

# UMA Recipe Profile

## Creation

To create an UMA recipe profile, find (or create) the _GameName/Resources/GameName/UMARecipeProfile_ folder (or any subfolder) in the project tab and right click.  Choose _Create > AnyRPG > UMARecipeProfile_.

![](<../.gitbook/assets/image (4).png>)

## Properties

An UMA recipe profile contains a single property, _UMA Recipe Profile Properties_, with the following fields.

| Name          | Description                                                                                                                                                                                                                                                            |
| ------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| UMA Recipes   | A list of UMA recipes that can potentially be displayed.  The recipes that match the target unit's UMA race will be displayed.  If multiple recipes that match the race can be applied to the same slot, the last one will always be used.                             |
| Shared Colors | <p>A list of UMA shared color data defining which colors will be shown for each defined shared color name that exists on the UMA recipe.<br><strong>Shared Colorname</strong><br>The name of an UMA shared color.<br><strong>Color</strong><br>A color to be used.</p> |

## Next Steps

* Add an UMA recipe profile to any [Equipment](items/equipment.md).
