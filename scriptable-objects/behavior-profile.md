---
description: >-
  A behavior profile is a list of commands that can be sent to a character unit
  at specified time intervals using Unity's SendMessage functionality.
---

# Behavior Profile

## Creation

To create a behavior profile, find (or create) the _GameName/Resources/GameName/BehaviorProfile_ folder in the project tab and right click.  Choose _Create > AnyRPG > BehaviorProfile_.

![](<../.gitbook/assets/image (125).png>)

## Properties

| Name                    | Description                                                                                                                              |
| ----------------------- | ---------------------------------------------------------------------------------------------------------------------------------------- |
| Behavior Nodes          | A list of [Behavior Nodes](behavior-profile.md#undefined).                                                                               |
| Prerequisite Conditions | A list of [Prerequisite Conditions](../shared-properties/prerequisite-conditions.md).                                                    |
| Automatic               | If true, the object that is using this behavior profile will automatically play the behavior when activated.                             |
| Allow Manual Start      | If true, this behavior will appear on the list of interaction options for this character unit and can be manually started by the player. |
| Repeatable              | If true, this behavior can be played more than once.                                                                                     |
| Looping                 | If true, this behavior will automatically play again when finished.                                                                      |

### Behavior Nodes

| Name                  | Description                                                                                                                                                                                                                                                              |
| --------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Start Time            | The time, in seconds, when the behavior node should play.                                                                                                                                                                                                                |
| Behavior Action Nodes | <p>A list of behavior action nodes.<br><strong>Behavior Method</strong><br>The name of the method to call using Unity's SendMessage function.<br><strong>Behavior Parameter</strong><br>A string parameter to send as the parameter to the <em>Behavior Method</em>.</p> |
