---
description: >-
  The Add UMA Support Wizard add UMA support to any game that does not yet have
  it.
---

# Add  UMA Support Wizard

## Accessing The Wizard

{% hint style="info" %}
The Add UMA Support Wizard is only available if you have the [AnyRPG UMA addon](../getting-started/managing-addons/uma-installation.md) installed.
{% endhint %}

The Add UMA Support Wizard requires that one of your game scenes with either a GameManager or SceneConfig object is open in the editor so that it can determine which game to install the content into.

The Add UMA Support Wizard can be opened by clicking _Tools_ in the menu bar, and selecting _AnyRPG > Wizard > UMA > Add UMA Support_.

<div align="left"><figure><img src="../.gitbook/assets/image (186).png" alt=""><figcaption></figcaption></figure></div>

## Content Created

The wizard adds the following content to any game.

### UMA GLIB Prefab Varient

In the _Prefab/GameManager_ folder you can find an UMA GLIB prefab variant.  This variant has also been added to the game loading scene.

### Scriptable Objects

#### Unit Profiles

In the _Resources/GameName/UnitProfile/Player_ folder you can find UMA human male and female unit profiles.

#### UMA Race

An UMA character race can be found in the _Resources/GameName/CharacterRace_ folder.

## Next Steps

Add the UMA unit profiles to the list of available unit profiles in the [game configuration](../getting-started/configuring-your-game.md).
