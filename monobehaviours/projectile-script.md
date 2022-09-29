---
description: >-
  A projectile script is attached to a prefab that will travel through the air
  toward a target such as fireballs, arrows, tornadoes, etc.
---

# Projectile Script

## Properties

| Name         | Description                                                                                    |
| ------------ | ---------------------------------------------------------------------------------------------- |
| Audio Source | A link to an audio source that will be used to play a sound while the projectile is in motion. |

## Dependencies

* A Collider marked as a trigger, and a Rigidbody marked as Kinematic are both required on the same GameObject in order for the projectile to detect a collission with a target.
* An Audio Source is required to play a sound while travelling toward a target.
