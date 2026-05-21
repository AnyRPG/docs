---
description: >-
  The Interactable monobehaviour is required on any Prefab that the player will
  be able to interact with.  It is also required on Prefabs that are remotely
  controlled by switches.
---

# Interactable

## Usage

All Interactables can have one or more interactable options.  The Interactable component allows the object to be interacted with, and the Interactable Options provide unique functionality and interaction options.

## Properties

Interactable has the following properties.

| Name                               | Description                                                                                                                                                                                                              |
| ---------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Show Tooltip                       | If true, a UI tooltip will be shown when the mouse hovers over the object.                                                                                                                                               |
| Interactable Name                  | The name of the object that will be shown in the mouseover tooltip.                                                                                                                                                      |
| Glow On Mouse Over                 | If true, the material of the object will be replaced with a glowing material while the mouse is hovering over it.                                                                                                        |
| Glow Color                         | The default color of the glow outline.  This will be overridden on character units depending on the faction relationship color.                                                                                          |
| Interaction Tooltip Text           | Set this value to override the default 'Interact' option for the gamepad interaction tooltip                                                                                                                             |
| Not Interactable                   | Set this value to prevent direct interaction from the player. This can be useful for interactables that only need to be activated with control switches.                                                                 |
| Interact With Any                  | Set this to true to allow triggering interaction with anything that has a collider, not just players.                                                                                                                    |
| Interact On Exit                   | Set this to true to cause the interaction to trigger on when something exits the collider.                                                                                                                               |
| Is Trigger                         | If true, interaction is triggered by a collider, and not by clicking with the mouse                                                                                                                                      |
| Suppress Interaction Window        | Set this to true to automatically activate the first interactable instead of opening the interaction window and presenting the player with interaction options.                                                          |
| Override Interaction Collider Size | If true, the InteractionRange collider will be set to the new extents in the Interaction Max Range field.                                                                                                                |
| Interaction Max Range              | For everything except character unit interactions, the interactor must be within this range of this objects collider. This does not apply to interactions triggered by switches.                                         |
| Interaction Points                 | The prefered locations that units wanting to interact will move to, based on NavMeshPath completeness.                                                                                                                   |
| Component Controller               | Reference to local component controller prefab with nameplate target, speakers, etc.                                                                                                                                     |
| Persistent Object Component        | [Persistent Object Properties](persistent-object.md)                                                                                                                                                                     |
| Persist Interactable Data          | Set this to true to save and load interactable data for this interactable. This is only necessary if the interactable has interactable options that need to save data, such as loot or a door that can be opened/closed. |
| Has Nameplate                      | Set this to true to have a nameplate appear over the object. The nameplate will show the interactable's name and any interactable options it has.                                                                        |
| Nameplate Props                    |                                                                                                                                                                                                                          |

## Nameplate Props

| Name                        | Description                                                                                                                                              |
| --------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Display Name                | This is what will be printed on the nameplate above the object. It will also override whatever value is set for the Interactable mouseover display name. |
| Override Nameplate Position | If true, the nameplate position will be set to this value.                                                                                               |
| Nameplate Position          | The position of the NamePlate anchor, relative to the unit pivot.                                                                                        |

## Dependencies

* Any interactable that will be directly interacted with needs a Collider component, so that it can be clicked on.
* One or more Interactable Option Components must be present for any interactions to be possible.
