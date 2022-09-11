---
description: Gain currency commands provide the player character with currencies.
---

# Gain Currency Command

{% embed url="https://youtu.be/3APSwGQC4nc" %}

## Creation

To create a gain currency command, find (or create) the _GameName/Resources/GameName/ChatCommand_ folder in the project tab and right click.  Choose _Create > AnyRPG > Chat Commands > Gain Currency Command_.

![](<../../.gitbook/assets/image (133).png>)

## Properties

| Name            | Description                                                                                   |
| --------------- | --------------------------------------------------------------------------------------------- |
| Fixed Currency  | If true, the command will always provide the currency listed in the _Currency Name_ property. |
| Currency Name   | The name of the currency to be provided if _Fixed Currency_ is true.                          |
| Fixed Amount    | If true, the command will always provide the amount listed in the _Currency Amount_ property. |
| Currency Amount | The amount of currency to be provided if _Fixed Amount_ is true.                              |

## Examples

| Command               | Effect                                              |
| --------------------- | --------------------------------------------------- |
| /gaingold             | Gain a predetermined amount of the gold currency.   |
| /gaincurrency silver  | Gain a predetermined amount of the silver currency. |
| /gaincurrency 10 gold | Gain 10 gold.                                       |
