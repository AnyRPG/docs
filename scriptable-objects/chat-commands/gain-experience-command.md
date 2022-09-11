---
description: Gain experience commands increase the players experience points.
---

# Gain Experience Command

{% embed url="https://youtu.be/3APSwGQC4nc" %}

## Creation <a href="#creation" id="creation"></a>

To create a gain experience command, find (or create) the _GameName/Resources/GameName/ChatCommand_ folder in the project tab and right click. Choose _Create > AnyRPG > Chat Commands > Gain Experience Command_.​​​

![](<../../.gitbook/assets/image (136).png>)

## Properties <a href="#properties" id="properties"></a>

| Name              | Description                                                                                                   |
| ----------------- | ------------------------------------------------------------------------------------------------------------- |
| Fixed Experience  | If true, the command will always provide the amount of experience listed in the _Experience Amount_ property. |
| Experience Amount | The amount of experience to gain if the _Fixed Experience_ property is true.                                  |

## Examples <a href="#undefined" id="undefined"></a>

| Command     | Effect               |
| ----------- | -------------------- |
| /gain100xp  | Gain 100 experience. |
| /gainxp 500 | Gain 500 experience. |
|             |                      |
