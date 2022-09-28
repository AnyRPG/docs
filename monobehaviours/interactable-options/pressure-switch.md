---
description: >-
  An Pressure Switch is a type of switch that is activated when a RigidBody with
  a certain weight moves into its collider.
---

# Pressure Switch

## Properties

| Name             | Description                                                                                                                                                 |
| ---------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Control Objects  | A list of links to other Interactable Options in the same scene.                                                                                            |
| Switch Group     | A list of other Switch-type Interactable Options.  All of the other options must be in the Open Position for this switch to activate its _Control Objects_. |
| Activation Limit | The number of times this switch can be activated.  0 is unlimited.                                                                                          |
| Minimum Weight   | The minimum weight a RigidBody must have to activate this switch.                                                                                           |

## Dependencies

* An Interactable Monobehavior must be on the same GameObject.
* For a pressure switch to do anything, it needs to have links to at least one other valid Interactable Option in the same scene.

