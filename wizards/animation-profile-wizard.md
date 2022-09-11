---
description: >-
  The Animation Profile Wizard will create an animation profile from a list of
  animations and optionally add the required events to attack animations.
---

# Animation Profile Wizard

{% embed url="https://youtu.be/alKWYpFfJeI" %}

## Accessing The Wizard

The Animation Profile Wizard requires that one of your game scenes with either a GameManager or SceneConfig object is open in the editor so that it can determine which game to install the content into.

The Animation Profile Wizard can be opened by clicking _Tools_ in the menu bar, and selecting _AnyRPG > Wizard > Animation Profile Wizard_.

![](<../.gitbook/assets/image (135).png>)

![](<../.gitbook/assets/image (106).png>)

## Options

| Name            | Description                                                                                                                                                                                                                                                |
| --------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Game Name       | The name of the game.  This will show on the main menu screen.The name of the game in your Unity project to install the template content in.  This will be automatically filled in if you have any scene with the GameManager or SceneConfig prefabs open. |
| Profile Name    | The name of the animation profile.  This is the name that will be called from abilities, weapons, unit prefab properties, etc.                                                                                                                             |
| Assign Priority | Determines whether clips added to the _Assign Clips_ property will be assigned as out of combat or in combat animations.                                                                                                                                   |
| Assign Clips    | Drag a list of animation clips into this list.  The wizard will attempt to assign them to the correct animations in the _Animations_ property based on their names.                                                                                        |
| Add Hit Events  | If true, any clips in the _Attack Clips_ list in the _Animations_ property that do not have a `Hit()` event will have one added.                                                                                                                           |
| Animations      | Lists of animations.  See [Animation Profile](../scriptable-objects/animation-profile.md) for a description of animation profile properties.                                                                                                               |

## Configuration

See [Animation Profile Configuration](../scriptable-objects/animation-profile.md#configuration).

## Content Created

After assigning the appropriate animations, click Create.

![](<../.gitbook/assets/image (110).png>)

### Scriptable Objects

#### Animation Profile

An [Animation Profile](../scriptable-objects/animation-profile.md) can be found at the _Resources/GameName/AnimationProfile_ folder.

![](<../.gitbook/assets/image (108).png>)

## Next Steps

See [Animation Profile Next Steps](../scriptable-objects/animation-profile.md#next-steps).
