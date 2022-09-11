---
description: >-
  An attachment profile is a mapping of user-friendly bone names to actual bone
  names, and allows spell effects and equipment to be properly attached to
  characters with completely different bone names.
---

# Attachment Profile

## Creation

To create an attachment profile, find (or create) the _GameName/Resources/GameName/AttachmentProfile_ folder in the project tab and right click.  Choose _Create > AnyRPG > AttachmentProfile_.

![](<../.gitbook/assets/image (102).png>)

## Properties

| Name                   | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| ---------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Attachment Point Nodes | <p>A list of attachment point nodes, which map user friendly bone names to actual bone names.<br><strong>Node Name</strong><br>The user friendly bone name which is referred to in the attachment node of the equipment, spell effect, etc.<br><strong>Position</strong></p><p>The position any object will be attached at, relative to the <em>Target Bone</em>.<br><strong>Rotation Is Global</strong><br>If true, the rotation property will be relative to world space.<br><strong>Rotation</strong><br>The rotation of the object being attached, relative to the target bone, or global if the <em>Rotation Is Global property</em> is true.<br><strong>Scale</strong><br>The scale of the object being attached.<br><strong>Target Bone</strong><br>The actual bone in the character/unit hierarchy that the object will be attached to.</p> |

## Next Steps

* Refer to an attachment profile in the _Ability Object List_ field of an [Ability Effect](ability-effects/).
* Refer to an attachment profile in the _Holdable Object List_ field of an [Ability](abilities/).
* Refer to an attachment profile in the _Holdable Object List_ field of a piece of [Equipment](items/equipment.md).
* Refer to an attachment profile in the _Ability Animation Object List_ or _Ability Object List_ fields of a Weapon Skill.
