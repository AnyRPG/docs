---
description: >-
  A load scene config creates a load scene interactable option, allowing the
  player to travel to another scene by interacting with it.
---

# Load Scene Config

## Creation

To create a load scene config, find (or create) the _GameName/Resources/GameName/InteractableOptionConfig_ folder in the project tab and right click.  Choose _Create > AnyRPG > Interactable > LoadSceneConfig_.

![](<../../.gitbook/assets/image (5).png>)

## Properties

| Name                     | Description                                                                                                                               |
| ------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------- |
| Location Tag             | The name of a tag to search for in the scene.  If the tag is found, the player will spawn at the location of the GameObject with the tag. |
| Override Spawn Location  | If true, the player will spawn at the Vector3 location in the _Spawn Location_ field.                                                     |
| Spawn Location           | The Vector3 location the player will spawn at if the _Override Spawn Location_ field is set to true.                                      |
| Override Spawn Direction | If true the player will spawn with their forward direction set to the Vector3 direction in the _Spawn Forward Direction_ field.           |
| Spawn Forward Direction  | The Vector3 direction that the player should be facing when they spawn if the _Override Spawn Direction_ field is set to true.            |
| Scene Name               | The name of the scene to load.                                                                                                            |

## Next Steps

* Add a load scene config to an Interactable to allow the player to load a scene by interacting with it.
