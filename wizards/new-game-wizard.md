---
description: >-
  The New Game Wizard will add a new game to your project and fully configure
  all the minimally required directories, scriptable objects, prefabs and scenes
  so it is ready to play immediately.
---

# New Game Wizard

{% embed url="https://youtu.be/gS8Ya4I8Yt0" %}

## Accessing The Wizard

The New Game Wizard can be opened by clicking _Tools_ in the menu bar, and selecting _AnyRPG > Wizard > New Game Wizard_.

![](<../.gitbook/assets/image (41).png>)

![](<../.gitbook/assets/image (36).png>)

## Options

| Name                        | Description                                                                                                                                                                                                                                                                              |
| --------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Game Name                   | The name of the game.  This will show on the main menu screen.                                                                                                                                                                                                                           |
| Game Version                | A text string describing the game version.  This will show on the main menu screen.                                                                                                                                                                                                      |
| Default Player Type         | <p>The type of character that will be available by default on the new game screen.<br>UMA : A Unity Multipurpose Avatar with customizable appearance.<br>Mecanim : A standard mecanim character with no customization options.</p>                                                       |
| Main Menu Music             | An audio clip to play when the main menu scene is open.                                                                                                                                                                                                                                  |
| New Game Music              | An audio clip to play when the new game window is open on the main menu.                                                                                                                                                                                                                 |
| First Scene Name            | The file name of the default scene that will load when a new game is started.  This will also show as the title for the minimap when that scene is open.                                                                                                                                 |
| Copy Existing Scene         | If this option is not chosen, the first scene will be based on a blank template with only a large flat plane for the player to move around on.  If this option is chosen, you can select an existing scene in the project to copy that will be used instead of the blank template scene. |
| Existing Scene              | If _Copy Existing Scene_ is selected, link the scene that should serve as the template for the first scene here.                                                                                                                                                                         |
| First Scene Ambient Sounds  | An audio clip of ambient environmental sounds to play when the first scene is open.                                                                                                                                                                                                      |
| First Scene Music           | An audio clip of background music to play when the first scene is open.                                                                                                                                                                                                                  |
| Install Gold Currency Group | Installs the _Gold Currency Group_ template that consists of gold, silver, and copper.                                                                                                                                                                                                   |
| Install Armor Classes       | Installs the RPG Armor Classes template that consists of cloth, leather, and plate armor classes.                                                                                                                                                                                        |
| Install Character Stats     | Installs the RPG Character Stats template that consists of stamina, intellect, strength, and agility.                                                                                                                                                                                    |
| Install Item Qualities      | Installs the RPG Item Qualities template that consists of the poor, common, uncommon, rare, epic, legendary, and heirloom item qualities.                                                                                                                                                |
| Install Power Resources     | Installs the RPG Power Resources template that consists of health, mana, rage, and energy.                                                                                                                                                                                               |
| Install Unit Toughnesses    | Installs the RPG Unit Toughnesses template package that consists of 2 man, 5 man, 10 man, 25 man, solo dungeon minion, and solo dungeon boss unit toughnesses.                                                                                                                           |
| Install Weapon Skills       | Installs the RPG Weapon Skills template package that consists of bow, crossbow, dagger, fist, one hand axe, one hand mace, one hand sword, shield, staff, two hand axe, two hand mace, two hand sword, unarmed, and wand weapon skills.                                                  |

## Creating A New Game

After choosing the appropriate options for your game, click Create.

![](<../.gitbook/assets/image (35).png>)

## Content Created

### Folder Structure

A folder structure similar to what is shown in the picture below will have been created.

![](<../.gitbook/assets/image (6) (1).png>)

### Game Manager Prefabs

In the Prefab/GameManager folder you can find 3 prefabs.  The purpose of each is discussed below.

![](<../.gitbook/assets/image (3) (1) (2) (1).png>)

#### GameManager

The Game Manager prefab contains all of the scripts necessary to run the game.  It also contains the global game configuration in the SystemConfigurationManager, which you can edit to customize global options for the game.

The Game Manager should only ever exist in the game loading scene, which the wizard will have setup already.

#### SceneConfig

The Scene Config prefab is a special prefab that can go in any scene to allow you to press the Play button in Unity and have the game load correctly.

#### UMA\_GLIB

The UMA Global Library is required for the Unity Multipurpose Avatar system to function properly, and will have already been placed in the game loading scene by the wizard.

### Portal Prefab

In the Prefab/Portal folder you can find a portal prefab.  This object can be placed in any scene to create a portal that your player can walk through to return to the first scene.

![](<../.gitbook/assets/image (27).png>)

### Scriptable Objects

#### Audio Profiles

If audio files were chosen on the New Game Wizard window, then AudioProfile scriptable objects will exist in the Resources/GameName/AudioProfile folder.  These objects contain links to the audio files that were selected.\
![](<../.gitbook/assets/image (19).png>)

#### Scene Nodes

Scene Nodes for the Main Menu and First Scene can be found in the Resources/GameName/SceneNode folder.  The objects contain metadata about the 2 scenes, including the name of the scene file on disk, the display name to be used in-game on on the minimap title, and the name of the audio profiles to play when that scene is open.

![](<../.gitbook/assets/image (97).png>)

#### System Effects

System Effects can be found in the Resources/GameName/AbilityEffect/System folder.  These are special visual and audio effects activated by the system when the player dies, when the player gains a level, and when a dead enemy has loot that can be collected.  The Game manager will have been automatically configured to use these effects.

![](<../.gitbook/assets/image (60).png>)

#### Unit Profiles

Unit profiles are character definitions and can be found in the Resources/GameName/UnitProfile/Player folder.  By default, a definition for an UMA character, and a standard mecanim character will have been created.  The Game Manager will have been configured to use whichever unity type you selected on the New Game Wizard screen.

![](<../.gitbook/assets/image (78).png>)

#### Other Scriptable Objects

Depending on which other options were selected under the Common RPG Building Blocks subheading on the New Game Wizard screen, you will find the appropriate scriptable objects in subfolders of the Resources/GameName folder.

### Scenes

#### Loading Scene

The loading scene is a special scene with the sole purpose of setting the Game Manager and UMA Global Library to [DontDestroyOnLoad](https://docs.unity3d.com/ScriptReference/Object.DontDestroyOnLoad.html) so they persist through any scene changes, and then running the startup process of the Game Manager to initialize the data factory and UI, before loading the main menu.

![](<../.gitbook/assets/image (54).png>)

#### First Scene

The first scene is the default scene that will load when a new game is started.  It will contain the _SceneConfig_ object, which is a special object that allows you to press play from that scene, and have the system automatically load the loading scene to perform game initialization.  The contents of the scene will either be a blank template level with a plane your character can stand on, or the contents of whatever scene you chose to copy when configuring the New Game Wizard.\
![](<../.gitbook/assets/image (77).png>)

### Build Settings

By default, both the loading scene and the first scene will have been added to the build settings, which can be access through the _File > Build Settings..._ option from the Unity editor menu bar.

![](<../.gitbook/assets/image (30).png>)

![](<../.gitbook/assets/image (16).png>)

## Playing the Game

After the wizard completes running, the First Scene will be open.  Press the Play button in the Unity editor to start playing.
