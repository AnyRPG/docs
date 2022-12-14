---
description: >-
  Character stats are attributes that define a character's aptitudes and can
  affect secondary stats, power resource amounts, and power resource
  regeneration rates.
---

# Character Stat

{% embed url="https://youtu.be/I7_8xPkXm9k" %}

## Creation

To create a character stat, find (or create) the _GameName/Resources/GameName/CharacterStat_ folder in the project tab and right click.  Choose _Create > AnyRPG > Character Stat_.

![](<../.gitbook/assets/image (104).png>)

## Specific Properties

These properties exist only in character stat scriptable objects.

| Name        | Description                                    |
| ----------- | ---------------------------------------------- |
| Global Stat | If true, all characters will receive the stat. |

## General Properties

These general properties exist anywhere primary stats are defined in other scriptable objects.

| Name                            | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| ------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Budget Per Level                | The amount of the stat that a character will receive for every level.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| Primary To Secondary Conversion | <p>The amount of each secondary stat that a character will gain for each point of the primary stat.<br><strong>Secondary Stat Type</strong><br><strong></strong>A secondary stat.<br><strong>Conversion Ratio</strong><br>The number of points of each secondary stat that will be gained per point of primary stat.<br><strong>Rated Conversion</strong><br>A rated conversion is for stats that are percentages. At level 1 you will need 100 points of this secondary stat for 100%, 200 points at level 2, etc. The percent chance at any level is equal to this value multiplied by (Total Stat Amount / Current Level). This allows you to increase of decrease the 100 point requirement for 100% chance.</p>                                                                                                                                                                                                                               |
| Primary To Resource Conversion  | <p>A list of <a href="power-resource.md">Power Resources</a> and the number of points of that resource gained per point of the primary stat.<br><strong>Resource Name</strong><br>The name of the <a href="power-resource.md">Power Resource</a> that will be increased.<br><strong>Resource Per Point</strong><br>The amount of the <a href="power-resource.md">Power Resource</a> that will be gained per point of Character Stat.</p>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| Regen                           | <p>A list of the amount of power resources that will be regenerated per tick per point of primary stat.<br><strong>Power Resource</strong><br>The name of the Power Resource that will be regenerated.<br><strong>Percent Per Tick</strong><br>The percentage of the Power Resource that will be regenerated per point of Character Stat every tick that the character is not in combat.<br><strong>Amount Per Tick</strong><br>The amount of the Power Resource that will be regenerated per point of Character Stat every tick that the character is not in combat.<br><strong>Combat Percent Per Tick</strong><br>The percentage of the Power Resource that will be regenerated per point of Character Stat every tick that the character is in combat.<br><strong>Combat Amount Per Tick</strong><br>The amount of the Power Resource that will be regenerated per point of Character Stat every tick that the character is not in combat.</p> |

## Next Steps

* Customize [Character Classes](character-class.md) by adding [Stat Scaling Nodes](../shared-properties/stat-scaling-nodes.md) that give them custom stat budgets, primary to secondary conversions, primary to resource conversions, and power resource regeneration rates.
* Customize [Character Races](character-race.md) by adding [Stat Scaling Nodes](../shared-properties/stat-scaling-nodes.md) that give them custom stat budgets, primary to secondary conversions, primary to resource conversions, and power resource regeneration rates.
* Customize [Class Specializations](class-specialization.md) by adding [Stat Scaling Nodes](../shared-properties/stat-scaling-nodes.md) that give them custom stat budgets, primary to secondary conversions, primary to resource conversions, and power resource regeneration rates.
* Customize [Unit Profiles](unit-profile.md) by adding [Stat Scaling Nodes](../shared-properties/stat-scaling-nodes.md) that give them custom stat budgets, primary to secondary conversions, primary to resource conversions, and power resource regeneration rates.
* Customize [Unit Types](unit-type.md) by adding [Stat Scaling Nodes](../shared-properties/stat-scaling-nodes.md) that give them custom stat budgets, primary to secondary conversions, primary to resource conversions, and power resource regeneration rates.
