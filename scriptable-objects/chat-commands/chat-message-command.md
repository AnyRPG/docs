---
description: Chat message commands allow the player to send messages.
---

# Chat message Command

{% embed url="https://youtu.be/3APSwGQC4nc" %}

## Creation

To create an action command, find (or create) the _GameName/Resources/GameName/ChatCommand_ folder in the project tab and right click.  Choose _Create > AnyRPG > Chat Commands > Chat Message Command_.

## Properties

| Name         | Description                                 |
| ------------ | ------------------------------------------- |
| Message Type | <p>One of:<br>Private<br>Group<br>Guild</p> |

## Examples

| Command                         | Effect                                             |
| ------------------------------- | -------------------------------------------------- |
| /private "Player Name" hi there | Sends the message "hi there" to "**Player Name**". |
| /group hi there                 | Sends the message "hi there" to the current group. |
| /guild hi there                 | Sends the message "hi there" to the current guild. |
