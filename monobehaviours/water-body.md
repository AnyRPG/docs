---
description: A Water Body is an enclosed area the player can float and swim within.
---

# Water Body

## Properties

| Name                           | Description                                                                                                                                                                                          |
| ------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| My Collider                    | A link to a Collider.                                                                                                                                                                                |
| Use Fog                        | If true, fog will be enabled when the camera is within the bounds of the collider to give a realistic under water effect by limiting the distance that the player can see.                           |
| Fog Color                      | The color of the fog to be used when the camera is in the water.                                                                                                                                     |
| Fog Density                    | The density of the fog.  More dense fog means the distance a player can see is smaller.                                                                                                              |
| Enter Water Audio Profile Name | An [Audio Profile](../scriptable-objects/audio-profile.md) containing a link to an audio clip to play for a splash sound when entering the water.                                                    |
| Swim Loop Audio Profile Name   | An [Audio Profile](../scriptable-objects/audio-profile.md) containing a link to an audio clip to loop when the player is swimming on the surface of the water.                                       |
| Swim Hits Audio Profile Name   | An [Audio Profile](../scriptable-objects/audio-profile.md) containing a link to audio clip to play whenever the players hands hit the water when the player is swimming on the surface of the water. |

## Dependencies

* A collider is required on the same GameObject as the Water Body so that players can be detected when they enter the water.
