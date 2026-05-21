---
description: >-
  An Activatable Object Interactable Option can enable and disable GameObjects
  at runtime by clicking on them.
---

# Activatable Object

## Properties

| Name         | Description                                      |
| ------------ | ------------------------------------------------ |
| Spawn Object | The GameObject that will be enabled or disabled. |

## Dependencies

* An Interactable Monobehavior must be on the same GameObject.
* An Animated Object triggers animations on an Animation Component, so an Animation Component is required.  The Animation Component is linked from a [property](activatable-object.md#undefined), so it does not need to be on the exact same GameObject as the Animation Object Monobehaviour.

