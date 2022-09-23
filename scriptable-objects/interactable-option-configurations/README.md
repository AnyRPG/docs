---
description: >-
  Interactable option configurations are shared configurations that allow for
  the re-use of specific interactable settings among different NPCs.
---

# Interactable Option Configurations

## Properties

All interactable option configurations share the following common properties.

| Name                    | Description                                                                                                                                                                                         |
| ----------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Interaction Panel Title | The text to display in the interaction panel window to activate the option.  This will only be shown if there is more than one option available.                                                    |
| Interaction Panel Image | The image to display beside the text in the interaction panel window to activate the option.  This will only be shown if there is more than one option available.                                   |
| Name Plate Image        | If there is no system option set in the System Configuration manager for the nameplate image of the interaction type, this image will be shown above the nameplate if the interaction is available. |
| Prerequisite Conditions | A list of [Prerequisite Conditions](../../shared-properties/prerequisite-conditions.md) that must be satisfied for the interaction option to be available.                                          |

## Next Steps

* Create shared interactable option configurations to be re-used among different NPCs.
* Use inline interactable option configurations in [Unit Profiles](../unit-profile.md) if a specific interactable option is needed that will no be shared or re-used.
