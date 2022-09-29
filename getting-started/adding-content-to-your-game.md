---
description: >-
  There are multiple types of content you can add to your game, and multiple
  ways to add that content.  This page provides a high level overview to get
  your started.
---

# Adding Content To Your Game

## Static 3D Models and Terrain

The process of adding static 3d models or terrain to a game built with AnyRPG is the same as adding them to any other game.  Just open a scene and use the Unity editor like normal.

## Wizards

AnyRPG includes multiple [Wizards](../wizards/wizards-introduction.md) that allow you, from a single screen, to automate the addition of certain types of content that would otherwise take many steps and involve the configuration of many objects.

See [Wizards Introduction](../wizards/wizards-introduction.md) for more information.

## Intangible Content (Scriptable Objects)

Intangible Content is any content that generally cannot be seen or touched directly, such as dialogs, quests, factions, and all the other unique elements that make up the actual story of your game.  It also includes metadata for objects you will interact with, such as information about what type of music should play when a certain scene is loaded.

AnyRPG uses Unity Scriptable Objects to store this type of content and loads it into an in-memory database when a game is launched.

See [Scriptable Objects Introduction](broken-reference) for more information.

## Monobehaviours

AnyRPG includes several types of Unity Monobehaviours that are added to GameObjects that permanently exist in scenes, or will be spawned into scenes at runtime.

These Monobehaviours control many things, including, but not limited to:

* How a player can interact with the environment.
* How the environment will change over time as the player progresses through the story.
* How certain objects should be positioned or move around the envionment in response to character or player actions.

See [Monobehaviours Introduction](../monobehaviours/monobehaviours-introduction.md) for more information.
