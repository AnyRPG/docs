---
description: >-
  A status effect group defines similar status effects, and prevents a character
  from having more than one effect from the group active at the same time.
---

# Status Effect Group

## Creation

To create a status effect group, find (or create) the _GameName/Resources/GameName/StatusEffectGroup_ folder in the project tab and right click.  Choose _Create > AnyRPG > StatusEffectGroup_.

![](<../.gitbook/assets/image (7).png>)

## Properties

| Name             | Description                                                                                                                                                                                                                                                                |
| ---------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Exclusive Option | <p>An enumeration of options controlling how effects are blocked are overwritten.<br><strong>Last</strong><br>The most recent effect always overwrites any earlier effects.<br><strong>First</strong><br>The first effect blocks any other effects from being applied.</p> |

## Next Steps

* Add a [Status Effect](ability-effects/status-effect.md) to a group by filling in its _Status Effect Group_ field.
