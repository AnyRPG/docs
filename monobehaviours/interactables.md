---
description: >-
  The Interactable monobehaviour is required on any Prefab that the player will
  be able to interact with.  It is also required on Prefabs that are remotely
  controlled by switches.
---

# Interactables

## Usage

Interactable inherits from the base class, [Spawnable](spawnable.md). All Interactables can have one or more interactable options.  The Interactable component allows the object to be interacted with, and the Interactable Options provide unique functionality and interaction options.

## Properties

In addition to the properties of the base class, [Spawnable](spawnable.md), Interactable has the following properties.

| Name                              | Description                                                                                                                                                                                    |
| --------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Show Tooltip                      | If true, a UI tooltip will be shown when the mouse hovers over the object.                                                                                                                     |
| Interactable Name                 | The name of the object that will be shown in the mouseover tooltip.                                                                                                                            |
| Glow On Mouse Over                | If true, the material of the object will be replaced with a glowing material while the mouse is hovering over it.                                                                              |
| Light Emission                    | If true, the glow emits light on objects around it.                                                                                                                                            |
| Glow Flash Speed                  | The time period in seconds between high and low intensity of the glow strength.                                                                                                                |
| Glow Min Intensity                | The minimum intensity the object should glow with.                                                                                                                                             |
| Glow Max Intensity                | The maximum intensity the object should glow with.                                                                                                                                             |
| Glow Color                        | The color of light to emit when glowing.                                                                                                                                                       |
| Temporary Material                | The glow material that should replace any normal materials on this object while glowing.                                                                                                       |
| Interaction Tooltip Text          | Set this value to override the default 'Interact' option for the gamepad interaction tooltip                                                                                                   |
| Not Interactable                  | Set this value to prevent direct interaction from the player. This can be useful for interactables that only need to be activated with control switches.                                       |
| Interact With Any                 | Set this to true to allow triggering interaction with anything that has a collider, not just players.                                                                                          |
| Interact On Exit                  | Set this to true to cause the interaction to trigger on when something exits the collider.                                                                                                     |
| Is Trigger                        | If true, interaction is triggered by a collider, and not by clicking with the mouse                                                                                                            |
| Suppress Interaction Window       | Set this to true to automatically activate the first interactable instead of opening the interaction window and presenting the player with interaction options.                                |
| Interaction Max Range             | For everything except character unit interactions, the interactor must be within this range of this objects collider. This does not apply to interactions triggered by switches.               |
| Check Options To Spawn            | If set to true, all interactable options must have [Prerequisites](../shared-properties/prerequisite-conditions.md) met, in addition to the interactable prerequisites, in order to spawn.     |
| Spawn Requires Valid Option       | Require a valid interactable option in addition to any [Preqrequisites](../shared-properties/prerequisite-conditions.md). For example, quests on a questgiver, a class changer, and dialogs.   |
| Despawn Requires No Valid Options | Require no valid interactable options in addition to any [Preqrequisites](../shared-properties/prerequisite-conditions.md). For example, quests on a questgiver, a class changer, and dialogs. |
| Component Controller              | Reference to local component controller prefab with nameplate target, speakers, etc.                                                                                                           |
| Unit Component Controller         | Reference to local component controller prefab with nameplate target, speakers, etc.                                                                                                           |

## Dependencies

* Any interactable that will be directly interacted with needs a Collider component, so that it can be clicked on.
* One or more Interactable Option Components must be present for any interactions to be possible.
