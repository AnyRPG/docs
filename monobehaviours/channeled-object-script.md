---
description: >-
  A channeled object script is attached to a prefab that should be used as a
  lightning bolt that travels from the caster to the target while channeling an
  ability.
---

# Channeled Object Script

## Properties

| Name           | Description                                                                                                                                               |
| -------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Start Object   | The game object where the lightning will emit from. If null, StartPosition is used.                                                                       |
| Start Position | The start position where the lightning will emit from. This is in world space if StartObject is null, otherwise this is offset from StartObject position. |
| End Object     | The game object where the lightning will end at. If null, EndPosition is used.                                                                            |
| End Position   | The end position where the lightning will end at. This is in world space if EndObject is null, otherwise this is offset from EndObject position.          |
| Generations    | How manu generations? Higher numbers create more line segments.                                                                                           |
| Duration       | How long each bolt should last before creating a new bolt. In ManualMode, the bolt will simply disappear after this amount of seconds.                    |
| Chaos Factor   | How chaotic should the lightning be? (0-1)                                                                                                                |
| Manual Mode    | In manual mode, the trigger method must be called to create a bolt.                                                                                       |
| Rows           | The number of rows in the texture. Used for animation.                                                                                                    |
| Columns        | The number of columns in the texture. Used for animation.                                                                                                 |
| Animation Mode | The animation mode for the lightning.                                                                                                                     |

## Dependencies

* A line renderer must be attached to the same prefab, using a material with a sprite sheet of a lightning bolt.
* If _Start Object_ and _End Object_ are used, the prefab should have 2 gameobjects as children (with no components on them) that will serve as the start and end point of the lightning bolt.
