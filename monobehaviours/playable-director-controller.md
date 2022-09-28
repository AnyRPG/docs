---
description: >-
  A playable director controller is attached to a prefab that contains a
  Playable Director component with a Unity Timeline, and is responsible for
  playing the timeline.
---

# Playable Director Controller

## Properties

A playable director controller has no properties.

## Usage

A playable director will be triggered to play its timeline when the name of the timeline matches the _TimeLine Name_ field in a [Cutscene](../scriptable-objects/cutscene.md).  The [Cutscene](../scriptable-objects/cutscene.md) can be started automatically upon loading the scene by the [Scene Node](../scriptable-objects/scene-node.md), or triggered manually through a [Cutscene Interactable](../scriptable-objects/interactable-option-configurations/cutscene-config.md).

## Dependencies

* A PlaybleDirector component should be attached to the same prefab.
