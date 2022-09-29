---
description: >-
  A Persistent Object will have its position saved, so when a game is loaded,
  the object appears in the last place it moved to, instead of its default
  position in the scene.
---

# Persistent Object

## Properties

A Persistent Object contains a single property, _Persistent Object Component_, with the following properties.

| Name                    | Description                                                                                                                                                                                         |
| ----------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Persist Object Position | If true, the object position is saved so that the object will spawn at the saved location next time a game is loaded. This requires at least one of _Save On Level Unload_, or _Save On Game Save_. |
| Save On Level Unload    | If true, the position will be saved when a level is unloaded.                                                                                                                                       |
| Save On Game Save       | If true, the position will be saved when the game is saved.                                                                                                                                         |

## Dependencies

* A UUID script is required, which is automatically added upon adding the Persistent Object script.
