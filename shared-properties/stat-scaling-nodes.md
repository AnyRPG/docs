---
description: >-
  Stat Scaling Nodes define primary stats and their budget per level.  Each
  point of primary stat can provide direct or rated amounts of secondary stats
  as well as direct amounts of power resources.
---

# Stat Scaling Nodes

## Properties

| Name                            | Description                                                                                                                                                                                                                                                                                      |
| ------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Stat Name                       | A [Character Stat](../scriptable-objects/character-stat.md).                                                                                                                                                                                                                                     |
| Budget Per Level                | The number of points of the stat that a character will gain for each level.                                                                                                                                                                                                                      |
| Primary To Secondary Conversion | <p>The amount of each secondary stat that a character will gain for each point of the primary stat.<br>See <a href="../scriptable-objects/character-stat.md#properties">Character Stat Properties</a> for field descriptions.</p>                                                                |
| Primary To Resource Conversion  | <p>A list of <a href="../scriptable-objects/power-resource.md">Power Resources</a> and the number of points of that resource gained per point of the primary stat.<br>See <a href="../scriptable-objects/character-stat.md#properties">Character Stat Properties</a> for field descriptions.</p> |
| Regen                           | <p>A list of the amount of <a href="../scriptable-objects/power-resource.md">Power Resources</a> that will be regenerated per point of primary stat every tick.<br>See <a href="../scriptable-objects/character-stat.md#properties">Character Stat Properties</a> for field descriptions.</p>    |
