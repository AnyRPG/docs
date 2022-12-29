---
description: >-
  A moveable prefab config creates a moveable prefab interactable option, which
  allows the prefab to be moved or rotated by interacting with a switch.
---

# Moveable Prefab Config

## Creation

To create a moveable prefab config, find (or create) the _GameName/Resources/GameName/InteractableOptionConfig_ folder in the project tab and right click.  Choose _Create > AnyRPG > Interactable > MoveablePrefabConfig_.

![](<../../.gitbook/assets/image (10) (1).png>)

## Properties

| Name           | Description                                                                                                                   |
| -------------- | ----------------------------------------------------------------------------------------------------------------------------- |
| Movement Speed | The speed that the prefab will move at.                                                                                       |
| Rotation Speed | The speed that the prefab will be rotated at.                                                                                 |
| Loop           | If true, the prefab will return to its starting position and rotation when done moving, and then continue its movement again. |

## Next Steps

* Add a moveable prefab config to an Interactable to allow it to be moved with a switch.
