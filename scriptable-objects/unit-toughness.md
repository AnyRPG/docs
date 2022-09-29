---
description: >-
  Unit Toughness defines which properties should be multiplied and by how much
  when scaling the base properties of a character to make it tougher.
---

# Unit Toughness

## Creation

To create a unit toughness, find (or create) the _GameName/Resources/GameName/UnitToughness_ folder in the project tab and right click.  Choose _Create > AnyRPG > UnitToughness_.

![](<../.gitbook/assets/image (1) (4) (1).png>)

## Properties

| Name                            | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| ------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Focus Projector Override Map    | <p>A list of properties that will override the default highlight circle shown on the ground when a character is highlighted.<br><strong>Source Color</strong><br>If the <a href="faction.md">Faction</a> relationship color matches this color, then the settings in this list element will be used.<br><strong>Projector Material</strong><br>The material to replace the default highlight image material.<br><strong>Tint Material</strong><br>If true, the <em>Projector Material</em> will also be tinted with the color.</p> |
| Currency Multiplier             | The amount that the total currency gained from a kill will be multiplied by.                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| Experience Multiplier           | The amount that the total experience gained from a kill will be multiplied by.                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| Default Resource Multiplier     | All [Power Resources](power-resource.md) will be multiplied by this value.                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| Resource Multipliers            | <p>A list of specific <a href="power-resource.md">Power Resources</a> to multiply.<br><strong>Resource Name</strong><br><strong></strong>The name of a <a href="power-resource.md">Power Resource</a> to multiply.<br><strong>Value Multiplier</strong><br><strong></strong>The amount to multiply the <a href="power-resource.md">Power Resource</a> by.</p>                                                                                                                                                                      |
| Default Primary Stat Multiplier | The amount to multiply all [Character Stats](character-stat.md) by.                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| Primary Stat Multipliers        | <p>A list of specific <a href="character-stat.md">Character Stats</a> to multiply.<br><strong>Stat Name</strong><br><strong></strong>The name of a <a href="character-stat.md">Character Stat</a> to multiply.<br><strong>Stat Multiplier</strong><br><strong></strong>The amount to multiply the <a href="character-stat.md">Character Stat</a> by.</p>                                                                                                                                                                           |

## Next Steps

* Add a unit toughness value to a [Unit Profile](unit-profile.md) to make it tougher.
