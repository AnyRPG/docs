---
description: Set level commands set the player level.
---

# Set Level Command

{% embed url="https://youtu.be/3APSwGQC4nc" %}

## Creation

To create a set level command, find (or create) the _GameName/Resources/GameName/ChatCommand_ folder in the project tab and right click.  Choose _Create > AnyRPG > Chat Commands > Set Level Command_.

![](<../../.gitbook/assets/image (119).png>)

## Properties

| Name         | Description                                                                                      |
| ------------ | ------------------------------------------------------------------------------------------------ |
| Fixed Level  | If true, the player level will always be set to the level specified in the _Level Number_ field. |
| Level Number | If _Fixed Level_ is set to true, this is the level the player will be set to.                    |

## Examples

| Command      | Effect                      |
| ------------ | --------------------------- |
| /setlevel 10 | Set the player to level 10. |
| /maxlevel    | Set the player to level 50. |
