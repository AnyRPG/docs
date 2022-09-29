---
description: >-
  An Scene Config is a special type of system script used to allow pressing play
  from any scene, and having resource selectors work in any scene.
---

# Scene Config

## Usage

A Scene Config Prefab will be automatically added to any scene created with the [New Scene Wizard](../wizards/new-scene-wizard.md).  It is not necessary to add one manually unless a scene is added manually, and not using the wizard.  Even then it is optional if you do not desire the ability to press play from that scene or use resource selectors in that scene.

## Properties

| Name                         | Description                                                                                                                                                                                  |
| ---------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| System Configuration Manager | A link to the Game Manager prefab on disk that should be used when building a database for resource selectors to work, or determining which scene is the correct loading scene for the game. |
| Load Game On Play            | If true, the game can be loaded from the current scene by pressing play in the Unity editor.                                                                                                 |

## Dependencies

* A properly configured Game Manager prefab is needed for the Scene Config to work.  The Game Manager prefab is added to any game created with the [New Game Wizard](../wizards/new-game-wizard.md).
