---
description: >-
  A combat strategy defines phases of a fight, which controls what abilities and
  buffs an AI character will use depending on their health.
---

# Combat Strategy

## Creation

To create a class specialization, find (or create) the _GameName/Resources/GameName/CombatStrategy_ folder in the project tab and right click.  Choose _Create > AnyRPG > Combat > CombatStrategy_.

![](<../.gitbook/assets/image (115).png>)

## Properties

| Name        | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| ----------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Phase Nodes | <p>A list of phases, defined by the health the AI has.<br><strong>Max Health Percent</strong><br>The phase will be started when the AI health drops to this level.<br><strong>Min Health Percent</strong><br>The phase will be ended when the AI health drops to this level.<br><strong>Phase Music Profile Name</strong><br>The <a href="audio-profile.md">Audio Profile</a> containing the links to the audio clips to play during the phase.<br><strong>Maintain Buff Names</strong><br>A list of <a href="abilities/">Abilities</a> to cast to buff the AI.<br><strong>Attack Ability Names</strong><br>A list of attack <a href="abilities/">Abilities</a> the AI will use against others during the phase.</p> |

## Next Steps

* Assign a combat strategy to a [Unit Profile](unit-profile.md).
