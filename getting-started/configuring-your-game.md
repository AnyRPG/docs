# Configuring your game

## The System Configuration Manager

All configuration options that apply to the entire game are set through the System Configuration Manager. &#x20;

After using the New Game Wizard to create your game, you can find the System Configuration Manager in the Game Manager prefab at the following directory path : _Games/YourGameName/Prefab/GameManager._

__![](<../.gitbook/assets/image (1).png>)__

## Settings

The System Configuration Manager has over 100 settings. They are grouped in common related themes, and listed below.

### Game Configuration

| Name                   | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Game Name              | The name of the game that will show on the main menu screen when the game is first launched.                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| Game Version.          | The version number that will show on the main menu screen when the game is first launched.                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| Load Resources Folders | <p>Because AnyRPG supports multiple games in the same project, it is necessary to only load the Scriptable Objects that apply to the correct game.  Each game has its own resources in subfolder of a Resources folder in the format <em>Resources/YourGameName</em>.<br>This has the added benefit of allowing the developer to have shared resources that can be re-used across multiple games.<br>This list contains the names of all Resources subfolders that should be loaded into memory when the game is launched.</p> |

### Scenes

| Name                  | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| --------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Initialization Scene  | <p>The name of the scene that contains the GameManager prefab.  In the launching process, the GameManager prefab is set to <code>DontDestroyOnLoad</code> and then the <em>Main Menu Scene</em> is loaded.<br>If the game is launched from a content scene that has a <a href="../monobehaviours/scene-config.md">Scene Config</a> prefab in it, that scene will be unloaded, and the <em>Initialization Scene</em> will be immediately loaded to start the launching process properly.</p> |
| Main Menu Scene       | <p>The name of the scene that contains the main menu, where the player can start new games or load existing saved games.<br>This name can be the name of the scene on disk, or the friendly name configured in a <a href="../scriptable-objects/scene-node.md">Scene Node</a>.</p>                                                                                                                                                                                                          |
| Default Starting Zone | <p>If your game is not configured to allow choosing a Faction when starting a game, or the the Faction's Default Starting Zone field is empty, then new players will start their adventures in this scene.<br>This name can be the name of the scene on disk, or the friendly name configured in a <a href="../scriptable-objects/scene-node.md">Scene Node</a>.</p>                                                                                                                        |

### New Game Options

| Name                             | Description                                                                                                                                                                                         |
| -------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Default Player Name              | <p>If <em>Use New Game Window</em> is false, the player will start a new game with this name.<br>If <em>Use New Game Window</em> is true, the player will have its name set to this by default.</p> |
| Use New Game Window              | If true, the player will be presented with a screen to customize the character name before launching a new game.                                                                                    |
| New Game Appearance              | If true, and _Use New Game Window_ is true, show the appearance tab in the New Game Window.                                                                                                         |
| New Game UMA Appearance          | If true, and _Use New Game Window_ is true, an UMA character creator will be shown when UMA characters are selected in the New Game Window.                                                         |
| New Game Class                   | If true, and _Use New Game Window_ is true, the player can select their [Character Class](../scriptable-objects/character-class.md) in the New Game Window.                                         |
| New Game Faction                 | If true, and _Use New Game Window_ is true, the player can select their [Faction](../scriptable-objects/faction.md) in the New Game Window.                                                         |
| New Game Specialization          | If true, and _Use New Game Window_ is true, and _New Game Class_ is true, the player can select their [Class Specialization](../scriptable-objects/class-specialization.md) in the New Game Window. |
| New Game Audio                   | An [Audio Profile](../scriptable-objects/audio-profile.md) that contains an audio clip to play while the New Game Window is open.                                                                   |
| Default Player Unit Profile Name | If _Use New Game Window_ is false, all new players will start the game using this [Unit Profile](../scriptable-objects/unit-profile.md).                                                            |
| Always Show Default Profiles     | If true, and _Use New Game Window_ is true, the default profiles will always be shown, in addition to any allowed by [Faction](../scriptable-objects/faction.md) (if used).                         |
| Character Creator Profile Names  | A list of [Unit Profiles](../scriptable-objects/unit-profile.md) to show in the New Game Window.                                                                                                    |

### TemplateEndTemplateStart

| Name | Description |
| ---- | ----------- |
|      |             |
|      |             |
|      |             |

### TemplateEnd
