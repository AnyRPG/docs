---
description: >-
  A quest giver config creates a quest giver interactable option, allowing the
  player to start or turn in quests when they interact with the character.
---

# Quest Giver Config

## Creation

To create a quest giver config, find (or create) the _GameName/Resources/GameName/InteractableOptionConfig_ folder in the project tab and right click.  Choose _Create > AnyRPG > Interactable > QuestGiverConfig_.

![](<../../.gitbook/assets/image (8).png>)

## Properties

| Name                      | Description                                                                                                                                                                  |
| ------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Quests                    | A list of [Quests](../quest.md) that can be started or turned in.                                                                                                            |
| Quest Giver Profile Names | A list of names of [Quest Giver Profiles](../quest-giver-profile.md), which contain shared lists of [Quests](../quest.md) that can be re-used across different quest givers. |

## Next Steps

* Add a quest giver config to a [Unit Profile](../unit-profile.md) to allow starting and turning in quests by interacting with the character.
