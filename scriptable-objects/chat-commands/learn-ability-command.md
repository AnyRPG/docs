---
description: Learn ability commands allow the player to learn abilities.
---

# Learn Ability Command

{% embed url="https://youtu.be/3APSwGQC4nc" %}

## Creation <a href="#creation" id="creation"></a>

To create a learn ability command, find (or create) the _GameName/Resources/GameName/ChatCommand_ folder in the project tab and right click. Choose _Create > AnyRPG > Chat Commands > Learn Ability Command_.​​​

![](<../../.gitbook/assets/image (120).png>)

## Properties <a href="#properties" id="properties"></a>

| Name          | Description                                                                                |
| ------------- | ------------------------------------------------------------------------------------------ |
| Fixed Ability | If true, this command will always learn the ability specified in the _Ability Name_ field. |
| Ability Name  | The ability to learn if the _Fixed Ability_ field is set to true.                          |

## Examples <a href="#examples" id="examples"></a>

| Command                 | Effect                          |
| ----------------------- | ------------------------------- |
| /learnability Red Wings | Learn the ability _Red Wings_.  |
| /learnbluewings         | Learn the ability _Blue Wings_. |
