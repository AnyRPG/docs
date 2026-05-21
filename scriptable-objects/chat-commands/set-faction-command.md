---
description: Set faction commands set the player's faction.
---

# Set Faction Command

{% embed url="https://youtu.be/3APSwGQC4nc" %}

## Creation

To create a set level command, find (or create) the _GameName/Resources/GameName/ChatCommand_ folder in the project tab and right click.  Choose _Create > AnyRPG > Chat Commands > Set Faction Command_.

## Properties

| Name          | Description                                                                                      |
| ------------- | ------------------------------------------------------------------------------------------------ |
| Fixed Faction | If true, the player faction will always be set to the one specified in the _Faction Name_ field. |
| Faction Nname | If _Fixed Faction_ is set to true, this is the faction the player will be set to.                |

## Examples

| Command              | Effect                              |
| -------------------- | ----------------------------------- |
| /setfaction faction1 | Set the player to faction faction1. |
| /setfaction2         | Set the player to faction faction2. |
