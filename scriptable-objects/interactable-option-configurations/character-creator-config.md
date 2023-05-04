---
description: >-
  A character creator config creates a character creator interactable option,
  which allows a character to open the character creator window, giving the
  player the ability to change their appearance.
---

# Character Creator Config

## Creation

To create a character creator config, find (or create) the _GameName/Resources/GameName/InteractableOptionConfig_ folder in the project tab and right click.  Choose _Create > AnyRPG > Interactable > CharacterCreatorConfig_.

![](<../../.gitbook/assets/image (4) (3).png>)

## Properties

| Name                | Description                                                                                                                                                                                                                                                                                                          |
| ------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Allow Gender Change | If true, the player can swap between male and female models, assuming the current [Race](../character-race.md) has options configured for both.                                                                                                                                                                      |
| Unit Profiles       | A list of valid [Unit Profiles](../unit-profile.md) that the character creator can edit.  If the list is empty, or the current player model is in the list, the current player model will be shown.  If the list is non-empty, and the current player model is not in the list, the first valid model will be shown. |

## Next Steps

* Add a character creator config to a [Unit Profile](../unit-profile.md) to allow the character to open the character creator window.
