---
description: >-
  An item quality can be assigned to an item, allowing that item to share
  similar settings with other items of the same quality like stat multipliers,
  icon background colors, and more.
---

# Item Quality

## Creation

To create an item quality, find (or create) the _GameName/Resources/GameName/ItemQuality_ folder in the project tab and right click.  Choose _Create > AnyRPG > ItemQuality_.

![](<../.gitbook/assets/image (117).png>)



## Properties

| Name                      | Description                                                                                                                                                                                                                                                             |
| ------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Stat Multiplier           | When an [Item](items/) does not have manual stats enabled, multiply the base automatic stats by this amount.                                                                                                                                                            |
| Allow Random Items        | If true, random [Items](items/) of this quality can be created.                                                                                                                                                                                                         |
| Random Weight             | When a random item quality is chosen, all weights are added up before a number if chosen.  This controls the chance an [Item](items/) of this quality will be created.  A larger number in relation to other numbers of other item qualities will give a higher chance. |
| Random Quality Prefix     | If not empty, and an [Item](items/) of this quality is created randomly, this prefix will be added to the [Item](items/) name.                                                                                                                                          |
| Random Stat Count         | If an [Item](items/) of this quality is created with random stats, this is the number of random stats that will be chosen.                                                                                                                                              |
| Dynamic Item Level        | If true, any [Item](items/) of this quality will automatically scale their level, regardless of whether they individually have level scaling enabled.                                                                                                                   |
| Buy Price Multiplier      | Multiply the base purchase price of any [Item](items/) of this quality by this amount.                                                                                                                                                                                  |
| Sell Price Multiplier     | Multiply the base vendor sell price of any [Item](items/) with this quality by this amount.                                                                                                                                                                             |
| Require Sell Confirmation | If true, a popup window will appear asking the player to confirm any time they try to sell an [Item](items/) with this quality.                                                                                                                                         |
| Quality Color             | The color that will be used for text and image backgrounds whenever an [Item](items/) of this quality is displayed in the UI.                                                                                                                                           |
| Tint Background Image     | If true, the background image if an [Item](items/) displayed in the UI will have its color set to this color, instead of black.                                                                                                                                         |

## Next Steps

* Assign this item quality to an [Item](items/).
