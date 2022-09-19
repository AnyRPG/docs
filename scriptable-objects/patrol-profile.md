---
description: >-
  A patrol profile defines where and how a character will patrol, including
  locations, timing, and speed.
---

# Patrol Profile

## Creation

To create a material profile, find (or create) the _GameName/Resources/GameName/PatrolProfile_ folder in the project tab and right click.  Choose _Create > AnyRPG > PatrolProfile_.

![](<../.gitbook/assets/image (2).png>)



## Properties

A patrol profile contains a single property, Patrol Properties, which consists of the following properties.

| Name                          | Description                                                                                                                                                                                                                   |
| ----------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Auto Start                    | If true, a character unit that uses this patrol will start the patrol automatically upon spawning or entering the patrol state.                                                                                               |
| Destination List              | A list of Vector3 coordinates that the unit will patrol to.                                                                                                                                                                   |
| Use Tags                      | If true, the unit will patrol to the destinations in the Destination Tag List instead of the destination list.  This is useful if the level geometry will change because it doesn't require re-creating the destination list. |
| Destination Tag List          | A list of tags.  The current scene will be searched for these tags, and the unit will patrol to the location of the tags.                                                                                                     |
| Random Destinations           | If true, destinations will be chosen randomly from the active destination list, rather than visited sequentially in order.                                                                                                    |
| Loop Destinations             | If true, the patrol will continue indefinitely, re-starting at the first destination when the last destination is reached.                                                                                                    |
| Despawn On Completion         | If true, the unit will despawn when the last destination is reached.                                                                                                                                                          |
| Max Destinations              | If set to any number other than 0 (infinite), the patrol will end after that number of destinations have been reached.                                                                                                        |
| Max Distance From Spawn Point | If the destination list is empty, and _Random Destinations_ is set to true, a random location that is less than or equal to this number of meters from the spawn point will be chosen.                                        |
| Destination Pause Time        | The amount of time, in seconds, that a unit will pause at each destination before continuing to the next destination.                                                                                                         |
| Movement Speed                | The speed, in meters per second, that the unit will travel at when patrolling.                                                                                                                                                |
| Save Position At Destination  | If true, the unit will attempt to save its position when it reaches a destination.  The next time a saved game is loaded, the unit will start at the saved position, instead of its usual spawn point.                        |

## Next Steps

* Assign a Patrol Profile to a [Unit Profile](unit-profile.md).
