---
description: >-
  A storage container allows the player to store items that will be persisted
  with the game save data.
---

# Storage Container Config

## Creation

To create a storage container config, find (or create) the _GameName/Resources/GameName/InteractableOptionConfig_ folder in the project tab and right click.  Choose _Create > AnyRPG > Interactable > StorageContainerConfig_.

## Properties

| Name                 | Description                                                                                                                                                                                                                                                |
| -------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Number Of Slots      | The number of item slots in the container.                                                                                                                                                                                                                 |
| Container Loot Table | The loot table that will be used to generate the contents of the container if it is empty when opened. This is only used if the container has not been opened before. Once the container is opened, the contents are saved and this loot table is ignored. |

## Next Steps

* Add a storage container config to an Interactable to allow the player to teleport to another scene by interacting with it.
