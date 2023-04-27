---
description: >-
  The New Equipment Set Wizard will create equipment, an equipment set for the
  equipment, an optional vendor collection, and an optional loot table.
---

# New Equipment Set Wizard

{% embed url="https://youtu.be/cxnt6oUNeWY" %}

## Accessing The Wizard

The New Equipment Set Wizard requires that one of your game scenes with either a GameManager or SceneConfig object is open in the editor so that it can determine which game to install the content into.  There is an UMA version, and a standard (mecanim) version of the wizard.

The standard New Equipment Set Wizard can be opened by clicking _Tools_ in the menu bar, and selecting _AnyRPG > Wizard > New Equipment Set Wizard_.

The UMA New Equipment Set Wizard can be opened by clicking _Tools_ in the menu bar, and selecting _AnyRPG > Wizard > UMA > New Equipment Set Wizard_.

![](<../.gitbook/assets/image (74).png>)

![](<../.gitbook/assets/image (20) (1).png>)

## Options

| Name                                                                                                    | Description                                                                                                                                                                                                                                                                                                                                        |
| ------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Game Name                                                                                               | The name of the game.  This will show on the main menu screen.The name of the game in your Unity project to install the template content in.  This will be automatically filled in if you have any scene with the GameManager or SceneConfig prefabs open.                                                                                         |
| Equipment Set Name                                                                                      | The name of the equipment set. If set bonuses are used, this name will show in the mouseover tooltip for equipment that is part of this set.                                                                                                                                                                                                       |
| Use Set Bonuses                                                                                         | If true, equipment that is part of this set will show which pieces of the set are equipped in the mouseover tooltip.  The character can also have different status effects applied depending on how many pieces of the set are equipped.                                                                                                           |
| Set Bonuses                                                                                             | A list of status effects to apply depending on how many pieces of the equipment set are equipped.  Each line represents the number of pieces that must be equipped, so blank lines must be provided inbetween bonuses if not every extra piece equipped is providing a bonus.                                                                      |
| Require Armor Class                                                                                     | If true, the character must know the armor class listed to be able to equip the item.                                                                                                                                                                                                                                                              |
| Armor Class                                                                                             | If an armor class is provided, the equipment will have the armor value determined based on what the default is for that armor class.  This can also affect whether or not the character is able to equip the item.                                                                                                                                 |
| Create Vendor Collection                                                                                | If true, a vendor collection will be created with all the equipment so that it can be purchased from a vendor.                                                                                                                                                                                                                                     |
| Vendor Collection Name                                                                                  | The display name of the vendor collection in the vendor window.                                                                                                                                                                                                                                                                                    |
| Create Loot Table                                                                                       | If true, a loot table will be created that can be assigned to enemies, allowing this equipment to be gained as a reward for defeating them.                                                                                                                                                                                                        |
| Item Quality                                                                                            | The item quality that will be assigned to all equipment in this set.                                                                                                                                                                                                                                                                               |
| Random Item Quality                                                                                     | If true, the equipment will have a random item quality assigned when looted, crafted, or purchased.                                                                                                                                                                                                                                                |
| Dynamic Level                                                                                           | If true, the equipment will scale up to match the character level.                                                                                                                                                                                                                                                                                 |
| Freeze Drop Level                                                                                       | If true, and dynamic level is set, the equipment will be fixed at the level the character was when the item was looted, crafted, or purchased.                                                                                                                                                                                                     |
| Level Cap                                                                                               | If this is set to anything other than zero, equipment with a dynamic level will have this value as the maximum level it can scale to or freeze at.                                                                                                                                                                                                 |
| Item Level                                                                                              | If dynamic level is false, the equipment will have this fixed level.                                                                                                                                                                                                                                                                               |
| Use Level                                                                                               | The level the character must be to equip this equipment.                                                                                                                                                                                                                                                                                           |
| Primary Stats                                                                                           | A list of primary stats that will apply to each piece of equipment.                                                                                                                                                                                                                                                                                |
| Random Secondary Stats                                                                                  | If true, the secondary stats will be chosen randomly from the list, up to the limit defined by the item quality.                                                                                                                                                                                                                                   |
| Secondary Stats                                                                                         | A list of secondary stats that will apply to each piece of equipment.                                                                                                                                                                                                                                                                              |
| Use \<PieceType>                                                                                        | For each type of equipment, if this is true, equipment will be created.                                                                                                                                                                                                                                                                            |
| \<PieceType> Name                                                                                       | For each type of equipment, the display name of that piece.                                                                                                                                                                                                                                                                                        |
| \<PieceType> Icon                                                                                       | For each type of equipment, the icon that will be used in the inventory, on the character window, etc.                                                                                                                                                                                                                                             |
| <p>&#x3C;PieceType> UMA Recipes<br><strong>(Only applies to the UMA version of the wizard)</strong></p> | Optional.  For each type of equipment, UMA recipes that will determine which UMA gear is applied to UMA characters when the gear is equipped.  Provide one recipe here for each race (male/female), and the correct item for the current race will be applied.  If this list is empty, or the character is not UMA, these values will be ignored.  |

## Content Created

After choosing the appropriate options for the scene, click Create.

![](<../.gitbook/assets/image (37).png>)

![](<../.gitbook/assets/image (69).png>)

### Scriptable Objects

#### Equipment Set

An equipment set can be found at the _Resources/GameName/EquipmentSet_ folder. It defines the equipment that belongs to the set, and any set bonuses.

![](<../.gitbook/assets/image (14) (1).png>)

![](<../.gitbook/assets/image (44).png>)

#### Equipment

Equipment can be found in the _Resources/GameName/Item/Equipment/Armor_ folder.  These objects contain all the information for each individual piece of equipment.

![](<../.gitbook/assets/image (4) (1) (1) (1).png>)

#### Vendor Collection

If selected, a vendor collection can be found in the _Resources/GameName/VendorCollection_ folder.  This can be added to a vendor to allow the purchase of the equipment.

![](<../.gitbook/assets/image (88).png>)

#### Loot Table

If selected, a loot table can be found in the _Resources/GameName/LootTable_ folder.  This can be added to a LootableCharacter interactable option on any character to allow the equipment to be looted when the character is defeated in combat.

![](<../.gitbook/assets/image (18) (1).png>)

## Next Steps

### Assign Gear to a Class or Specialization

If you want a character class or specialization to start new games wearing the equipment, you can assign it to the class or specialization as starting equipment.

![](<../.gitbook/assets/image (113).png>)

### Make Gear Purchasable

You can add the gear to a vendor by adding it to the _Vendor Collection Names_ list on the _VendorProps Interactable Option_ on the Unit Profile scriptable object of any NPC.  A Sample vendor can be installed by using the [Template Content Wizard](template-content-wizard.md) and searching for _Vendor NPC_.

![](<../.gitbook/assets/image (130).png>)

![](<../.gitbook/assets/image (124).png>)

### Make Gear Lootable

Add a _LootableCharacterProps_ to any _Unit Profile_ and add the new loot table for this equipment to the Loot Table Names list.  When you defeat that character in combat, you will have a chance to loot one of the items.

![](<../.gitbook/assets/image (103).png>)
