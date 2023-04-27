---
description: >-
  A swappable mesh model profile contains all of the information about a
  swappable mesh model so that the character editor and equipment can properly
  enable or disable the correct meshes.
---

# Swappable Mesh Model Profile

## Creation

To create a swappable mesh model profile, find (or create) the _GameName/Resources/GameName/SwappableMeshModelProfile_ folder in the project tab and right click.  Choose _Create > AnyRPG > SwappableMeshModelProfile_.

![](<../.gitbook/assets/image (5).png>)

## Properties

Swappable mesh model profiles, contain one property, Model Options, with the following fields.

| Name           | Description                                                                                     |
| -------------- | ----------------------------------------------------------------------------------------------- |
| Mesh Groups    | A list of [Mesh Group Properties](swappable-mesh-model-profile.md#mesh-group-properties).       |
| Group Defaults | A list of [Group Default Properties](swappable-mesh-model-profile.md#group-default-properties). |

### Mesh Group Properties

Mesh group properties contains a list of mesh group configurations, with the following fields.

| Name        | Description                                                                                                                                                                                                                  |
| ----------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Group Name  | The name of the group that should be shown in the character creator.                                                                                                                                                         |
| Hidden      | If true, the player will not see this group in the character appearance editor.                                                                                                                                              |
| Optional    | If true, the player can choose to not display any meshes from this group.                                                                                                                                                    |
| Display As  | <p><strong>List</strong><br>Options should be displayed vertically as text with an optional image beside it.<br><strong>Grid</strong><br>Options should be displayed as a grid of images, with no text.</p>                  |
| Hides Group | If this field is not empty, and any mesh from this group is chosen, the mesh group named in this field will be disabled and not shown on the character.  This can be useful if you want (for example) a helmet to hide hair. |
| Meshes      | A list of [Mesh Options](swappable-mesh-model-profile.md#mesh-options).                                                                                                                                                      |

#### Mesh Options

Defines the friendly (display name) of a mesh, and the name of the GameObject the mesh is located on.

| Name         | Description                                                                 |
| ------------ | --------------------------------------------------------------------------- |
| Display Name | The friendly name of the mesh that should be shown in the character editor. |
| Icon         | An image that will be shown in the character editor for this option.        |
| Mesh Name    | The name of the GameObject the mesh is attached to.                         |

### Group Default Properties

Group default properties define which option should be active for which group when no other option is chosen.  These are required so that some mesh is showing, instead of all meshes being disabled.

| Name        | Description                                                                |
| ----------- | -------------------------------------------------------------------------- |
| Group Name  | The name of the Option Group that this default applies to.                 |
| Option Name | The friendly name of the mesh option that should be visible for the group. |

## Next Steps

* Add a swappable mesh model profile to a [Unit Prefab Profile](unit-prefab-profile.md).
