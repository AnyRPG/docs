---
description: >-
  A music player config creates a music player interactable option, allowing the
  player to open a window with a list of audio clips and play them.
---

# Music Player Config

## Creation

To create a music player config, find (or create) the _GameName/Resources/GameName/InteractableOptionConfig_ folder in the project tab and right click.  Choose _Create > AnyRPG > Interactable > MusicPlayerConfig_.

![](<../../.gitbook/assets/image (7) (2).png>)

## Properties

| Name                | Description                                                                                                                                                                                                                                                                                                                                                                       |
| ------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Audio Type          | <p>The type of sound to play.  This affects which audio source will be used.<br><strong>Music</strong><br>The sound will be played through the background music audio source.<br><strong>Ambient</strong><br>The sound will be played through the ambient sounds audio source.<br><strong>Effect</strong><br>The sound will be played through the sound effects audio source.</p> |
| Audio Profile Names | A list of the names of [Audio Profiles](../audio-profile.md) that contain lists of audio clips that can be played.                                                                                                                                                                                                                                                                |

## Next Steps

* Add a music player config to an Interactable to allow opening the music player window.
