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

### In Game Character Creator

| Name                      | Description                                                                                                                                                    |
| ------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Use First Creator Profile | If true, when the character creator is used in-game, the character will be forced to use the first character creator profile, rather than their current model. |

### Inventory

| Name                    | Description                                                                                                                                                                                  |
| ----------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Default Inventory Slots | The number of slots the player inventory contains, without any [Bags](../scriptable-objects/items/bag.md) equipped.                                                                          |
| Default Bank Slots      | The number of slots the [Bank](../scriptable-objects/interactable-option-configurations/bank-config.md) contains, without any [Bags](../scriptable-objects/items/bag.md) equipped.           |
| Max Inventory Bags      | The maximum number of bags a player can have equipped on their character.                                                                                                                    |
| Max Bank Bags           | The maximum number of bags a player can have equipped at the [Bank](../scriptable-objects/interactable-option-configurations/bank-config.md).                                                |
| Default Backpack Item   | If this field is not null, the player will have this item equipped as their backpack when starting a new game.                                                                               |
| Default Bank Contents   | A list of [Items](../scriptable-objects/items/) that the player will have in their [Bank](../scriptable-objects/interactable-option-configurations/bank-config.md) when starting a new game. |

### Controller

| Name                                | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| ----------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Default Controller Configuration    | <p>The controller configuration that will be enabled by default the first time the game is launched.  This can be changed by the player in the in-game options menu.<br><strong>Mouse And Keyboard</strong><br>Mouse and Keyboard control will be enabled and the player will use strafe mode as the movement default.  Mouse and Keyboard action bars will be shown.<br><strong>Game Pad</strong><br>Game Pad control will be enabled and the player will use free run mode as the movement default.  Game Pad action bars will be shown.</p> |
| Max Turn Speed                      | The maximum turn speed in degrees per second.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| Walk Speed                          | The default character walk speed in meters per second.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| Run Speed                           | The default character run speed in meters per second.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| Swim Speed                          | The default character swim speed in meters per second.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| Fly Speed                           | The default character fly speed in meters per second.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| Glide Speed                         | The default character glide speed in meters per second.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| Glide Fall Speed                    | The speed the character will fall while gliding in meters per second.                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| Use Fall Damage                     | If true, the player will take damage when falling from heights.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| Fall Damage Per Meter               | If fall damage is used, the amount of damage per meter fallen the player will take.                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| Fall Damage Min Distance            | If fall damage is used, the minimum distance the player must fall before damage is taken.                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| Fall Damage Audio Clip              | The audio clip to play when fall damage is taken.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| Fall Damage Audio                   | The [Audio Profile](../scriptable-objects/audio-profile.md) to play when fall damage is taken. If this value is set, it will override the _Fall Damage Audio Clip_ setting.                                                                                                                                                                                                                                                                                                                                                                    |
| Use Third Party Movement Controller | THIS FEATURE IS DEPRECATED. DO NOT USE.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| Allow Auto Attack                   | If true, the player will automatically attack with the current auto-attack even when no abilities are actively used. If a third party movement controller is used, disable this to prevent movement lock in combat.                                                                                                                                                                                                                                                                                                                            |

### Camera

| Name                           | Description                              |
| ------------------------------ | ---------------------------------------- |
| Use Third Party Camera Control | THIS FEATURE IS DEPRECATED.  DO NOT USE. |
| Third Party Camera             | THIS FEATURE IS DEPRECATED.  DO NOT USE. |
| System Animation Profile Name  |                                          |

### Animation

| Name                          | Description                                                                                                                                                                                                                                     |
| ----------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| System Animation Profile Name | This [Animation Profile](../scriptable-objects/animation-profile.md) should contain references to all the default animations that are on the default animation controller so the system knows which animations to replace when overriding them. |
| Sync Movement Animation Speed | If true, movement animations will be sped up or slowed down to match the actual speed (in m/s) the character is moving at. This will reduce foot sliding, but may result in more jerky looking movement.                                        |

### Character Animation Configuration

| Name                           | Description                                                                                                                                                                                  |
| ------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Default Animation Profile Name | This [Animation Profile](../scriptable-objects/animation-profile.md) will override the system animations included in the engine when no other unit or weapon specific animations are in use. |
| Default Animation Controller   | The animation controller that will be used to animate characters by default.                                                                                                                 |

### Level Values

| Name                  | Description                                                                                    |
| --------------------- | ---------------------------------------------------------------------------------------------- |
| Max Level             | The character cannot level up past this level.                                                 |
| XP Required Per Level | Every level, the amount of experience you need for the next level is increased by this amount. |

### Currency

| Name                    | Description                                                                                                                                                                                                                      |
| ----------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Currency Group Name     | A [Currency Group](../scriptable-objects/currency-group.md) that will be shown by default in tooltips and the Vendor UI window.                                                                                                  |
| Vendor Price Multiplier | When selling an [Item](../scriptable-objects/items/) to a [Vendor](../scriptable-objects/interactable-option-configurations/vendor-config.md), the offered amount will be the regular purchase amount multiplied by this number. |

### TemplateStart

| Name | Description |
| ---- | ----------- |
|      |             |
|      |             |
|      |             |

### TemplateEnd
