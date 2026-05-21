---
description: Character group commands allow the player to perform group management.
---

# Character Group Command

{% embed url="https://youtu.be/3APSwGQC4nc" %}

## Creation

To create an action command, find (or create) the _GameName/Resources/GameName/ChatCommand_ folder in the project tab and right click.  Choose _Create > AnyRPG > Chat Commands > Character Group Command_.

## Properties

| Name         | Description                                                                |
| ------------ | -------------------------------------------------------------------------- |
| Command Type | <p>Options:<br>Invite<br>Kick<br>Leave<br>Disband<br>Promote<br>Demote</p> |

## Examples

| Command             | Effect                                                                                                 |
| ------------------- | ------------------------------------------------------------------------------------------------------ |
| /kick PlayerName    | Remove PlayerName from the group.                                                                      |
| /invite PlayerName  | Invite Playername to the group.                                                                        |
| /leave              | Leave the group.                                                                                       |
| /disband            | Disband the group.                                                                                     |
| /promote PlayerName | Promote PlayerName to assistant or leader depending on whether they are currently member or assistant. |
| /demote PlayerName  | Demote PlayerName to member.                                                                           |
