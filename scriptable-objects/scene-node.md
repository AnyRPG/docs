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

#### Scene File

| Name              | Description                                                                                                                                               |
| ----------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Use Regional File | If true, look for the resource description with the same name as the resource, plus the string 'Scene' and use the _Display Name_ field as the file name. |
| Scene File        | The name of the scene file, without a path, as it is found in the Unity Build Settings.                                                                   |

#### Scene Audio

| Name                         | Description                                                                                                                                                    |
| ---------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Day Ambient Sounds Profile   | The name of an [Audio Profile](audio-profile.md) that contains a link to an audio clip to play in the background during the day while the scene is active.     |
| Day Ambient Sounds Audio     | A link to an audio clip to play in the background during the day while the scene is active. This will override any [Audio Profile](audio-profile.md) chosen.   |
| Night Ambient Sounds Profile | The name of an [Audio Profile](audio-profile.md) that contains a link to an audio clip to play in the background during the night while the scene is active.   |
| Night Ambient Sounds Audio   | A link to an audio clip to play in the background during the night while the scene is active. This will override any [Audio Profile](audio-profile.md) chosen. |
| Background Music Profile     | The name of an [Audio Profile](audio-profile.md) that contains a link to an audio clip to be used as the background music when this scene is loaded.           |

#### Movement Audio

| Name                       | Description                                                                                                                                                                                                                                                                                                 |
| -------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Movement Loop Profile Name | The name of an [Audio Profile](audio-profile.md) that contains a link to an audio clip to be used as the movement loop (footstep loop) when this scene is loaded.                                                                                                                                           |
| Movement Hit Profile Name  | The name of The name of an [Audio Profile](audio-profile.md) that contains a link to an audio clip to be used as the footstep hit sounds when this scene is loaded.                                                                                                                                         |
| Foot Step Profiles         | A list of audio profiles containing footstep sounds to play in response to `FootStep()` animation events, depending on what terrain layer the character is moving on. The list index is matched to the terrain layers index. Eg: list item one will be played when the character is over terrain layer one. |

#### Scene Options

| Name                     | Description                                                                                                                                                                                                     |
| ------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Allow Mount              | If true, the character can ride a mount in this scene.                                                                                                                                                          |
| Suppress Character Spawn | If true, the player will not be automatically spawned when this scene is loaded.                                                                                                                                |
| Suppress Main Camera     | If true, the main camera will not active when this scene is loaded.  This is useful if the scene will be used for a [Cutscene](cutscene.md) and there is already a [Cutscene](cutscene.md) camera in the scene. |
| Auto Play Cutscene Name  | The name of a [Cutscene](cutscene.md) to play automatically when this scene is loaded.                                                                                                                          |

#### Environmental Settings

| Name                    | Description                                                                                           |
| ----------------------- | ----------------------------------------------------------------------------------------------------- |
| Environment State Names | The names of [Environment State Profiles](environment-state-profile.md) that can apply to this scene. |

#### Time Of Day Settings

| Name                     | Description                                                                                                                                                                                                                                                                                       |
| ------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Sun Rotation Mode        | <p><strong>None</strong></p><p>Do not rotate the sun.</p><p><strong>Sun</strong></p><p>Rotate the sun. Best if the skybox already includes a sun.</p><p><strong>Parent</strong></p><p>Rotate the gameobject that is the parent of the sun. Best if the sun is a physical object in the scene.</p> |
| Use Default Sun Angle    | If true, the default sun angle from the System Configuration Manager will be used instead of the value below.                                                                                                                                                                                     |
| Sun Angle                | The number of degrees around the X axis that the sun will be rotated compared to world space. 0 is pointing directly North, 90 is pointing straight down (directly over the player head), 180 is pointing directly South.                                                                         |
| Rotate Sun Color         | If true, the color of light the sun emits will be changed over time.                                                                                                                                                                                                                              |
| Use Default Sun Gradient | If true, the Sun Gradient from the System Configuration Manager will be used instead of the gradient below.                                                                                                                                                                                       |
| Sun Gradient             | A color gradient to use for the sun color. The ends represent midnight, and the center is noon. The alpha value controls sun light intensity and skybox blending.                                                                                                                                 |
| Blended Skybox           | If true, the skybox is assumed to be using the BlendedSkybox shader, and will change based on the alpha property of the sunGradient over time.                                                                                                                                                    |
| Rotate Skybox            | If true, the skybox will be rotated as time passes.                                                                                                                                                                                                                                               |
| Skybox Rotation Offset   | The offset rotation required to position the skybox so the sun is in the correct position at midnight.                                                                                                                                                                                            |
| Reverse Skybox Rotation  | If true, the skybox will be rotated counter clockwise. This should be used for sun angles between 0 and 90 degrees.                                                                                                                                                                               |

#### Weather Settings

| Name               | Description                                                                                                                                                                                                                                                                       |
| ------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Min Weather Length | The minimum number of in-game seconds a certain weather type should last for.                                                                                                                                                                                                     |
| Max Weather Length | The maximum number of in-game seconds a certain weather type should last for.                                                                                                                                                                                                     |
| No Weather Weigh   | A weighted value that determines the chance that clear weather will be chosen when the weather changes.                                                                                                                                                                           |
| Weather Weights    | <p>A weighted of list of potential weather that can be chosen when the weather changes.<br><strong>Weather</strong><br>A Weather Profile that defines the weather settings.<br><strong>Weight</strong><br>A weighted value that determines the chance this weather is chosen.</p> |
