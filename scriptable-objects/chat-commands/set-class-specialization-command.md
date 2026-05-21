---
description: >-
  Set class specialization commands set the player's character class
  specialization.
---

# Set Class Specialization Command

{% embed url="https://youtu.be/3APSwGQC4nc" %}

## Creation

To create a set level command, find (or create) the _GameName/Resources/GameName/ChatCommand_ folder in the project tab and right click.  Choose _Create > AnyRPG > Chat Commands > Set Class Specialization Command_.

## Properties

| Name                       | Description                                                                                                                |
| -------------------------- | -------------------------------------------------------------------------------------------------------------------------- |
| Fixed Class Specialization | If true, all parameters will be ignored, and the character class will be the one in the _Class Specialization Name_ field. |
| Class Specialization Name  | The name of the class specialization to set if _Fixed Class Specialization_ is true.                                       |

## Examples

| Command                    | Effect                           |
| -------------------------- | -------------------------------- |
| /setclassspecalization ice | Set the Character Class to Ice.  |
| /setfire                   | Set the Character Class to Fire. |
