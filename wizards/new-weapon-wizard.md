---
description: >-
  The new weapon wizard creates weapon items and special weapon handle prefabs
  that ensure a weapon is in the correct orientation when equipped.
---

# New Weapon Wizard

{% embed url="https://youtu.be/xnlPVCeMfnE" %}

## Accessing the Wizard

The new weapon wizard requires that one of your game scenes with either a GameManager or SceneConfig object is open in the editor so that it can determine which game to install the content into.

The New Weapon Wizard can be opened by clicking _Tools_ in the menu bar, and selecting _AnyRPG > Wizard > New Weapon Wizard_.

![](<../.gitbook/assets/image (75).png>)

![](<../.gitbook/assets/image (31).png>)

## Settings

| Name                         | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| ---------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Game Name                    | The name of the game in your Unity project to install the template content in.  This will be automatically filled in if you have any scene with the GameManager or SceneConfig prefabs open.                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| Weapon Prefab                | Drag an FBX or prefab into this slot, and that model will be used as the weapon model.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| Weapon Name                  | The weapon name that will appear in tooltips, vendor lists, loot windows, etc.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| Icon                         | The image to be used to represent the weapon in the inventory, character screen, vendor lists, loot windows, etc.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| Weapon Slot Type             | <p><strong>Main Hand Only</strong><br>This weapon can only be equipped in the main hand slot.  Any other valid weapon can still be equipped in the off hand slot.<br><strong>Off Hand Only</strong><br>This weapon can only be equipped in the off hand slot.  Any other valid weapon can still be equipped in the main hand slot.<br><strong>Any Hand</strong><br>This weapon can be equipped in the main hand or off hand slot.  Any other weapon can be equipped in the other slot.<br><strong>Two Hand</strong><br>This weapon takes up both hands.  It will appear in the main hand slot, and remove any other weapon that is equipped in the off hand slot.</p> |
| Weapon Type                  | The weapon type setting controls which animations and effects will be played when the weapon is used in combat.   It will also determine which attachment point the weapon is attached to when it is sheathed on the character.                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| Asymmetrical Weapon          | Most weapons are symmetrical and will look the same if held in the main hand or off hand.  For asymmetrical weapons such as claws, this should be set to true and separate handle prefabs will be created for the left and right hands.                                                                                                                                                                                                                                                                                                                                                                                                                               |
| Projectile Name              | The base name that will be assigned for the projectile prefabs and prefab profiles. Leave this blank if the weapon is not ranged.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| Projectile Prefab            | A Prefab to use for the projectile if this is a ranged weapon.  Leave this blank if the weapon is not ranged.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| Use Projectile In Animations | For ranged weapons only.  Should the projectile be shown during attack animations such as pulling an arrow from the quiver and drawing the bow string.  This should not be checked if the ranged weapon does not have a special projectile prefab.  In that case, the default projectile settings from the weapon type will apply.                                                                                                                                                                                                                                                                                                                                    |
| Use Projectile In Abilities  | For ranged weapons only.  Should the projectile be shown during flight to the target after the attack animation is finished. This should not be checked if the ranged weapon does not have a special projectile prefab.  In that case, the default projectile settings from the weapon type will apply.                                                                                                                                                                                                                                                                                                                                                               |

## Content Created

After choosing all the settings, click Create to run the wizard.

![](<../.gitbook/assets/image (82).png>)

The following content will be created.

### Weapon Handle Prefab

Weapon handle, projectile handle, and projectile prefabs can be found in the _GameName/Prefab/Handle/Weapon_ folder.  The weapon handle is a convenient prefab that contains the weapon model along with a handle that is a visual indicator to help set the correct scale (size) and rotation so that the weapon will look good when held or sheathed.

![](<../.gitbook/assets/image (52).png>)

### Prefab Profiles

Prefab profiles, a type of scriptable object that contains the link to the prefab, can be found in the _Gamename/Resources/GameName/PrefabProfile/Weapon_ folder.

### Weapon Item

The weapon item Scriptable Object can be found in the _GameName/Resources/GameName/Item/Equipment/Weapon_ folder.

![](<../.gitbook/assets/image (63).png>)

## Adjusting the Weapon Handle

### Weapons

The handle object in the weapon handle prefab is a visual indicator that shows what the size and orientation of the weapon should be when gripped in a character's hand. The blue (z) axis is the forward direction of the hand, the yellow (y) axis is the top of the hand, and the red (x) axis is the right side of the hand.

![](<../.gitbook/assets/image (51).png>)

Set the scale of the weapon model larger or smaller if necessary until the handle looks about the right size in relation to it.  You can imagine that if gripped, the handle would fit perfectly in a fist.

Set the rotation and position of the weapon model so that it would look correct if the handle was gripped in a hand with the character's arm straight in front of them.

![](<../.gitbook/assets/image (43).png>)

Disable the Handle object so that it is not visible, and save the changes to the weapon handle prefab.

### Projectiles

The steps for projectiles are similar to the steps for weapons.  When you open the prefab, you will see a sample projectile that represents the correct position and rotation.

![](<../.gitbook/assets/image (80).png>)

Align the projectile so it matches the position and rotation of the sample projectile, then disable all other objects in the prefab so only the projectile is visible, and save the changes.\
![](<../.gitbook/assets/image (56).png>)

## Next Steps

To make the weapon available in game you may want to take any of the following actions.

* Configure the weapon by adding an item quality, setting a purchase price, or requiring a specific weapon skill to equip the weapon.
* Add the weapon to the default equipment for a character class or specialization.
* Add the weapon to a vendor collection and make it available on a vendor to purchase.
* Add the weapon to a loot table so it can be obtained by defeating an enemy.
