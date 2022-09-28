---
description: >-
  An Moveable Object Interactable Option moves and/or rotates an object between
  its initial position in the scene and a defined position.
---

# Moveable Object

## Properties

| Name             | Description                                                                                                                                         |
| ---------------- | --------------------------------------------------------------------------------------------------------------------------------------------------- |
| Switch Only      | If true, this option can only be interacted with via a switch.                                                                                      |
| Moveable Object  | A link to the prefab which will be moved and/or rotated.                                                                                            |
| Movement Speed   | The speed, in meters per second, the object will move at.                                                                                           |
| Rotation Speed   | The speed, in degrees per second, the object will rotate at.                                                                                        |
| Delay Time       | The amount of seconds to delay inbetween open and close actions when looping.                                                                       |
| Loop             | If true, the object should continue moving and rotating between the start and end positions until the Interactable Option is interacted with again. |
| Target Position  | The Vector3 target position to move to.                                                                                                             |
| Target Rotation  | The Vector3 target rotation to rotate to.                                                                                                           |
| Open Audio Clip  | A link to an Audio Clip to play when changing to the open (starting) position.                                                                      |
| Close Audio Clip | A link to an Audio Clip to play when changing to the closed (ending) position.                                                                      |

## Dependencies

* An Interactable Monobehavior must be on the same GameObject.
* An Moveable Object moves a prefab, so a prefab that is intended to be moved must be present in the scene.  This can be any prefab and does not have to be in the same heirarchy as the Moveable Object Monobehaviour.

