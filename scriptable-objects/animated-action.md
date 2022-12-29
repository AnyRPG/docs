---
description: Animated Actions allow the character to perform any animation.
---

# Animated Action

{% embed url="https://youtu.be/UR4pH60Rluo" %}

## Creation

To create an animated action, find (or create) the _GameName/Resources/GameName/AnimatedAction_ folder in the project tab and right click.  Choose _Create > AnyRPG > AnimatedAction_.

![](<../.gitbook/assets/image (99) (1) (1).png>)

## Properties

| Name                   | Description                                                                                                                                                                                  |
| ---------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Animation Clip         | The animation that the character will play when this action is performed.                                                                                                                    |
| Animation Profile Name | An animation profile containing animations.  The character will play the first cast clip when the action is performed.  This property is only used if the _AnimationClip_ property is empty. |
| Casting Audio Profile  | The name of an audio profile containing an audio file to play when the action is performed.                                                                                                  |
| Holdable Object List   | A List of prefab profiles to spawn when the action is performed.                                                                                                                             |

## Usage

Animated actions can be used in the following scriptable objects.

* [ActionEffectItem](items/action-effect-item.md)
* [PowerResourcePotion](items/power-resource-potion.md)
