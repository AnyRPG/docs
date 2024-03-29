---
description: >-
  A unit profile defines all the information related to a character, including
  both the character configuration, and properties of the physical model.
---

# Unit Profile

## Creation

To create a unit profile, find (or create) the _GameName/Resources/GameName/UnitProfile_ folder in the project tab and right click.  Choose _Create > AnyRPG > UnitProfile_.

![](<../.gitbook/assets/image (1) (2) (3).png>)

## Properties

The default properties of a character unit are listed below.  Some of these properties can be overridden if this character is used as a player.

### Unit Prefab

| Name                     | Description                                                                                                                                                             |
| ------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Automatic Prefab Profile | If true, the unit prefab is loaded by searching for a [UnitPrefabProfile](unit-prefab-profile.md) with the same name as this resource.                                  |
| Prefab Profile Name      | The name of the prefab profile that contains the prefab that represents this unit.  Only used if _Automatic Prefab Profile_ and _Use Inline Prefab Props_ are not true. |
| Use Inline Prefab Props  | If true, the unit prefab is loaded from the inline _Unit Prefab Props_ field.                                                                                           |
| Unit Prefab Props        | [Unit Prefab Profile](unit-prefab-profile.md) properties.                                                                                                               |

### Unit Settings

| Name           | Description                                           |
| -------------- | ----------------------------------------------------- |
| Is UMA Unit    | Deprecated, not currently used.                       |
| Is Pet         | If true, this unit can be captured and kept as a pet. |
| Flight Capable | If true, this unit can fly.                           |
| Glide Capable  | If true, this unit can glide.                         |

### Character

| Name                      | Description                                                                                |
| ------------------------- | ------------------------------------------------------------------------------------------ |
| Character Name            | The name of the character, which will be shown in unit frames and nameplates.              |
| Title                     | A title that will be shown below the name in the nameplate.                                |
| Faction Name              | The name of the [Faction](faction.md) that this character belongs to.                      |
| Unit Type Name            | The name of the [Unit Type](unit-type.md) of this character.                               |
| Character Race Name       | The name of the [Character Race](character-race.md) of this character.                     |
| Character Class Name      | The name of the [Character Class](character-class.md) of this character.                   |
| Class Specialization Name | The name of the [Class Specialization](class-specialization.md) of this character.         |
| Spawn Dead                | If true, the character will spawn dead.                                                    |
| Prevent Auto Despawn      | If true, the character will not despawn when it does.                                      |
| Default Toughness         | The name of a [Unit Toughness](unit-toughness.md) that defines how tough the character is. |

### Voice

