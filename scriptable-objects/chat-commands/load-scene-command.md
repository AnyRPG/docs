---
description: Load scene commands immediately load a scene.
---

# Load Scene Command

{% embed url="https://youtu.be/3APSwGQC4nc" %}

## Creation <a href="#creation" id="creation"></a>

To create a load scene command, find (or create) the _GameName/Resources/GameName/ChatCommand_ folder in the project tab and right click. Choose _Create > AnyRPG > Chat Commands > Load Scene Command_.​​​

![](<../../.gitbook/assets/image (3).png>)

## Properties

| Name        | Description                                                                      |
| ----------- | -------------------------------------------------------------------------------- |
| Fixed Scene | If true, the scene loaded will be the scene listed in the _Scene Name_ property. |
| Scene Name  | The name of the scene to be loaded if the _Fixed Scene_ property is true.        |

## Examples

| Command               | Effect                       |
| --------------------- | ---------------------------- |
| /warp                 | Load a predefined scene.     |
| /loadscene Soul Forge | Load the _Soul Forge_ scene. |
