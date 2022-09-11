---
description: >-
  An audio profile contains a list of one or more audio clips to play, and can
  be used for many purposes, including music and sound effects.
---

# Audio Profile

## Creation

To create an audio profile, find (or create) the _GameName/Resources/GameName/AudioProfile_ folder in the project tab and right click.  Choose _Create > AnyRPG > AudioProfile_.

![](<../.gitbook/assets/image (123).png>)

## Properties

| Name        | Description                                                                                                       |
| ----------- | ----------------------------------------------------------------------------------------------------------------- |
| Artist Name | A text field to enter the name of the artist that composed the audio file.  Not currently used in the default UI. |
| Audio Clips | A list of audio files.                                                                                            |

## Next Steps

* Refer to an audio profile to be used as ambient sounds or background music from a [Scene Node](scene-node.md).
* Refer to an audio profile to be used as the default hit sound for a [Weapon](items/weapon.md) in the _Default Hit Audio Profile_ field.
* Refer to an audio profile to be used as the hit sound for a specific [Weapon Skill](weapon-skill.md) in the _On Hit Audio Profiles_ list.
* Refer to an audio profile to be used as the animation hit or casting audio for an [Ability](abilities/).
* Refer to an audio profile to be used as the hit audio in the _On Hit Audio Profile Names_ field of an [Ability Effect](ability-effects/).
