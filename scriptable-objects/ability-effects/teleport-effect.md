---
description: A teleport effect teleports the caster to another scene.
---

# Teleport Effect

## Creation

To create a teleport effect, find (or create) the _GameName/Resources/GameName/AbilityEffect_ folder (or any subfolder) in the project tab and right click.  Choose _Create > AnyRPG > Abilities > Effects > TeleportEffect_.

![](<../../.gitbook/assets/image (6).png>)

## Properties

In addition to all the properties of its parent class, [Fixed Length Effect](./#fixed-length-effect-properties), teleport effects have the following properties.

| Name                     | Description                                                                                                                               |
| ------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------- |
| Level Name               | The name of the [Scene](../scene-node.md) to load.                                                                                        |
| Location Tag             | The name of a tag to search for in the scene.  If the tag is found, the player will spawn at the location of the GameObject with the tag. |
| Override Spawn Location  | If true, the player will spawn at the Vector3 location in the _Spawn Location_ field.                                                     |
| Spawn Location           | The Vector3 location the player will spawn at if the _Override Spawn Location_ field is set to true.                                      |
| Override Spawn Direction | If true the player will spawn with their forward direction set to the Vector3 direction in the _Spawn Forward Direction_ field.           |
| Spawn Forward Direction  | The Vector3 direction that the player should be facing when they spawn if the _Override Spawn Direction_ field is set to true.            |

## Next steps

* Add a teleport effect to an [Ability](../abilities/).
* Add a teleport effect to another [Ability Effect](./) to chain them together.
