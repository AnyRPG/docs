---
description: >-
  A unit spawn controller config creates a unit spawn controller interactable
  option, allowing the player to spawn character units from a popup window.
---

# Unit Spawn Controller Config

## Creation

To create a unit spawn controller config, find (or create) the _GameName/Resources/GameName/InteractableOptionConfig_ folder in the project tab and right click.  Choose _Create > AnyRPG > Interactable > UnitSpawnControllerConfig_.

![](<../../.gitbook/assets/image (10).png>)

## Properties

| Name                 | Description                                                                 |
| -------------------- | --------------------------------------------------------------------------- |
| Unit Profile Names   | A list of names of [Unit Profiles](../unit-profile.md) that can be spawned. |
| Unit Spawn Node List | A list of Unit Spawn Nodes where the character units will be spawned.       |

## Next Steps

* Add a unit spawn controller config to an Interactable to allow spawning character units when interacting with it.
