# Ability Effects

Ability Effects are separated into small pieces of related functionality, and can be chained together like building blocks to build up quite complex spells. The 3 main groups of functionality are:

1. Attached effects are tracked by the CharacterStats class on the actual character, have a length that can be extended or refreshed, and are capable of both directly affecting a character's stats, and performing additional effects over their lifetime.
2. Targeting and timing effects are responsible for deciding when and where to trigger additional effects. They may choose valid targets from a group of targets, direct the motion of physical prefabs, and determine how long spell effects remain in the game before they are destroyed. They cannot perform any direct action on a character, but can call any other effect, including effects which can perform actions on characters.
3. Action effects perform actions on characters. Current action capabilities include resurrection, teleportation, healing, and damage dealing.

<img src="../../.gitbook/assets/image (55).png" alt="" data-size="original">
