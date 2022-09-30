---
description: >-
  The New Scene Wizard will add a new scene to your project based on an existing
  scene, or using a blank template scene.
---

# New Scene Wizard

{% embed url="https://youtu.be/Qs83JxD0o0A" %}

## Accessing The Wizard

The New Scene Wizard requires that one of your game scenes with either a GameManager or SceneConfig object is open in the editor so that it can determine which game to install the content into.

The New Scene Wizard can be opened by clicking _Tools_ in the menu bar, and selecting _AnyRPG > Wizard > New Scene Wizard_.

![](<../.gitbook/assets/image (65).png>)

![](<../.gitbook/assets/image (17) (1).png>)

## Options

| Name                     | Description                                                                                                                                                                                                                                                                        |
| ------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Game Name                | The name of the game.  This will show on the main menu screen.The name of the game in your Unity project to install the template content in.  This will be automatically filled in if you have any scene with the GameManager or SceneConfig prefabs open.                         |
| Scene Name               | The file name of the new scene. This will also show as the title for the minimap when that scene is open.                                                                                                                                                                          |
| Copy Existing Scene      | If this option is not chosen, the scene will be based on a blank template with only a large flat plane for the player to move around on.  If this option is chosen, you can select an existing scene in the project to copy that will be used instead of the blank template scene. |
| Existing Scene           | If _Copy Existing Scene_ is selected, link the scene that should serve as the template for the first scene here.                                                                                                                                                                   |
| New Scene Ambient Sounds | An audio clip of ambient environmental sounds to play when the scene is open.                                                                                                                                                                                                      |
| New Scene Music          | An audio clip of background music to play when the scene is open.                                                                                                                                                                                                                  |

## Content Created

After choosing the appropriate options for the scene, click Create.

![](<../.gitbook/assets/image (39).png>)

### Portal Prefab

In the _Prefab/Portal_ folder you can find a portal prefab.  This object can be placed in any scene to create a portal that your player can walk through to return to the new scene.

![](<../.gitbook/assets/image (11) (1).png>)

### Scriptable Objects

#### Audio Profiles

If audio files were chosen on the New Game Wizard window, then AudioProfile scriptable objects will exist in the _Resources/GameName/AudioProfile_ folder.  These objects contain links to the audio files that were selected.

![](<../.gitbook/assets/image (13) (1) (1).png>)

#### Scene Node

Scene Node for the new scene can be found in the _Resources/GameName/SceneNode_ folder.  The objects contain metadata about the scene, including the name of the scene file on disk, the display name to be used in-game on on the minimap title, and the name of the audio profiles to play when that scene is open.

![](<../.gitbook/assets/image (64).png>)

### Scene

The new scene can be found in the GameName/Scenes/SceneName folder. It will contain the _SceneConfig_ object, which is a special object that allows you to press play from that scene, and have the system automatically load the loading scene to perform game initialization.  The contents of the scene will either be a blank template level with a plane your character can stand on, or the contents of whatever scene you chose to copy when configuring the New Scene Wizard.

![](<../.gitbook/assets/image (15) (1).png>)

### Build Settings

By default, the new scene will have been added to the build settings, which can be access through the _File > Build Settings..._ option from the Unity editor menu bar.

![](<../.gitbook/assets/image (30).png>)

![](<../.gitbook/assets/image (16) (1).png>)

## Next Steps

### Scene Cleanup

If you copied a demo scene from a Unity package, you will likely have to clean up the scene so that it works properly.  Many demo scenes come with a simple player and camera.  Since AnyRPG has a camera and a player, you will likely need to remove these types of objects from the scene.

![](<../.gitbook/assets/image (46).png>)

### Default Spawn Location

By default, the player will spawn at the world origin (0,0,0).  To make the player spawn at a location of your choosing, search your project hierarchy for the _DefaultSpawnLocation_ prefab and drag it into the scene where you want the player to spawn.  Rotate the _DefaultSpawnLocation_ prefab so the forward (z) axis is facing the direction you want the player facing when they spawn.

![](<../.gitbook/assets/image (91).png>)

### Add A Portal To Load The Scene

Decide what other scenes the player should be able to travel to this scene from and add portals to them.  The New Scene Wizard created a portal prefab to use, so find it and drag it into the other scene(s).

![](<../.gitbook/assets/image (9) (1).png>)
