---
description: >-
  A unit prefab profile contains information needed to configure the GameObject
  prefab that represents the character model for any character.
---

# Unit Prefab Profile

## Creation

To create a unit prefab profile, find (or create) the _GameName/Resources/GameName/UnitPrefabProfile_ folder in the project tab and right click.  Choose _Create > AnyRPG > UnitPrefabProfile_.

![](<../.gitbook/assets/image (3) (3).png>)

## Properties

| Name                          | Description                                                                                                                                                                                 |
| ----------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Unit Prefab                   | A link to a prefab that will be used for the character unit.  The unit prefab does not have to, but can optionally, include a model.                                                        |
| Model Prefab                  | A link to a prefab that will be used for the character model if the model is separate from the _Unit Prefab_.                                                                               |
| Model Provider                |                                                                                                                                                                                             |
| Animation Profile Name        | The name of an [Animation Profile](animation-profile.md) that will be used for the model animations.                                                                                        |
| Use Inline Animation Props    | If true, the _Animation Props_ field will be used for animation properties, instead of a shared [Animation Profile](animation-profile.md).                                                  |
| Animation Props               | Inline properties of an [Animation Profile](animation-profile.md).                                                                                                                          |
| Rotate Model                  | If true, the model will be rotated to face in the direction of travel.  This option should be used if no strafe animations exist for the model.                                             |
| Name Plate Props              | Nameplate, unit frame, and unit preview settings.  See [Name Plate Properties](unit-prefab-profile.md#properties-1).                                                                        |
| Position                      | If being used as a mount, the Vector3 position in relation to the _Target Bone_ the character will be mounted to when riding.                                                               |
| Rotation Is Global            | If true, and being used as a mount, the value in the _Rotation_ field will be considered global (relative to world space) instead of local.                                                 |
| Rotation                      | If being used as a mount, the Vector3 rotation in relation to the _Target Bone_ the character will be mounted to when riding.                                                               |
| Scale                         | If being used as a mount, the Vector3 scale of the character when riding.                                                                                                                   |
| Target Bone                   | If being used as a mount, the bone the character will be attached to when riding.                                                                                                           |
| Attachment Profile Name       | The [Attachment Profile](attachment-profile.md) used to lookup actual bone names when attaching prefabs (holdable objects) to the character model.                                          |
| Float Height                  | When floating in water, the height from the bottom of the character that the water line will sit at.                                                                                        |
| Add Float Height To Transform | If true, the height of the _Float Transform_ will be added to the _Float Height_. If false, the _Float Transform_ height will replace the _Float Height_ if the _Float Transform_ is found. |
| Float Transform               | The name of a bone that should be used for the water line when floating.                                                                                                                    |

### Name Plate Properties

| Name                                | Description                                                                                                                                                     |
| ----------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Display Name                        | The name that is printed on the nameplate above the character model. This value will also override whatever is set for the interactable mouseover display name. |
| Suppress Name Plate                 | If true, no nameplate will be shown above this character.                                                                                                       |
| Suppress Faction                    | If true, the faction will not be shown on the nameplate.                                                                                                        |
| Override Nameplate Position         | If true, the nameplate position will be shown at the manual value in the _Name Plate Position_ field.                                                           |
| Use Snap Shot                       | If true, a snapshot of the target will be used.  If false, the [Unit Profile](unit-profile.md) image will be used.                                              |
| Unit Frame Target                   | The name of a bone that the camera will look at when taking a snapshot for the unit frame.                                                                      |
| Unit Frame Camera Look Offset       | Any Vector3 offset that the camera will look at relative to the _Unit Frame Target_.                                                                            |
| Unit Frame Camera Position Offset   | The position of the unit frame camera relative to the _Unit Frame Target_.                                                                                      |
| Unit Preview Target                 | The name of a bone that the camera will look when displaying the character in a full body unit preview window.                                                  |
| Unit Preview Camera Look Offset     | Any Vector3 offset that the camera will look at relative to the _Unit Preview Target_.                                                                          |
| Unit Preview Camera Position Offset | The position of the unit preview camera relative to the _Unit Preview Target_.                                                                                  |

### Model Provider Properties

Currently, there are 2 model providers: UMAModelProvider and SwappableMeshModelProvider.  The UMA model provider can be used on UMA units, and the swappable mesh model provider can be used on units that contain multiple meshes that can be enabled or disabled to change appearance.

#### UMAModelProvider Properties

| Name               | Description                                                                                      |
| ------------------ | ------------------------------------------------------------------------------------------------ |
| Use Inline Options | If true, the options in the _Inline Options_ field will be used instead of the _Shared Options_. |
| Inline Options     | [UMA Model Profile Properties](uma-model-profile.md#properties).                                 |
| Shared Options     | The name of an [UMA Model Profile](uma-model-profile.md).                                        |

#### SwappableMeshModelProvider Properties

| Name               | Description                                                                                      |
| ------------------ | ------------------------------------------------------------------------------------------------ |
| Use Inline Options | If true, the options in the _Inline Options_ field will be used instead of the _Shared Options_. |
| Inline Options     | [Swappable Mesh Model Profile Properties](swappable-mesh-model-profile.md#properties).           |
| Shared Options     | The name of a [Swappable Mesh Model Profile](swappable-mesh-model-profile.md).                   |

## Next Steps

* Add a unit prefab profile to a [Unit Profile](unit-profile.md).
