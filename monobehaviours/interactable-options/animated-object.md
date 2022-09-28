---
description: >-
  An Animated Object Interactable Option is responsible for triggering an
  animation on an Animation component.
---

# Animated Object

## Properties

| Name                 | Description                                                                                                                                                |
| -------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Switch Only          | If true, this option can only be interacted with via a switch.                                                                                             |
| Animation Component  | A link to an Animation Component containing animations to play.                                                                                            |
| Open Animation Clip  | A link to an Animation Clip to play when changing to the open position.                                                                                    |
| Open Audio Clip      | A link to an Audio Clip to play when changing to the open position.                                                                                        |
| Open Audio Profile   | The name of an [Audio Profile](../../scriptable-objects/audio-profile.md) containing a link to an Audio Clip to play when changing to the open position.   |
| Close Animation Clip | A link to an Animation Clip to play when changing to the closed position.                                                                                  |
| Close Audio Clip     | A link to an Audio Clip to play when changing to the closed position.                                                                                      |
| Close Audio Profile  | The name of an [Audio Profile](../../scriptable-objects/audio-profile.md) containing a link to an Audio Clip to play when changing to the closed position. |

## Dependencies

* An Interactable Monobehavior must be on the same GameObject.
* An Animated Object triggers animations on an Animation Component, so an Animation Component is required.  The Animation Component is linked from a [property](animated-object.md#undefined), so it does not need to be on the exact same GameObject as the Animation Object Monobehaviour.

