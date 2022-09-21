---
description: Gain item commands add items to the players inventory.
---

# Gain Item Command

{% embed url="https://youtu.be/3APSwGQC4nc" %}

## Creation <a href="#creation" id="creation"></a>

To create a gain item command, find (or create) the _GameName/Resources/GameName/ChatCommand_ folder in the project tab and right click. Choose _Create > AnyRPG > Chat Commands > Gain Item Command_.​​​

![](<../../.gitbook/assets/image (111) (1).png>)

## Properties

| Name       | Description                                                                     |
| ---------- | ------------------------------------------------------------------------------- |
| Fixed Item | If true, the item provided will be the item listed in the _Item Name_ property. |
| Item Name  | The name of the item to be provided if the _Fixed Item_ property is true.       |

## Examples

| Command                        | Effect                                          |
| ------------------------------ | ----------------------------------------------- |
| /gainsword                     | Gain the item defined in the Item Name property |
| /gainitem Basic One Hand Sword | Gain the item named _Basic One Hand Sword_.     |
