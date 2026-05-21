---
description: Set character class commands set the player's character class.
---

# Set Character Class Command

{% embed url="https://youtu.be/3APSwGQC4nc" %}

## Creation

To create a set level command, find (or create) the _GameName/Resources/GameName/ChatCommand_ folder in the project tab and right click.  Choose _Create > AnyRPG > Chat Commands > Set Character Class Command_.

## Properties

| Name                  | Description                                                                                                           |
| --------------------- | --------------------------------------------------------------------------------------------------------------------- |
| Fixed Character Class | If true, all parameters will be ignored, and the character class will be the one in the _Character Class Name_ field. |
| Character Class Name  | The name of the character class to set if _Fixed Character Class_ is true.                                            |

## Examples

| Command                    | Effect                              |
| -------------------------- | ----------------------------------- |
| /setcharacterclass warrior | Set the Character Class to Warrior. |
| /setmage                   | Set the Character Class to Mage.    |
