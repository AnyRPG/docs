---
description: >-
  A voice profile contains lists of audio clips to play in response to certain
  actions being performed by a character.
---

# Voice Profile

## Creation

To create a voice profile, find (or create) the _GameName/Resources/GameName/VoiceProfile_ folder in the project tab and right click.  Choose _Create > AnyRPG > VoiceProfile_.

![](<../.gitbook/assets/image (11).png>)

## Properties

| Name                  | Description                                                                                                       |
| --------------------- | ----------------------------------------------------------------------------------------------------------------- |
| Aggro                 | List of sound files to choose from when an NPC that is not in combat aggros other characters.                     |
| Attack                | List of audio clips to choose from when character performs an attack on other characters.                         |
| Damage                | List of audio clips to choose from when character takes damage.                                                   |
| Jump                  | List of audio clips to choose from when character jumps.                                                          |
| Fall Damage           | List of audio clips to choose from when character takes fall damage.                                              |
| Death                 | List of audio clips to choose from when character dies.                                                           |
| Victory               | List of audio clips to choose from when the character kills another character.                                    |
| Start Interact        | List of audio clips to choose from when the character starts interacting.                                         |
| Start Vendor Interact | List of audio clips to choose from when the character starts interacting with a vendor.                           |
| Stop Interact         | List of audio clips to choose from when the character stops interacting (closes an interaction window).           |
| Stop Vendor Interact  | List of audio clips to choose from when the character stops interacting with a vendor (closes the vendor window). |

## Next Steps

* Add a voice profile to a [Unit Profile](unit-profile.md) to allow that character to use the audio clips.

