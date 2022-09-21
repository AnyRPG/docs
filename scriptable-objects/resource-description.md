---
description: >-
  A Resource Description is a multi-purpose file that can be used to overwrite
  the display names and icons of other types of scriptable objects.  It can also
  be used to support different languages.
---

# Resource Description

## Creation

To create a resource description, find (or create) the _GameName/Resources/GameName/ResourceDescription_ folder in the project tab and right click.  Choose _Create > AnyRPG > ResourceDescription_.

![](../.gitbook/assets/image.png)

## Properties

| Name                  | Description                                                                                                                                               |
| --------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Resource Name         | This field is generally used as the lookup name (database key) when looking up a resource description.                                                    |
| Display Name          | The text in this field will override the _Display Name_ field of whatever scriptable object this resource description is being used for.                  |
| Icon                  | The image linked in this field will override the _Icon_ field of whatever scriptable object this resource description is being used for.                  |
| Icon Background Image | The image linked in this field will override the _Icon Background Image_ field of whatever scriptable object this resource description is being used for. |
| Description           | The text in this field will override the _Description_ field of whatever scriptable object this resource description is being used for.                   |

## Next Steps

* Use a resource description to override settings in [Items](items/).
* Use a resource description to override settings in [Abilities](abilities/).
* Use a resource description to override the display name of a scene file.
