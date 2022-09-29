---
description: >-
  A Movement Sound Area changes the sound of footsteps for any character in
  motion in the area.  This can be used to change default footsteps to water
  splashes, gravel crunches, grass swishing etc.
---

# Movement Sound Area

## Properties

| Name                       | Description                                                                                                                                                                                                                                 |
| -------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Movement Loop Profile Name | The name of an [Audio Profile](../scriptable-objects/audio-profile.md) containing a looping audio clip that will be played while the a character is in motion.                                                                              |
| Movement Hit Profile Name  | The name of an [Audio Profile](../scriptable-objects/audio-profile.md) containing a list of footstep hit sounds that will be played whenever a characters feet hit the ground in response to `PlayFootStep` or `PlayStep` animation events. |

## Dependencies

* A collider marked as a trigger is required on the same GameObject as the script so that it can detect when a character enters the area.
