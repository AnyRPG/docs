---
description: >-
  A scene node contains configuration information for a scene file, including
  background music and many other settings.
---

# Scene Node

## Creation

To create a scene node, find (or create) the _GameName/Resources/GameName/SceneNode_ folder in the project tab and right click.  Choose _Create > AnyRPG > SceneNodes > SceneNode_.

![](<../.gitbook/assets/image (1) (2) (1) (1).png>)

## Properties

| Name                       | Description                                                                                                                                                                                                     |
| -------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Use Regional File          | If true, look for the resource description with the same name as the resource, plus the string 'Scene' and use the _Display Name_ field as the file name.                                                       |
| Scene File                 | The name of the scene file, without a path, as it is found in the Unity Build Settings.                                                                                                                         |
| Ambient Music Profile      | The name of an [Audio Profile](audio-profile.md) that contains a link to an audio clip to be used as the ambient sounds when this scene is loaded.                                                              |
| Background Music Profile   | The name of an [Audio Profile](audio-profile.md) that contains a link to an audio clip to be used as the background music when this scene is loaded.                                                            |
| Movement Loop Profile Name | The name of an [Audio Profile](audio-profile.md) that contains a link to an audio clip to be used as the movement loop (footstep loop) when this scene is loaded.                                               |
| Movement Hit Profile Name  | The name of The name of an [Audio Profile](audio-profile.md) that contains a link to an audio clip to be used as the footstep hit sounds when this scene is loaded.                                             |
| Allow Mount                | If true, the character can ride a mount in this scene.                                                                                                                                                          |
| Suppress Character Spawn   | If true, the player will not be automatically spawned when this scene is loaded.                                                                                                                                |
| Suppress Main Camera       | If true, the main camera will not active when this scene is loaded.  This is useful if the scene will be used for a [Cutscene](cutscene.md) and there is already a [Cutscene](cutscene.md) camera in the scene. |
| Auto Play Cutscene Name    | The name of a [Cutscene](cutscene.md) to play automatically when this scene is loaded.                                                                                                                          |
| Environment State Names    | The names of [Environment State Profiles](environment-state-profile.md) that can apply to this scene.                                                                                                           |
