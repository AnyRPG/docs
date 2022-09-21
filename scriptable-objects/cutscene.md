---
description: >-
  A cutscene is a convenient way of displaying important events by moving the
  camera to predefined points, showing subtitles, and optionally triggering a
  timeline to make objects perform actions.
---

# Cutscene

## Creation

To create a cutscene, find (or create) the _GameName/Resources/GameName/Cutscene_ folder in the project tab and right click.  Choose _Create > AnyRPG > Cutscene_.

![](<../.gitbook/assets/image (114) (1).png>)

## Properties

| Name                       | Description                                                                                                       |
| -------------------------- | ----------------------------------------------------------------------------------------------------------------- |
| Repeatable                 | If true, this cutscene can be played more than once.                                                              |
| Require Player Unit Spawn  | If true, the player unit must be spawned in the world for this cutscene to play.                                  |
| Use Default Faction Colors | If true, player faction will be ignored, and default faction relationship colors will be used for health bars.    |
| Timeline Name              | The name of a Unity Timeline to trigger when this cutscene is played.                                             |
| Load Scene Name            | The name of a scene to load to play this cutscene.                                                                |
| Unload Scene On End        | If true, the scene that was active before the cutscene played will be loaded when the cutscene ends.              |
| Auto Advance Subtitles     | <p>If true, the subtitles will be played automatically.<br>If false, the timeline will control the subtitles.</p> |
| Subtitle Properties        | [Subtitle Properties](cutscene.md#undefined)                                                                      |

### Subtitle Properties

| Name               | Description                                                                                                                                                                                                                                                                                                           |
| ------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Audio Profile Name | The name of an audio profile to play when the cutscene is started.                                                                                                                                                                                                                                                    |
| Subtitle Nodes     | <p>A list of subtitle text and times.<br><strong>Start Time</strong><br>The time, in seconds after the start of the cutscene, to show the text.<br><strong>Show Time</strong><br>The time, in seconds, that the text should be active after being shown.<br><strong>Description</strong><br>The text to be shown.</p> |

## Next Steps

* Configure a [Scene Node](scene-node.md) to automatically play a cutscene when the scene loads.
* Configure a [Cutscene Interactable](interactable-option-configurations/cutscene-config.md) option to play a cutscene when interacted with.
