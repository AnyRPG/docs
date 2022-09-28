---
description: >-
  The Spawnable monobehaviour allows spawning and despawning of other Prefabs
  based on Prerequisite Conditions being satisfied.
---

# Spawnable

## Usage

Spawnables are the way AnyRPG deals with the need for physical objects in the world to appear or disappear as the game story progresses.  There is no limitation to what can be spawned, from small things like shrubs or trees, up to entire buildings.

## Properties

| Name                    | Description                                                                                                                                                             |
| ----------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Prefab Profile Name     | A [Prefab Profile](../scriptable-objects/prefab-profile.md) containing a link to a Prefab that will be spawned.                                                         |
| Spawn Delay             | The amount of seconds to delay spawning the prefab once all the [Prerequisites](../shared-properties/prerequisite-conditions.md) are met and the object can be spawned. |
| Spawn Reference         | If the Interactable does not spawn any objects, but instead is always visible, link the GameObject in this field.                                                       |
| Despawn Object          | If true, and there is an object spawned, and the _Prerequisite Conditions_ are no longer met, despawn it.                                                               |
| Prerequisite Conditions | [Prerequisite Conditions](../shared-properties/prerequisite-conditions.md) that must be satisfied for the object to spawn.                                              |

## Dependencies

* Spawnable does not have any dependencies, and can be placed on a Prefab with no other components.
