---
description: >-
  An equipment model profile contains information about how gear will be
  displayed when an item is equipped.
---

# Equipment Model Profile

## Creation

To create an equipment model profile, find (or create) the _GameName/Resources/GameName/EquipmentModelProfile_ folder (or any subfolder) in the project tab and right click.  Choose _Create > AnyRPG > EquipmentModelProfile_.

![](<../.gitbook/assets/image (4) (2) (1).png>)

## Properties

UMA Equipment Model properties will be used when the character model is configured as an UMA model.

| Name             | Description                                                                                                                                            |
| ---------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Equipment Models | A list of equipment model providers that will be used to display the gear, depending on what equipment model is used.  Valid options are listed below. |

### UMAEquipmentModel

UMA Equipment Model properties will be used when the character model is configured as an UMA model.

| Name          | Description                                                                                                                                                                                                                                                            |
| ------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| UMA Recipes   | A list of UMA recipes that can potentially be displayed.  The recipes that match the target unit's UMA race will be displayed.  If multiple recipes that match the race can be applied to the same slot, the last one will always be used.                             |
| Shared Colors | <p>A list of UMA shared color data defining which colors will be shown for each defined shared color name that exists on the UMA recipe.<br><strong>Shared Colorname</strong><br>The name of an UMA shared color.<br><strong>Color</strong><br>A color to be used.</p> |

### SwappableMeshEquipmentModel

Swappable Mesh Equipment Model properties will be used when the character model is configured as a swappable mesh model.  It contains a list of mesh option names to apply.

| Name        | Description                                                                                                                       |
| ----------- | --------------------------------------------------------------------------------------------------------------------------------- |
| Group Name  | The name of a mesh option group to configure.                                                                                     |
| Option Name | The name of the mesh option to activate for the group.  Note that this is the friendly name, and not the name of the actual mesh. |

### PrefabEquipmentModel

Prefab Equipment Model properties will be used no matter what model type is configured, because they attach objects to bones and aren't reliant on specific model configuration.

| Name                 | Description                                                                                                                           |
| -------------------- | ------------------------------------------------------------------------------------------------------------------------------------- |
| Holdable Object List | A list of holdable object properties.  These are the same properties that can be found on [Equipment](items/equipment.md#properties). |

## Next Steps

* Add an equipment model profile to any [Equipment](items/equipment.md).
