---
description: Guild commands allow the player to manage guilds.
---

# Guild Command

{% embed url="https://youtu.be/3APSwGQC4nc" %}

## Creation

To create an action command, find (or create) the _GameName/Resources/GameName/ChatCommand_ folder in the project tab and right click.  Choose _Create > AnyRPG > Chat Commands > Guild Command_.

## Properties

| Name         | Description                                                    |
| ------------ | -------------------------------------------------------------- |
| Command Type | <p>One of:<br>Invite<br>Kick<br>Leave<br>Promote<br>Demote</p> |

## Examples

| Command              | Effect                                                                                                 |
| -------------------- | ------------------------------------------------------------------------------------------------------ |
| /ginvite PlayerName  | Invite PlayerName to the guild.                                                                        |
| /gkick PlayerName    | Remove PlayerName from the guild.                                                                      |
| /gleave              | Leave the guild.                                                                                       |
| /gpromote PlayerName | Promote PlayerName to assistant or leader depending on whether they are currently member or assistant. |
| /gdemote PlayerName  | Demote PlayerName to member.                                                                           |
