---
description: >-
  The new character wizard helps you import character models and set them up as
  NPC or player characters.
---

# New Character Wizard

{% embed url="https://youtu.be/pAybYbYyE0A" %}

## Accessing the Wizard

The new character wizard requires that one of your game scenes with either a GameManager or SceneConfig object is open in the editor so that it can determine which game to install the content into.

The Template Content Wizard can be opened by clicking _Tools_ in the menu bar, and selecting _AnyRPG > Wizard > New Character Wizard_.

![](<../.gitbook/assets/image (62).png>)

![](<../.gitbook/assets/image (25).png>)

## Settings

| Name                            | Description                                                                                                                                                                                                                                                |
| ------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Game Name                       | The name of the game in your Unity project to install the template content in.  This will be automatically filled in if you have any scene with the GameManager or SceneConfig prefabs open.                                                               |
| Create Unit Spawn Node          | If true, a prefab that can spawn this character will be created.  This is useful if the character will be used as an enemy or NPC.                                                                                                                         |
| Set As Default Player Character | If true, the GameManager will be updated to use this character as the default player character.                                                                                                                                                            |
| Character Model                 | Drag an FBX or prefab into this slot, and that model will be used as the character model.                                                                                                                                                                  |
| Head Bone                       | The bone that the camera will look at when taking a picture for the unit frame.  This should be automatically filled in when the character model field is filled if it has a common name, but you can enter the bone name manually if has an unusual name. |
| Attachment Profile              | An attachment profile contains a mapping of English names such as "Left Hand" to actual bones for attaching weapons.  If the character is an UMA model, choose UMA, otherwise choose Humanoid.                                                             |
| Add Weapon Attachments          | If true, several prefabs that contain attachment points for all common weapon types will be added to the model.  This is not necessary for UMA characters.                                                                                                 |
| Left Hand Bone                  | The name of the bone to attach the left hand attachment prefab to.                                                                                                                                                                                         |
| Right Hand Bone                 | The name of the bone to attach the right hand attachment Prefab to.                                                                                                                                                                                        |
| Left Arm Bone                   | The name of the bone to attach the shield attachment to.                                                                                                                                                                                                   |
| Hip Bone                        | The name of the bone to attach the hip attachment prefab to.                                                                                                                                                                                               |
| Spine Bone                      | The name of the bone to attach the spine attachment prefab to.  This will also be used as the floating point in the Unit Profile; meaning when a character is floating in the water, everything below this bone will be submerged.                         |
| Character Name                  | For NPCs, the name that will show above the characters head.  For players, the name that will show in the character model selection screen when starting a new game.                                                                                       |
| Portrait Image                  | For players, the image that will show beside the character name in the character selection screen.                                                                                                                                                         |
| Animations                      | If this character has custom animations, enter them in this list to override the default character animations used by the system.                                                                                                                          |

## Running the Wizard

Once you have filled in all the settings, click _Create_.

![](<../.gitbook/assets/image (49).png>)

## Adjusting Weapon Attachments

Every character model is different and will have different dimensions and bone orientations.  You will need to adjust the weapon attachment to ensure they have the correct orientation so that weapons properly line up with the hip, spine, hands etc when sheathed or held.

Open the character prefab that can be found in the GameName/Prefab/Character folder.

![](<../.gitbook/assets/image (67).png>)

Find the attachments that have been added to the model.

![](<../.gitbook/assets/image (92).png>)

For each attachment, find the preview models included, and enable them so they are visible in the scene view.

![](<../.gitbook/assets/image (94).png>)

Rotate and move the attachments directly (not the preview models) until everything looks aligned properly on the character.

![](<../.gitbook/assets/image (85).png>)

In the case of the spine and hip attachments, you can move/rotate the attachments directly, or the pivots, whichever you prefer.

![](<../.gitbook/assets/image (72).png>)

![](<../.gitbook/assets/image (3) (1).png>)

Once everything looks properly aligned, you can disable the weapon previews and save your changes.  When the character equips weapons in-game they should now have the correct positioning and alignment.&#x20;

## Spawning NPC Characters In Game

If the character is an NPC, find the Unit Spawn Node under the GameName/Prefab/UnitSpawnNode/Character folder in your project and drag it into the location in the scene you want to spawn in.  When you start playing your game, the character will appear at that location.

![](<../.gitbook/assets/image (23).png>)

## Player Characters

If the character is a player character and you selected the set as default player character option, it will be set in the Game Manager.

If you forgot to set that option, you can add the unit profile name to the _Default Player Unit Profile Name_ field in the Game Manager.  If you want to have multiple choices of player models, you can add them to the _Character Creator Profile Names_ list.

![](<../.gitbook/assets/image (58).png>)

![](<../.gitbook/assets/image (73).png>)
