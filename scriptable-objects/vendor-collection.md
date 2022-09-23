---
description: A vendor collection is a list of items that can be sold by a vendor.
---

# Vendor Collection

## Creation

To create a vendor collection, find (or create) the _GameName/Resources/GameName/VendorCollection_ folder in the project tab and right click.  Choose _Create > AnyRPG > VendorCollection_.

![](<../.gitbook/assets/image (7).png>)

## Properties

Vendor Collections have a single property, _Vendor Items_, which is a list with each element having the following fields.

| Name              | Description                                                                                                                                                       |
| ----------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Item Name         | The name of an [Item](items/) that can be purchased.                                                                                                              |
| Quantity          | The amount of this [Item](items/) that can be purchased.  This field is ignored if _Unlimited_ is true.                                                           |
| Unlimited         | If true, there is no limit to the number of this [Item](items/) that can be purchased.                                                                            |
| Item Quality Name | The name of an [Item Quality](item-quality.md).  If this field is not empty, the [Item](items/) purchased will be of this quality instead of its default quality. |

## Next Steps

* Add a vendor collection to a [Vendor](interactable-option-configurations/vendor-config.md).
