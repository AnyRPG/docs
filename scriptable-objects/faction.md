---
description: >-
  Factions allow for groups of characters to have the same relationship
  disposition toward other groups of characters.
---

# Faction

## Creation

To create a faction, find (or create) the _GameName/Resources/GameName/Faction_ folder in the project tab and right click.  Choose _Create > AnyRPG > Factions > Faction_.

![](../.gitbook/assets/image.png)



## Properties

| Name                            | Description                                                                                                                                                                                                                                                                                                                                                                                                                |
| ------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| New Game Option                 | If true, this faction can be chosen as the faction the player will be part of when starting a new game.                                                                                                                                                                                                                                                                                                                    |
| Default Starting Zone           | The zone ([Scene](scene-node.md)) that new players will start in if this faction is chosen when starting a new game.                                                                                                                                                                                                                                                                                                       |
| Default Starting Location Tag   | If not empty, players starting as this faction will spawn at the transform with this tag.                                                                                                                                                                                                                                                                                                                                  |
| Hide Default Profiles           | If true, hide any default unit profiles when this faction is used.                                                                                                                                                                                                                                                                                                                                                         |
| Character Creator Profile Names | A list of [Unit Profiles](unit-profile.md) that the player can choose from when starting as this faction.                                                                                                                                                                                                                                                                                                                  |
| Equipment Names                 | A list of [Equipment](items/equipment.md) that will be worn by a new player when starting the game as this faction.                                                                                                                                                                                                                                                                                                        |
| Default Disposition             | The disposition (relationship) that this faction has toward any faction not specifically in its disposition list.                                                                                                                                                                                                                                                                                                          |
| Disposition List                | <p>A list of factions and the dispositions that this faction will have toward them.<br><strong>Faction Name</strong><br>The name of a faction<br><strong>Disposition</strong><br>The disposition (relationship) that this faction will have toward them.</p>                                                                                                                                                               |
| Capabilities                    | A list of [Capabilities](../shared-properties/capabilities.md) that any character that is part of this faction will have.                                                                                                                                                                                                                                                                                                  |
| Class Capability List           | <p>A list of character classes, and the capabilities that those classes will have.<br><strong>Character Classes</strong><br>A list of <a href="character-class.md">Character Classes</a>.<br><strong>Capabilities</strong><br>The specific <a href="../shared-properties/capabilities.md">Capabilities</a> that any <a href="character-class.md">Character Class</a> in the <em>Character Classes</em> list will have.</p> |

## Next Steps

* Configure the System Configuration Manager to allow choosing a faction when starting a new game.
