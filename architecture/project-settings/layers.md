# Layers

The table below lists the required layers and their purpose.

| Layer | Name           | Source          | Usage                                                                                                                                                                                                                                    |
| ----- | -------------- | --------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 0     | Default        | Unity           | Projectors will shine on this layer. Invector controller requires anything walkable to use this layer.                                                                                                                                   |
| 1     | TransparentFX  | Unity           |                                                                                                                                                                                                                                          |
| 2     | Ignore Raycast | Unity           | Player Nameplate uses this layer to prevent accidental highlight of player unit.                                                                                                                                                         |
| 3     |                | Unity           |                                                                                                                                                                                                                                          |
| 4     | Water          | Unity           |                                                                                                                                                                                                                                          |
| 5     | UI             | Unity           |                                                                                                                                                                                                                                          |
| 6     |                | Unity           |                                                                                                                                                                                                                                          |
| 7     |                | Unity           |                                                                                                                                                                                                                                          |
| 8     | Player         | Invector/AnyRPG | <p>Used to allow camera to ignore anything that is not the player in player unit frame and character panel.<br>Many packages like Invector also rely on this player being set to this layer so they can find it.</p>                     |
| 9     | Enemy          | Invector        |                                                                                                                                                                                                                                          |
| 10    | CompanionAI    | Invector        |                                                                                                                                                                                                                                          |
| 11    | Triggers       | Invector        |                                                                                                                                                                                                                                          |
| 12    | StopMove       | Invector        |                                                                                                                                                                                                                                          |
| 13    | Action         | Invector        |                                                                                                                                                                                                                                          |
| 14    | HeadTrack      | Invector        |                                                                                                                                                                                                                                          |
| 15    | BodyPart       | Invector        |                                                                                                                                                                                                                                          |
| 16    | BlockAIRayCast | Invector        |                                                                                                                                                                                                                                          |
| 17    | Equipment      | AnyRPG          | Set anything attached to the player to this layer to prevent it from interfering with ground detection or projectors.                                                                                                                    |
| 18    | FireLayer      | Package         | Unused. This was probably from an import of a VFX package.                                                                                                                                                                               |
| 19    | PlayerPreview  | AnyRPG          | Used by the load game screen to allow the camera to ignore anything that is not a player preview.                                                                                                                                        |
| 20    | SpellEffects   | AnyRPG          | Used to ignore raycasts, collision, and all but the main camera rendering spell effects.                                                                                                                                                 |
| 21    | MiniMap        | AnyRPG          | Anything on this layer will only be rendered by the minimap camera. Used for interactable icons such as questgiver showing on the minimap.                                                                                               |
| 22    | CharacterUnit  | AnyRPG          | CharacterUnit is the layer that all characters should be placed on. This allows them to show in unit frames and is required for an AOE ability to target anything to avoid spending time processing hits against the ground, props, etc. |
| 23    | UnitPreview    | AnyRPG          | Unit previews such as unit spawn control panelswill place their targets on this layer so other cameras don't render them.                                                                                                                |
| 24    | PetPreview     | AnyRPG          | Pet previews such as pet journals will place their targets on this layer so other cameras don't render them.                                                                                                                             |
| 25    | Interactable   | AnyRPG          | Used to render non character units in Unit frames without rendering the environment.                                                                                                                                                     |
| 26    |                | Unused          |                                                                                                                                                                                                                                          |
| 27    |                | Unused          |                                                                                                                                                                                                                                          |
| 28    |                | Unused          |                                                                                                                                                                                                                                          |
| 29    |                | Unused          |                                                                                                                                                                                                                                          |
| 30    |                | Unused          |                                                                                                                                                                                                                                          |
| 31    | AlwaysVisible  | Package         | The Sun Temple uses this layer to make certain things in the background always visible regardless of culling distances.                                                                                                                  |