---
description: A dropped item can be picked up.
---

# Dropped Item

{% hint style="info" %}
A dropped item is a special type of interactable used by the system when players drop items on the ground.  It is not designed to be placed in a scene, as its data is saved as ephemeral, and removed when the item is picked up and added to the inventory.  There is a special prefab already configured for this purpose linked in the system, and under normal circumstances, you would never need to directly add this to any interactable.
{% endhint %}

## Properties

An Dropped item does not have any properties other than the properties shared by all [Interactable Option Configs](../../scriptable-objects/interactable-option-configurations/#properties).

## Dependencies

* An Interactable Monobehavior must be on the same GameObject.
