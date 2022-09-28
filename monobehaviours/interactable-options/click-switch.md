---
description: >-
  An Click Switch can be activated locally (by the player) or remotely (by
  another switch) and is responsible for activating other Interactable Options.
---

# Click Switch

## Properties

| Name            | Description                                                                                                                                                 |
| --------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Control Objects | A list of links to other Interactable Options in the same scene.                                                                                            |
| Switch Group    | A list of other Switch-type Interactable Options.  All of the other options must be in the Open Position for this switch to activate its _Control Objects_. |

## Dependencies

* An Interactable Monobehavior must be on the same GameObject.
* For a click switch to do anything, it needs to have links to at least one other valid Interactable Option in the same scene.

