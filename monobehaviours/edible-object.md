---
description: >-
  An Edible Object Script is used on an object that should appear to be eaten or
  drunk by swapping out 3d models over a certain time period.
---

# Edible Object

## Usage

An Edible Object has no 3d model attached directly to the GameObject.  Instead it has multiple 3d models as child GameObjects.  The first object should be the model to use when the object is full. As many objects as are desired can be added after that to represent the different stages of eating or drinking until the last object, representing a fully eaten or used up model.

The first object should be active in the heirarchy by default, and all others should be non active.  The active status of each will be managed by the script as it progresses through showing them.

## Properties

| Name              | Description                                                    |
| ----------------- | -------------------------------------------------------------- |
| Interval          | The time in seconds between changing to the next object.       |
| Keep Last Visible | If true, the last object will stay visible after its interval. |

## Dependencies

* One or more child GameObjects should exist for the script to cycle through as the object is consumed.
