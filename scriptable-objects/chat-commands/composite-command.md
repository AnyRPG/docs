---
description: Composite commands trigger one or more chat commands of any type.
---

# Composite Command

{% embed url="https://youtu.be/3APSwGQC4nc" %}

## Creation

To create a composite command, find (or create) the _GameName/Resources/GameName/ChatCommand_ folder in the project tab and right click.  Choose _Create > AnyRPG > Chat Commands > Composite Command_.

![](<../../.gitbook/assets/image (137).png>)

## Properties

| Name          | Description                         |
| ------------- | ----------------------------------- |
| Chat Commands | A list of chat commands to trigger. |

## Examples

| Command     | Effect                                                                               |
| ----------- | ------------------------------------------------------------------------------------ |
| /learnwings | <p>Triggers the commands:<br>/learnability Red Wings<br>/learnability Blue Wings</p> |
| /boost      | <p>Triggers the commands:<br>/setlevel 10<br>/gaincurrency gold 100</p>              |
|             |                                                                                      |
