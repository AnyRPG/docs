---
description: >-
  A currency group is a collection of currencies that can be automatically
  converted using defined exchange rates, similar to dollars and cents in the
  real world.
---

# Currency Group

## Creation

To create a currency group, find (or create) the _GameName/Resources/GameName/CurrencyGroup_ folder in the project tab and right click.  Choose _Create > AnyRPG > Currencies > CurrencyGroup_.

![](<../.gitbook/assets/image (132).png>)

## Properties

| Name                 | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| -------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Base Currency Name   | The name of the smallest unit of [Currency](currency.md) in this group.                                                                                                                                                                                                                                                                                                                                                                                                 |
| Base Currency        | A direct link to the scriptable object that defines the smallest unit of [Currency](currency.md) in this group.                                                                                                                                                                                                                                                                                                                                                         |
| Currency Group Rates | <p>A list of currencies and exchange rates relative to the base <a href="currency.md">Currency</a>.<br><strong>Currency Name</strong><br>The name of the unit of currency.<br><strong>Currency</strong><br>A direct link to the scriptable object that defines the unit of currency.<br><strong>Base Multiple</strong><br>The number of units of the base <a href="currency.md">Currency</a> that make up a single unit of this <a href="currency.md">Currency</a>.</p> |

## Next Steps

* Define a currency group as the default currency group in the System Configuration Manager, which will display that currency group in vendor windows when buying or selling items.