| Name                   | Description                                                                                                                                                                       |
| ---------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Voice Profile          | A [Voice Profile](voice-profile.md) that contains voice audio clips to play.                                                                                                      |
| Use Inline Voice Props | If true, the [Voice Profile](voice-profile.md) is loaded from the inline settings below, instead of the shared voice profile above.                                               |
| Voice Props            | If _Use Inline Voice Props_ is true, the [Voice Profile Properties](voice-profile.md#properties) here will be used instead of the shared [Voice Profile](voice-profile.md) above. |

### Configuration

| Name                   | Description                                                                                                                                                                                                                                                       |
| ---------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Capabilities           | [Capabilities](../shared-properties/capabilities.md) the character has.                                                                                                                                                                                           |
| Primary Stats          | A list of [Character Stat General Properties](character-stat.md#general-properties).                                                                                                                                                                              |
| Power Resources        | A list of [Power Resources](power-resource.md) the character has.                                                                                                                                                                                                 |
| Use Provider Equipment | By default NPCs only equip the [Equipment](items/equipment.md) listed in the _Equipment Name List_.  If true, NPCs will equip all [Equipment](items/equipment.md) from any provider, including [Character Class](character-class.md), [Faction](faction.md), etc. |
| Equipment Name List    | A list of [Equipment](items/equipment.md) that the character will have equipped by default.                                                                                                                                                                       |

### Combat

| Name                      | Description                                                                                                      |
| ------------------------- | ---------------------------------------------------------------------------------------------------------------- |
| Is Aggressive             | If true, the unit will attack anything in its aggro radius, based on the [Faction](faction.md) relationship.     |
| Aggro Radius              | The radius of the aggro sphere around this unit. Set to 0 to disable aggro.                                      |
| Automatic Combat Strategy | If true, a [Combat Strategy](combat-strategy.md) matching the unit name will be looked up, and used if found.    |
| Combat Strategy Name      | The name of a [Combat Strategy](combat-strategy.md) to use.                                                      |
| Default Hit Effects       | [Ability Effects](ability-effects/) to cast on the target when the performing an unarmed standard (auto) attack. |

### Movement

| Name                         | Description                                                                                                                                                                                                                                                                                                                                                                                               |
| ---------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Is Mobile                    | If true, the character can move.                                                                                                                                                                                                                                                                                                                                                                          |
| Footstep Type                | <p><strong>None</strong></p><p>Do not play footsteps.</p><p><strong>Unit</strong></p><p>Play the footsteps configured below. <strong>Environment</strong></p><p>Play the footsteps based on the terrain. <strong>UnitFallback</strong></p><p>Try environment, then fallback to unit if no environment sound available.<br><strong>Both</strong><br>Play environment and unit sounds at the same time.</p> |
| Play On Footstep             | If true, individual footstep sounds will play when the foot hits the ground, instead of playing a repeating footsteps loop when moving.                                                                                                                                                                                                                                                                   |
| Movement Audio Profile Names | A list of [Audio Profiles](audio-profile.md) that contain audio clips that will be played when the unit is in motion.  If _Play On Footstep_ is true, the audio clips will by cycled through as the feet hit the ground.                                                                                                                                                                                  |

### Patrol

| Name              | Description                                                            |
| ----------------- | ---------------------------------------------------------------------- |
| Use Inline Patrol | If true, the patrol defined in the _Patrol Config_ field will be used. |
| Patrol Config     | [Patrol](patrol-profile.md) properties.                                |
| Patrol Names      | The names of [Patrol Profiles](patrol-profile.md) to use.              |

### Interaction

| Name                        | Description                                                                                                                                                                             |
| --------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Face Interaction Target     | If true, and the character is an NPC, it will turn and face any player that interacts with it.                                                                                          |
| Interaction Max Range       | The maximum range at which this character can be interacted with if it is an NPC.                                                                                                       |
| Interactable Options        | A list of named [Interactable Options](interactable-option-configurations/) that define which [Interactables](interactable-option-configurations/) this character has, if it is an NPC. |
| Inline Interactable Options | [Interactable Option Configurations](interactable-option-configurations/) that define which [Interactables](interactable-option-configurations/) this character has, if it is an NPC.   |

### Object Persistence

| Name                    | Description                                                                                                                                                                                                                                                     |
| ----------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Persist Object Position | If true, the object position is saved so that the object will spawn at the saved location next time a game is loaded. This requires at least one of _Save On Level Unload_, _Save On Game Save_, or a save setting in a [Patrol](patrol-profile.md) to be true. |
| Save On Level Unload    | If true, the position will be saved when a level is unloaded.                                                                                                                                                                                                   |
| Save On Game Save       | If true, the position will be saved when the game is saved.                                                                                                                                                                                                     |
| Overwrite Unit UUID     | If true, the automatic UUID assigned to the unit will be overwritten with the UUID in the _UUID_ field.                                                                                                                                                         |
| UUID                    | An automatically created Universally Unique Identifier used to ensure that all objects with saved position data do not overwrite another object's data.                                                                                                         |

## Next Steps

* Add a unit profile to the _Default Player Unit Profile Name_ field in the System Configuration Manager to make this unit the default when a new game is started.
* Add a unit profile to the _Character Creator Profile Names_ list in the System Configuration Manager to allow a player to choose this unit from a list of units when starting a new game.
* Add a unit profile to the _Character Creator Profile Names_ list in a [Faction](faction.md) to allow a player to choose this unit from a list of units when starting a new game as a specific [Faction](faction.md).
