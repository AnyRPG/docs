---
description: >-
  An environmental effect area is an area where any player that enters will have
  some type of environmental effect applied to him, such as lightning damage,
  lava damage, poison damage, etc.
---

# Environmental Effect Area

## Properties

| Name                 | Description                                                                                                                   |
| -------------------- | ----------------------------------------------------------------------------------------------------------------------------- |
| Tick Rate            | The number of seconds that should elapse between each tick of [Ability Effects](../scriptable-objects/ability-effects/).      |
| Ability Effect Names | A list of [Ability Effects](../scriptable-objects/ability-effects/) to apply to any characters inside the area on every tick. |

## Dependencies

* A box collider is required on the same GameObject as the script.  It should be marked as a trigger so that it can detect when a character enters the area.
