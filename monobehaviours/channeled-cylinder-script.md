---
description: >-
  A channeled cylinder script is attached to a prefab that should be used as a
  laser beam that travels from the caster to the target while channeling an
  ability.
---

# Channeled Cylinder Script

## Properties

| Name           | Description                                                                                                                                               |
| -------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Start Object   | The game object where the lightning will emit from. If null, StartPosition is used.                                                                       |
| Start Position | The start position where the lightning will emit from. This is in world space if StartObject is null, otherwise this is offset from StartObject position. |
| End Object     | The game object where the lightning will end at. If null, EndPosition is used.                                                                            |
| End Position   | The end position where the lightning will end at. This is in world space if EndObject is null, otherwise this is offset from EndObject position.          |

## Dependencies

* A channeled cylinder script should be used on a Unity cylinder.
